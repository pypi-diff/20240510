# Comparing `tmp/scikit-surgeryvtk-2.1.1.tar.gz` & `tmp/scikit-surgeryvtk-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-surgeryvtk-2.1.1.tar", last modified: Sat Feb 24 10:16:56 2024, max compression
+gzip compressed data, was "scikit-surgeryvtk-2.1.2.tar", last modified: Fri May 10 18:06:40 2024, max compression
```

## Comparing `scikit-surgeryvtk-2.1.1.tar` & `scikit-surgeryvtk-2.1.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.736554 scikit-surgeryvtk-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-02-24 10:16:56.736554 scikit-surgeryvtk-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.728553 scikit-surgeryvtk-2.1.1/scikit_surgeryvtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-02-24 10:16:56.000000 scikit-surgeryvtk-2.1.1/scikit_surgeryvtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-02-24 10:16:56.000000 scikit-surgeryvtk-2.1.1/scikit_surgeryvtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 10:16:56.000000 scikit-surgeryvtk-2.1.1/scikit_surgeryvtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-24 10:16:56.000000 scikit-surgeryvtk-2.1.1/scikit_surgeryvtk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-24 10:16:56.000000 scikit-surgeryvtk-2.1.1/scikit_surgeryvtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-24 10:16:56.000000 scikit-surgeryvtk-2.1.1/scikit_surgeryvtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-24 10:16:56.736554 scikit-surgeryvtk-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.736554 scikit-surgeryvtk-2.1.1/sksurgeryvtk/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-24 10:16:56.736554 scikit-surgeryvtk-2.1.1/sksurgeryvtk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.728553 scikit-surgeryvtk-2.1.1/sksurgeryvtk/camera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/camera/vtk_camera_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.728553 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/outline_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/surface_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    24905 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/voxelise.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_base_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_cylinder_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_image_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_point_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_sphere_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_surface_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_surface_model_directory_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.728553 scikit-surgeryvtk-2.1.1/sksurgeryvtk/text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/text/text_overlay.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.732553 scikit-surgeryvtk-2.1.1/sksurgeryvtk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/utils/matrix_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/utils/platform_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/utils/polydata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/utils/projection_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.732553 scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9975 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/vtk_interlaced_stereo_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/vtk_lus_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29147 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/vtk_overlay_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/vtk_rendering_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/vtk_reslice_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.724553 scikit-surgeryvtk-2.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.732553 scikit-surgeryvtk-2.1.1/tests/camera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/tests/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/tests/camera/test_liver_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-02-24 10:16:48.000000 scikit-surgeryvtk-2.1.1/tests/camera/test_vtk_camera_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.732553 scikit-surgeryvtk-2.1.1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/models/test_surface_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12732 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/models/test_voxelise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/models/test_vtk_cylinder_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/models/test_vtk_image_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/models/test_vtk_point_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/models/test_vtk_sphere_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/models/test_vtk_surface_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/models/test_vtk_surface_model_directory_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/models/test_vtk_unstructured_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.736554 scikit-surgeryvtk-2.1.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/utils/test_matrix_utills.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/utils/test_polydata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/utils/test_projection_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:56.736554 scikit-surgeryvtk-2.1.1/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/widgets/test_interlaced_stereo_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/widgets/test_lus_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15673 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/widgets/test_rendering_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/widgets/test_vtk_overlay_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/widgets/test_vtk_overlay_window_5_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/widgets/test_vtk_overlay_window_with_outlines.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/tests/widgets/test_vtk_reslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    68611 2024-02-24 10:16:49.000000 scikit-surgeryvtk-2.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.622861 scikit-surgeryvtk-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-10 18:06:40.622861 scikit-surgeryvtk-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.610861 scikit-surgeryvtk-2.1.2/scikit_surgeryvtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-10 18:06:40.000000 scikit-surgeryvtk-2.1.2/scikit_surgeryvtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-10 18:06:40.000000 scikit-surgeryvtk-2.1.2/scikit_surgeryvtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 18:06:40.000000 scikit-surgeryvtk-2.1.2/scikit_surgeryvtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 18:06:40.000000 scikit-surgeryvtk-2.1.2/scikit_surgeryvtk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 18:06:40.000000 scikit-surgeryvtk-2.1.2/scikit_surgeryvtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 18:06:40.000000 scikit-surgeryvtk-2.1.2/scikit_surgeryvtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-10 18:06:40.622861 scikit-surgeryvtk-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.622861 scikit-surgeryvtk-2.1.2/sksurgeryvtk/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-10 18:06:40.622861 scikit-surgeryvtk-2.1.2/sksurgeryvtk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.614861 scikit-surgeryvtk-2.1.2/sksurgeryvtk/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/camera/vtk_camera_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.614861 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/outline_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/surface_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24905 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/voxelise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_base_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_cylinder_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_image_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_point_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_sphere_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_surface_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_surface_model_directory_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.614861 scikit-surgeryvtk-2.1.2/sksurgeryvtk/text/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/text/text_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.614861 scikit-surgeryvtk-2.1.2/sksurgeryvtk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/utils/matrix_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/utils/platform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/utils/polydata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/utils/projection_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.618861 scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9975 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/vtk_interlaced_stereo_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/vtk_lus_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29638 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/vtk_overlay_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/vtk_rendering_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/vtk_reslice_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.610861 scikit-surgeryvtk-2.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.618861 scikit-surgeryvtk-2.1.2/tests/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/tests/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/tests/camera/test_liver_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-05-10 18:06:29.000000 scikit-surgeryvtk-2.1.2/tests/camera/test_vtk_camera_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.618861 scikit-surgeryvtk-2.1.2/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/models/test_surface_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12732 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/models/test_voxelise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/models/test_vtk_cylinder_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/models/test_vtk_image_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/models/test_vtk_point_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/models/test_vtk_sphere_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/models/test_vtk_surface_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/models/test_vtk_surface_model_directory_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/models/test_vtk_unstructured_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.618861 scikit-surgeryvtk-2.1.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/utils/test_matrix_utills.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/utils/test_polydata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/utils/test_projection_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:40.622861 scikit-surgeryvtk-2.1.2/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/widgets/test_interlaced_stereo_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/widgets/test_lus_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15673 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/widgets/test_rendering_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/widgets/test_vtk_overlay_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/widgets/test_vtk_overlay_window_5_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/widgets/test_vtk_overlay_window_with_outlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/tests/widgets/test_vtk_reslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68611 2024-05-10 18:06:30.000000 scikit-surgeryvtk-2.1.2/versioneer.py
```

### Comparing `scikit-surgeryvtk-2.1.1/LICENSE` & `scikit-surgeryvtk-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/PKG-INFO` & `scikit-surgeryvtk-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-surgeryvtk
-Version: 2.1.1
+Version: 2.1.2
 Summary: scikit-surgeryvtk implements VTK for Image Guided Surgery applications
 Home-page: https://github.com/SciKit-Surgery/scikit-surgeryvtk
 Author: Thomas Dowrick
 Author-email: t.dowrick@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgeryvtk
         ===============================
