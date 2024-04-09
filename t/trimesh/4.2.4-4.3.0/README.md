# Comparing `tmp/trimesh-4.2.4.tar.gz` & `tmp/trimesh-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimesh-4.2.4.tar", last modified: Sun Mar 31 22:52:15 2024, max compression
+gzip compressed data, was "trimesh-4.3.0.tar", last modified: Tue Apr  9 18:10:18 2024, max compression
```

## Comparing `trimesh-4.2.4.tar` & `trimesh-4.3.0.tar`

### file list

```diff
@@ -1,262 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.447944 trimesh-4.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-31 22:52:06.000000 trimesh-4.2.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-03-31 22:52:15.447944 trimesh-4.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-03-31 22:52:06.000000 trimesh-4.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-03-31 22:52:06.000000 trimesh-4.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 22:52:15.447944 trimesh-4.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.419944 trimesh-4.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_3dxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_3mf.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_adjacency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_arc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_binvox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_convex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_crash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_curvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_dae.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_dxf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_except.py
--rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_fill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)    41146 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_gltf.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_gmsh.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_inertia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_integralmeancurvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_loaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_medial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_minimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_mutate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_normals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_nsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_path_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_pbr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_permutate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_ply.py
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_poses.py
--rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_proximity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_ray.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_remesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_runlength.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_scenegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_section.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_splines.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_texture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_trackball.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_triangles.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_unwrap.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_urdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18466 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_vertices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-03-31 22:52:06.000000 trimesh-4.2.4/tests/test_voxel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.427944 trimesh-4.2.4/trimesh/
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   102604 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/convex.py
--rw-r--r--   0 runner    (1001) docker     (127)    43290 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/curvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.431944 trimesh-4.2.4/trimesh/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/binvox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/dae.py
--rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    68462 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/gltf.py
--rw-r--r--   0 runner    (1001) docker     (127)    21659 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    34419 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/off.py
--rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/ply.py
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/stl.py
--rw-r--r--   0 runner    (1001) docker     (127)    15866 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/threedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/threemf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/urdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/xaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/exchange/xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    30523 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    26162 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/inertia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.431944 trimesh-4.2.4/trimesh/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/interfaces/blender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/interfaces/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/interfaces/gmsh.py
--rw-r--r--   0 runner    (1001) docker     (127)    28268 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/intersections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/nsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/parent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.435944 trimesh-4.2.4/trimesh/path/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/arc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.435944 trimesh-4.2.4/trimesh/path/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33119 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/exchange/dxf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/exchange/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/exchange/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/exchange/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23095 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/exchange/svg_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/intersections.py
--rw-r--r--   0 runner    (1001) docker     (127)    26100 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    31112 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/segments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/path/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/permutate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19968 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/poses.py
--rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/proximity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.439944 trimesh-4.2.4/trimesh/ray/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/ray/ray_pyembree.py
--rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/ray/ray_triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/ray/ray_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    40188 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/remesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.439944 trimesh-4.2.4/trimesh/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.439944 trimesh-4.2.4/trimesh/resources/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    24785 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/gltf2.schema.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.439944 trimesh-4.2.4/trimesh/resources/schema/primitive/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/primitive/box.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/primitive/capsule.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/primitive/cylinder.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/primitive/extrusion.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/primitive/primitive.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/primitive/scenegraph.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/primitive/sphere.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/primitive/transform.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/primitive/trimesh.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/primitive/wkt.polygon.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/schema/urdf.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.439944 trimesh-4.2.4/trimesh/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/templates/base.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/templates/blender_boolean.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/templates/blender_unwrap.py.template
--rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/templates/dxf.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/templates/path.svg
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/templates/ply.json
--rw-r--r--   0 runner    (1001) docker     (127)   167999 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/templates/viewer.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/resources/units_to_inches.json
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.443944 trimesh-4.2.4/trimesh/scene/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/scene/cameras.py
--rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/scene/lighting.py
--rw-r--r--   0 runner    (1001) docker     (127)    48032 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/scene/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/scene/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)    74263 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21710 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/triangles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    66719 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.443944 trimesh-4.2.4/trimesh/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/viewer/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/viewer/trackball.py
--rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/viewer/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    30971 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/viewer/windowed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.443944 trimesh-4.2.4/trimesh/visual/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/visual/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    29109 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/visual/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/visual/gloss.py
--rw-r--r--   0 runner    (1001) docker     (127)    34678 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/visual/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/visual/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/visual/texture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.447944 trimesh-4.2.4/trimesh/voxel/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/voxel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/voxel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/voxel/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)    27755 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/voxel/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/voxel/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/voxel/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/voxel/runlength.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-03-31 22:52:06.000000 trimesh-4.2.4/trimesh/voxel/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:52:15.447944 trimesh-4.2.4/trimesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-03-31 22:52:15.000000 trimesh-4.2.4/trimesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-03-31 22:52:15.000000 trimesh-4.2.4/trimesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 22:52:15.000000 trimesh-4.2.4/trimesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-31 22:52:15.000000 trimesh-4.2.4/trimesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-31 22:52:15.000000 trimesh-4.2.4/trimesh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.148617 trimesh-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-09 18:10:07.000000 trimesh-4.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-09 18:10:18.148617 trimesh-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-04-09 18:10:07.000000 trimesh-4.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-09 18:10:07.000000 trimesh-4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:10:18.148617 trimesh-4.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.120616 trimesh-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_3dxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_3mf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_adjacency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_binvox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_convex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_curvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_dae.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_dxf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_except.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41146 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_gltf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_integralmeancurvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_medial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_mutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_normals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_nsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_path_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_pbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_permutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_ply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_remesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_runlength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_scenegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_splines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_texture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_trackball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_triangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_unwrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_urdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18466 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_vertices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-09 18:10:07.000000 trimesh-4.3.0/tests/test_voxel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.128616 trimesh-4.3.0/trimesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102604 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/convex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45776 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.132617 trimesh-4.3.0/trimesh/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/binvox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/dae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68462 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21659 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34419 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/off.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/ply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15866 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/threedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/threemf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/urdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/xaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/exchange/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30523 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26162 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/inertia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.132617 trimesh-4.3.0/trimesh/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/interfaces/blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/interfaces/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/interfaces/gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28268 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/intersections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/nsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/parent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.136617 trimesh-4.3.0/trimesh/path/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.136617 trimesh-4.3.0/trimesh/path/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33119 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/dxf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23095 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/exchange/svg_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/intersections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26100 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31112 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/path/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/permutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19968 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/proximity.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.136617 trimesh-4.3.0/trimesh/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/ray/ray_pyembree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/ray/ray_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/ray/ray_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40188 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/remesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.136617 trimesh-4.3.0/trimesh/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/creation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.140617 trimesh-4.3.0/trimesh/resources/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24785 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/gltf2.schema.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.140617 trimesh-4.3.0/trimesh/resources/schema/primitive/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/box.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/capsule.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/cylinder.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/extrusion.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/primitive.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/scenegraph.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/sphere.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/transform.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/trimesh.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/primitive/wkt.polygon.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/schema/urdf.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.140617 trimesh-4.3.0/trimesh/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/base.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/blender_boolean.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/blender_unwrap.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/dxf.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/path.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/ply.json
+-rw-r--r--   0 runner    (1001) docker     (127)   167999 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/templates/viewer.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/resources/units_to_inches.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.144617 trimesh-4.3.0/trimesh/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/scene/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/scene/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48032 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/scene/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/scene/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74544 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21710 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/triangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66709 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.144617 trimesh-4.3.0/trimesh/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/viewer/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/viewer/trackball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/viewer/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30971 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/viewer/windowed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.144617 trimesh-4.3.0/trimesh/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29109 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/gloss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34678 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/visual/texture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.144617 trimesh-4.3.0/trimesh/voxel/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27755 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/runlength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-09 18:10:07.000000 trimesh-4.3.0/trimesh/voxel/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:10:18.144617 trimesh-4.3.0/trimesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-09 18:10:18.000000 trimesh-4.3.0/trimesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-09 18:10:18.000000 trimesh-4.3.0/trimesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:10:18.000000 trimesh-4.3.0/trimesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 18:10:18.000000 trimesh-4.3.0/trimesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 18:10:18.000000 trimesh-4.3.0/trimesh.egg-info/top_level.txt
```

### Comparing `trimesh-4.2.4/LICENSE.md` & `trimesh-4.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/PKG-INFO` & `trimesh-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimesh
-Version: 4.2.4
+Version: 4.3.0
 Summary: Import, export, process, analyze and view triangular meshes.
 Author-email: Michael Dawson-Haggerty <mikedh@kerfed.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Michael Dawson-Haggerty
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,14 +75,15 @@
 Requires-Dist: cascadio; extra == "recommend"
 Requires-Dist: manifold3d>=2.3.0; extra == "recommend"
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coveralls; extra == "test"
 Requires-Dist: pyright; extra == "test"
 Requires-Dist: ezdxf; extra == "test"
+Requires-Dist: gmsh>=4.12.1; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pymeshlab; extra == "test"
 Requires-Dist: pyinstrument; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: pytest-beartype; python_version >= "3.10" and extra == "test"
 Provides-Extra: all
```

### Comparing `trimesh-4.2.4/README.md` & `trimesh-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/pyproject.toml` & `trimesh-4.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools >= 61.0", "wheel"]
 
 [project]
 name = "trimesh"
 requires-python = ">=3.7"
-version = "4.2.4"
+version = "4.3.0"
 authors = [{name = "Michael Dawson-Haggerty", email = "mikedh@kerfed.com"}]
 license = {file = "LICENSE.md"}
 description = "Import, export, process, analyze and view triangular meshes."
 keywords = ["graphics", "mesh", "geometry", "3D"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
@@ -98,14 +98,15 @@
 # this is the list of everything that is ever added anywhere
 # mostly useful for getting our test coverage up
 test = [
     "pytest-cov",
     "coveralls",
     "pyright",
     "ezdxf",
+    "gmsh>=4.12.1",
     "pytest",
     "pymeshlab",
     "pyinstrument",
     "matplotlib",
     "ruff",
     "pytest-beartype; python_version>='3.10'"
 ]
@@ -129,15 +130,16 @@
     "E", # style errors
     "F", # flakes
     "I", # import sorting
     "RUF", # ruff specific rules
     "UP", # upgrade
     "W", # style warnings
     "YTT", # sys.version
-    "ISC002"
+    "ISC002",
+    "NPY201"
 ]
 
 ignore = [
   "C901", # Comprehension is too complex (11 > 10)
   "N802", # Function name should be lowercase
   "N806", # Variable in function should be lowercase
   "E501", # Line too long ({width} > {limit} characters)
```

### Comparing `trimesh-4.2.4/tests/test_3dxml.py` & `trimesh-4.3.0/tests/test_3dxml.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_3mf.py` & `trimesh-4.3.0/tests/test_3mf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_adjacency.py` & `trimesh-4.3.0/tests/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_align.py` & `trimesh-4.3.0/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_arc.py` & `trimesh-4.3.0/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_base.py` & `trimesh-4.3.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_binvox.py` & `trimesh-4.3.0/tests/test_binvox.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_boolean.py` & `trimesh-4.3.0/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_bounds.py` & `trimesh-4.3.0/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_cache.py` & `trimesh-4.3.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_camera.py` & `trimesh-4.3.0/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_collision.py` & `trimesh-4.3.0/tests/test_collision.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_color.py` & `trimesh-4.3.0/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_convex.py` & `trimesh-4.3.0/tests/test_convex.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_copy.py` & `trimesh-4.3.0/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_crash.py` & `trimesh-4.3.0/tests/test_crash.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_creation.py` & `trimesh-4.3.0/tests/test_creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,26 +143,40 @@
         )
         perim = []
         for _i in range(n_comps):
             perim.append(vec)
             vec = g.np.dot(rotmat, vec)
         poly = g.Polygon(perim)
 
+        # --- test open sweep
         # Create 3D path
         angles = g.np.linspace(0, 8 * g.np.pi, 1000)
         x = angles / 10.0
         y = g.np.cos(angles)
         z = g.np.sin(angles)
         path = g.np.c_[x, y, z]
 
         # Extrude
         for engine in self.engines:
             mesh = g.trimesh.creation.sweep_polygon(poly, path, engine=engine)
             assert mesh.is_volume
 
+        # --- test closed sweep
+        # Create 3D path
+        angles = g.np.linspace(0, 2 * 0.999 * g.np.pi, 1000)
+        x = g.np.zeros((1000,))
+        y = g.np.cos(angles)
+        z = g.np.sin(angles)
+        path_closed = g.np.c_[x, y, z]
+
+        # Extrude
+        for engine in self.engines:
+            mesh = g.trimesh.creation.sweep_polygon(poly, path_closed, engine=engine)
+            assert mesh.is_volume
+
     def test_annulus(self):
         """
         Basic tests of annular cylinder creation
         """
 
         # run through transforms
         transforms = [None]
```

### Comparing `trimesh-4.2.4/tests/test_curvature.py` & `trimesh-4.3.0/tests/test_curvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_dae.py` & `trimesh-4.3.0/tests/test_dae.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_decomposition.py` & `trimesh-4.3.0/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_dxf.py` & `trimesh-4.3.0/tests/test_dxf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_edges.py` & `trimesh-4.3.0/tests/test_edges.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_encoding.py` & `trimesh-4.3.0/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_except.py` & `trimesh-4.3.0/tests/test_except.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_export.py` & `trimesh-4.3.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_extrude.py` & `trimesh-4.3.0/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_facets.py` & `trimesh-4.3.0/tests/test_facets.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_fill.py` & `trimesh-4.3.0/tests/test_fill.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_geom.py` & `trimesh-4.3.0/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_gltf.py` & `trimesh-4.3.0/tests/test_gltf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_gmsh.py` & `trimesh-4.3.0/tests/test_gmsh.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,16 +19,25 @@
         result = g.trimesh.interfaces.gmsh.to_volume(m)
         assert len(result) > 0
 
     def test_load(self):
         if gmsh is None:
             return
         r = g.trimesh.interfaces.gmsh.load_gmsh(
-            g.os.path.join(g.dir_models, "wrench.STEP")
+            g.os.path.join(g.dir_models, "featuretype.STEP")
         )
         assert isinstance(r, dict)
         assert len(g.trimesh.Trimesh(**r).faces) > 0
 
+    def test_to_volume(self):
+        if gmsh is None:
+            return
+        m = g.trimesh.creation.box()
+
+        r = g.trimesh.interfaces.gmsh.to_volume(mesh=m)
+
+        assert isinstance(r, bytes)
+
 
 if __name__ == "__main__":
     g.trimesh.util.attach_to_log()
     g.unittest.main()
```

### Comparing `trimesh-4.2.4/tests/test_graph.py` & `trimesh-4.3.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_grouping.py` & `trimesh-4.3.0/tests/test_grouping.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_html.py` & `trimesh-4.3.0/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_identifier.py` & `trimesh-4.3.0/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_import.py` & `trimesh-4.3.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_inertia.py` & `trimesh-4.3.0/tests/test_inertia.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_integralmeancurvature.py` & `trimesh-4.3.0/tests/test_integralmeancurvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_interval.py` & `trimesh-4.3.0/tests/test_interval.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_light.py` & `trimesh-4.3.0/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_loaded.py` & `trimesh-4.3.0/tests/test_loaded.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_medial.py` & `trimesh-4.3.0/tests/test_medial.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_merge.py` & `trimesh-4.3.0/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_mesh.py` & `trimesh-4.3.0/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_meta.py` & `trimesh-4.3.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_minimal.py` & `trimesh-4.3.0/tests/test_minimal.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_mutate.py` & `trimesh-4.3.0/tests/test_mutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_normals.py` & `trimesh-4.3.0/tests/test_normals.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_nsphere.py` & `trimesh-4.3.0/tests/test_nsphere.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_obj.py` & `trimesh-4.3.0/tests/test_obj.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_off.py` & `trimesh-4.3.0/tests/test_off.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_operators.py` & `trimesh-4.3.0/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_packing.py` & `trimesh-4.3.0/tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_path_creation.py` & `trimesh-4.3.0/tests/test_path_creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_pathlib.py` & `trimesh-4.3.0/tests/test_pathlib.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_paths.py` & `trimesh-4.3.0/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_pbr.py` & `trimesh-4.3.0/tests/test_pbr.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_permutate.py` & `trimesh-4.3.0/tests/test_permutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_ply.py` & `trimesh-4.3.0/tests/test_ply.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_points.py` & `trimesh-4.3.0/tests/test_points.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_polygons.py` & `trimesh-4.3.0/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_poses.py` & `trimesh-4.3.0/tests/test_poses.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_primitives.py` & `trimesh-4.3.0/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_proximity.py` & `trimesh-4.3.0/tests/test_proximity.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_raster.py` & `trimesh-4.3.0/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_ray.py` & `trimesh-4.3.0/tests/test_ray.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_registration.py` & `trimesh-4.3.0/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_remesh.py` & `trimesh-4.3.0/tests/test_remesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_render.py` & `trimesh-4.3.0/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_repair.py` & `trimesh-4.3.0/tests/test_repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_repr.py` & `trimesh-4.3.0/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_resolvers.py` & `trimesh-4.3.0/tests/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_runlength.py` & `trimesh-4.3.0/tests/test_runlength.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_sample.py` & `trimesh-4.3.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_scene.py` & `trimesh-4.3.0/tests/test_scene.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_scenegraph.py` & `trimesh-4.3.0/tests/test_scenegraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,21 +202,21 @@
         # compare the EnforcedForest shortest path algo
         # to the more general networkx.shortest_path algo
         if g.sys.version_info < (3, 7):
             # old networkx is a lot different
             return
 
         tf = g.trimesh.transformations