```

### Comparing `scikit-surgeryvtk-2.1.1/README.rst` & `scikit-surgeryvtk-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/scikit_surgeryvtk.egg-info/PKG-INFO` & `scikit-surgeryvtk-2.1.2/scikit_surgeryvtk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scikit-surgeryvtk
-Version: 2.1.1
+Version: 2.1.2
 Summary: scikit-surgeryvtk implements VTK for Image Guided Surgery applications
 Home-page: https://github.com/SciKit-Surgery/scikit-surgeryvtk
 Author: Thomas Dowrick
 Author-email: t.dowrick@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgeryvtk
         ===============================
```

### Comparing `scikit-surgeryvtk-2.1.1/scikit_surgeryvtk.egg-info/SOURCES.txt` & `scikit-surgeryvtk-2.1.2/scikit_surgeryvtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/setup.py` & `scikit-surgeryvtk-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/camera/vtk_camera_model.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/camera/vtk_camera_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/outline_render.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/outline_render.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/surface_model_loader.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/surface_model_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/voxelise.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/voxelise.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_base_actor.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_base_actor.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_base_model.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_base_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_cylinder_model.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_cylinder_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_grid_model.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_grid_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_image_model.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_image_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_point_model.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_point_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_sphere_model.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_sphere_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_surface_model.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_surface_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/models/vtk_surface_model_directory_loader.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/models/vtk_surface_model_directory_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/text/text_overlay.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/text/text_overlay.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/utils/matrix_utils.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/utils/matrix_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/utils/polydata_utils.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/utils/polydata_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/utils/projection_utils.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/utils/projection_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/vtk_interlaced_stereo_window.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/vtk_interlaced_stereo_window.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/vtk_lus_simulator.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/vtk_lus_simulator.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/vtk_overlay_window.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/vtk_overlay_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# pylint: disable=too-many-instance-attributes, no-name-in-module
+# pylint: disable=too-many-instance-attributes, no-name-in-module, too-many-statements
 # pylint:disable=super-with-arguments, too-many-arguments, line-too-long, too-many-public-methods
 
 """
 Module to provide a set of VTK renderers that can be used to create an Augmented Reality viewer.
 
 Expected usage:
 
@@ -90,14 +90,16 @@
         init_pose=False,
         reset_camera=True,
         init_widget=True,
         video_in_layer_0=True,  # For backwards compatibility, prior to 3rd Feb 2024.
         video_in_layer_2=False,  # For backwards compatibility, prior to 3rd Feb 2024.
         layer_2_video_mask=None,  # For masking in Layer 3
         use_depth_peeling=True,  # Historically, has defaulted to true.
+        layer_1_interactive=True, # For backwards compatibility, prior to 3rd Feb 2024.
+        layer_3_interactive=False # For backwards compatibility, prior to 3rd Feb 2024.
     ):
         """
         Constructs a new VTKOverlayWindow.
         """
         super(VTKOverlayWindow, self).__init__()
 
         # Take and cache/store constructor arguments.
@@ -176,14 +178,18 @@
         self.layer_0_camera = self.layer_0_renderer.GetActiveCamera()
         self.layer_0_camera.ParallelProjectionOn()
 
         # Create and setup layer 1 (VTK scene) renderer.
         self.layer_1_renderer = vtk.vtkRenderer()
         self.layer_1_renderer.SetLayer(1)
         self.layer_1_renderer.LightFollowCameraOn()
+        if layer_1_interactive:
+            self.layer_1_renderer.InteractiveOn()
+        else:
+            self.layer_1_renderer.InteractiveOff()
 
         # Create and setup layer 2 (masked video) renderer.
         self.layer_2_image_actor = vtk.vtkImageActor()
         self.layer_2_image_actor.SetInputData(self.rgba_image_importer.GetOutput())
         self.layer_2_image_actor.VisibilityOff()
         self.layer_2_renderer = vtk.vtkRenderer()
         self.layer_2_renderer.SetLayer(2)
@@ -192,14 +198,18 @@
         self.layer_2_camera = self.layer_2_renderer.GetActiveCamera()
         self.layer_2_camera.ParallelProjectionOn()
 
         # Create and setup layer 3 (VTK scene) renderer.
         self.layer_3_renderer = vtk.vtkRenderer()
         self.layer_3_renderer.SetLayer(3)
         self.layer_3_renderer.LightFollowCameraOn()
+        if layer_3_interactive:
+            self.layer_3_renderer.InteractiveOn()
+        else:
+            self.layer_3_renderer.InteractiveOff()
 
         # Create and setup layer 4 (Overlay's, like text annotations) renderer.
         self.layer_4_renderer = vtk.vtkRenderer()
         self.layer_4_renderer.SetLayer(4)
         self.layer_4_renderer.LightFollowCameraOn()
         self.layer_4_renderer.InteractiveOff()
```

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/vtk_rendering_generator.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/vtk_rendering_generator.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/sksurgeryvtk/widgets/vtk_reslice_widget.py` & `scikit-surgeryvtk-2.1.2/sksurgeryvtk/widgets/vtk_reslice_widget.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/camera/test_liver_overlay.py` & `scikit-surgeryvtk-2.1.2/tests/camera/test_liver_overlay.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/camera/test_vtk_camera_model.py` & `scikit-surgeryvtk-2.1.2/tests/camera/test_vtk_camera_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/models/test_surface_model_loader.py` & `scikit-surgeryvtk-2.1.2/tests/models/test_surface_model_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/models/test_voxelise.py` & `scikit-surgeryvtk-2.1.2/tests/models/test_voxelise.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/models/test_vtk_cylinder_model.py` & `scikit-surgeryvtk-2.1.2/tests/models/test_vtk_cylinder_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/models/test_vtk_image_model.py` & `scikit-surgeryvtk-2.1.2/tests/models/test_vtk_image_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/models/test_vtk_point_model.py` & `scikit-surgeryvtk-2.1.2/tests/models/test_vtk_point_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/models/test_vtk_sphere_model.py` & `scikit-surgeryvtk-2.1.2/tests/models/test_vtk_sphere_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/models/test_vtk_surface_model.py` & `scikit-surgeryvtk-2.1.2/tests/models/test_vtk_surface_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/models/test_vtk_surface_model_directory_loader.py` & `scikit-surgeryvtk-2.1.2/tests/models/test_vtk_surface_model_directory_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/models/test_vtk_unstructured_grid.py` & `scikit-surgeryvtk-2.1.2/tests/models/test_vtk_unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/utils/test_matrix_utills.py` & `scikit-surgeryvtk-2.1.2/tests/utils/test_matrix_utills.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/utils/test_polydata_utils.py` & `scikit-surgeryvtk-2.1.2/tests/utils/test_polydata_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/utils/test_projection_utils.py` & `scikit-surgeryvtk-2.1.2/tests/utils/test_projection_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/widgets/test_interlaced_stereo_window.py` & `scikit-surgeryvtk-2.1.2/tests/widgets/test_interlaced_stereo_window.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/widgets/test_lus_simulator.py` & `scikit-surgeryvtk-2.1.2/tests/widgets/test_lus_simulator.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/widgets/test_rendering_generator.py` & `scikit-surgeryvtk-2.1.2/tests/widgets/test_rendering_generator.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/widgets/test_vtk_overlay_window.py` & `scikit-surgeryvtk-2.1.2/tests/widgets/test_vtk_overlay_window.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/widgets/test_vtk_overlay_window_5_layers.py` & `scikit-surgeryvtk-2.1.2/tests/widgets/test_vtk_overlay_window_5_layers.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/widgets/test_vtk_overlay_window_with_outlines.py` & `scikit-surgeryvtk-2.1.2/tests/widgets/test_vtk_overlay_window_with_outlines.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/tests/widgets/test_vtk_reslice.py` & `scikit-surgeryvtk-2.1.2/tests/widgets/test_vtk_reslice.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.1.1/versioneer.py` & `scikit-surgeryvtk-2.1.2/versioneer.py`

 * *Files identical despite different names*