-        # start with creating a random tree
-        edgelist = {}
-        tree = g.nx.random_tree(n=1000, seed=0, create_using=g.nx.DiGraph)
-        edges = list(tree.edges)
+        # start with a known good random tree
+        edges = [tuple(row) for row in g.data["random_tree"]]
+        tree = g.nx.from_edgelist(edges, create_using=g.nx.DiGraph)
 
         r_choices = g.random((len(edges), 2))
         r_matrices = g.random_transforms(len(edges))
+        edgelist = {}
         for e, r_choice, r_mat in zip(edges, r_choices, r_matrices):
             data = {}
             if r_choice[0] > 0.5:
                 # if a matrix is omitted but an edge exists it is
                 # the same as passing an identity matrix
                 data["matrix"] = r_mat
             if r_choice[1] > 0.4:
```

### Comparing `trimesh-4.2.4/tests/test_section.py` & `trimesh-4.3.0/tests/test_section.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_segments.py` & `trimesh-4.3.0/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_simplify.py` & `trimesh-4.3.0/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_smooth.py` & `trimesh-4.3.0/tests/test_smooth.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_smoothing.py` & `trimesh-4.3.0/tests/test_smoothing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_splines.py` & `trimesh-4.3.0/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_stl.py` & `trimesh-4.3.0/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_svg.py` & `trimesh-4.3.0/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_texture.py` & `trimesh-4.3.0/tests/test_texture.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_thickness.py` & `trimesh-4.3.0/tests/test_thickness.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_trackball.py` & `trimesh-4.3.0/tests/test_trackball.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_transformations.py` & `trimesh-4.3.0/tests/test_transformations.py`

 * *Files 6% similar despite different names*

```diff
@@ -223,11 +223,36 @@
             )
             # get it from a numeric scalar
             n = euler(*rot)
 
             # they should be the same matrix
             assert g.np.allclose(s, n)
 
+    def test_symbolic_translate(self):
+        # some of the functions have been modified to support `sympy.Symbol`
+        # values which is useful for calculating final rotations symbolically
+        try:
+            import sympy as sp
+        except BaseException:
+            return
+
+        translate = g.trimesh.transformations.translation_matrix
+
+        x, y, z = sp.symbols("x y z")
+
+        m = translate([x, y, z])
+
+        for T in g.random((100, 3)):
+            # get the euler matrix evaluated from the symbolic matrix
+            s = g.np.array(
+                m.subs({x: T[0], y: T[1], z: T[2]}).evalf(), dtype=g.np.float64
+            )
+            # get it from a numeric scalar
+            n = translate(T)
+
+            # they should be the same matrix
+            assert g.np.allclose(s, n)
+
 
 if __name__ == "__main__":
     g.trimesh.util.attach_to_log()
     g.unittest.main()
```

### Comparing `trimesh-4.2.4/tests/test_triangles.py` & `trimesh-4.3.0/tests/test_triangles.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_units.py` & `trimesh-4.3.0/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_unwrap.py` & `trimesh-4.3.0/tests/test_unwrap.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_upstream.py` & `trimesh-4.3.0/tests/test_upstream.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_urdf.py` & `trimesh-4.3.0/tests/test_urdf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_util.py` & `trimesh-4.3.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_vector.py` & `trimesh-4.3.0/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_vertices.py` & `trimesh-4.3.0/tests/test_vertices.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_viewer.py` & `trimesh-4.3.0/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_visual.py` & `trimesh-4.3.0/tests/test_visual.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/tests/test_voxel.py` & `trimesh-4.3.0/tests/test_voxel.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/__init__.py` & `trimesh-4.3.0/trimesh/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/base.py` & `trimesh-4.3.0/trimesh/base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/boolean.py` & `trimesh-4.3.0/trimesh/boolean.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/bounds.py` & `trimesh-4.3.0/trimesh/bounds.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/caching.py` & `trimesh-4.3.0/trimesh/caching.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/collision.py` & `trimesh-4.3.0/trimesh/collision.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/comparison.py` & `trimesh-4.3.0/trimesh/comparison.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/constants.py` & `trimesh-4.3.0/trimesh/constants.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/convex.py` & `trimesh-4.3.0/trimesh/convex.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/creation.py` & `trimesh-4.3.0/trimesh/creation.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import numpy as np
 
 from . import exceptions, grouping, triangles, util
 from . import transformations as tf
 from .base import Trimesh
 from .constants import log, tol
 from .geometry import align_vectors, faces_to_edges, plane_transform
+from .resources import get_json
 from .typed import ArrayLike, Dict, Integer, Number, Optional
 
 try:
     # shapely is a soft dependency
     from shapely.geometry import Polygon
     from shapely.wkb import loads as load_wkb
 except BaseException as E:
@@ -28,14 +29,17 @@
     load_wkb = exceptions.ExceptionWrapper(E)
 
 try:
     from mapbox_earcut import triangulate_float64 as _tri_earcut
 except BaseException as E:
     _tri_earcut = exceptions.ExceptionWrapper(E)
 
+# get stored values for simple box and icosahedron primitives
+_data = get_json("creation.json")
+
 
 def revolve(
     linestring: ArrayLike,
     angle: Optional[Number] = None,
     sections: Optional[Integer] = None,
     transform: Optional[ArrayLike] = None,
     **kwargs,
@@ -202,118 +206,229 @@
     mesh = extrude_triangulation(
         vertices=vertices, faces=faces, height=height, transform=transform, **kwargs
     )
     return mesh
 
 
 def sweep_polygon(
-    polygon: "Polygon", path: ArrayLike, angles: Optional[ArrayLike] = None, **kwargs
-):
+    polygon: "Polygon",
+    path: ArrayLike,
+    angles: Optional[ArrayLike] = None,
+    cap: bool = True,
+    connect: bool = True,
+    kwargs: Optional[Dict] = None,
+    **triangulation,
+) -> Trimesh:
     """
-    Extrude a 2D shapely polygon into a 3D mesh along an
-    arbitrary 3D path. Doesn't handle sharp curvature well.
+    Extrude a 2D polygon into a 3D mesh along a 3D path. Note that this
+    does *not* handle the case where there is very sharp curvature leading
+    the polygon to intersect the plane of a previous slice, and does *not*
+    scale the polygon along the induced normal to result in a constant cross section.
 
+    You may want to resample your path with a B-spline, i.e:
+      `trimesh.path.simplify.resample_spline(path, smooth=0.2, count=100)`
 
     Parameters
     ----------
     polygon : shapely.geometry.Polygon
       Profile to sweep along path
     path : (n, 3) float
       A path in 3D
-    angles :  (n,) float
+    angles : (n,) float
       Optional rotation angle relative to prior vertex
-      at each vertex
-    **kwargs : dict
-      Passed to `triangulate_polygon`.
+      at each vertex.
+    cap
+      If an open path is passed apply a cap to both ends.
+    connect
+      If a closed path is passed connect the sweep into
+      a single watertight mesh.
+    kwargs : dict
+      Passed to the mesh constructor.
+    **triangulation
+      Passed to `triangulate_polygon`, i.e. `engine='triangle'`
+
     Returns
     -------
     mesh : trimesh.Trimesh
       Geometry of result
     """
 
     path = np.asanyarray(path, dtype=np.float64)
     if not util.is_shape(path, (-1, 3)):
         raise ValueError("Path must be (n, 3)!")
 
+    if angles is not None:
+        angles = np.asanyarray(angles, dtype=np.float64)
+        if angles.shape != (len(path),):
+            raise ValueError(angles.shape)
+    else:
+        # set all angles to zero
+        angles = np.zeros(len(path), dtype=np.float64)
+
+    # check to see if path is closed i.e. first and last vertex are the same
+    closed = np.linalg.norm(path[0] - path[-1]) < tol.merge
     # Extract 2D vertices and triangulation
-    verts_2d = np.array(polygon.exterior.coords)[:-1]
-    base_verts_2d, faces_2d = triangulate_polygon(polygon, **kwargs)
-    n = len(verts_2d)
-
-    # Create basis for first planar polygon cap
-    x, y, z = util.generate_basis(path[0] - path[1])
-    tf_mat = np.ones((4, 4))
-    tf_mat[:3, :3] = np.c_[x, y, z]
-    tf_mat[:3, 3] = path[0]
-
-    # Compute 3D locations of those vertices
-    verts_3d = np.c_[verts_2d, np.zeros(n)]
-    verts_3d = tf.transform_points(verts_3d, tf_mat)
-    base_verts_3d = np.c_[base_verts_2d, np.zeros(len(base_verts_2d))]
-    base_verts_3d = tf.transform_points(base_verts_3d, tf_mat)
-
-    # keep matching sequence of vertices and 0- indexed faces
-    vertices = [base_verts_3d]
-    faces = [faces_2d]
-
-    # Compute plane normals for each turn --
-    # each turn induces a plane halfway between the two vectors
-    v1s = util.unitize(path[1:-1] - path[:-2])
-    v2s = util.unitize(path[1:-1] - path[2:])
-    norms = np.cross(np.cross(v1s, v2s), v1s + v2s)
-    norms[(norms == 0.0).all(1)] = v1s[(norms == 0.0).all(1)]
-    norms = util.unitize(norms)
-    final_v1 = util.unitize(path[-1] - path[-2])
-    norms = np.vstack((norms, final_v1))
-    v1s = np.vstack((v1s, final_v1))
-
-    # Create all side walls by projecting the 3d vertices into each plane
-    # in succession
-    for i in range(len(norms)):
-        verts_3d_prev = verts_3d
-
-        # Rotate if needed
-        if angles is not None:
-            tf_mat = tf.rotation_matrix(angles[i], norms[i], path[i])
-            verts_3d_prev = tf.transform_points(verts_3d_prev, tf_mat)
-
-        # Project vertices onto plane in 3D
-        ds = np.einsum("ij,j->i", (path[i + 1] - verts_3d_prev), norms[i])
-        ds = ds / np.dot(v1s[i], norms[i])
-
-        verts_3d_new = np.einsum("i,j->ij", ds, v1s[i]) + verts_3d_prev
-
-        # Add to face and vertex lists
-        new_faces = [[i + n, (i + 1) % n, i] for i in range(n)]
-        new_faces.extend([[(i - 1) % n + n, i + n, i] for i in range(n)])
-
-        # save faces and vertices into a sequence
-        faces.append(np.array(new_faces))
-        vertices.append(np.vstack((verts_3d, verts_3d_new)))
-
-        verts_3d = verts_3d_new
-
-    # do the main stack operation from a sequence to (n,3) arrays
-    # doing one vstack provides a substantial speedup by
-    # avoiding a bunch of temporary  allocations
-    vertices, faces = util.append_faces(vertices, faces)
-
-    # Create final cap
-    x, y, z = util.generate_basis(path[-1] - path[-2])
-    vecs = verts_3d - path[-1]
-    coords = np.c_[np.einsum("ij,j->i", vecs, x), np.einsum("ij,j->i", vecs, y)]
-    base_verts_2d, faces_2d = triangulate_polygon(Polygon(coords), **kwargs)
-    base_verts_3d = (
-        np.einsum("i,j->ij", base_verts_2d[:, 0], x)
-        + np.einsum("i,j->ij", base_verts_2d[:, 1], y)
-    ) + path[-1]
-    faces = np.vstack((faces, faces_2d + len(vertices)))
-    vertices = np.vstack((vertices, base_verts_3d))
+    vertices_2D, faces_2D = triangulate_polygon(polygon, **triangulation)
+
+    # stack the `(n, 3)` faces into `(3 * n, 2)` edges
+    edges = faces_to_edges(faces_2D)
+    # edges which only occur once are on the boundary of the polygon
+    # since the triangulation may have subdivided the boundary of the
+    # shapely polygon, we need to find it again
+    edges_unique = grouping.group_rows(np.sort(edges, axis=1), require_count=1)
+    # subset the vertices to only ones included in the boundary
+    unique, inverse = np.unique(edges[edges_unique].reshape(-1), return_inverse=True)
+    # take only the vertices in the boundary
+    # and stack them with zeros and ones so we can use dot
+    # products to transform them all over the place
+    vertices_tf = np.column_stack(
+        (vertices_2D[unique], np.zeros(len(unique)), np.ones(len(unique)))
+    )
+    # the indices of vertices_tf
+    boundary = inverse.reshape((-1, 2))
+
+    # now create the normals for the plane each slice will lie on
+    # consider the simple path with 3 vertices and therefore 2 vectors:
+    # - the first plane will be exactly along the first vector
+    # - the second plane will be the average of the two vectors
+    # - the last plane will be exactly along the last vector
+    # and each plane origin will be the corresponding vertex on the path
+    vector = util.unitize(path[1:] - path[:-1])
+    # unitize instead of / 2 as they may be degenerate / zero
+    vector_mean = util.unitize(vector[1:] + vector[:-1])
+    # collect the vectors into plane normals
+    normal = np.concatenate([[vector[0]], vector_mean, [vector[-1]]], axis=0)
+
+    if closed and connect:
+        # if we have a closed loop average the first and last planes
+        normal[0] = util.unitize(normal[[0, -1]].mean(axis=0))
+
+    # planes should have one unit normal and one vertex each
+    assert normal.shape == path.shape
+
+    # get the spherical coordinates for the normal vectors
+    theta, phi = util.vector_to_spherical(normal).T
+
+    # collect the trig values into numpy arrays we can compose into matrices
+    cos_theta, sin_theta = np.cos(theta), np.sin(theta)
+    cos_phi, sin_phi = np.cos(phi), np.sin(phi)
+    cos_roll, sin_roll = np.cos(angles), np.sin(angles)
+
+    # we want a rotation which will be the identity for a Z+ vector
+    # this was constructed and unrolled from the following sympy block
+    # theta, phi, roll = sp.symbols("theta phi roll")
+    # matrix = (
+    #     tf.rotation_matrix(roll, [0, 0, 1]) @
+    #     tf.rotation_matrix(phi, [1, 0, 0]) @
+    #     tf.rotation_matrix((sp.pi / 2) - theta, [0, 0, 1])
+    # ).inv()
+    # matrix.simplify()
+
+    # shorthand for stacking
+    zeros = np.zeros(len(theta))
+    ones = np.ones(len(theta))
+
+    # stack initially as one unrolled matrix per row
+    transforms = np.column_stack(
+        [
+            -sin_roll * cos_phi * cos_theta + sin_theta * cos_roll,
+            sin_roll * sin_theta + cos_phi * cos_roll * cos_theta,
+            sin_phi * cos_theta,
+            path[:, 0],
+            -sin_roll * sin_theta * cos_phi - cos_roll * cos_theta,
+            -sin_roll * cos_theta + sin_theta * cos_phi * cos_roll,
+            sin_phi * sin_theta,
+            path[:, 1],
+            sin_phi * sin_roll,
+            -sin_phi * cos_roll,
+            cos_phi,
+            path[:, 2],
+            zeros,
+            zeros,
+            zeros,
+            ones,
+        ]
+    ).reshape((-1, 4, 4))
 
-    return Trimesh(vertices, faces)
+    if tol.strict:
+        # make sure that each transform moves the Z+ vector to the requested normal
+        for n, matrix in zip(normal, transforms):
+            check = tf.transform_points([[0.0, 0.0, 1.0]], matrix, translate=False)[0]
+            assert np.allclose(check, n)
+
+    # apply transforms to prebaked homogeneous coordinates
+    vertices_3D = np.concatenate(
+        [np.dot(vertices_tf, matrix.T) for matrix in transforms], axis=0
+    )[:, :3]
+
+    # now construct the faces with one group of boundary faces per slice
+    stride = len(unique)
+    boundary_next = boundary + stride
+    faces_slice = np.column_stack(
+        [boundary, boundary_next[:, :1], boundary_next[:, ::-1], boundary[:, 1:]]
+    ).reshape((-1, 3))
+
+    # offset the slices
+    faces = [faces_slice + offset for offset in np.arange(len(path) - 1) * stride]
+
+    # connect only applies to closed paths
+    if closed and connect:
+        # the last slice will not be required
+        max_vertex = (len(path) - 1) * stride
+        # clip off the duplicated vertices
+        vertices_3D = vertices_3D[:max_vertex]
+        # apply the modulus in-place to a conservative subset
+        faces[-1] %= max_vertex
+    elif cap:
+        # these are indices of `vertices_2D` that were not on the boundary
+        # which can happen for triangulation algorithms that added vertices
+        # we don't currently support that but you could append the unconsumed
+        # vertices and then update the mapping below to reflect that
+        unconsumed = set(unique).difference(faces_2D.ravel())
+        if len(unconsumed) > 0:
+            raise NotImplementedError("triangulation added vertices: no logic to cap!")
+
+        # map the 2D faces to the order we used
+        mapped = np.zeros(unique.max() + 2, dtype=np.int64)
+        mapped[unique] = np.arange(len(unique))
+
+        # now should correspond to the first vertex block
+        cap_zero = mapped[faces_2D]
+        # winding will be along +Z so flip for the bottom cap
+        faces.append(np.fliplr(cap_zero))
+        # offset the end cap
+        faces.append(cap_zero + stride * (len(path) - 1))
+
+    if kwargs is None:
+        kwargs = {}
+
+    if "process" not in kwargs:
+        # we should be constructing clean meshes here
+        # so we don't need to run an expensive verex merge
+        kwargs["process"] = False
+
+    # stack the faces used
+    faces = np.concatenate(faces, axis=0)
+
+    # generate the mesh from the face data
+    mesh = Trimesh(vertices=vertices_3D, faces=faces, **kwargs)
+
+    if tol.strict:
+        # we should not have included any unused vertices
+        assert len(np.unique(faces)) == len(vertices_3D)
+
+        if cap:
+            # mesh should always be a volume if cap is true
+            assert mesh.is_volume
+
+        if closed and connect:
+            assert mesh.is_volume
+            assert mesh.body_count == 1
+
+    return mesh
 
 
 def extrude_triangulation(
     vertices: ArrayLike,
     faces: ArrayLike,
     height: Number,
     transform: Optional[ArrayLike] = None,
@@ -583,20 +698,18 @@
         passed to Trimesh to create box
 
     Returns
     ------------
     geometry : trimesh.Trimesh
       Mesh of a cuboid
     """
-    # vertices of the cube
-    vertices = np.array(
-        [0, 0, 0, 0, 0, 1, 0, 1, 0, 0, 1, 1, 1, 0, 0, 1, 0, 1, 1, 1, 0, 1, 1, 1],
-        order="C",
-        dtype=np.float64,
-    ).reshape((-1, 3))
+    # vertices of the cube from reference
+    vertices = np.array(_data["box"]["vertices"], order="C", dtype=np.float64)
+    faces = np.array(_data["box"]["faces"], order="C", dtype=np.int64)
+    face_normals = np.array(_data["box"]["face_normals"], order="C", dtype=np.float64)
 
     # resize cube based on passed extents
     if bounds is not None:
         if transform is not None or extents is not None:
             raise ValueError("`bounds` overrides `extents`/`transform`!")
         bounds = np.array(bounds, dtype=np.float64)
         if bounds.shape != (2, 3):
@@ -610,96 +723,14 @@
             raise ValueError("Extents must be (3,)!")
         vertices -= 0.5
         vertices *= extents
     else:
         vertices -= 0.5
         extents = np.asarray((1.0, 1.0, 1.0), dtype=np.float64)
 
-    # hardcoded face indices
-    # TODO : make less lol?
-    faces = [
-        1,
-        3,
-        0,
-        4,
-        1,
-        0,
-        0,
-        3,
-        2,
-        2,
-        4,
-        0,
-        1,
-        7,
-        3,
-        5,
-        1,
-        4,
-        5,
-        7,
-        1,
-        3,
-        7,
-        2,
-        6,
-        4,
-        2,
-        2,
-        7,
-        6,
-        6,
-        5,
-        4,
-        7,
-        5,
-        6,
-    ]
-    faces = np.array(faces, order="C", dtype=np.int64).reshape((-1, 3))
-
-    face_normals = [
-        -1,
-        0,
-        0,
-        0,
-        -1,
-        0,
-        -1,
-        0,
-        0,
-        0,
-        0,
-        -1,
-        0,
-        0,
-        1,
-        0,
-        -1,
-        0,
-        0,
-        0,
-        1,
-        0,
-        1,
-        0,
-        0,
-        0,
-        -1,
-        0,
-        1,
-        0,
-        1,
-        0,
-        0,
-        1,
-        0,
-        0,
-    ]
-    face_normals = np.asanyarray(face_normals, order="C", dtype=np.float64).reshape(-1, 3)
-
     if "metadata" not in kwargs:
         kwargs["metadata"] = {}
     kwargs["metadata"].update({"shape": "box", "extents": extents})
 
     box = Trimesh(
         vertices=vertices, faces=faces, face_normals=face_normals, process=False, **kwargs
     )
@@ -721,119 +752,17 @@
       Passed through to `Trimesh` constructor.
 
     Returns
     -------------
     ico : trimesh.Trimesh
       Icosahederon centered at the origin.
     """
-    t = (1.0 + 5.0**0.5) / 2.0
-    vertices = [
-        -1,
-        t,
-        0,
-        1,
-        t,
-        0,
-        -1,
-        -t,
-        0,
-        1,
-        -t,
-        0,
-        0,
-        -1,
-        t,
-        0,
-        1,
-        t,
-        0,
-        -1,
-        -t,
-        0,
-        1,
-        -t,
-        t,
-        0,
-        -1,
-        t,
-        0,
-        1,
-        -t,
-        0,
-        -1,
-        -t,
-        0,
-        1,
-    ]
-    faces = [
-        0,
-        11,
-        5,
-        0,
-        5,
-        1,
-        0,
-        1,
-        7,
-        0,
-        7,
-        10,
-        0,
-        10,
-        11,
-        1,
-        5,
-        9,
-        5,
-        11,
-        4,
-        11,
-        10,
-        2,
-        10,
-        7,
-        6,
-        7,
-        1,
-        8,
-        3,
-        9,
-        4,
-        3,
-        4,
-        2,
-        3,
-        2,
-        6,
-        3,
-        6,
-        8,
-        3,
-        8,
-        9,
-        4,
-        9,
-        5,
-        2,
-        4,
-        11,
-        6,
-        2,
-        10,
-        8,
-        6,
-        7,
-        9,
-        8,
-        1,
-    ]
-    # scale vertices so each vertex radius is 1.0
-    vertices = np.reshape(vertices, (-1, 3)) / np.sqrt(2.0 + t)
-    faces = np.reshape(faces, (-1, 3))
-
+    # get stored pre-baked primitive values
+    vertices = np.array(_data["icosahedron"]["vertices"], dtype=np.float64)
+    faces = np.array(_data["icosahedron"]["faces"], dtype=np.int64)
     return Trimesh(
         vertices=vertices, faces=faces, process=kwargs.pop("process", False), **kwargs
     )
 
 
 def icosphere(subdivisions: Integer = 3, radius: Number = 1.0, **kwargs):
     """
```

### Comparing `trimesh-4.2.4/trimesh/curvature.py` & `trimesh-4.3.0/trimesh/curvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/decomposition.py` & `trimesh-4.3.0/trimesh/decomposition.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exceptions.py` & `trimesh-4.3.0/trimesh/exceptions.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/binvox.py` & `trimesh-4.3.0/trimesh/exchange/binvox.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/cascade.py` & `trimesh-4.3.0/trimesh/exchange/cascade.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/dae.py` & `trimesh-4.3.0/trimesh/exchange/dae.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/export.py` & `trimesh-4.3.0/trimesh/exchange/export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/gltf.py` & `trimesh-4.3.0/trimesh/exchange/gltf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/load.py` & `trimesh-4.3.0/trimesh/exchange/load.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/misc.py` & `trimesh-4.3.0/trimesh/exchange/misc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/obj.py` & `trimesh-4.3.0/trimesh/exchange/obj.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/off.py` & `trimesh-4.3.0/trimesh/exchange/off.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/ply.py` & `trimesh-4.3.0/trimesh/exchange/ply.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/stl.py` & `trimesh-4.3.0/trimesh/exchange/stl.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/threedxml.py` & `trimesh-4.3.0/trimesh/exchange/threedxml.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/threemf.py` & `trimesh-4.3.0/trimesh/exchange/threemf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/urdf.py` & `trimesh-4.3.0/trimesh/exchange/urdf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/xaml.py` & `trimesh-4.3.0/trimesh/exchange/xaml.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/exchange/xyz.py` & `trimesh-4.3.0/trimesh/exchange/xyz.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/geometry.py` & `trimesh-4.3.0/trimesh/geometry.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/graph.py` & `trimesh-4.3.0/trimesh/graph.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/grouping.py` & `trimesh-4.3.0/trimesh/grouping.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/inertia.py` & `trimesh-4.3.0/trimesh/inertia.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/interfaces/blender.py` & `trimesh-4.3.0/trimesh/interfaces/blender.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/interfaces/generic.py` & `trimesh-4.3.0/trimesh/interfaces/generic.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/interfaces/gmsh.py` & `trimesh-4.3.0/trimesh/interfaces/gmsh.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,44 @@
+import os
 import tempfile
+import warnings
 
 import numpy as np
 
+from ..constants import log
+from ..typed import Integer, Number, Optional
+
+# the old `gmsh-sdk` package is deprecated and
+# has a different incompatible API!
+_min_gmsh = (4, 12, 1)
+
+
+_warning = " ".join(
+    [
+        "`trimesh.interfaces.gmsh` is deprecated and will be removed January 2025!",
+        "There are *many* gmsh options on PyPi: `scikit-gmsh` `gmsh` `pygmsh` `gmsh-sdk`,",
+        "users should pick one of those and use it directly. If STEP loading is the only",
+        "thing needed you may want `pip install cascadio` which uses OpenCASCADE more",
+        "directly and will immediatly enable STEP as a loadable format in trimesh.",
+    ]
+)
+
 
 def load_gmsh(file_name, gmsh_args=None):
     """
     Returns a surface mesh from CAD model in Open Cascade
     Breap (.brep), Step (.stp or .step) and Iges formats
     Or returns a surface mesh from 3D volume mesh using gmsh.
 
     For a list of possible options to pass to GMSH, check:
     http://gmsh.info/doc/texinfo/gmsh.html
 
-    An easy way to install the GMSH SDK is through the `gmsh-sdk`
+    An easy way to install the GMSH SDK is through the `gmsh`
     package on PyPi, which downloads and sets up gmsh:
-        >>> pip install gmsh-sdk
+        >>> pip install gmsh
 
     Parameters
     --------------
     file_name : str
       Location of the file to be imported
     gmsh_args : (n, 2) list
       List of (parameter, value) pairs to be passed to
@@ -27,18 +47,27 @@
       Maximum length of an element in the volume mesh
 
     Returns
     ------------
     mesh : trimesh.Trimesh
       Surface mesh of input geometry
     """
+    warnings.warn(_warning, category=DeprecationWarning, stacklevel=2)
+
     # use STL as an intermediate format
     # do import here to avoid very occasional segfaults
     import gmsh
 
+    # the deprecated `pip install gmsh-sdk` package has an entirely different API
+    # require a minimum version here
+    if tuple(int(i) for i in gmsh.__version__.split(".")) < _min_gmsh:
+        raise ImportError(
+            f"`gmsh.__version__ < {_min_gmsh}`: run `pip install --upgrade gmsh`"
+        )
+
     from ..exchange.stl import load_stl
 
     # start with default args for the meshing step
     # Mesh.Algorithm=2 MeshAdapt/Delaunay, there are others but they may include quads
     # With this planes are meshed using Delaunay and cylinders are meshed
     # using MeshAdapt
     args = [
@@ -71,17 +100,27 @@
                 "Supported formats are: BREP (.brep), STEP (.stp or .step), "
                 + "IGES (.igs or .iges), Nastran (.bdf), Gmsh (.msh), Abaqus (*.inp), "
                 + "Diffpack (*.diff), Inria Medit (*.mesh)"
             )
     else:
         raise ValueError("No import since no file was provided!")
 
-    # if we initialize with sys.argv it could be anything
-    if not gmsh.isInitialized():
+    # hmmm
+    init = False
+    try:
+        if hasattr(gmsh, "isInitialized"):
+            init = gmsh.isInitialized()
+        elif hasattr(gmsh, "is_initialized"):
+            init = gmsh.is_initialized()
+    except BaseException:
+        log.debug("gmsh unexpected", exc_info=True)
+
+    if not init:
         gmsh.initialize()
+
     gmsh.option.setNumber("General.Terminal", 1)
     gmsh.model.add("Surface_Mesh_Generation")
     # loop through our numbered args which do things, stuff
     for arg in args:
         gmsh.option.setNumber(*arg)
 
     gmsh.open(file_name)
@@ -110,21 +149,27 @@
         kwargs = load_stl(f)
 
     gmsh.finalize()
 
     return kwargs
 
 
-def to_volume(mesh, file_name=None, max_element=None, mesher_id=1):
+def to_volume(
+    mesh,
+    file_name: Optional[str] = None,
+    file_type: Optional[str] = None,
+    max_element: Optional[Number] = None,
+    mesher_id: Integer = 1,
+) -> bytes:
     """
     Convert a surface mesh to a 3D volume mesh generated by gmsh.
 
-    An easy way to install the gmsh sdk is through the gmsh-sdk
+    An easy way to install the gmsh sdk is through the gmsh
     package on pypi, which downloads and sets up gmsh:
-        pip install gmsh-sdk
+        pip install gmsh
 
     Algorithm details, although check gmsh docs for more information:
     The "Delaunay" algorithm is split into three separate steps.
     First, an initial mesh of the union of all the volumes in the model is performed,
     without inserting points in the volume. The surface mesh is then recovered using H.
     Si's boundary recovery algorithm Tetgen/BR. Then a three-dimensional version of the
     2D Delaunay algorithm described above is applied to insert points in the volume to
@@ -137,92 +182,99 @@
     anisotropic tetrahedralizations
 
 
     Parameters
     --------------
     mesh : trimesh.Trimesh
       Surface mesh of input geometry
-    file_name : str or None
+    file_type
       Location to save output, in .msh (gmsh) or .bdf (Nastran) format
     max_element : float or None
       Maximum length of an element in the volume mesh
     mesher_id : int
       3D unstructured algorithms:
       1: Delaunay, 3: Initial mesh only, 4: Frontal, 7: MMG3D, 9: R-tree, 10: HXT
 
     Returns
     ------------
     data : None or bytes
       MSH data, only returned if file_name is None
 
     """
+    warnings.warn(_warning, category=DeprecationWarning, stacklevel=2)
+
     # do import here to avoid very occasional segfaults
     import gmsh
 
+    if tuple(int(i) for i in gmsh.__version__.split(".")) < _min_gmsh:
+        raise ImportError(
+            f"`gmsh.__version__ < {_min_gmsh}`: run `pip install --upgrade gmsh`"
+        )
+
     # checks mesher selection
     if mesher_id not in [1, 3, 4, 7, 9, 10]:
         raise ValueError("unavailable mesher selected!")
     else:
         mesher_id = int(mesher_id)
 
     # set max element length to a best guess if not specified
     if max_element is None:
         max_element = np.sqrt(np.mean(mesh.area_faces))
 
     if file_name is not None:
-        # check extensions to make sure it is supported format
-        if not any(
-            file_name.lower().endswith(e)
-            for e in [".bdf", ".msh", ".inp", ".diff", ".mesh"]
-        ):
-            raise ValueError(
-                "Only Nastran (.bdf), Gmsh (.msh), Abaqus (*.inp), "
-                + "Diffpack (*.diff) and Inria Medit (*.mesh) formats "
-                + "are available!"
-            )
+        file_type = file_name.split(".")[-1].lower()
+    elif file_type is not None:
+        file_type = file_type.lower().strip(".")
+    else:
+        file_type = "msh"
 
-    # exports to disk for gmsh to read using a temp file
-    mesh_file = tempfile.NamedTemporaryFile(suffix=".stl", delete=False)
-    mesh_file.close()
-    mesh.export(mesh_file.name)
+    if file_type not in ["bdf", "msh", "inp", "diff", "mesh"]:
+        raise ValueError(
+            "Only Nastran (`bdf`), Gmsh (`msh`), Abaqus (`inp`), "
+            + "Diffpack (`diff`) and Inria Medit (`mesh`) formats "
+            + "are available!"
+        )
+
+    # use a temporary directory for input and output
+    with tempfile.TemporaryDirectory() as D:
+        mesh_file = os.path.join(D, "input.stl")
+        mesh.export(mesh_file)
 
-    # starts Gmsh Python API script
-    gmsh.initialize()
-    gmsh.option.setNumber("General.Terminal", 1)
-    gmsh.model.add("Nastran_stl")
+        # starts Gmsh Python API script
+        gmsh.initialize()
+        gmsh.option.setNumber("General.Terminal", 1)
+        gmsh.model.add("Nastran_stl")
 
-    gmsh.merge(mesh_file.name)
-    dimtag = gmsh.model.getEntities()[0]
-    dim = dimtag[0]
-    tag = dimtag[1]
-
-    surf_loop = gmsh.model.geo.addSurfaceLoop([tag])
-    gmsh.model.geo.addVolume([surf_loop])
-    gmsh.model.geo.synchronize()
-
-    # We can then generate a 3D mesh...
-    gmsh.option.setNumber("Mesh.Algorithm3D", mesher_id)
-    gmsh.option.setNumber("Mesh.CharacteristicLengthMax", max_element)
-    gmsh.model.mesh.generate(3)
-
-    dimtag2 = gmsh.model.getEntities()[1]
-    dim2 = dimtag2[0]
-    tag2 = dimtag2[1]
-    p2 = gmsh.model.addPhysicalGroup(dim2, [tag2])
-    gmsh.model.setPhysicalName(dim, p2, "Nastran_bdf")
-
-    data = None
-    # if file name is None, return msh data using a tempfile
-    if file_name is None:
-        out_data = tempfile.NamedTemporaryFile(suffix=".msh", delete=False)
-        # windows gets mad if two processes try to open the same file
-        out_data.close()
-        gmsh.write(out_data.name)
-        with open(out_data.name, "rb") as f:
+        gmsh.merge(mesh_file)
+        dimtag = gmsh.model.getEntities()[0]
+        dim = dimtag[0]
+        tag = dimtag[1]
+
+        surf_loop = gmsh.model.geo.addSurfaceLoop([tag])
+        gmsh.model.geo.addVolume([surf_loop])
+        gmsh.model.geo.synchronize()
+
+        # We can then generate a 3D mesh...
+        gmsh.option.setNumber("Mesh.Algorithm3D", mesher_id)
+        gmsh.option.setNumber("Mesh.CharacteristicLengthMax", max_element)
+        gmsh.model.mesh.generate(3)
+
+        dimtag2 = gmsh.model.getEntities()[1]
+        dim2 = dimtag2[0]
+        tag2 = dimtag2[1]
+        p2 = gmsh.model.addPhysicalGroup(dim2, [tag2])
+        gmsh.model.setPhysicalName(dim, p2, "Nastran_bdf")
+
+        out_path = os.path.join(D, f"temp.{file_type}")
+        gmsh.write(out_path)
+        with open(out_path, "rb") as f:
             data = f.read()
-    else:
-        gmsh.write(file_name)
 
     # close up shop
     gmsh.finalize()
 
+    # write the data
+    if file_name is not None:
+        with open(os.path.abspath(os.path.expanduser(file_name)), "wb") as f:
+            f.write(data)
+
     return data
```

### Comparing `trimesh-4.2.4/trimesh/intersections.py` & `trimesh-4.3.0/trimesh/intersections.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/interval.py` & `trimesh-4.3.0/trimesh/interval.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/nsphere.py` & `trimesh-4.3.0/trimesh/nsphere.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/parent.py` & `trimesh-4.3.0/trimesh/parent.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/arc.py` & `trimesh-4.3.0/trimesh/path/arc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/creation.py` & `trimesh-4.3.0/trimesh/path/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/curve.py` & `trimesh-4.3.0/trimesh/path/curve.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/entities.py` & `trimesh-4.3.0/trimesh/path/entities.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/exchange/dxf.py` & `trimesh-4.3.0/trimesh/path/exchange/dxf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/exchange/export.py` & `trimesh-4.3.0/trimesh/path/exchange/export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/exchange/load.py` & `trimesh-4.3.0/trimesh/path/exchange/load.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/exchange/misc.py` & `trimesh-4.3.0/trimesh/path/exchange/misc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/exchange/svg_io.py` & `trimesh-4.3.0/trimesh/path/exchange/svg_io.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/intersections.py` & `trimesh-4.3.0/trimesh/path/intersections.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/packing.py` & `trimesh-4.3.0/trimesh/path/packing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/path.py` & `trimesh-4.3.0/trimesh/path/path.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/polygons.py` & `trimesh-4.3.0/trimesh/path/polygons.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/raster.py` & `trimesh-4.3.0/trimesh/path/raster.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/repair.py` & `trimesh-4.3.0/trimesh/path/repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/segments.py` & `trimesh-4.3.0/trimesh/path/segments.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/simplify.py` & `trimesh-4.3.0/trimesh/path/simplify.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/traversal.py` & `trimesh-4.3.0/trimesh/path/traversal.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/path/util.py` & `trimesh-4.3.0/trimesh/path/util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/permutate.py` & `trimesh-4.3.0/trimesh/permutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/points.py` & `trimesh-4.3.0/trimesh/points.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/poses.py` & `trimesh-4.3.0/trimesh/poses.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/primitives.py` & `trimesh-4.3.0/trimesh/primitives.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/proximity.py` & `trimesh-4.3.0/trimesh/proximity.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/ray/ray_pyembree.py` & `trimesh-4.3.0/trimesh/ray/ray_pyembree.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/ray/ray_triangle.py` & `trimesh-4.3.0/trimesh/ray/ray_triangle.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/ray/ray_util.py` & `trimesh-4.3.0/trimesh/ray/ray_util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/registration.py` & `trimesh-4.3.0/trimesh/registration.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/remesh.py` & `trimesh-4.3.0/trimesh/remesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/rendering.py` & `trimesh-4.3.0/trimesh/rendering.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/repair.py` & `trimesh-4.3.0/trimesh/repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resolvers.py` & `trimesh-4.3.0/trimesh/resolvers.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/__init__.py` & `trimesh-4.3.0/trimesh/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/schema/gltf2.schema.zip` & `trimesh-4.3.0/trimesh/resources/schema/gltf2.schema.zip`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/schema/primitive/box.schema.json` & `trimesh-4.3.0/trimesh/resources/schema/primitive/box.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/schema/primitive/capsule.schema.json` & `trimesh-4.3.0/trimesh/resources/schema/primitive/capsule.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/schema/primitive/cylinder.schema.json` & `trimesh-4.3.0/trimesh/resources/schema/primitive/cylinder.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/schema/primitive/extrusion.schema.json` & `trimesh-4.3.0/trimesh/resources/schema/primitive/extrusion.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/schema/primitive/scenegraph.schema.json` & `trimesh-4.3.0/trimesh/resources/schema/primitive/scenegraph.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/schema/primitive/sphere.schema.json` & `trimesh-4.3.0/trimesh/resources/schema/primitive/sphere.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/schema/primitive/trimesh.schema.json` & `trimesh-4.3.0/trimesh/resources/schema/primitive/trimesh.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/schema/urdf.xsd` & `trimesh-4.3.0/trimesh/resources/schema/urdf.xsd`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/templates/blender_boolean.py.tmpl` & `trimesh-4.3.0/trimesh/resources/templates/blender_boolean.py.tmpl`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/templates/blender_unwrap.py.template` & `trimesh-4.3.0/trimesh/resources/templates/blender_unwrap.py.template`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/templates/dxf.json` & `trimesh-4.3.0/trimesh/resources/templates/dxf.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/templates/viewer.zip` & `trimesh-4.3.0/trimesh/resources/templates/viewer.zip`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/resources/units_to_inches.json` & `trimesh-4.3.0/trimesh/resources/units_to_inches.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/sample.py` & `trimesh-4.3.0/trimesh/sample.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/scene/cameras.py` & `trimesh-4.3.0/trimesh/scene/cameras.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/scene/lighting.py` & `trimesh-4.3.0/trimesh/scene/lighting.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/scene/scene.py` & `trimesh-4.3.0/trimesh/scene/scene.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/scene/transforms.py` & `trimesh-4.3.0/trimesh/scene/transforms.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/schemas.py` & `trimesh-4.3.0/trimesh/schemas.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/smoothing.py` & `trimesh-4.3.0/trimesh/smoothing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/transformations.py` & `trimesh-4.3.0/trimesh/transformations.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,15 @@
 >>> v2 = np.dot(v0, M[:3,:3].T)
 >>> np.allclose(unit_vector(v1), unit_vector(v2))
 True
 
 """
 
 import numpy as np
+from numpy.typing import ArrayLike, NDArray
 
 _IDENTITY = np.eye(4)
 _IDENTITY.flags["WRITEABLE"] = False
 
 
 def identity_matrix():
     """Return 4x4 identity/unit matrix.
@@ -224,18 +225,28 @@
     >>> v = np.random.random(3) - 0.5
     >>> np.allclose(v, translation_matrix(v)[:3, 3])
     True
 
     """
     # are we 2D or 3D
     dim = len(direction)
+
     # start with identity matrix
-    M = np.identity(dim + 1)
+
+    if any("sympy" in str(type(v)) for v in direction):
+        # if we have been passed input values as sympy.Symbol
+        from sympy import eye
+
+        M = eye(dim + 1)
+    else:
+        M = np.eye(dim + 1)
+
     # apply the offset
     M[:dim, dim] = direction[:dim]
+
     return M
 
 
 def translation_from_matrix(matrix):
     """Return translation vector from translation matrix.
 
     >>> v0 = np.random.random(3) - 0.5
@@ -340,27 +351,28 @@
     >>> I = np.identity(4, np.float64)
     >>> np.allclose(I, rotation_matrix(np.pi*2, direc))
     True
     >>> np.allclose(2, np.trace(rotation_matrix(np.pi/2,direc,point)))
     True
 
     """
-    if type(angle).__name__ == "Symbol":
+    if "sympy" in str(type(angle)):
         # special case sympy symbolic angles
         import sympy as sp
 
         symbolic = True
         sina = sp.sin(angle)
         cosa = sp.cos(angle)
     else:
         symbolic = False
         sina = np.sin(angle)
         cosa = np.cos(angle)
 
     direction = unit_vector(direction[:3])
+
     # rotation matrix around unit vector
     M = np.diag([cosa, cosa, cosa, 1.0])
     M[:3, :3] += np.outer(direction, direction) * (1.0 - cosa)
 
     direction = direction * sina
     M[:3, :3] += np.array(
         [
@@ -1120,15 +1132,15 @@
     k = _NEXT_AXIS[i - parity + 1]
 
     if frame:
         ai, ak = ak, ai
     if parity:
         ai, aj, ak = -ai, -aj, -ak
 
-    if type(ai).__name__ == "Symbol":
+    if "sympy" in str(type(ai)):
         # if we have been passed input values as sympy.Symbol
         # use symbolic cosine and identity matrix
         from sympy import cos, eye, sin
 
         M = eye(4)
     else:
         sin, cos = np.sin, np.cos
@@ -2127,15 +2139,17 @@
                 np.dot(matrix, [0,0,1,0])
 
     """
     result = euler_matrix(0.0, phi, theta, axes=axes)
     return result
 
 
-def transform_points(points, matrix, translate=True):
+def transform_points(
+    points: ArrayLike, matrix: ArrayLike, translate: bool = True
+) -> NDArray[np.float64]:
     """
     Returns points rotated by a homogeneous
     transformation matrix.
 
     If points are (n, 2) matrix must be (3, 3)
     If points are (n, 3) matrix must be (4, 4)
```

### Comparing `trimesh-4.2.4/trimesh/triangles.py` & `trimesh-4.3.0/trimesh/triangles.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/typed.py` & `trimesh-4.3.0/trimesh/typed.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/units.py` & `trimesh-4.3.0/trimesh/units.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/util.py` & `trimesh-4.3.0/trimesh/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -466,15 +466,15 @@
     spherical = np.zeros((len(cartesian), 2), dtype=np.float64)
     spherical[valid] = np.column_stack((np.arctan2(y, x), np.arccos(z)))
     return spherical
 
 
 def spherical_to_vector(spherical):
     """
-    Convert a set of (n, 2) spherical vectors to (n, 3) vectors
+    Convert an array of `(n, 2)` spherical angles to `(n, 3)` unit vectors.
 
     Parameters
     ------------
     spherical : (n , 2) float
        Angles, in radians
 
     Returns
@@ -485,16 +485,15 @@
     spherical = np.asanyarray(spherical, dtype=np.float64)
     if not is_shape(spherical, (-1, 2)):
         raise ValueError("spherical coordinates must be (n, 2)!")
 
     theta, phi = spherical.T
     st, ct = np.sin(theta), np.cos(theta)
     sp, cp = np.sin(phi), np.cos(phi)
-    vectors = np.column_stack((ct * sp, st * sp, cp))
-    return vectors
+    return np.column_stack((ct * sp, st * sp, cp))
 
 
 def pairwise(iterable):
     """
     For an iterable, group values into pairs.
 
     Parameters
```

### Comparing `trimesh-4.2.4/trimesh/version.py` & `trimesh-4.3.0/trimesh/version.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/viewer/__init__.py` & `trimesh-4.3.0/trimesh/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/viewer/notebook.py` & `trimesh-4.3.0/trimesh/viewer/notebook.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/viewer/trackball.py` & `trimesh-4.3.0/trimesh/viewer/trackball.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/viewer/widget.py` & `trimesh-4.3.0/trimesh/viewer/widget.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/viewer/windowed.py` & `trimesh-4.3.0/trimesh/viewer/windowed.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/visual/__init__.py` & `trimesh-4.3.0/trimesh/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/visual/base.py` & `trimesh-4.3.0/trimesh/visual/base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/visual/color.py` & `trimesh-4.3.0/trimesh/visual/color.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/visual/gloss.py` & `trimesh-4.3.0/trimesh/visual/gloss.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/visual/material.py` & `trimesh-4.3.0/trimesh/visual/material.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/visual/objects.py` & `trimesh-4.3.0/trimesh/visual/objects.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/visual/texture.py` & `trimesh-4.3.0/trimesh/visual/texture.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
                 masks[i][f] = a
             # find the most commonly occurring attribute (i.e. UV coordinate)
             # and use that index note that this is doing a float conversion
             # and then median before converting back to int: could also do this as
             # a column diff and sort but this seemed easier and is fast enough
             # turn default attribute value of -1 to nan before median computation
             # and use nanmedian to compute the median ignoring the nan values
-            masks_nan = np.where(masks != -1, masks, np.NaN)
+            masks_nan = np.where(masks != -1, masks, np.nan)
             result.append(np.nanmedian(masks_nan, axis=0).astype(np.int64))
 
         return result
 
     # stack into pairs of (vertex index, texture index)
     stackable = [np.asanyarray(faces).reshape(-1)]
     # append multiple args to the correlated stack
```

### Comparing `trimesh-4.2.4/trimesh/voxel/base.py` & `trimesh-4.3.0/trimesh/voxel/base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/voxel/creation.py` & `trimesh-4.3.0/trimesh/voxel/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/voxel/encoding.py` & `trimesh-4.3.0/trimesh/voxel/encoding.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/voxel/morphology.py` & `trimesh-4.3.0/trimesh/voxel/morphology.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/voxel/ops.py` & `trimesh-4.3.0/trimesh/voxel/ops.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/voxel/runlength.py` & `trimesh-4.3.0/trimesh/voxel/runlength.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh/voxel/transforms.py` & `trimesh-4.3.0/trimesh/voxel/transforms.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.2.4/trimesh.egg-info/PKG-INFO` & `trimesh-4.3.0/trimesh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimesh
-Version: 4.2.4
+Version: 4.3.0
 Summary: Import, export, process, analyze and view triangular meshes.
 Author-email: Michael Dawson-Haggerty <mikedh@kerfed.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Michael Dawson-Haggerty
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,14 +75,15 @@
 Requires-Dist: cascadio; extra == "recommend"
 Requires-Dist: manifold3d>=2.3.0; extra == "recommend"
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coveralls; extra == "test"
 Requires-Dist: pyright; extra == "test"
 Requires-Dist: ezdxf; extra == "test"
+Requires-Dist: gmsh>=4.12.1; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pymeshlab; extra == "test"
 Requires-Dist: pyinstrument; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: pytest-beartype; python_version >= "3.10" and extra == "test"
 Provides-Extra: all
```

### Comparing `trimesh-4.2.4/trimesh.egg-info/SOURCES.txt` & `trimesh-4.3.0/trimesh.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 tests/test_simplify.py
 tests/test_smooth.py
 tests/test_smoothing.py
 tests/test_splines.py
 tests/test_step.py
 tests/test_stl.py
 tests/test_svg.py
+tests/test_sweep.py
 tests/test_texture.py
 tests/test_thickness.py
 tests/test_trackball.py
 tests/test_transformations.py
 tests/test_triangles.py
 tests/test_typed.py
 tests/test_units.py
@@ -191,14 +192,15 @@
 trimesh/path/exchange/misc.py
 trimesh/path/exchange/svg_io.py
 trimesh/ray/__init__.py
 trimesh/ray/ray_pyembree.py
 trimesh/ray/ray_triangle.py
 trimesh/ray/ray_util.py
 trimesh/resources/__init__.py
+trimesh/resources/creation.json
 trimesh/resources/units_to_inches.json
 trimesh/resources/schema/README.md
 trimesh/resources/schema/gltf2.schema.zip
 trimesh/resources/schema/urdf.xsd
 trimesh/resources/schema/primitive/box.schema.json
 trimesh/resources/schema/primitive/capsule.schema.json
 trimesh/resources/schema/primitive/cylinder.schema.json
```

