# Comparing `tmp/autoarray-2024.1.27.4.tar.gz` & `tmp/autoarray-2024.5.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoarray-2024.1.27.4.tar", last modified: Sat Jan 27 19:56:35 2024, max compression
+gzip compressed data, was "autoarray-2024.5.16.0.tar", last modified: Thu May 16 09:58:00 2024, max compression
```

## Comparing `autoarray-2024.1.27.4.tar` & `autoarray-2024.5.16.0.tar`

### file list

```diff
@@ -1,321 +1,453 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.324685 autoarray-2024.1.27.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-01-27 19:56:35.324685 autoarray-2024.1.27.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.280685 autoarray-2024.1.27.4/autoarray/
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/abstract_ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.280685 autoarray-2024.1.27.4/autoarray/config/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/grids.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/logging.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.280685 autoarray-2024.1.27.4/autoarray/config/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/visualize/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/visualize/general.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/visualize/include.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/visualize/mat_wrap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/visualize/mat_wrap_1d.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/visualize/mat_wrap_2d.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/config/visualize/plots.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.280685 autoarray-2024.1.27.4/autoarray/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.284685 autoarray-2024.1.27.4/autoarray/dataset/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/abstract/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/abstract/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/abstract/w_tilde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.284685 autoarray-2024.1.27.4/autoarray/dataset/imaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/imaging/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/imaging/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/imaging/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/imaging/w_tilde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.284685 autoarray-2024.1.27.4/autoarray/dataset/interferometer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/interferometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/interferometer/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/interferometer/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/interferometer/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/interferometer/w_tilde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.284685 autoarray-2024.1.27.4/autoarray/dataset/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/mock/mock_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.284685 autoarray-2024.1.27.4/autoarray/dataset/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/plot/imaging_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/plot/interferometer_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    20528 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/dataset/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.284685 autoarray-2024.1.27.4/autoarray/fit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12800 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/fit_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/fit_imaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/fit_interferometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/fit_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.288685 autoarray-2024.1.27.4/autoarray/fit/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/mock/mock_fit_imaging.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/mock/mock_fit_interferometer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.288685 autoarray-2024.1.27.4/autoarray/fit/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11871 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/plot/fit_imaging_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/plot/fit_interferometer_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fit/plot/fit_vector_yx_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.288685 autoarray-2024.1.27.4/autoarray/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/geometry/abstract_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/geometry/geometry_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/geometry/geometry_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/geometry/geometry_2d_irregular.py
--rw-r--r--   0 runner    (1001) docker     (127)    27690 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/geometry/geometry_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.288685 autoarray-2024.1.27.4/autoarray/inversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.288685 autoarray-2024.1.27.4/autoarray/inversion/inversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37084 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.292685 autoarray-2024.1.27.4/autoarray/inversion/inversion/imaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/imaging/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    34720 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/imaging/inversion_imaging_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/imaging/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    27382 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/imaging/w_tilde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.292685 autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/lop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/w_tilde.py
--rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/inversion_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/inversion/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.292685 autoarray-2024.1.27.4/autoarray/inversion/linear_obj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/linear_obj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/linear_obj/func_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/linear_obj/linear_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/linear_obj/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/linear_obj/unique_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.292685 autoarray-2024.1.27.4/autoarray/inversion/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/mock/mock_image_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/mock/mock_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/mock/mock_inversion_imaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/mock/mock_inversion_interferometer.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/mock/mock_linear_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/mock/mock_linear_obj_func_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/mock/mock_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/mock/mock_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/mock/mock_pixelization.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/mock/mock_regularization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.296685 autoarray-2024.1.27.4/autoarray/inversion/pixelization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.296685 autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/abstract_weighted.py
--rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/hilbert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/hilbert_balanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/overlay.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.296685 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21226 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/delaunay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/mapper_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)    29131 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/mapper_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/rectangular.py
--rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/voronoi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.300685 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/delaunay.py
--rw-r--r--   0 runner    (1001) docker     (127)    23753 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/mesh_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/rectangular.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/triangulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/voronoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/voronoi_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/pixelization/pixelization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.300685 autoarray-2024.1.27.4/autoarray/inversion/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14086 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/plot/inversion_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/plot/mapper_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.300685 autoarray-2024.1.27.4/autoarray/inversion/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8892 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/adaptive_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/adaptive_brightness_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/brightness_zeroth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/constant_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/constant_zeroth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/exponential_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/gaussian_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/matern_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    15315 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/regularization_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/inversion/regularization/zeroth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.300685 autoarray-2024.1.27.4/autoarray/layout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/layout/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/layout/layout_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    14064 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/layout/region.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.304685 autoarray-2024.1.27.4/autoarray/mask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/abstract_mask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.304685 autoarray-2024.1.27.4/autoarray/mask/derive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/derive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/derive/grid_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/derive/grid_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    21875 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/derive/indexes_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/derive/mask_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    21304 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/derive/mask_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/mask_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/mask_1d_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    41571 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/mask_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    48200 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/mask_2d_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.304685 autoarray-2024.1.27.4/autoarray/mask/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mask/mock/mock_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/numba_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.304685 autoarray-2024.1.27.4/autoarray/operators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22050 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/operators/convolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.304685 autoarray-2024.1.27.4/autoarray/operators/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/operators/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/operators/mock/mock_convolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/operators/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/operators/transformer_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.308685 autoarray-2024.1.27.4/autoarray/plot/
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/abstract_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/auto_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.308685 autoarray-2024.1.27.4/autoarray/plot/get_visuals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/get_visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/get_visuals/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/get_visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/get_visuals/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.308685 autoarray-2024.1.27.4/autoarray/plot/include/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/include/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/include/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/include/one_d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/include/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.308685 autoarray-2024.1.27.4/autoarray/plot/mat_plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/mat_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/mat_plot/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/mat_plot/one_d.py
--rw-r--r--   0 runner    (1001) docker     (127)    27917 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/mat_plot/two_d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/multi_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.308685 autoarray-2024.1.27.4/autoarray/plot/visuals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/visuals/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/visuals/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.308685 autoarray-2024.1.27.4/autoarray/plot/wrap/
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.312685 autoarray-2024.1.27.4/autoarray/plot/wrap/base/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/cmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/colorbar_tickparams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/legend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/tickparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    13857 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/title.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/base/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.312685 autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/avxline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/fill_between.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/yx_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/yx_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    44375 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/segmentdata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.316685 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/array_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/border_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/grid_errorbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/grid_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/grid_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/index_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/interpolated_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/mask_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/mesh_grid_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/origin_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/parallel_overscan_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/patch_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/positions_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/serial_overscan_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/serial_prescan_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/vector_yx_quiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/voronoi_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22232 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/preloads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.316685 autoarray-2024.1.27.4/autoarray/structures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/abstract_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.320685 autoarray-2024.1.27.4/autoarray/structures/arrays/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/arrays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/arrays/array_1d_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    32718 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/arrays/array_2d_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/arrays/irregular.py
--rw-r--r--   0 runner    (1001) docker     (127)    21350 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/arrays/kernel_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14198 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/arrays/uniform_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    47027 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/arrays/uniform_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.320685 autoarray-2024.1.27.4/autoarray/structures/grids/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/grids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/grids/grid_1d_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    34337 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/grids/grid_2d_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    20066 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/grids/irregular_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    41071 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/grids/iterate_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/grids/sparse_2d_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/grids/transformed_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    18071 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/grids/uniform_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    48290 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/grids/uniform_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.320685 autoarray-2024.1.27.4/autoarray/structures/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/mesh/abstract_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/mesh/delaunay_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/mesh/rectangular_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/mesh/triangulation_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/mesh/voronoi_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.324685 autoarray-2024.1.27.4/autoarray/structures/mock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/mock/mock_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/mock/mock_structure_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.324685 autoarray-2024.1.27.4/autoarray/structures/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/plot/structure_plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)    23623 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/structure_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.324685 autoarray-2024.1.27.4/autoarray/structures/vectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/vectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/vectors/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/vectors/irregular.py
--rw-r--r--   0 runner    (1001) docker     (127)    21606 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/vectors/uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/structures/visibilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.324685 autoarray-2024.1.27.4/autoarray/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/util/cholesky_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/util/fnnls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/autoarray/util/misc_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 19:56:35.324685 autoarray-2024.1.27.4/autoarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-01-27 19:56:35.000000 autoarray-2024.1.27.4/autoarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-27 19:56:35.324685 autoarray-2024.1.27.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-01-27 19:56:28.000000 autoarray-2024.1.27.4/setup.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:00.024013 autoarray-2024.5.16.0/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.748503 autoarray-2024.5.16.0/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.810999 autoarray-2024.5.16.0/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3073 2023-10-16 17:02:45.000000 autoarray-2024.5.16.0/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      385 2022-12-02 11:50:15.000000 autoarray-2024.5.16.0/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1007 2024-05-16 09:58:00.023000 autoarray-2024.5.16.0/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       87 2022-05-03 18:33:14.000000 autoarray-2024.5.16.0/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.830000 autoarray-2024.5.16.0/autoarray/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4943 2024-05-16 09:55:27.000000 autoarray-2024.5.16.0/autoarray/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9312 2024-05-13 10:25:20.000000 autoarray-2024.5.16.0/autoarray/abstract_ndarray.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.839999 autoarray-2024.5.16.0/autoarray/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/autoarray/config/.gitignore
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      630 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/autoarray/config/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1675 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       57 2022-11-29 17:43:26.000000 autoarray-2024.5.16.0/autoarray/config/grids.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      415 2023-08-14 09:39:51.000000 autoarray-2024.5.16.0/autoarray/config/logging.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.861011 autoarray-2024.5.16.0/autoarray/config/visualize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      696 2022-12-02 11:50:15.000000 autoarray-2024.5.16.0/autoarray/config/visualize/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3465 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/config/visualize/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1412 2024-01-15 12:12:47.000000 autoarray-2024.5.16.0/autoarray/config/visualize/include.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4233 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/autoarray/config/visualize/mat_wrap.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1209 2022-12-02 11:50:15.000000 autoarray-2024.5.16.0/autoarray/config/visualize/mat_wrap_1d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4875 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/config/visualize/mat_wrap_2d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4789 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/config/visualize/plots.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.868033 autoarray-2024.5.16.0/autoarray/dataset/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/autoarray/dataset/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.876000 autoarray-2024.5.16.0/autoarray/dataset/abstract/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/dataset/abstract/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10760 2024-05-15 19:41:20.000000 autoarray-2024.5.16.0/autoarray/dataset/abstract/dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1750 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/autoarray/dataset/abstract/w_tilde.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1548 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/dataset/dataset_model.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.884999 autoarray-2024.5.16.0/autoarray/dataset/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/dataset/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17613 2024-05-10 14:36:59.000000 autoarray-2024.5.16.0/autoarray/dataset/imaging/dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5663 2024-04-29 15:20:48.000000 autoarray-2024.5.16.0/autoarray/dataset/imaging/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1839 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/dataset/imaging/w_tilde.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.898001 autoarray-2024.5.16.0/autoarray/dataset/interferometer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/dataset/interferometer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11165 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/dataset/interferometer/dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3858 2024-04-29 15:20:42.000000 autoarray-2024.5.16.0/autoarray/dataset/interferometer/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2115 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/dataset/interferometer/w_tilde.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.902999 autoarray-2024.5.16.0/autoarray/dataset/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/dataset/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      337 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/dataset/mock/mock_dataset.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.911999 autoarray-2024.5.16.0/autoarray/dataset/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/dataset/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9153 2024-01-17 11:15:32.000000 autoarray-2024.5.16.0/autoarray/dataset/plot/imaging_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12213 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/dataset/plot/interferometer_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20385 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/dataset/preprocess.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3138 2023-10-20 17:11:28.000000 autoarray-2024.5.16.0/autoarray/exc.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.921999 autoarray-2024.5.16.0/autoarray/fit/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/autoarray/fit/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12815 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/fit/fit_dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2418 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/fit/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5869 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/fit/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15583 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/fit/fit_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.932000 autoarray-2024.5.16.0/autoarray/fit/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/fit/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1387 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/fit/mock/mock_fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      894 2024-05-01 14:46:48.000000 autoarray-2024.5.16.0/autoarray/fit/mock/mock_fit_interferometer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.943000 autoarray-2024.5.16.0/autoarray/fit/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/fit/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11871 2024-05-01 14:27:38.000000 autoarray-2024.5.16.0/autoarray/fit/plot/fit_imaging_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22629 2024-04-29 15:20:45.000000 autoarray-2024.5.16.0/autoarray/fit/plot/fit_interferometer_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10436 2023-06-07 16:55:31.000000 autoarray-2024.5.16.0/autoarray/fit/plot/fit_vector_yx_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14332 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.959999 autoarray-2024.5.16.0/autoarray/geometry/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/autoarray/geometry/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1065 2024-04-29 15:20:42.000000 autoarray-2024.5.16.0/autoarray/geometry/abstract_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2768 2024-04-29 15:20:41.000000 autoarray-2024.5.16.0/autoarray/geometry/geometry_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12447 2024-04-29 15:20:47.000000 autoarray-2024.5.16.0/autoarray/geometry/geometry_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1687 2023-05-11 17:33:46.000000 autoarray-2024.5.16.0/autoarray/geometry/geometry_2d_irregular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27678 2024-05-13 10:11:06.000000 autoarray-2024.5.16.0/autoarray/geometry/geometry_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.962000 autoarray-2024.5.16.0/autoarray/inversion/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-19 14:59:34.000000 autoarray-2024.5.16.0/autoarray/inversion/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:58.983999 autoarray-2024.5.16.0/autoarray/inversion/inversion/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:42.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38133 2024-05-15 16:46:48.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4178 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/dataset_interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10654 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/factory.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.002020 autoarray-2024.5.16.0/autoarray/inversion/inversion/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11945 2024-04-29 15:20:45.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/imaging/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34720 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/imaging/inversion_imaging_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12006 2024-04-29 15:20:41.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/imaging/mapping.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27385 2024-04-29 15:20:44.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/imaging/w_tilde.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.024000 autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6016 2024-04-29 15:20:39.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5655 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5331 2024-04-29 15:20:44.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/lop.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7905 2024-04-29 15:20:42.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/mapping.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9442 2024-04-29 15:20:40.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/w_tilde.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12805 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/inversion_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    42565 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/inversion_util_secret.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38687 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/inversion_util_secret_clean.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6746 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/inversion/inversion/settings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.039000 autoarray-2024.5.16.0/autoarray/inversion/linear_obj/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/inversion/linear_obj/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5036 2024-04-29 15:20:47.000000 autoarray-2024.5.16.0/autoarray/inversion/linear_obj/func_list.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7263 2024-04-29 15:20:47.000000 autoarray-2024.5.16.0/autoarray/inversion/linear_obj/linear_obj.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1859 2024-04-29 15:20:47.000000 autoarray-2024.5.16.0/autoarray/inversion/linear_obj/neighbors.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1701 2024-04-29 15:20:41.000000 autoarray-2024.5.16.0/autoarray/inversion/linear_obj/unique_mappings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.076002 autoarray-2024.5.16.0/autoarray/inversion/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/inversion/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      845 2024-04-29 15:20:46.000000 autoarray-2024.5.16.0/autoarray/inversion/mock/mock_image_mesh.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6950 2024-04-29 15:20:44.000000 autoarray-2024.5.16.0/autoarray/inversion/mock/mock_inversion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3318 2024-04-29 15:20:40.000000 autoarray-2024.5.16.0/autoarray/inversion/mock/mock_inversion_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1290 2024-04-29 15:20:38.000000 autoarray-2024.5.16.0/autoarray/inversion/mock/mock_inversion_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      888 2024-04-29 15:20:38.000000 autoarray-2024.5.16.0/autoarray/inversion/mock/mock_linear_obj.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      912 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/inversion/mock/mock_linear_obj_func_list.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2500 2024-04-29 15:20:42.000000 autoarray-2024.5.16.0/autoarray/inversion/mock/mock_mapper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1901 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/inversion/mock/mock_mesh.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1231 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/inversion/mock/mock_pixelization.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      508 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/autoarray/inversion/mock/mock_regularization.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.087000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10342 2024-04-29 15:20:39.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/border_relocator.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.109000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/image_mesh/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       88 2024-03-24 17:56:45.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/image_mesh/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9012 2024-04-29 15:20:47.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/image_mesh/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2341 2024-05-15 20:01:49.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/image_mesh/abstract_weighted.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10133 2024-05-13 10:25:20.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/image_mesh/hilbert.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4064 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/image_mesh/kmeans.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8398 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/image_mesh/overlay.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.134999 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21878 2024-05-06 13:10:25.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9457 2024-04-29 15:20:41.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/delaunay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3837 2024-05-15 19:41:18.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/factory.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4174 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/mapper_grids.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29454 2024-05-13 10:25:20.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/mapper_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6111 2024-05-06 12:44:46.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/rectangular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11929 2024-05-10 14:36:59.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/voronoi.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.162999 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2023-12-20 09:29:20.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5733 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2968 2023-12-20 09:29:20.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/delaunay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23739 2024-05-13 10:25:20.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/mesh_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6852 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/rectangular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4773 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/triangulation.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2939 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/voronoi.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2291 2023-12-20 09:29:20.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/voronoi_nn.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8508 2023-12-20 09:29:20.000000 autoarray-2024.5.16.0/autoarray/inversion/pixelization/pixelization.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.167999 autoarray-2024.5.16.0/autoarray/inversion/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/inversion/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17177 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/inversion/plot/inversion_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7049 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/inversion/plot/mapper_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.210999 autoarray-2024.5.16.0/autoarray/inversion/regularization/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      592 2024-01-26 13:57:43.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8892 2024-04-29 15:20:41.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4920 2024-04-29 15:20:38.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/adaptive_brightness.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4736 2024-04-29 15:20:40.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/adaptive_brightness_split.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5250 2024-04-29 15:20:45.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3512 2024-04-29 15:20:41.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/brightness_zeroth.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3043 2024-04-29 15:20:45.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/constant.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3215 2024-04-29 15:20:42.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/constant_split.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2185 2024-04-29 15:20:41.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/constant_zeroth.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4685 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/exponential_kernel.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4677 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/gaussian_kernel.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6521 2024-04-29 15:20:46.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/matern_kernel.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15315 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/regularization_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3082 2024-04-29 15:20:47.000000 autoarray-2024.5.16.0/autoarray/inversion/regularization/zeroth.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.221001 autoarray-2024.5.16.0/autoarray/layout/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-06-17 13:08:16.000000 autoarray-2024.5.16.0/autoarray/layout/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11364 2023-09-03 20:07:31.000000 autoarray-2024.5.16.0/autoarray/layout/layout.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7309 2024-04-29 15:20:39.000000 autoarray-2024.5.16.0/autoarray/layout/layout_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14064 2024-04-29 15:20:42.000000 autoarray-2024.5.16.0/autoarray/layout/region.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.237000 autoarray-2024.5.16.0/autoarray/mask/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/autoarray/mask/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4577 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/mask/abstract_mask.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.256008 autoarray-2024.5.16.0/autoarray/mask/derive/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-29 16:03:57.000000 autoarray-2024.5.16.0/autoarray/mask/derive/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3322 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/mask/derive/grid_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10614 2024-04-29 15:20:46.000000 autoarray-2024.5.16.0/autoarray/mask/derive/grid_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15460 2024-04-29 15:20:42.000000 autoarray-2024.5.16.0/autoarray/mask/derive/indexes_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3866 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/mask/derive/mask_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14728 2024-04-29 15:20:41.000000 autoarray-2024.5.16.0/autoarray/mask/derive/mask_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8075 2024-04-29 15:20:41.000000 autoarray-2024.5.16.0/autoarray/mask/mask_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2267 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/mask/mask_1d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38908 2024-04-29 15:20:39.000000 autoarray-2024.5.16.0/autoarray/mask/mask_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35823 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/mask/mask_2d_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.262001 autoarray-2024.5.16.0/autoarray/mask/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/mask/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/autoarray/mask/mock/mock_mask.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1584 2024-05-01 14:46:48.000000 autoarray-2024.5.16.0/autoarray/mock.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5062 2024-02-21 10:34:11.000000 autoarray-2024.5.16.0/autoarray/numba_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1935 2024-04-29 15:20:45.000000 autoarray-2024.5.16.0/autoarray/numpy_wrapper.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.278001 autoarray-2024.5.16.0/autoarray/operators/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/autoarray/operators/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3068 2024-05-15 16:46:48.000000 autoarray-2024.5.16.0/autoarray/operators/contour.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21843 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/operators/convolver.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.284000 autoarray-2024.5.16.0/autoarray/operators/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/operators/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      244 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/operators/mock/mock_convolver.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.302018 autoarray-2024.5.16.0/autoarray/operators/over_sampling/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/operators/over_sampling/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      483 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/operators/over_sampling/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2875 2024-05-01 17:32:00.000000 autoarray-2024.5.16.0/autoarray/operators/over_sampling/decorator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      270 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/operators/over_sampling/grid_oversampled.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13425 2024-05-13 09:02:28.000000 autoarray-2024.5.16.0/autoarray/operators/over_sampling/iterate.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15271 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/operators/over_sampling/over_sample_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16361 2024-05-13 09:02:28.000000 autoarray-2024.5.16.0/autoarray/operators/over_sampling/uniform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11074 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/operators/transformer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7717 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/operators/transformer_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.313006 autoarray-2024.5.16.0/autoarray/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3783 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8065 2023-08-14 09:39:51.000000 autoarray-2024.5.16.0/autoarray/plot/abstract_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      477 2023-06-03 16:38:13.000000 autoarray-2024.5.16.0/autoarray/plot/auto_labels.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.323000 autoarray-2024.5.16.0/autoarray/plot/get_visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/get_visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2662 2023-11-08 09:56:15.000000 autoarray-2024.5.16.0/autoarray/plot/get_visuals/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2394 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/get_visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9324 2024-04-18 18:12:37.000000 autoarray-2024.5.16.0/autoarray/plot/get_visuals/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.334002 autoarray-2024.5.16.0/autoarray/plot/include/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/include/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1718 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/include/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1263 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/include/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4182 2022-12-21 13:25:52.000000 autoarray-2024.5.16.0/autoarray/plot/include/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.344000 autoarray-2024.5.16.0/autoarray/plot/mat_plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/mat_plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10714 2024-03-12 16:47:43.000000 autoarray-2024.5.16.0/autoarray/plot/mat_plot/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11601 2024-04-29 15:20:47.000000 autoarray-2024.5.16.0/autoarray/plot/mat_plot/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28162 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/plot/mat_plot/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6279 2023-10-03 12:12:33.000000 autoarray-2024.5.16.0/autoarray/plot/multi_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.354999 autoarray-2024.5.16.0/autoarray/plot/visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2690 2023-05-12 10:15:02.000000 autoarray-2024.5.16.0/autoarray/plot/visuals/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1262 2024-04-29 15:20:41.000000 autoarray-2024.5.16.0/autoarray/plot/visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4004 2024-05-15 16:46:48.000000 autoarray-2024.5.16.0/autoarray/plot/visuals/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.359999 autoarray-2024.5.16.0/autoarray/plot/wrap/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2310 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.412999 autoarray-2024.5.16.0/autoarray/plot/wrap/base/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      469 2023-02-12 10:45:24.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6975 2024-04-29 15:20:47.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      544 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/annotate.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1900 2024-04-29 15:20:40.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/axis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3739 2024-04-29 15:20:40.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/cmap.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7208 2024-04-29 15:20:46.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/colorbar.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      446 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/colorbar_tickparams.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3042 2023-07-26 14:24:44.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/figure.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2865 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/label.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      829 2023-06-13 14:48:59.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/legend.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6731 2024-05-13 10:25:20.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/output.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      525 2023-12-07 11:13:21.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/text.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      542 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/tickparams.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13857 2024-04-29 15:20:39.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/ticks.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1000 2024-01-15 12:12:47.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/title.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2242 2023-06-12 12:16:27.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/base/units.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.432999 autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      133 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      586 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1961 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/avxline.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1826 2024-04-29 15:20:41.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/fill_between.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3052 2024-04-29 15:20:46.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/yx_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2024-04-29 15:20:44.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/yx_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44375 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/segmentdata.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.514999 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      856 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      586 2024-05-07 15:04:57.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      778 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/array_overlay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      318 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/border_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3658 2024-04-29 15:20:42.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/contour.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5120 2024-04-29 15:20:42.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/grid_errorbar.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5556 2024-05-15 16:46:48.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/grid_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5274 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/grid_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      304 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/index_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      316 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/index_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4841 2024-04-29 15:20:38.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/interpolated_reconstruction.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      300 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/mask_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      288 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/mesh_grid_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      310 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/origin_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      279 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/parallel_overscan_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1029 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/patch_overlay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      321 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/positions_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/serial_overscan_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      273 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/serial_prescan_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1222 2022-11-11 15:49:29.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/vector_yx_quiver.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3952 2024-04-29 15:20:39.000000 autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/voronoi_drawer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22217 2024-04-29 15:20:42.000000 autoarray-2024.5.16.0/autoarray/preloads.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.525999 autoarray-2024.5.16.0/autoarray/structures/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-08-13 18:02:25.000000 autoarray-2024.5.16.0/autoarray/structures/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2603 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/structures/abstract_structure.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.548000 autoarray-2024.5.16.0/autoarray/structures/arrays/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-11 15:40:14.000000 autoarray-2024.5.16.0/autoarray/structures/arrays/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9393 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/structures/arrays/array_1d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29992 2024-05-13 09:17:05.000000 autoarray-2024.5.16.0/autoarray/structures/arrays/array_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2083 2024-04-29 15:20:37.000000 autoarray-2024.5.16.0/autoarray/structures/arrays/irregular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20252 2024-04-29 15:20:44.000000 autoarray-2024.5.16.0/autoarray/structures/arrays/kernel_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12613 2024-04-29 15:20:39.000000 autoarray-2024.5.16.0/autoarray/structures/arrays/uniform_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36027 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/structures/arrays/uniform_2d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.571998 autoarray-2024.5.16.0/autoarray/structures/decorators/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      273 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/structures/decorators/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5649 2024-05-13 10:25:20.000000 autoarray-2024.5.16.0/autoarray/structures/decorators/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4192 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/structures/decorators/project_grid.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4397 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/structures/decorators/relocate_radial.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5442 2024-05-13 09:29:46.000000 autoarray-2024.5.16.0/autoarray/structures/decorators/to_array.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5363 2024-04-29 15:20:46.000000 autoarray-2024.5.16.0/autoarray/structures/decorators/to_grid.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2194 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/structures/decorators/to_projected.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4838 2024-04-29 15:20:40.000000 autoarray-2024.5.16.0/autoarray/structures/decorators/to_vector_yx.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2189 2024-04-29 15:20:46.000000 autoarray-2024.5.16.0/autoarray/structures/decorators/transform.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.591009 autoarray-2024.5.16.0/autoarray/structures/grids/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-11 15:32:21.000000 autoarray-2024.5.16.0/autoarray/structures/grids/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7914 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/structures/grids/grid_1d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30877 2024-05-07 12:49:32.000000 autoarray-2024.5.16.0/autoarray/structures/grids/grid_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14649 2024-04-29 15:20:44.000000 autoarray-2024.5.16.0/autoarray/structures/grids/irregular_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2693 2024-04-29 15:20:37.000000 autoarray-2024.5.16.0/autoarray/structures/grids/sparse_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11372 2024-04-29 15:20:40.000000 autoarray-2024.5.16.0/autoarray/structures/grids/uniform_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39060 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/structures/grids/uniform_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1579 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/autoarray/structures/header.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.605999 autoarray-2024.5.16.0/autoarray/structures/mesh/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/structures/mesh/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1500 2024-04-29 15:20:45.000000 autoarray-2024.5.16.0/autoarray/structures/mesh/abstract_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3544 2024-04-29 15:20:40.000000 autoarray-2024.5.16.0/autoarray/structures/mesh/delaunay_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7852 2024-04-29 15:20:37.000000 autoarray-2024.5.16.0/autoarray/structures/mesh/rectangular_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9472 2024-04-29 15:20:46.000000 autoarray-2024.5.16.0/autoarray/structures/mesh/triangulation_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3645 2024-04-29 15:20:38.000000 autoarray-2024.5.16.0/autoarray/structures/mesh/voronoi_2d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.613999 autoarray-2024.5.16.0/autoarray/structures/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/structures/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10687 2024-04-29 15:20:46.000000 autoarray-2024.5.16.0/autoarray/structures/mock/mock_decorators.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2871 2024-04-29 15:20:44.000000 autoarray-2024.5.16.0/autoarray/structures/mock/mock_grid.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.617998 autoarray-2024.5.16.0/autoarray/structures/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/structures/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8073 2024-04-29 15:20:44.000000 autoarray-2024.5.16.0/autoarray/structures/plot/structure_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.630000 autoarray-2024.5.16.0/autoarray/structures/vectors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/structures/vectors/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1028 2024-04-29 15:20:39.000000 autoarray-2024.5.16.0/autoarray/structures/vectors/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5752 2024-04-29 15:20:44.000000 autoarray-2024.5.16.0/autoarray/structures/vectors/irregular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15693 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/structures/vectors/uniform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10146 2024-04-29 15:20:38.000000 autoarray-2024.5.16.0/autoarray/structures/visibilities.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1561 2024-05-13 17:21:51.000000 autoarray-2024.5.16.0/autoarray/type.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.642001 autoarray-2024.5.16.0/autoarray/util/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1352 2024-04-17 12:48:41.000000 autoarray-2024.5.16.0/autoarray/util/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2646 2024-05-06 12:25:30.000000 autoarray-2024.5.16.0/autoarray/util/cholesky_funcs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5402 2024-04-29 15:20:38.000000 autoarray-2024.5.16.0/autoarray/util/fnnls.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2603 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/misc_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.647003 autoarray-2024.5.16.0/autoarray/util/nn/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1731 2023-03-21 17:41:19.000000 autoarray-2024.5.16.0/autoarray/util/nn/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3897 2024-04-29 15:20:43.000000 autoarray-2024.5.16.0/autoarray/util/nn/nn_py.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.650007 autoarray-2024.5.16.0/autoarray/util/nn/src/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1248 2022-12-20 22:03:05.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/README.md
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.826001 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      558 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/.indent.pro
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5420 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/CHANGELOG
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1190 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/CUSTOMISE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1343 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3231 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      166 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/config.h.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   141175 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/configure
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2745 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/configure.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19071 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/delaunay.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1261 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/delaunay.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2408 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/delaunay_internal.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3877 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/distribute.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      717 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/distribute.h
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.830000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.855999 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/1/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      233 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/1/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      603 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/1/generate.awk
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       64 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/1/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/1/suptitle.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/1/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1430 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/1/viewexample.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.894000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/2/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1258 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/2/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   240932 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/2/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      518 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/2/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      835 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/2/mpitest.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/2/suptitle.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      760 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/2/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      997 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/2/viewdata.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1229 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/2/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2958 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/2/viewinterp.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.916999 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/3/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1300 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/3/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      440 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/3/generate-data.awk
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      235 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/3/generate-points.awk
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       46 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/3/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      627 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/3/test.sh
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.949000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/4/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      556 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/4/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   132840 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/4/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       56 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/4/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      740 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/4/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      999 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/4/viewdata.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1244 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/4/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2966 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/4/viewinterp.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:57:59.980999 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/5/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      456 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/5/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1407289 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/5/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       54 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/5/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      461 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/5/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      536 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/5/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2981 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/5/viewinterp.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2614 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/5/viewinterp2.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:00.002020 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/6/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      613 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/6/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   165065 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/6/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       45 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/6/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      425 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/6/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       34 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/6/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2979 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/6/viewinterp.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      655 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/examples/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22150 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/hash.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2040 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/hash.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4772 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/install-sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1398 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/istack.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      767 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/istack.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      600 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/istack_internal.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4154 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/lpi.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3271 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/makefile.example
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3217 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/makefile.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3145 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/makefile_autolens
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36312 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/minell.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      920 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/minell.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      668 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/mkinstalldirs
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      891 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nan.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10955 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nn.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      949 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nn_internal.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11021 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nnai.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30764 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nnbathy.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2344 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nncommon-vulnerable.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14340 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nncommon.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      390 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nncommon.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nnconfig.h.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2220 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nnhpi_customized.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40728 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nnpi.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      183 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/nnpi.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4699 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/preader.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      740 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/preader.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2326 2024-04-29 15:20:37.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/sample.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   652743 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/triangle.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21562 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/triangle.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      425 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/autoarray/util/nn/src/nn/version.c
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:00.020999 autoarray-2024.5.16.0/autoarray.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15341 2024-05-16 09:57:58.000000 autoarray-2024.5.16.0/autoarray.egg-info/SOURCES.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:00.011006 autoarray-2024.5.16.0/docs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/docs/Makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3624 2023-05-10 13:41:54.000000 autoarray-2024.5.16.0/docs/conf.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       26 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/docs/index.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      795 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/docs/make.bat
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      148 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/eden.ini
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-05-16 09:58:00.017999 autoarray-2024.5.16.0/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2021-06-17 13:08:16.000000 autoarray-2024.5.16.0/files/eden.ini
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      546 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/files/release.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      626 2021-04-02 09:27:57.000000 autoarray-2024.5.16.0/files/to_do_list
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       71 2024-03-09 18:35:12.000000 autoarray-2024.5.16.0/optional_requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      210 2022-11-04 15:14:02.000000 autoarray-2024.5.16.0/readthedocs.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      150 2023-10-16 17:02:45.000000 autoarray-2024.5.16.0/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2024-05-16 09:58:00.024013 autoarray-2024.5.16.0/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2037 2024-05-16 09:56:09.000000 autoarray-2024.5.16.0/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2024-02-28 10:46:32.000000 autoarray-2024.5.16.0/to_do_list
```

### Comparing `autoarray-2024.1.27.4/LICENSE` & `autoarray-2024.5.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/__init__.py` & `autoarray-2024.5.16.0/autoarray/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,42 +3,36 @@
 from . import util
 from . import fixtures
 from . import mock as m
 from .numba_util import profile_func
 from .preloads import Preloads
 from .dataset import preprocess
 from .dataset.abstract.dataset import AbstractDataset
-from .dataset.abstract.settings import AbstractSettingsDataset
 from .dataset.abstract.w_tilde import AbstractWTilde
-from .dataset.imaging.settings import SettingsImaging
 from .dataset.imaging.dataset import Imaging
 from .dataset.imaging.simulator import SimulatorImaging
 from .dataset.imaging.w_tilde import WTildeImaging
 from .dataset.interferometer.dataset import Interferometer
-from .dataset.interferometer.settings import SettingsInterferometer
 from .dataset.interferometer.simulator import SimulatorInterferometer
 from .dataset.interferometer.w_tilde import WTildeInterferometer
+from .dataset.dataset_model import DatasetModel
 from .fit.fit_dataset import FitDataset
 from .fit.fit_imaging import FitImaging
 from .fit.fit_interferometer import FitInterferometer
 from .geometry.geometry_2d import Geometry2D
 from .inversion.pixelization.mappers.abstract import AbstractMapper
 from .inversion.pixelization import mesh
 from .inversion.pixelization import image_mesh
 from .inversion import regularization as reg
 from .inversion.inversion.settings import SettingsInversion
 from .inversion.inversion.abstract import AbstractInversion
 from .inversion.regularization.abstract import AbstractRegularization
 from .inversion.inversion.factory import inversion_from as Inversion
-from .inversion.inversion.factory import (
-    inversion_imaging_unpacked_from as InversionImaging,
-)
-from .inversion.inversion.factory import (
-    inversion_interferometer_unpacked_from as InversionInterferometer,
-)
+from .inversion.inversion.dataset_interface import DatasetInterface
+from .inversion.pixelization.border_relocator import BorderRelocator
 from .inversion.pixelization.pixelization import Pixelization
 from .inversion.pixelization.mappers.abstract import AbstractMapper
 from .inversion.pixelization.mappers.mapper_grids import MapperGrids
 from .inversion.pixelization.mappers.factory import mapper_from as Mapper
 from .inversion.pixelization.mappers.rectangular import MapperRectangularNoInterp
 from .inversion.pixelization.mappers.delaunay import MapperDelaunay
 from .inversion.pixelization.mappers.voronoi import MapperVoronoiNoInterp
@@ -59,35 +53,42 @@
 from .mask.derive.grid_2d import DeriveGrid2D
 from .mask.mask_1d import Mask1D
 from .mask.mask_2d import Mask2D
 from .operators.convolver import Convolver
 from .operators.convolver import Convolver
 from .operators.transformer import TransformerDFT
 from .operators.transformer import TransformerNUFFT
+from .operators.over_sampling.decorator import over_sample
+from .operators.contour import Grid2DContour
 from .layout.layout import Layout1D
 from .layout.layout import Layout2D
 from .structures.arrays.uniform_1d import Array1D
 from .structures.arrays.uniform_2d import Array2D
 from .structures.arrays.irregular import ArrayIrregular
 from .structures.grids.uniform_1d import Grid1D
 from .structures.grids.uniform_2d import Grid2D
-from .structures.grids.iterate_2d import Grid2DIterate
+from .operators.over_sampling.decorator import perform_over_sampling_from
+from .operators.over_sampling.grid_oversampled import Grid2DOverSampled
+from .operators.over_sampling.uniform import OverSamplingUniform
+from .operators.over_sampling.iterate import OverSamplingIterate
+from .operators.over_sampling.uniform import OverSamplerUniform
+from .operators.over_sampling.iterate import OverSamplerIterate
 from .structures.grids.irregular_2d import Grid2DIrregular
 from .structures.grids.irregular_2d import Grid2DIrregularUniform
 from .structures.mesh.rectangular_2d import Mesh2DRectangular
 from .structures.mesh.voronoi_2d import Mesh2DVoronoi
 from .structures.mesh.delaunay_2d import Mesh2DDelaunay
 from .structures.arrays.kernel_2d import Kernel2D
 from .structures.vectors.uniform import VectorYX2D
 from .structures.vectors.irregular import VectorYX2DIrregular
-from .structures import structure_decorators as grid_dec
+from .structures import decorators as grid_dec
 from .structures.header import Header
 from .layout.region import Region1D
 from .layout.region import Region2D
 from .structures.visibilities import Visibilities
 from .structures.visibilities import VisibilitiesNoiseMap
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2024.1.27.4"
+__version__ = "2024.5.16.0"
```

### Comparing `autoarray-2024.1.27.4/autoarray/abstract_ndarray.py` & `autoarray-2024.5.16.0/autoarray/plot/get_visuals/one_d.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,54 @@
-from __future__ import annotations
-from abc import ABC
-from abc import abstractmethod
-import numpy as np
-from pathlib import Path
-from typing import Union, TYPE_CHECKING
+from autoarray.plot.get_visuals.abstract import AbstractGetVisuals
+from autoarray.plot.include.one_d import Include1D
+from autoarray.plot.visuals.one_d import Visuals1D
+from autoarray.structures.arrays.uniform_1d import Array1D
 
-from autoconf import conf
 
-if TYPE_CHECKING:
-    from autoarray.structures.abstract_structure import Structure
-
-from autoarray.structures.arrays import array_2d_util
-
-
-class AbstractNDArray(np.ndarray, ABC):
-    def __reduce__(self):
-        pickled_state = super().__reduce__()
-
-        class_dict = {}
-        for key, value in self.__dict__.items():
-            class_dict[key] = value
-        new_state = pickled_state[2] + (class_dict,)
+class GetVisuals1D(AbstractGetVisuals):
+    def __init__(self, include: Include1D, visuals: Visuals1D):
+        """
+        Class which gets 1D attributes and adds them to a `Visuals1D` objects, such that they are plotted on 1D figures.
 
-        return pickled_state[0], pickled_state[1], new_state
+        For a visual to be extracted and added for plotting, it must have a `True` value in its corresponding entry in
+        the `Include1D` object. If this entry is `False`, the `GetVisuals1D.get` method returns a None and the attribute
+        is omitted from the plot.
 
-    # noinspection PyMethodOverriding
-    def __setstate__(self, state):
-        for key, value in state[-1].items():
-            setattr(self, key, value)
-        super().__setstate__(state[0:-1])
+        The `GetVisuals1D` class adds new visuals to a pre-existing `Visuals1D` object that is passed to its `__init__`
+        method. This only adds a new entry if the visual are not already in this object.
 
-    @property
-    @abstractmethod
-    def native(self) -> Structure:
+        Parameters
+        ----------
+        include
+            Sets which 1D visuals are included on the figure that is to be plotted (only entries which are `True`
+            are extracted via the `GetVisuals1D` object).
+        visuals
+            The pre-existing visuals of the plotter which new visuals are added too via the `GetVisuals1D` class.
         """
-        Returns the data structure in its `native` format which contains all unmaksed values to the native dimensions.
+        super().__init__(include=include, visuals=visuals)
+
+    def via_array_1d_from(self, array_1d: Array1D) -> Visuals1D:
         """
+        From an `Array1D` get its attributes that can be plotted and return them in a `Visuals1D` object.
 
-    @staticmethod
-    def flip_hdu_for_ds9(values):
-        if conf.instance["general"]["fits"]["flip_for_ds9"]:
-            return np.flipud(values)
-        return values
+        Only attributes not already in `self.visuals` and with `True` entries in the `Include1D` object are extracted
+        for plotting.
 
-    def output_to_fits(self, file_path: Union[Path, str], overwrite: bool = False):
-        """
-        Output the grid to a .fits file.
+        From an `Array1D` the following attributes can be extracted for plotting:
+
+        - origin: the (y,x) origin of the 1D array's coordinate system.
+        - mask: the mask of the 1D array.
 
         Parameters
         ----------
-        file_path
-            The path the file is output to, including the filename and the .fits extension, e.g. '/path/to/filename.fits'
-        overwrite
-            If a file already exists at the path, if overwrite=True it is overwritten else an error is raised.
+        array
+            The 1D array whose attributes are extracted for plotting.
+
+        Returns
+        -------
+        Visuals1D
+            The collection of attributes that are plotted by a `Plotter` object.
         """
-        array_2d_util.numpy_array_2d_to_fits(
-            array_2d=self.native, file_path=file_path, overwrite=overwrite
+        return self.visuals + self.visuals.__class__(
+            origin=self.get("origin", array_1d.origin),
+            mask=self.get("mask", array_1d.mask),
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/config/README.rst` & `autoarray-2024.5.16.0/autoarray/config/README.rst`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/config/general.yaml` & `autoarray-2024.5.16.0/autoarray/config/general.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 inversion:
   check_reconstruction: true          # If True, the inversion's reconstruction is checked to ensure the solution of a meshs's mapper is not an invalid solution where the values are all the same.
   use_positive_only_solver: true      # If True, inversion's use a positive-only linear algebra solver by default, which is slower but prevents unphysical negative values in the reconstructed solutuion.
   no_regularization_add_to_curvature_diag_value : 1.0e-3 # The default value added to the curvature matrix's diagonal when regularization is not applied to a linear object, which prevents inversion's failing due to the matrix being singular.
   positive_only_uses_p_initial: true  # If True, the positive-only solver of an inversion's uses an initial guess of the reconstructed data's values as which values should be positive, speeding up the solver.
-  relocate_pix_border: false          # If True, by default a pixelization's border is used to relocate all pixels outside its border to the border.
+  use_border_relocator: false          # If True, by default a pixelization's border is used to relocate all pixels outside its border to the border.
   reconstruction_vmax_factor: 0.5     # Plots of an Inversion's reconstruction use the reconstructed data's bright value multiplied by this factor.
 numba:
   use_numba: true
   cache: false
   nopython: true
   parallel: false
 pixelization:
```

### Comparing `autoarray-2024.1.27.4/autoarray/config/visualize/README.rst` & `autoarray-2024.5.16.0/autoarray/config/visualize/README.rst`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/config/visualize/general.yaml` & `autoarray-2024.5.16.0/autoarray/config/visualize/general.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 general:
   backend: default                      # The matploblib backend used for visualization. `default` uses the system default, can specifiy specific backend (e.g. TKAgg, Qt5Agg, WXAgg).
   imshow_origin: upper                  # The `origin` input of `imshow`, determining if pixel values are ascending or descending on the y-axis.
-  log10_min_value: 1.0e-4               # If a quantitiy with negative values is being plotted on a log10 scale, all values below this value are rounded up to it (e.g. to remove negative values).
+  log10_min_value: 1.0e-4               # If negative values are being plotted on a log10 scale, values below this value are rounded up to it (e.g. to remove negative values).
+  log10_max_value: 1.0e99               # If positive values are being plotted on a log10 scale, values above this value are rounded down to it (e.g. to prevent white blobs).
   zoom_around_mask: true                # If True, plots of data structures with a mask automatically zoom in the masked region.
   disable_zoom_for_fits: true           # If True, the zoom-in around the masked region is disabled when outputting .fits files, which is useful to retain the same dimensions as the input data.
 inversion:
   reconstruction_vmax_factor: 0.5
+  total_mappings_pixels : 8                 # The number of source pixels used when plotting the subplot_mappings of a pixelization.
 zoom:
   plane_percent: 0.01
   inversion_percent: 0.01               # Plots of an Inversion's reconstruction use the reconstructed data's bright value multiplied by this factor.
 subplot_shape:                          # The shape of a subplots for figures with an input number of subplots (e.g. for a figure with 4 subplots, the shape is (2, 2)).
   1: (1, 1)                             # The shape of subplots for a figure with 1 subplot.
   2: (1, 2)                             # The shape of subplots for a figure with 2 subplots.
   4: (2, 2)                             # The shape of subplots for a figure with 4 (or less than the above value) of subplots.
```

### Comparing `autoarray-2024.1.27.4/autoarray/config/visualize/include.yaml` & `autoarray-2024.5.16.0/autoarray/config/visualize/include.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/config/visualize/mat_wrap.yaml` & `autoarray-2024.5.16.0/autoarray/config/visualize/mat_wrap.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/config/visualize/mat_wrap_1d.yaml` & `autoarray-2024.5.16.0/autoarray/config/visualize/mat_wrap_1d.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/config/visualize/mat_wrap_2d.yaml` & `autoarray-2024.5.16.0/autoarray/config/visualize/mat_wrap_2d.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,21 @@
     c: r,g,b,m,y,k
     marker: .
     s: 20
   subplot:
     c: r,g,b,m,y,k
     marker: .
     s: 20
+IndexPlot:        # wrapper for `plt.plot()`: customize indexes (e.g. data / source plane or frame objects of an Inversion)
+  figure:
+    c: r,g,b,m,y,k
+    linewidth: 3
+  subplot:
+    c: r,g,b,m,y,k
+    linewidth: 3
 MaskScatter:         # wrapper for `plt.scatter()`: customize the appearance of 2D masks.
   figure:
     c: k
     marker: x
     s: 10
   subplot:
     c: k
```

### Comparing `autoarray-2024.1.27.4/autoarray/config/visualize/plots.yaml` & `autoarray-2024.5.16.0/autoarray/config/visualize/plots.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,22 @@
   residual_map: false                      # Plot individual plots of the residual-map?
   normalized_residual_map: false           # Plot individual plots of the normalized-residual-map?
   chi_squared_map: false                   # Plot individual plots of the chi-squared-map?
   residual_flux_fraction: false            # Plot individual plots of the residual_flux_fraction?
 fit_imaging: {}                            # Settings for plots of fits to imaging datasets (e.g. FitImagingPlotter).
 inversion:                                 # Settings for plots of inversions (e.g. InversionPlotter).
   subplot_inversion: true                  # Plot subplot of all quantities in each inversion (e.g. reconstrucuted image, reconstruction)?
+  subplot_mappings: true                   # Plot subplot of the image-to-source pixels mappings of each pixelization?
   all_at_end_png: true                     # Plot all individual plots listed below as .png (even if False)?
   all_at_end_fits: true                    # Plot all individual plots listed below as .fits (even if False)?
   all_at_end_pdf: false                    # Plot all individual plots listed below as publication-quality .pdf (even if False)?
   data_subtracted: false                   # Plot individual plots of the data with the other inversion linear objects subtracted?
   errors: false                            # Plot image of the errors of every mesh-pixel reconstructed value?
-  mesh_pixels_per_image_pixels : false     # Plot the number of image-plane mesh pixels per masked data pixels?
+  sub_pixels_per_image_pixels: false       # Plot the number of sub pixels per masked data pixels?
+  mesh_pixels_per_image_pixels: false      # Plot the number of image-plane mesh pixels per masked data pixels?
   reconstructed_image: false               # Plot image of the reconstructed data (e.g. in the image-plane)?
   reconstruction: false                    # Plot the reconstructed inversion (e.g. the pixelization's mesh in the source-plane)?
   regularization_weights: false            # Plot the effective regularization weight of every inversion mesh pixel?
 interferometer:                            # Settings for plots of interferometer datasets (e.g. InterferometerPlotter).
   amplitudes_vs_uv_distances: false
   phases_vs_uv_distances: false
   uv_wavelengths: false
```

### Comparing `autoarray-2024.1.27.4/autoarray/dataset/abstract/w_tilde.py` & `autoarray-2024.5.16.0/autoarray/dataset/abstract/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/dataset/imaging/dataset.py` & `autoarray-2024.5.16.0/autoarray/dataset/imaging/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import numpy as np
 from pathlib import Path
 from typing import Optional, Union
 
 from autoconf import cached_property
 
 from autoarray.dataset.abstract.dataset import AbstractDataset
-from autoarray.dataset.imaging.settings import SettingsImaging
 from autoarray.dataset.imaging.w_tilde import WTildeImaging
 from autoarray.structures.arrays.uniform_2d import Array2D
 from autoarray.operators.convolver import Convolver
 from autoarray.structures.grids.uniform_2d import Grid2D
+from autoarray.operators.over_sampling.abstract import AbstractOverSampling
 from autoarray.structures.arrays.kernel_2d import Kernel2D
 from autoarray.mask.mask_2d import Mask2D
 from autoarray import type as ty
 
 from autoarray import exc
 from autoarray.inversion.inversion.imaging import inversion_imaging_util
 
@@ -24,33 +24,78 @@
 class Imaging(AbstractDataset):
     def __init__(
         self,
         data: Array2D,
         noise_map: Optional[Array2D] = None,
         psf: Optional[Kernel2D] = None,
         noise_covariance_matrix: Optional[np.ndarray] = None,
-        settings: SettingsImaging = SettingsImaging(),
+        over_sampling: Optional[AbstractOverSampling] = None,
+        over_sampling_pixelization: Optional[AbstractOverSampling] = None,
         pad_for_convolver: bool = False,
+        use_normalized_psf: Optional[bool] = True,
         check_noise_map: bool = True,
     ):
         """
-        A class containing an imaging dataset, including the image data, noise-map and a point spread function (PSF).
+        An imaging dataset, containing the image data, noise-map, PSF and associated quantities
+        for calculations like the grid.
+
+        This object is the input to the `FitImaging` object, which fits the dataset with a model image and quantifies
+        the goodness-of-fit via a residual map, likelihood, chi-squared and other quantities.
+
+        The following quantities of the imaging data are available and used for the following tasks:
+
+        - `data`: The image data, which shows the signal that is analysed and fitted with a model image.
+
+        - `noise_map`: The RMS standard deviation error in every pixel, which is used to compute the chi-squared value
+        and likelihood of a fit.
+
+        - `psf`: The Point Spread Function of the data, used to perform 2D convolution on images to produce a model
+        image which is compared to the data.
+
+        Datasets also contains following properties:
+
+        - `grid`: A grids of (y,x) coordinates which align with the image pixels, whereby each coordinate corresponds to
+        the centre of an image pixel. This may be used in fits to calculate the model image of the imaging data.
+
+        - `grid_pixelization`: A grid of (y,x) coordinates which align with the pixels of a pixelization. This grid
+        is specifically used for pixelizations computed via the `invserion` module, which often use different
+        oversampling and sub-size values to the grid above.
+
+        The `over_sampling` and `over_sampling_pixelization` define how over sampling is performed for these grids.
+
+        This is used in the project PyAutoGalaxy to load imaging data of a galaxy and fit it with galaxy light profiles.
+        It is used in PyAutoLens to load imaging data of a strong lens and fit it with a lens model.
 
         Parameters
         ----------
         data
-            The array of the image data, for example in units of electrons per second.
+            The array of the image data containing the signal that is fitted (in PyAutoGalaxy and PyAutoLens the
+            recommended units are electrons per second).
         noise_map
-            An array describing the RMS standard deviation error in each pixel, for example in units of electrons per
-            second.
+            An array describing the RMS standard deviation error in each pixel used for computing quantities like the
+            chi-squared in a fit (in PyAutoGalaxy and PyAutoLens the recommended units are electrons per second).
         psf
-            An array describing the Point Spread Function kernel of the image which accounts for diffraction due to the
-            telescope optics via 2D convolution.
-        settings
-            Controls settings of how the dataset is set up (e.g. the types of grids used to perform calculations).
+            The Point Spread Function kernel of the image which accounts for diffraction due to the telescope optics
+            via 2D convolution.
+        noise_covariance_matrix
+            A noise-map covariance matrix representing the covariance between noise in every `data` value, which
+            can be used via a bespoke fit to account for correlated noise in the data.
+        over_sampling
+            How over sampling is performed for the grid which performs calculations not associated with a pixelization.
+            In PyAutoGalaxy and PyAutoLens this is light profile calculations.
+        over_sampling_pixelization
+            How over sampling is performed for the grid which is associated with a pixelization, which is therefore
+            passed into the calculations performed in the `inversion` module.
+        pad_for_convolver
+            The PSF convolution may extend beyond the edges of the image mask, which can lead to edge effects in the
+            convolved image. If `True`, the image and noise-map are padded to ensure the PSF convolution does not
+            extend beyond the edge of the image.
+        use_normalized_psf
+            If `True`, the PSF kernel values are rescaled such that they sum to 1.0. This can be important for ensuring
+            the PSF kernel does not change the overall normalization of the image when it is convolved with it.
         check_noise_map
             If True, the noise-map is checked to ensure all values are above zero.
         """
 
         self.unmasked = None
 
         self.pad_for_convolver = pad_for_convolver
@@ -77,32 +122,35 @@
                     f"the image and noise-map yourself."
                 )
 
         super().__init__(
             data=data,
             noise_map=noise_map,
             noise_covariance_matrix=noise_covariance_matrix,
-            settings=settings,
+            over_sampling=over_sampling,
+            over_sampling_pixelization=over_sampling_pixelization,
         )
 
+        self.use_normalized_psf = use_normalized_psf
+
         if self.noise_map.native is not None and check_noise_map:
             if ((self.noise_map.native <= 0.0) * np.invert(self.noise_map.mask)).any():
                 zero_entries = np.argwhere(self.noise_map.native <= 0.0)
 
                 raise exc.DatasetException(
                     f"""
                     A value in the noise-map of the dataset is {np.min(self.noise_map)}. 
 
                     This is less than or equal to zero, and therefore an ill-defined value which must be corrected.
                     
                     The 2D indexes of the arrays in the native noise map array are {zero_entries}.
                     """
                 )
 
-        if psf is not None and settings.use_normalized_psf:
+        if psf is not None and use_normalized_psf:
             psf = Kernel2D.no_mask(
                 values=psf.native, pixel_scales=psf.pixel_scales, normalize=True
             )
 
         self.psf = psf
 
     @cached_property
@@ -119,15 +167,15 @@
 
         Returns
         -------
         The blurring grid given the mask of the imaging data.
         """
 
         return self.grid.blurring_grid_via_kernel_shape_from(
-            kernel_shape_native=self.psf.shape_native
+            kernel_shape_native=self.psf.shape_native,
         )
 
     @cached_property
     def convolver(self):
         """
         Returns a `Convolver` from a mask and 2D PSF kernel.
 
@@ -166,16 +214,16 @@
         logger.info("IMAGING - Computing W-Tilde... May take a moment.")
 
         (
             curvature_preload,
             indexes,
             lengths,
         ) = inversion_imaging_util.w_tilde_curvature_preload_imaging_from(
-            noise_map_native=self.noise_map.native,
-            kernel_native=self.psf.native,
+            noise_map_native=np.array(self.noise_map.native),
+            kernel_native=np.array(self.psf.native),
             native_index_for_slim_index=self.mask.derive_indexes.native_for_slim,
         )
 
         return WTildeImaging(
             curvature_preload=curvature_preload,
             indexes=indexes.astype("int"),
             lengths=lengths.astype("int"),
@@ -189,14 +237,16 @@
         data_path: Union[Path, str],
         noise_map_path: Union[Path, str],
         data_hdu: int = 0,
         noise_map_hdu: int = 0,
         psf_path: Optional[Union[Path, str]] = None,
         psf_hdu: int = 0,
         noise_covariance_matrix: Optional[np.ndarray] = None,
+        over_sampling: Optional[AbstractOverSampling] = None,
+        over_sampling_pixelization: Optional[AbstractOverSampling] = None,
     ) -> "Imaging":
         """
         Load an imaging dataset from multiple .fits file.
 
         For each attribute of the imaging data (e.g. `data`, `noise_map`, `pre_cti_data`) the path to
         the .fits and the `hdu` containing the data can be specified.
 
@@ -251,14 +301,16 @@
             psf = None
 
         return Imaging(
             data=data,
             noise_map=noise_map,
             psf=psf,
             noise_covariance_matrix=noise_covariance_matrix,
+            over_sampling=over_sampling,
+            over_sampling_pixelization=over_sampling_pixelization,
         )
 
     def apply_mask(self, mask: Mask2D) -> "Imaging":
         """
         Apply a mask to the imaging dataset, whereby the mask is applied to the image data, noise-map and other
         quantities one-by-one.
 
@@ -272,19 +324,17 @@
             The 2D mask that is applied to the image.
         """
         if self.data.mask.is_all_false:
             unmasked_dataset = self
         else:
             unmasked_dataset = self.unmasked
 
-        data = Array2D(values=unmasked_dataset.data.native, mask=mask.derive_mask.sub_1)
+        data = Array2D(values=unmasked_dataset.data.native, mask=mask)
 
-        noise_map = Array2D(
-            values=unmasked_dataset.noise_map.native, mask=mask.derive_mask.sub_1
-        )
+        noise_map = Array2D(values=unmasked_dataset.noise_map.native, mask=mask)
 
         if unmasked_dataset.noise_covariance_matrix is not None:
             noise_covariance_matrix = unmasked_dataset.noise_covariance_matrix
 
             noise_covariance_matrix = np.delete(
                 noise_covariance_matrix, mask.derive_indexes.masked_slim, 0
             )
@@ -296,47 +346,27 @@
             noise_covariance_matrix = None
 
         dataset = Imaging(
             data=data,
             noise_map=noise_map,
             psf=self.psf,
             noise_covariance_matrix=noise_covariance_matrix,
-            settings=self.settings,
+            over_sampling=self.over_sampling,
+            over_sampling_pixelization=self.over_sampling_pixelization,
             pad_for_convolver=True,
         )
 
         dataset.unmasked = unmasked_dataset
 
         logger.info(
             f"IMAGING - Data masked, contains a total of {mask.pixels_in_mask} image-pixels"
         )
 
         return dataset
 
-    def apply_settings(self, settings: SettingsImaging) -> "Imaging":
-        """
-        Returns a new instance of the imaging with the input `SettingsImaging` applied to them.
-
-        This can be used to update settings like the types of grids associated with the dataset that are used
-        to perform calculations or putting a limit of the dataset's signal-to-noise.
-
-        Parameters
-        ----------
-        settings
-            The settings for the imaging data that control things like the grids used for calculations.
-        """
-        return Imaging(
-            data=self.data,
-            noise_map=self.noise_map,
-            psf=self.psf,
-            noise_covariance_matrix=self.noise_covariance_matrix,
-            settings=settings,
-            pad_for_convolver=self.pad_for_convolver,
-        )
-
     def output_to_fits(
         self,
         data_path: Union[Path, str],
         psf_path: Optional[Union[Path, str]] = None,
         noise_map_path: Optional[Union[Path, str]] = None,
         overwrite: bool = False,
     ):
```

### Comparing `autoarray-2024.1.27.4/autoarray/dataset/imaging/simulator.py` & `autoarray-2024.5.16.0/autoarray/dataset/imaging/simulator.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 class SimulatorImaging:
     def __init__(
         self,
         exposure_time: float,
         background_sky_level: float = 0.0,
+        subtract_background_sky: bool = True,
         psf: Kernel2D = None,
         normalize_psf: bool = True,
         add_poisson_noise: bool = True,
         noise_if_add_noise_false: float = 0.1,
         noise_seed: int = -1,
     ):
         """
@@ -43,14 +44,16 @@
 
         Parameters
         ----------
         exposure_time
             The exposure time of the simulated imaging.
         background_sky_level
             The level of the background sky of the simulated imaging.
+        subtract_background_sky
+            If `True`, the background sky level is subtracted from the simulated dataset, otherwise it is left in.
         psf
             An array describing the PSF kernel of the image.
         normalize_psf
             If `True`, the PSF kernel is normalized so all values sum to 1.0.
         add_poisson_noise
             Whether Poisson noise corresponding to photon count statistics on the imaging observation is added.
         noise_if_add_noise_false
@@ -65,15 +68,15 @@
                 psf = psf.normalized
             self.psf = psf
         else:
             self.psf = Kernel2D.no_blur(pixel_scales=1.0)
 
         self.exposure_time = exposure_time
         self.background_sky_level = background_sky_level
-
+        self.subtract_background_sky = subtract_background_sky
         self.add_poisson_noise = add_poisson_noise
         self.noise_if_add_noise_false = noise_if_add_noise_false
         self.noise_seed = noise_seed
 
     def via_image_from(self, image: Array2D) -> Imaging:
         """
         Simulate an `Imaging` dataset from an input image.
@@ -123,15 +126,16 @@
 
         if np.isnan(noise_map).any():
             raise exc.DatasetException(
                 "The noise-map has NaN values in it. This suggests your exposure time and / or"
                 "background sky levels are too low, creating signal counts at or close to 0.0."
             )
 
-        image = image - background_sky_map
+        if self.subtract_background_sky:
+            image = image - background_sky_map
 
         mask = Mask2D.all_false(
             shape_native=image.shape_native, pixel_scales=image.pixel_scales
         )
 
         image = Array2D(values=image, mask=mask)
```

### Comparing `autoarray-2024.1.27.4/autoarray/dataset/imaging/w_tilde.py` & `autoarray-2024.5.16.0/autoarray/dataset/imaging/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/dataset/interferometer/simulator.py` & `autoarray-2024.5.16.0/autoarray/dataset/interferometer/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,8 +89,9 @@
             )
 
         return Interferometer(
             data=visibilities,
             noise_map=noise_map,
             uv_wavelengths=transformer.uv_wavelengths,
             real_space_mask=image.mask,
+            transformer_class=self.transformer_class,
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/dataset/interferometer/w_tilde.py` & `autoarray-2024.5.16.0/autoarray/dataset/interferometer/w_tilde.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         The w_tilde formalism performs linear algebra formalism in a way that speeds up the construction of  the
         simultaneous linear equations by bypassing the construction of a `mapping_matrix` and precomputing the
         Fourier transform operations performed using the interferometer's `uv_wavelengths`.
 
         Parameters
         ----------
         w_matrix
-            The w_tilde matrix used to construct the data vector during an inversion.
+            The w_tilde matrix used by the w-tilde formalism to construct the data vector and
+            curvature matrix during an inversion efficiently..
         curvature_preload
             A matrix which uses the interferometer `uv_wavelengths` to preload as much of the computation of the
             curvature matrix as possible.
         dirty_image
             The real-space image of the visibilities computed via the transform, which is used to construct the
             curvature matrix.
         real_space_mask
```

### Comparing `autoarray-2024.1.27.4/autoarray/dataset/plot/imaging_plotters.py` & `autoarray-2024.5.16.0/autoarray/dataset/plot/imaging_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/dataset/plot/interferometer_plotters.py` & `autoarray-2024.5.16.0/autoarray/dataset/plot/interferometer_plotters.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,22 +108,22 @@
             Whether to make a 2D plot (via `imshow`) of the dirty noise map.
         dirty_signal_to_noise_map
             Whether to make a 2D plot (via `imshow`) of the dirty signal-to-noise map.
         """
 
         if data:
             self.mat_plot_2d.plot_grid(
-                grid=self.dataset.visibilities.in_grid,
+                grid=self.dataset.data.in_grid,
                 visuals_2d=self.visuals_2d,
                 auto_labels=AutoLabels(title="Visibilities", filename="data"),
             )
 
         if noise_map:
             self.mat_plot_2d.plot_grid(
-                grid=self.dataset.visibilities.in_grid,
+                grid=self.dataset.data.in_grid,
                 visuals_2d=self.visuals_2d,
                 color_array=self.dataset.noise_map.real,
                 auto_labels=AutoLabels(title="Noise-Map", filename="noise_map"),
             )
 
         if u_wavelengths:
             self.mat_plot_1d.plot_yx(
```

### Comparing `autoarray-2024.1.27.4/autoarray/dataset/preprocess.py` & `autoarray-2024.5.16.0/autoarray/dataset/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     Parameters
     ----------
     array_eps
         The array which is converted from electrons per seconds to counts.
     exposure_time_map
         The exposure time at every data-point of the array.
     """
-    return np.multiply(array_eps, exposure_time_map)
+    return array_eps * exposure_time_map
 
 
 def array_counts_to_eps(array_counts, exposure_time_map):
     """
     Convert an array in units of electrons per second to counts, using an exposure time map containing the exposure
     time at every point in the array.
 
@@ -55,15 +55,15 @@
     Parameters
     ----------
     array_counts
         The array which is converted from counts to electrons per seconds.
     exposure_time_map
         The exposure time at every data-point of the array.
     """
-    return np.divide(array_counts, exposure_time_map)
+    return array_counts / exposure_time_map
 
 
 def array_eps_to_adus(array_eps, exposure_time_map, gain):
     """
     Convert an array in units of electrons per second to adus, using an exposure time map containing the exposure
     time at every point in the array and the instrument gain.
 
@@ -76,15 +76,15 @@
     array_eps
         The array which is converted from electrons per seconds to adus.
     exposure_time_map
         The exposure time at every data-point of the array.
     gain
         The gain of the instrument used in the conversion to / from counts and ADUs.
     """
-    return np.multiply(array_eps, exposure_time_map) / gain
+    return (array_eps * exposure_time_map) / gain
 
 
 def array_adus_to_eps(array_adus, exposure_time_map, gain):
     """
     Convert an array in units of electrons per second to adus, using an exposure time map containing the exposure
     time at every point in the array and the instrument gain.
 
@@ -97,15 +97,15 @@
     array_adus
         The array which is converted from adus to electrons per seconds
     exposure_time_map
         The exposure time at every data-point of the array.
     gain
         The gain of the instrument used in the conversion to / from counts and ADUs.
     """
-    return np.divide(gain * array_adus, exposure_time_map)
+    return (gain * array_adus) / exposure_time_map
 
 
 def array_counts_to_counts_per_second(array_counts, exposure_time):
     if exposure_time is None:
         raise exc.ArrayException(
             "Cannot convert a Frame2D to units counts per second without an exposure time attribute (exposure_time = None)."
         )
@@ -144,15 +144,17 @@
     Parameters
     ----------
     data_eps
         The data in electrons second used to estimate the Poisson noise in every data point.
     exposure_time_map
         The exposure time at every data-point of the data.
     """
-    return np.sqrt(np.abs(data_eps * exposure_time_map)) / exposure_time_map
+    return data_eps.with_new_array(
+        np.abs(data_eps * exposure_time_map) ** 0.5 / exposure_time_map
+    )
 
 
 def noise_map_via_weight_map_from(weight_map):
     """
     Setup the noise-map from a weight map, which is a form of noise-map that comes via HST image-reduction and
     the software package MultiDrizzle.
 
@@ -168,15 +170,15 @@
     pixel_scales
         The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
     weight_map
         The weight-value of each pixel which is converted to a variance.
     """
     np.seterr(divide="ignore")
-    noise_map = 1.0 / np.sqrt(weight_map)
+    noise_map = 1.0 / weight_map**0.5
     noise_map[noise_map > 1.0e8] = 1.0e8
     return noise_map
 
 
 def noise_map_via_inverse_noise_map_from(inverse_noise_map):
     """
     Setup the noise-map from an inverse noise-map.
@@ -209,22 +211,20 @@
     exposure_time_map
         The exposure time at every data-point of the data.
     background_noise_map
         The RMS standard deviation error in every data point due to a background component of the noise-map in units
         of electrons per second.
     """
     return (
-        np.sqrt(
-            (
-                np.abs(data_eps * exposure_time_map)
-                + np.square(background_noise_map * exposure_time_map)
-            )
+        (
+            abs(data_eps * exposure_time_map)
+            + (background_noise_map * exposure_time_map) ** 2
         )
-        / exposure_time_map
-    )
+        ** 0.5
+    ) / exposure_time_map
 
 
 def noise_map_via_data_eps_exposure_time_map_and_background_variances_from(
     data_eps, exposure_time_map, background_variances
 ):
     """
     This is the same as `noise_map_via_data_eps_exposure_time_map_and_background_noise_map_from`, however the
@@ -237,22 +237,17 @@
     exposure_time_map
         The exposure time at every data-point of the data.
     background_noise_map
         The variance in every data point due to a background component of the noise-map in units
         of electrons per second.
     """
     return (
-        np.sqrt(
-            (
-                np.abs(data_eps * exposure_time_map)
-                + (background_variances * exposure_time_map)
-            )
-        )
-        / exposure_time_map
-    )
+        (abs(data_eps * exposure_time_map) + (background_variances * exposure_time_map))
+        ** 0.5
+    ) / exposure_time_map
 
 
 def edges_from(image, no_edges):
     """
     Extract the edges of an input image and return them as a concatenated 1D ndarray.
 
     These edges are typically empty regions of an image that may contain the background sky, which can be used
@@ -367,15 +362,15 @@
         The RMS standard deviation error in every data point due to a background component of the noise-map in units
         of electrons per second.
     """
     inverse_background_noise_map = 1.0 / background_noise_map
     relative_background_noise_map = inverse_background_noise_map / np.max(
         inverse_background_noise_map
     )
-    return np.abs(exposure_time * (relative_background_noise_map))
+    return abs(exposure_time * relative_background_noise_map)
 
 
 def setup_random_seed(seed):
     """Setup the random seed. If the input seed is -1, the code will use a random seed for every run. If it is \
     positive, that seed is used for all runs, thereby giving reproducible results.
 
     Parameters
@@ -509,15 +504,15 @@
 
     from autoarray.mask.mask_2d import Mask2D
     from autoarray.structures.arrays.uniform_1d import Array1D
     from autoarray.structures.arrays.uniform_2d import Array2D
 
     # TODO : Refacotr into a util
 
-    signal_to_noise_map = np.divide(data, noise_map)
+    signal_to_noise_map = data / noise_map
     signal_to_noise_map[signal_to_noise_map < 0] = 0
 
     if noise_limit_mask is None:
         noise_limit_mask = np.full(fill_value=False, shape=data.shape_native)
 
     noise_map_limit = np.where(
         (signal_to_noise_map.native > signal_to_noise_limit)
```

### Comparing `autoarray-2024.1.27.4/autoarray/exc.py` & `autoarray-2024.5.16.0/autoarray/exc.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/fit/fit_dataset.py` & `autoarray-2024.5.16.0/autoarray/fit/fit_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import warnings
 from abc import ABC
 from abc import abstractmethod
 from typing import Dict, Optional
 
 import numpy as np
 
-from autoarray import type as ty
-from autoarray.dataset.abstract.dataset import AbstractDataset
+from autoarray.dataset.dataset_model import DatasetModel
 from autoarray.fit import fit_util
 from autoarray.inversion.inversion.abstract import AbstractInversion
-from autoarray.mask.abstract_mask import Mask
+from autoarray.mask.mask_2d import Mask2D
+
 from autoarray.numba_util import profile_func
-from autoarray.structures.abstract_structure import Structure
+from autoarray import type as ty
 
 
 class AbstractFitInversion(ABC):
     @property
     @abstractmethod
     def data(self) -> ty.DataLike:
-        pass
+        """
+        Overwrite this method to returns the data of the dataset.
+        """
 
     @property
     @abstractmethod
-    def noise_map(self) -> ty.NoiseMapLike:
-        pass
+    def noise_map(self) -> ty.DataLike:
+        """
+        Overwrite this method to returns the noise-map of the dataset.
+        """
 
     @property
     @abstractmethod
     def model_data(self) -> ty.DataLike:
         """
         Overwrite this method so it returns the model-data which is fitted to the input data.
         """
@@ -35,40 +39,40 @@
     @property
     def signal_to_noise_map(self) -> ty.DataLike:
         """
         The signal-to-noise_map of the dataset and noise-map which are fitted.
         """
         warnings.filterwarnings("ignore")
 
-        signal_to_noise_map = np.divide(self.data, self.noise_map)
+        signal_to_noise_map = self.data / self.noise_map
         signal_to_noise_map[signal_to_noise_map < 0] = 0
         return signal_to_noise_map
 
     @property
-    def residual_map(self) -> Structure:
+    def residual_map(self) -> ty.DataLike:
         """
         Returns the residual-map between the masked dataset and model data, where:
 
         Residuals = (Data - Model_Data).
         """
         return fit_util.residual_map_from(data=self.data, model_data=self.model_data)
 
     @property
-    def normalized_residual_map(self) -> Structure:
+    def normalized_residual_map(self) -> ty.DataLike:
         """
         Returns the normalized residual-map between the masked dataset and model data, where:
 
         Normalized_Residual = (Data - Model_Data) / Noise
         """
         return fit_util.normalized_residual_map_from(
             residual_map=self.residual_map, noise_map=self.noise_map
         )
 
     @property
-    def chi_squared_map(self) -> Structure:
+    def chi_squared_map(self) -> ty.DataLike:
         """
         Returns the chi-squared-map between the residual-map and noise-map, where:
 
         Chi_Squared = ((Residuals) / (Noise)) ** 2.0 = ((Data - Model)**2.0)/(Variances)
         """
         return fit_util.chi_squared_map_from(
             residual_map=self.residual_map, noise_map=self.noise_map
@@ -98,55 +102,34 @@
         Log Likelihood = -0.5*[Chi_Squared_Term + Noise_Term] (see functions above for these definitions)
         """
         return fit_util.log_likelihood_from(
             chi_squared=self.chi_squared, noise_normalization=self.noise_normalization
         )
 
 
-class SimpleFit(AbstractFitInversion):
-    def __init__(self, data, model_data, noise_map):
-        self._data = data
-        self._model_data = model_data
-        self._noise_map = noise_map
-
-    @property
-    def data(self) -> ty.DataLike:
-        return self._data
-
-    @property
-    def noise_map(self) -> ty.NoiseMapLike:
-        return self._noise_map
-
-    @property
-    def model_data(self) -> ty.DataLike:
-        return self._model_data
-
-
 class FitDataset(AbstractFitInversion):
     # noinspection PyUnresolvedReferences
     def __init__(
         self,
-        dataset: AbstractDataset,
+        dataset,
         use_mask_in_fit: bool = False,
+        dataset_model: DatasetModel = None,
         run_time_dict: Optional[Dict] = None,
     ):
         """Class to fit a masked dataset where the dataset's data structures are any dimension.
 
         Parameters
         ----------
-        dataset : MaskedDataset
+        dataset
             The masked dataset (data, mask, noise-map, etc.) that is fitted.
-        model_data
-            The model data the masked dataset is fitted with.
-        inversion : Inversion
-            If the fit uses an `Inversion` this is the instance of the object used to perform the fit. This determines
-            if the `log_likelihood` or `log_evidence` is used as the `figure_of_merit`.
         use_mask_in_fit
             If `True`, masked data points are omitted from the fit. If `False` they are not (in most use cases the
             `dataset` will have been processed to remove masked points, for example the `slim` representation).
+        dataset_model
+            Attributes which allow for parts of a dataset to be treated as a model (e.g. the background sky level).
 
         Attributes
         -----------
         residual_map
             The residual-map of the fit (data - model_data).
         chi_squared_map
             The chi-squared-map of the fit ((data - model_data) / noise_maps ) **2.0
@@ -158,61 +141,74 @@
         noise_normalization
             The overall normalization term of the noise_map, summed over every data point.
         log_likelihood
             The overall log likelihood of the model's fit to the dataset, summed over evey data point.
         """
         self.dataset = dataset
         self.use_mask_in_fit = use_mask_in_fit
-
+        self.dataset_model = dataset_model or DatasetModel()
         self.run_time_dict = run_time_dict
 
     @property
-    @abstractmethod
-    def mask(self) -> Mask:
-        """
-        Overwrite this method so it returns the mask of the dataset which is fitted to the input data.
-        """
+    def mask(self) -> Mask2D:
+        return self.dataset.mask
+
+    @property
+    def grid(self) -> ty.Grid2DLike:
+        return self.dataset.grid.subtracted_from(offset=self.dataset_model.grid_offset)
+
+    @property
+    def grid_pixelization(self) -> ty.Grid2DLike:
+        return self.dataset.grid_pixelization.subtracted_from(
+            offset=self.dataset_model.grid_offset
+        )
+
+    @property
+    def blurring_grid(self) -> ty.Grid2DLike:
+        return self.dataset.blurring_grid.subtracted_from(
+            offset=self.dataset_model.grid_offset
+        )
 
     @property
     def data(self) -> ty.DataLike:
         return self.dataset.data
 
     @property
-    def noise_map(self) -> ty.NoiseMapLike:
+    def noise_map(self) -> ty.DataLike:
         return self.dataset.noise_map
 
     @property
-    def residual_map(self) -> Structure:
+    def residual_map(self) -> ty.DataLike:
         """
         Returns the residual-map between the masked dataset and model data, where:
 
         Residuals = (Data - Model_Data).
         """
 
         if self.use_mask_in_fit:
             return fit_util.residual_map_with_mask_from(
                 data=self.data, model_data=self.model_data, mask=self.mask
             )
         return super().residual_map
 
     @property
-    def normalized_residual_map(self) -> Structure:
+    def normalized_residual_map(self) -> ty.DataLike:
         """
         Returns the normalized residual-map between the masked dataset and model data, where:
 
         Normalized_Residual = (Data - Model_Data) / Noise
         """
         if self.use_mask_in_fit:
             return fit_util.normalized_residual_map_with_mask_from(
                 residual_map=self.residual_map, noise_map=self.noise_map, mask=self.mask
             )
         return super().normalized_residual_map
 
     @property
-    def chi_squared_map(self) -> Structure:
+    def chi_squared_map(self) -> ty.DataLike:
         """
         Returns the chi-squared-map between the residual-map and noise-map, where:
 
         Chi_Squared = ((Residuals) / (Noise)) ** 2.0 = ((Data - Model)**2.0)/(Variances)
         """
         if self.use_mask_in_fit:
             return fit_util.chi_squared_map_with_mask_from(
@@ -303,18 +299,21 @@
 
     @property
     @profile_func
     def figure_of_merit(self) -> float:
         if self.inversion is not None:
             return self.log_evidence
 
-        return self.log_likelihood
+        try:
+            return self.log_likelihood.array
+        except AttributeError:
+            return self.log_likelihood
 
     @property
-    def residual_flux_fraction_map(self) -> Structure:
+    def residual_flux_fraction_map(self) -> ty.DataLike:
         """
         Returns the residual flux fraction map, which shows the fraction of signal in each pixel that is not fitted
         by the model, therefore where:
 
         Residual_Flux_Fraction = ((Residuals) / (Data)) = ((Data - Model))/(Data)
 
         This quantity is not used for computing the log likelihood, but is available for plotting and inspection.
```

### Comparing `autoarray-2024.1.27.4/autoarray/fit/fit_imaging.py` & `autoarray-2024.5.16.0/autoarray/fit/fit_imaging.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, Optional
 
 from autoarray.dataset.imaging.dataset import Imaging
+from autoarray.dataset.dataset_model import DatasetModel
 from autoarray.fit.fit_dataset import FitDataset
-from autoarray.mask.mask_2d import Mask2D
 from autoarray.structures.arrays.uniform_2d import Array2D
 
+from autoarray import type as ty
+
 
 class FitImaging(FitDataset):
     def __init__(
         self,
         dataset: Imaging,
         use_mask_in_fit: bool = False,
+        dataset_model: DatasetModel = None,
         run_time_dict: Optional[Dict] = None,
     ):
         """
         Class to fit a masked imaging dataset.
 
         Parameters
         ----------
-        dataset : MaskedImaging
-            The masked imaging dataset that is fitted.
-        model_image
-            The model image the masked imaging is fitted with.
-        inversion : Inversion
-            If the fit uses an `Inversion` this is the instance of the object used to perform the fit. This determines
-            if the `log_likelihood` or `log_evidence` is used as the `figure_of_merit`.
+        dataset
+            The masked dataset that is fitted.
+        dataset_model
+            Attributes which allow for parts of a dataset to be treated as a model (e.g. the background sky level).
         use_mask_in_fit
             If `True`, masked data points are omitted from the fit. If `False` they are not (in most use cases the
             `dataset` will have been processed to remove masked points, for example the `slim` representation).
 
         Attributes
         -----------
         residual_map
@@ -45,29 +45,20 @@
         log_likelihood
             The overall log likelihood of the model's fit to the dataset, summed over evey data point.
         """
 
         super().__init__(
             dataset=dataset,
             use_mask_in_fit=use_mask_in_fit,
+            dataset_model=dataset_model,
             run_time_dict=run_time_dict,
         )
 
     @property
-    def imaging(self) -> Imaging:
-        return self.dataset
-
-    @property
-    def image(self) -> Array2D:
-        return self.data
-
-    @property
-    def model_image(self) -> Array2D:
-        return self.model_data
-
-    @property
-    def mask(self) -> Mask2D:
-        return self.dataset.mask
+    def data(self) -> ty.DataLike:
+        if self.dataset_model.background_sky_level != 0.0:
+            return self.dataset.data - self.dataset_model.background_sky_level
+        return self.dataset.data
 
     @property
     def blurred_image(self) -> Array2D:
         raise NotImplementedError
```

### Comparing `autoarray-2024.1.27.4/autoarray/fit/fit_interferometer.py` & `autoarray-2024.5.16.0/autoarray/fit/fit_interferometer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import numpy as np
-from typing import Dict, Optional, Union
+from typing import Dict, Optional
 
 from autoarray.dataset.interferometer.dataset import Interferometer
+
+from autoarray.dataset.dataset_model import DatasetModel
 from autoarray.structures.arrays.uniform_2d import Array2D
 from autoarray.structures.visibilities import Visibilities
 from autoarray.fit.fit_dataset import FitDataset
 
 from autoarray.fit import fit_util
 from autoarray import type as ty
 
 
 class FitInterferometer(FitDataset):
     def __init__(
         self,
         dataset: Interferometer,
+        dataset_model: DatasetModel = None,
         use_mask_in_fit: bool = False,
         run_time_dict: Optional[Dict] = None,
     ):
-        """Class to fit a masked interferometer dataset.
+        """
+        Class to fit a masked interferometer dataset.
 
         Parameters
         ----------
         dataset : MaskedInterferometer
             The masked interferometer dataset that is fitted.
+        dataset_model
+            Attributes which allow for parts of a dataset to be treated as a model (e.g. the background sky level).
         model_data : Visibilities
             The model visibilities the masked imaging is fitted with.
         inversion : Inversion
             If the fit uses an `Inversion` this is the instance of the object used to perform the fit. This determines
             if the `log_likelihood` or `log_evidence` is used as the `figure_of_merit`.
         use_mask_in_fit
             If `True`, masked data points are omitted from the fit. If `False` they are not (in most use cases the
@@ -47,92 +53,82 @@
             The overall normalization term of the noise_map, summed over every data point.
         log_likelihood
             The overall log likelihood of the model's fit to the dataset, summed over evey data point.
         """
 
         super().__init__(
             dataset=dataset,
+            dataset_model=dataset_model,
             use_mask_in_fit=use_mask_in_fit,
             run_time_dict=run_time_dict,
         )
 
     @property
     def mask(self) -> np.ndarray:
         return np.full(shape=self.data.shape, fill_value=False)
 
     @property
-    def interferometer(self) -> Interferometer:
-        return self.dataset
-
-    @property
     def transformer(self) -> ty.Transformer:
         return self.dataset.transformer
 
     @property
-    def visibilities(self) -> Visibilities:
-        return self.data
-
-    @property
-    def model_visibilities(self) -> Visibilities:
-        return self.model_data
-
-    @property
     def normalized_residual_map(self) -> np.ndarray:
         """
         Returns the normalized residual-map between the masked dataset and model data, where:
 
         Normalized_Residual = (Data - Model_Data) / Noise
         """
-        return fit_util.normalized_residual_map_complex_with_mask_from(
-            residual_map=self.residual_map, noise_map=self.noise_map, mask=self.mask
+        return fit_util.normalized_residual_map_complex_from(
+            residual_map=self.residual_map,
+            noise_map=self.noise_map,
         )
 
     @property
     def chi_squared_map(self) -> np.ndarray:
         """
         Returns the chi-squared-map between the residual-map and noise-map, where:
 
         Chi_Squared = ((Residuals) / (Noise)) ** 2.0 = ((Data - Model)**2.0)/(Variances)
         """
-        return fit_util.chi_squared_map_complex_with_mask_from(
-            residual_map=self.residual_map, noise_map=self.noise_map, mask=self.mask
+        return fit_util.chi_squared_map_complex_from(
+            residual_map=self.residual_map,
+            noise_map=self.noise_map,
         )
 
     @property
     def signal_to_noise_map(self) -> np.ndarray:
-        """The signal-to-noise_map of the dataset and noise-map which are fitted."""
-        signal_to_noise_map_real = np.divide(
-            np.real(self.data), np.real(self.noise_map)
-        )
+        """
+        The signal-to-noise_map of the dataset and noise-map which are fitted."""
+        signal_to_noise_map_real = self.data.real / self.noise_map.real
+
         signal_to_noise_map_real[signal_to_noise_map_real < 0] = 0.0
-        signal_to_noise_map_imag = np.divide(
-            np.imag(self.data), np.imag(self.noise_map)
-        )
+        signal_to_noise_map_imag = self.data.imag / self.noise_map.imag
+
         signal_to_noise_map_imag[signal_to_noise_map_imag < 0] = 0.0
 
         return signal_to_noise_map_real + 1.0j * signal_to_noise_map_imag
 
     @property
     def chi_squared(self) -> float:
         """
         Returns the chi-squared terms of the model data's fit to an dataset, by summing the chi-squared-map.
         """
-        return fit_util.chi_squared_complex_with_mask_from(
-            chi_squared_map=self.chi_squared_map, mask=self.mask
+        return fit_util.chi_squared_complex_from(
+            chi_squared_map=self.chi_squared_map,
         )
 
     @property
     def noise_normalization(self) -> float:
         """
         Returns the noise-map normalization term of the noise-map, summing the noise_map value in every pixel as:
 
         [Noise_Term] = sum(log(2*pi*[Noise]**2.0))
         """
-        return fit_util.noise_normalization_complex_with_mask_from(
-            noise_map=self.noise_map, mask=self.mask
+        return fit_util.noise_normalization_complex_from(
+            noise_map=self.noise_map,
         )
 
     @property
     def dirty_image(self) -> Array2D:
         return self.transformer.image_from(visibilities=self.data)
 
     @property
```

### Comparing `autoarray-2024.1.27.4/autoarray/fit/fit_util.py` & `autoarray-2024.5.16.0/autoarray/fit/fit_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,109 @@
+from functools import wraps
+
 import numpy as np
 
+from autoarray.numpy_wrapper import numpy as npw
 from autoarray.mask.abstract_mask import Mask
 
+from autoarray import type as ty
+
+
+def to_new_array(func):
+    @wraps(func)
+    def wrapper(**kwargs):
+        result = func(**kwargs)
+        try:
+            return list(kwargs.values())[0].with_new_array(result)
+        except AttributeError:
+            return result
+
+    return wrapper
 
-def residual_map_from(*, data: np.ndarray, model_data: np.ndarray) -> np.ndarray:
+
+def residual_map_from(*, data: ty.DataLike, model_data: ty.DataLike) -> ty.DataLike:
     """
     Returns the residual-map of the fit of model-data to a masked dataset, where:
 
     Residuals = (Data - Model_Data).
 
     Parameters
     ----------
     data
         The data that is fitted.
     mask
         The mask applied to the dataset, where `False` entries are included in the calculation.
     model_data
         The model data used to fit the data.
     """
-    return np.subtract(data, model_data, out=np.zeros_like(data))
+    return data - model_data
 
 
 def normalized_residual_map_from(
-    *, residual_map: np.ndarray, noise_map: np.ndarray
-) -> np.ndarray:
+    *, residual_map: ty.DataLike, noise_map: ty.DataLike
+) -> ty.DataLike:
     """
     Returns the normalized residual-map of the fit of model-data to a masked dataset, where:
 
     Normalized_Residual = (Data - Model_Data) / Noise
 
     Parameters
     ----------
     residual_map
         The residual-map of the model-data fit to the dataset.
     noise_map
         The noise-map of the dataset.
     mask
         The mask applied to the residual-map, where `False` entries are included in the calculation.
     """
-    return np.divide(residual_map, noise_map, out=np.zeros_like(residual_map))
+    return residual_map / noise_map
 
 
 def chi_squared_map_from(
-    *, residual_map: np.ndarray, noise_map: np.ndarray
-) -> np.ndarray:
+    *, residual_map: ty.DataLike, noise_map: ty.DataLike
+) -> ty.DataLike:
     """
     Returns the chi-squared-map of the fit of model-data to a masked dataset, where:
 
     Chi_Squared = ((Residuals) / (Noise)) ** 2.0 = ((Data - Model)**2.0)/(Variances)
 
     Parameters
     ----------
     residual_map
         The residual-map of the model-data fit to the dataset.
     noise_map
         The noise-map of the dataset.
     """
-    return np.square(
-        np.divide(residual_map, noise_map, out=np.zeros_like(residual_map))
-    )
+    return (residual_map / noise_map) ** 2.0
 
 
-def chi_squared_from(*, chi_squared_map: np.ndarray) -> float:
+def chi_squared_from(*, chi_squared_map: ty.DataLike) -> float:
     """
     Returns the chi-squared terms of a model data's fit to an dataset, by summing the chi-squared-map.
 
     Parameters
     ----------
     chi_squared_map
         The chi-squared-map of values of the model-data fit to the dataset.
     """
     return float(np.sum(chi_squared_map))
 
 
-def noise_normalization_from(*, noise_map: np.ndarray) -> float:
+def noise_normalization_from(*, noise_map: ty.DataLike) -> float:
     """
     Returns the noise-map normalization term of the noise-map, summing the noise_map value in every pixel as:
 
     [Noise_Term] = sum(log(2*pi*[Noise]**2.0))
 
     Parameters
     ----------
     noise_map
         The masked noise-map of the dataset.
     """
-    return float(np.sum(np.log(2 * np.pi * noise_map**2.0)))
+    return npw.sum(npw.log(2 * np.pi * noise_map**2.0))
 
 
 def normalized_residual_map_complex_from(
     *, residual_map: np.ndarray, noise_map: np.ndarray
 ) -> np.ndarray:
     """
     Returns the normalized residual-map of the fit of complex model-data to a dataset, where:
@@ -98,24 +113,19 @@
     Parameters
     ----------
     residual_map
         The residual-map of the model-data fit to the dataset.
     noise_map
         The noise-map of the dataset.
     """
-    normalized_residual_map_real = np.divide(
-        residual_map.real,
-        noise_map.real,
-        out=np.zeros_like(residual_map, dtype="complex128"),
+    normalized_residual_map_real = (residual_map.real / noise_map.real).astype(
+        "complex128"
     )
-
-    normalized_residual_map_imag = np.divide(
-        residual_map.imag,
-        noise_map.imag,
-        out=np.zeros_like(residual_map, dtype="complex128"),
+    normalized_residual_map_imag = (residual_map.imag / noise_map.imag).astype(
+        "complex128"
     )
 
     return normalized_residual_map_real + 1j * normalized_residual_map_imag
 
 
 def chi_squared_map_complex_from(
     *, residual_map: np.ndarray, noise_map: np.ndarray
@@ -128,20 +138,16 @@
     Parameters
     ----------
     residual_map
         The residual-map of the model-data fit to the dataset.
     noise_map
         The noise-map of the dataset.
     """
-    chi_squared_map_real = np.square(
-        np.divide(residual_map.real, noise_map.real, out=np.zeros_like(residual_map))
-    )
-    chi_squared_map_imag = np.square(
-        np.divide(residual_map.imag, noise_map.imag, out=np.zeros_like(residual_map))
-    )
+    chi_squared_map_real = (residual_map.real / noise_map.real) ** 2
+    chi_squared_map_imag = (residual_map.imag / noise_map.imag) ** 2
     return chi_squared_map_real + 1j * chi_squared_map_imag
 
 
 def chi_squared_complex_from(*, chi_squared_map: np.ndarray) -> float:
     """
     Returns the chi-squared terms of each complex model data's fit to a masked dataset, by summing the masked
     chi-squared-map of the fit.
@@ -149,38 +155,39 @@
     The chi-squared values in masked pixels are omitted from the calculation.
 
     Parameters
     ----------
     chi_squared_map
         The chi-squared-map of values of the model-data fit to the dataset.
     """
-    chi_squared_real = float(np.sum(chi_squared_map.real))
-    chi_squared_imag = float(np.sum(chi_squared_map.imag))
+    chi_squared_real = np.sum(chi_squared_map.real)
+    chi_squared_imag = np.sum(chi_squared_map.imag)
     return chi_squared_real + chi_squared_imag
 
 
 def noise_normalization_complex_from(*, noise_map: np.ndarray) -> float:
     """
     Returns the noise-map normalization terms of a complex noise-map, summing the noise_map value in every pixel as:
 
     [Noise_Term] = sum(log(2*pi*[Noise]**2.0))
 
     Parameters
     ----------
     noise_map
         The masked noise-map of the dataset.
     """
-    noise_normalization_real = float(np.sum(np.log(2 * np.pi * noise_map.real**2.0)))
-    noise_normalization_imag = float(np.sum(np.log(2 * np.pi * noise_map.imag**2.0)))
+    noise_normalization_real = np.sum(np.log(2 * np.pi * noise_map.real**2.0))
+    noise_normalization_imag = np.sum(np.log(2 * np.pi * noise_map.imag**2.0))
     return noise_normalization_real + noise_normalization_imag
 
 
+@to_new_array
 def residual_map_with_mask_from(
-    *, data: np.ndarray, mask: Mask, model_data: np.ndarray
-) -> np.ndarray:
+    *, data: ty.DataLike, mask: Mask, model_data: ty.DataLike
+) -> ty.DataLike:
     """
     Returns the residual-map of the fit of model-data to a masked dataset, where:
 
     Residuals = (Data - Model_Data).
 
     The residual-map values in masked pixels are returned as zero.
 
@@ -194,17 +201,18 @@
         The model data used to fit the data.
     """
     return np.subtract(
         data, model_data, out=np.zeros_like(data), where=np.asarray(mask) == 0
     )
 
 
+@to_new_array
 def normalized_residual_map_with_mask_from(
-    *, residual_map: np.ndarray, noise_map: np.ndarray, mask: Mask
-) -> np.ndarray:
+    *, residual_map: ty.DataLike, noise_map: ty.DataLike, mask: Mask
+) -> ty.DataLike:
     """
     Returns the normalized residual-map of the fit of model-data to a masked dataset, where:
 
     Normalized_Residual = (Data - Model_Data) / Noise
 
     The normalized residual-map values in masked pixels are returned as zero.
 
@@ -221,17 +229,18 @@
         residual_map,
         noise_map,
         out=np.zeros_like(residual_map),
         where=np.asarray(mask) == 0,
     )
 
 
+@to_new_array
 def chi_squared_map_with_mask_from(
-    *, residual_map: np.ndarray, noise_map: np.ndarray, mask: Mask
-) -> np.ndarray:
+    *, residual_map: ty.DataLike, noise_map: ty.DataLike, mask: Mask
+) -> ty.DataLike:
     """
     Returnss the chi-squared-map of the fit of model-data to a masked dataset, where:
 
     Chi_Squared = ((Residuals) / (Noise)) ** 2.0 = ((Data - Model)**2.0)/(Variances)
 
     The chi-squared-map values in masked pixels are returned as zero.
 
@@ -250,15 +259,15 @@
             noise_map,
             out=np.zeros_like(residual_map),
             where=np.asarray(mask) == 0,
         )
     )
 
 
-def chi_squared_with_mask_from(*, chi_squared_map: np.ndarray, mask: Mask) -> float:
+def chi_squared_with_mask_from(*, chi_squared_map: ty.DataLike, mask: Mask) -> float:
     """
     Returns the chi-squared terms of each model data's fit to a masked dataset, by summing the masked
     chi-squared-map of the fit.
 
     The chi-squared values in masked pixels are omitted from the calculation.
 
     Parameters
@@ -268,15 +277,15 @@
     mask
         The mask applied to the chi-squared-map, where `False` entries are included in the calculation.
     """
     return float(np.sum(chi_squared_map[np.asarray(mask) == 0]))
 
 
 def chi_squared_with_mask_fast_from(
-    *, data: np.ndarray, mask: Mask, model_data: np.ndarray, noise_map: np.ndarray
+    *, data: ty.DataLike, mask: Mask, model_data: ty.DataLike, noise_map: ty.DataLike
 ) -> float:
     """
     Returns the chi-squared terms of each model data's fit to a masked dataset, by summing the masked
     chi-squared-map of the fit.
 
     The chi-squared values in masked pixels are omitted from the calculation.
 
@@ -290,15 +299,14 @@
     Parameters
     ----------
     chi_squared_map
         The chi-squared-map of values of the model-data fit to the dataset.
     mask
         The mask applied to the chi-squared-map, where `False` entries are included in the calculation.
     """
-
     return float(
         np.sum(
             np.square(
                 np.divide(
                     np.subtract(
                         data,
                         model_data,
@@ -306,15 +314,15 @@
                     noise_map[np.asarray(mask) == 0],
                 )
             )
         )
     )
 
 
-def noise_normalization_with_mask_from(*, noise_map: np.ndarray, mask: Mask) -> float:
+def noise_normalization_with_mask_from(*, noise_map: ty.DataLike, mask: Mask) -> float:
     """
     Returns the noise-map normalization terms of masked noise-map, summing the noise_map value in every pixel as:
 
     [Noise_Term] = sum(log(2*pi*[Noise]**2.0))
 
     The noise-map values in masked pixels are omitted from the calculation.
 
@@ -324,112 +332,16 @@
         The masked noise-map of the dataset.
     mask
         The mask applied to the noise-map, where `False` entries are included in the calculation.
     """
     return float(np.sum(np.log(2 * np.pi * noise_map[np.asarray(mask) == 0] ** 2.0)))
 
 
-def normalized_residual_map_complex_with_mask_from(
-    *, residual_map: np.ndarray, noise_map: np.ndarray, mask: Mask
-) -> np.ndarray:
-    """
-    Returns the normalized residual-map of the fit of complex model-data to a masked dataset, where:
-
-    Normalized_Residual = (Data - Model_Data) / Noise
-
-    The normalized residual-map values in masked pixels are returned as zero.
-
-    Parameters
-    ----------
-    residual_map
-        The residual-map of the model-data fit to the dataset.
-    noise_map
-        The noise-map of the dataset.
-    mask
-        The mask applied to the residual-map, where `False` entries are included in the calculation.
-    """
-    normalized_residual_map_real = np.divide(
-        residual_map.real,
-        noise_map.real,
-        out=np.zeros_like(residual_map.real),
-        where=np.asarray(mask) == 0,
-    )
-
-    normalized_residual_map_imag = np.divide(
-        residual_map.imag,
-        noise_map.imag,
-        out=np.zeros_like(residual_map.imag),
-        where=np.asarray(mask) == 0,
-    )
-
-    return normalized_residual_map_real + 1j * normalized_residual_map_imag
-
-
-def chi_squared_map_complex_with_mask_from(
-    *, residual_map: np.ndarray, noise_map: np.ndarray, mask: Mask
-) -> np.ndarray:
-    """
-    Returnss the chi-squared-map of the fit of complex model-data to a masked dataset, where:
-
-    Chi_Squared = ((Residuals) / (Noise)) ** 2.0 = ((Data - Model)**2.0)/(Variances)
-
-    The chi-squared-map values in masked pixels are returned as zero.
-
-    Parameters
-    ----------
-    residual_map
-        The residual-map of the model-data fit to the dataset.
-    noise_map
-        The noise-map of the dataset.
-    mask
-        The mask applied to the residual-map, where `False` entries are included in the calculation.
-    """
-
-    chi_squared_map_real = np.square(
-        np.divide(
-            residual_map.real,
-            noise_map.real,
-            out=np.zeros_like(residual_map.real),
-            where=np.asarray(mask) == 0,
-        )
-    )
-    chi_squared_map_imag = np.square(
-        np.divide(
-            residual_map.imag,
-            noise_map.imag,
-            out=np.zeros_like(residual_map.imag),
-            where=np.asarray(mask) == 0,
-        )
-    )
-    return chi_squared_map_real + 1j * chi_squared_map_imag
-
-
-def chi_squared_complex_with_mask_from(
-    *, chi_squared_map: np.ndarray, mask: Mask
-) -> float:
-    """
-    Returns the chi-squared terms of each complex model data's fit to a masked dataset, by summing the masked
-    chi-squared-map of the fit.
-
-    The chi-squared values in masked pixels are omitted from the calculation.
-
-    Parameters
-    ----------
-    chi_squared_map
-        The chi-squared-map of values of the model-data fit to the dataset.
-    mask
-        The mask applied to the chi-squared-map, where `False` entries are included in the calculation.
-    """
-    chi_squared_real = float(np.sum(chi_squared_map[np.asarray(mask) == 0].real))
-    chi_squared_imag = float(np.sum(chi_squared_map[np.asarray(mask) == 0].imag))
-    return chi_squared_real + chi_squared_imag
-
-
 def chi_squared_with_noise_covariance_from(
-    *, residual_map: np.ndarray, noise_covariance_matrix_inv: np.ndarray
+    *, residual_map: ty.DataLike, noise_covariance_matrix_inv: np.ndarray
 ) -> float:
     """
     Returns the chi-squared value of the fit of model-data to a masked dataset, where
     the noise correlation is described by a covariance matrix of n^2 x n^2 dimensions.
 
     Chi_Squared = r C^{-1} r, where C^{-1} is the inverse of the covariance matrix
 
@@ -440,54 +352,28 @@
     noise_covariance_matrix_inv
         The inverse of the noise covariance matrix.
     """
 
     return residual_map @ noise_covariance_matrix_inv @ residual_map
 
 
-def noise_normalization_complex_with_mask_from(
-    *, noise_map: np.ndarray, mask: Mask
-) -> float:
-    """
-    Returns the noise-map normalization terms of a complex masked noise-map, summing the noise_map value in every pixel as:
-
-    [Noise_Term] = sum(log(2*pi*[Noise]**2.0))
-
-    The noise-map values in masked pixels are omitted from the calculation.
-
-    Parameters
-    ----------
-    noise_map
-        The masked noise-map of the dataset.
-    mask
-        The mask applied to the noise-map, where `False` entries are included in the calculation.
-    """
-    noise_normalization_real = float(
-        np.sum(np.log(2 * np.pi * noise_map[np.asarray(mask) == 0].real ** 2.0))
-    )
-    noise_normalization_imag = float(
-        np.sum(np.log(2 * np.pi * noise_map[np.asarray(mask) == 0].imag ** 2.0))
-    )
-    return noise_normalization_real + noise_normalization_imag
-
-
 def log_likelihood_from(*, chi_squared: float, noise_normalization: float) -> float:
     """
     Returns the log likelihood of each model data point's fit to the dataset, where:
 
     Log Likelihood = -0.5*[Chi_Squared_Term + Noise_Term] (see functions above for these definitions)
 
     Parameters
     ----------
     chi_squared
         The chi-squared term for the model-data fit to the dataset.
     noise_normalization
         The normalization noise_map-term for the dataset's noise-map.
     """
-    return float(-0.5 * (chi_squared + noise_normalization))
+    return -0.5 * (chi_squared + noise_normalization)
 
 
 def log_likelihood_with_regularization_from(
     *, chi_squared: float, regularization_term: float, noise_normalization: float
 ) -> float:
     """
     Returns the log likelihood of an inversion's fit to the dataset, including a regularization term which comes from
@@ -501,15 +387,15 @@
         The chi-squared term of the inversion's fit to the dataset.
     regularization_term
         The regularization term of the inversion, which is the sum of the difference between reconstructed
         flux of every pixel multiplied by the regularization coefficient.
     noise_normalization
         The normalization noise_map-term for the dataset's noise-map.
     """
-    return float(-0.5 * (chi_squared + regularization_term + noise_normalization))
+    return -0.5 * (chi_squared + regularization_term + noise_normalization)
 
 
 def log_evidence_from(
     *,
     chi_squared: float,
     regularization_term: float,
     log_curvature_regularization_term: float,
@@ -533,23 +419,20 @@
     log_curvature_regularization_term
         The log of the determinant of the sum of the curvature and regularization matrices.
     log_regularization_term
         The log of the determinant o the regularization matrix.
     noise_normalization
         The normalization noise_map-term for the dataset's noise-map.
     """
-    return float(
-        -0.5
-        * (
-            chi_squared
-            + regularization_term
-            + log_curvature_regularization_term
-            - log_regularization_term
-            + noise_normalization
-        )
+    return -0.5 * (
+        chi_squared
+        + regularization_term
+        + log_curvature_regularization_term
+        - log_regularization_term
+        + noise_normalization
     )
 
 
 def residual_flux_fraction_map_from(
     *, residual_map: np.ndarray, data: np.ndarray
 ) -> np.ndarray:
     """
```

### Comparing `autoarray-2024.1.27.4/autoarray/fit/mock/mock_fit_imaging.py` & `autoarray-2024.5.16.0/autoarray/fit/mock/mock_fit_imaging.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 from typing import Dict, Optional
 
 from autoarray.dataset.mock.mock_dataset import MockDataset
+from autoarray.dataset.dataset_model import DatasetModel
 from autoarray.fit.fit_imaging import FitImaging
 
 
 class MockFitImaging(FitImaging):
     def __init__(
         self,
         dataset=MockDataset(),
+        dataset_model: Optional[DatasetModel] = None,
         use_mask_in_fit: bool = False,
         noise_map=None,
         model_data=None,
         inversion=None,
         blurred_image=None,
         run_time_dict: Optional[Dict] = None,
     ):
         super().__init__(
             dataset=dataset,
+            dataset_model=dataset_model,
             use_mask_in_fit=use_mask_in_fit,
             run_time_dict=run_time_dict,
         )
 
         self._noise_map = noise_map
         self._model_data = model_data
         self._inversion = inversion
         self._blurred_image = blurred_image
 
     @property
-    def noise_map(self):
-        return self._noise_map if self._noise_map is not None else super().noise_map
-
-    @property
     def model_data(self):
         return self._model_data
 
     @property
+    def noise_map(self):
+        return self._noise_map if self._noise_map is not None else super().noise_map
+
+    @property
     def inversion(self):
         return self._inversion if self._inversion is not None else super().inversion
 
     @property
     def blurred_image(self):
-        return (
-            self._blurred_image
-            if self._blurred_image is not None
-            else super().blurred_image
-        )
+        return self._blurred_image if self._blurred_image is not None else None
```

### Comparing `autoarray-2024.1.27.4/autoarray/fit/mock/mock_fit_interferometer.py` & `autoarray-2024.5.16.0/autoarray/fit/mock/mock_fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/fit/plot/fit_imaging_plotters.py` & `autoarray-2024.5.16.0/autoarray/fit/plot/fit_imaging_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/fit/plot/fit_interferometer_plotters.py` & `autoarray-2024.5.16.0/autoarray/fit/plot/fit_interferometer_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/fit/plot/fit_vector_yx_plotters.py` & `autoarray-2024.5.16.0/autoarray/fit/plot/fit_vector_yx_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/fixtures.py` & `autoarray-2024.5.16.0/autoarray/fixtures.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,15 @@
 
 import autoarray as aa
 
 
 def make_mask_1d_7():
     mask = np.array([True, True, False, False, False, True, True])
 
-    return aa.Mask1D(mask=mask, pixel_scales=(1.0,), sub_size=1)
-
-
-def make_sub_mask_1d_7():
-    mask = np.array([True, True, False, False, False, True, True])
-
-    return aa.Mask1D(mask=mask, pixel_scales=(1.0,), sub_size=2)
+    return aa.Mask1D(mask=mask, pixel_scales=(1.0,))
 
 
 def make_mask_2d_7x7():
     mask = np.array(
         [
             [True, True, True, True, True, True, True],
             [True, True, True, True, True, True, True],
@@ -24,31 +18,15 @@
             [True, True, False, False, False, True, True],
             [True, True, False, False, False, True, True],
             [True, True, True, True, True, True, True],
             [True, True, True, True, True, True, True],
         ]
     )
 
-    return aa.Mask2D(mask=mask, pixel_scales=(1.0, 1.0), sub_size=1)
-
-
-def make_sub_mask_2d_7x7():
-    mask = np.array(
-        [
-            [True, True, True, True, True, True, True],
-            [True, True, True, True, True, True, True],
-            [True, True, False, False, False, True, True],
-            [True, True, False, False, False, True, True],
-            [True, True, False, False, False, True, True],
-            [True, True, True, True, True, True, True],
-            [True, True, True, True, True, True, True],
-        ]
-    )
-
-    return aa.Mask2D(mask=mask, sub_size=2, pixel_scales=(1.0, 1.0))
+    return aa.Mask2D(mask=mask, pixel_scales=(1.0, 1.0))
 
 
 def make_mask_2d_7x7_1_pix():
     mask = np.array(
         [
             [True, True, True, True, True, True, True],
             [True, True, True, True, True, True, True],
@@ -103,39 +81,25 @@
 # GRIDS #
 
 
 def make_grid_1d_7():
     return aa.Grid1D.from_mask(mask=make_mask_1d_7())
 
 
-def make_sub_grid_1d_7():
-    return aa.Grid1D.from_mask(mask=make_sub_mask_1d_7())
-
-
 def make_grid_2d_7x7():
     return aa.Grid2D.from_mask(mask=make_mask_2d_7x7())
 
 
-def make_sub_grid_2d_7x7():
-    return aa.Grid2D.from_mask(mask=make_sub_mask_2d_7x7())
-
-
-def make_grid_2d_iterate_7x7():
-    return aa.Grid2DIterate.from_mask(
-        mask=make_mask_2d_7x7(), fractional_accuracy=0.9999, sub_steps=[2, 4, 8, 16]
-    )
-
-
-def make_sub_grid_2d_7x7_simple():
-    sub_grid_2d_7x7 = make_sub_grid_2d_7x7()
-    sub_grid_2d_7x7[0] = np.array([1.0, 1.0])
-    sub_grid_2d_7x7[1] = np.array([1.0, 0.0])
-    sub_grid_2d_7x7[2] = np.array([1.0, 1.0])
-    sub_grid_2d_7x7[3] = np.array([1.0, 0.0])
-    return sub_grid_2d_7x7
+def make_grid_2d_7x7_simple():
+    grid_2d_7x7 = make_grid_2d_7x7()
+    grid_2d_7x7[0] = np.array([1.0, 1.0])
+    grid_2d_7x7[1] = np.array([1.0, 0.0])
+    grid_2d_7x7[2] = np.array([1.0, 1.0])
+    grid_2d_7x7[3] = np.array([1.0, 0.0])
+    return grid_2d_7x7
 
 
 def make_blurring_grid_2d_7x7():
     return aa.Grid2D.from_mask(mask=make_blurring_mask_2d_7x7())
 
 
 # CONVOLVERS #
@@ -184,30 +148,51 @@
 
 
 def make_imaging_7x7():
     return aa.Imaging(
         data=make_image_7x7(),
         psf=make_psf_3x3(),
         noise_map=make_noise_map_7x7(),
+        over_sampling=aa.OverSamplingUniform(sub_size=1),
+    )
+
+
+def make_imaging_7x7_sub_2():
+    return aa.Imaging(
+        data=make_image_7x7(),
+        psf=make_psf_3x3(),
+        noise_map=make_noise_map_7x7(),
+        over_sampling=aa.OverSamplingUniform(sub_size=2),
     )
 
 
 def make_imaging_covariance_7x7():
     return aa.Imaging(
         data=make_image_7x7(),
         psf=make_psf_3x3(),
         noise_covariance_matrix=make_noise_covariance_matrix_7x7(),
+        over_sampling=aa.OverSamplingUniform(sub_size=1),
     )
 
 
 def make_imaging_7x7_no_blur():
     return aa.Imaging(
         data=make_image_7x7(),
         psf=make_psf_3x3_no_blur(),
         noise_map=make_noise_map_7x7(),
+        over_sampling=aa.OverSamplingUniform(sub_size=1),
+    )
+
+
+def make_imaging_7x7_no_blur_sub_2():
+    return aa.Imaging(
+        data=make_image_7x7(),
+        psf=make_psf_3x3_no_blur(),
+        noise_map=make_noise_map_7x7(),
+        over_sampling=aa.OverSamplingUniform(sub_size=2),
     )
 
 
 def make_visibilities_7():
     return aa.Visibilities.full(shape_slim=(7,), fill_value=1.0)
 
 
@@ -234,54 +219,49 @@
 
 
 def make_interferometer_7():
     return aa.Interferometer(
         data=make_visibilities_7(),
         noise_map=make_visibilities_noise_map_7(),
         uv_wavelengths=make_uv_wavelengths_7x2(),
-        real_space_mask=make_sub_mask_2d_7x7(),
-        settings=aa.SettingsInterferometer(
-            grid_class=aa.Grid2D, sub_size=1, transformer_class=aa.TransformerDFT
-        ),
+        real_space_mask=make_mask_2d_7x7(),
+        transformer_class=aa.TransformerDFT,
+        over_sampling_pixelization=aa.OverSamplingUniform(sub_size=1),
     )
 
 
 def make_interferometer_7_no_fft():
     return aa.Interferometer(
         data=make_visibilities_7(),
         noise_map=make_visibilities_noise_map_7(),
         uv_wavelengths=make_uv_wavelengths_7x2_no_fft(),
-        real_space_mask=make_sub_mask_2d_7x7(),
-        settings=aa.SettingsInterferometer(
-            grid_class=aa.Grid2D, sub_size=1, transformer_class=aa.TransformerDFT
-        ),
+        real_space_mask=make_mask_2d_7x7(),
+        transformer_class=aa.TransformerDFT,
+        over_sampling_pixelization=aa.OverSamplingUniform(sub_size=1),
     )
 
 
 def make_interferometer_7_grid():
     return aa.Interferometer(
         data=make_visibilities_7(),
         noise_map=make_visibilities_noise_map_7(),
         uv_wavelengths=make_uv_wavelengths_7x2(),
-        real_space_mask=make_sub_mask_2d_7x7(),
-        settings=aa.SettingsInterferometer(
-            sub_size=1, transformer_class=aa.TransformerDFT
-        ),
+        real_space_mask=make_mask_2d_7x7(),
+        transformer_class=aa.TransformerDFT,
+        over_sampling_pixelization=aa.OverSamplingUniform(sub_size=1),
     )
 
 
 def make_interferometer_7_lop():
     return aa.Interferometer(
         data=make_visibilities_7(),
         noise_map=make_visibilities_noise_map_7(),
         uv_wavelengths=make_uv_wavelengths_7x2(),
         real_space_mask=make_mask_2d_7x7(),
-        settings=aa.SettingsInterferometer(
-            sub_size_pixelization=1, transformer_class=aa.TransformerNUFFT
-        ),
+        transformer_class=aa.TransformerNUFFT,
     )
 
 
 def make_transformer_7x7_7():
     return aa.TransformerDFT(
         uv_wavelengths=make_uv_wavelengths_7x2(), real_space_mask=make_mask_2d_7x7()
     )
@@ -304,14 +284,20 @@
 
 def make_masked_imaging_7x7_no_blur():
     imaging_7x7 = make_imaging_7x7_no_blur()
 
     return imaging_7x7.apply_mask(mask=make_mask_2d_7x7())
 
 
+def make_masked_imaging_7x7_no_blur_sub_2():
+    imaging_7x7 = make_imaging_7x7_no_blur_sub_2()
+
+    return imaging_7x7.apply_mask(mask=make_mask_2d_7x7())
+
+
 def make_model_image_7x7():
     imaging_7x7 = make_masked_imaging_7x7()
 
     return 5.0 * imaging_7x7.data
 
 
 def make_imaging_fit_x1_plane_7x7():
@@ -323,15 +309,15 @@
         dataset=imaging_7x7, use_mask_in_fit=False, model_data=model_data
     )
 
 
 def make_fit_interferometer_7():
     interferometer_7 = make_interferometer_7()
 
-    model_data = 5.0 * interferometer_7.visibilities
+    model_data = 5.0 * interferometer_7.data
 
     return aa.m.MockFitInterferometer(
         dataset=interferometer_7, use_mask_in_fit=False, model_data=model_data
     )
 
 
 def make_regularization_constant():
@@ -364,15 +350,15 @@
 
 def make_regularization_matern_kernel():
     return aa.reg.MaternKernel(coefficient=1.0, scale=0.5, nu=0.7)
 
 
 def make_rectangular_mesh_grid_3x3():
     return aa.Mesh2DRectangular.overlay_grid(
-        grid=make_sub_grid_2d_7x7(), shape_native=(3, 3)
+        grid=make_over_sampler_2d_7x7().over_sampled_grid, shape_native=(3, 3)
     )
 
 
 def make_delaunay_mesh_grid_9():
     grid_9 = aa.Grid2D.no_mask(
         values=[
             [0.6, -0.3],
@@ -410,62 +396,90 @@
     )
 
     return aa.Mesh2DVoronoi(
         values=grid_9,
     )
 
 
+def make_over_sampler_2d_7x7():
+    return aa.OverSamplerUniform(mask=make_mask_2d_7x7(), sub_size=2)
+
+
+def make_border_relocator_2d_7x7():
+    return aa.BorderRelocator(
+        mask=make_mask_2d_7x7(), sub_size=np.array([2, 2, 2, 2, 2, 2, 2, 2, 2])
+    )
+
+
 def make_rectangular_mapper_7x7_3x3():
     mapper_grids = aa.MapperGrids(
-        source_plane_data_grid=make_sub_grid_2d_7x7(),
+        mask=make_mask_2d_7x7(),
+        source_plane_data_grid=make_over_sampler_2d_7x7().over_sampled_grid,
         source_plane_mesh_grid=make_rectangular_mesh_grid_3x3(),
         image_plane_mesh_grid=None,
         adapt_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
     )
 
     return aa.MapperRectangularNoInterp(
-        mapper_grids=mapper_grids, regularization=make_regularization_constant()
+        mapper_grids=mapper_grids,
+        over_sampler=make_over_sampler_2d_7x7(),
+        border_relocator=make_border_relocator_2d_7x7(),
+        regularization=make_regularization_constant(),
     )
 
 
 def make_delaunay_mapper_9_3x3():
     mapper_grids = aa.MapperGrids(
-        source_plane_data_grid=make_sub_grid_2d_7x7(),
+        mask=make_mask_2d_7x7(),
+        source_plane_data_grid=make_over_sampler_2d_7x7().over_sampled_grid,
         source_plane_mesh_grid=make_delaunay_mesh_grid_9(),
         image_plane_mesh_grid=aa.Grid2D.uniform(shape_native=(3, 3), pixel_scales=0.1),
         adapt_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
     )
 
     return aa.MapperDelaunay(
-        mapper_grids=mapper_grids, regularization=make_regularization_constant()
+        mapper_grids=mapper_grids,
+        over_sampler=make_over_sampler_2d_7x7(),
+        border_relocator=make_border_relocator_2d_7x7(),
+        regularization=make_regularization_constant(),
     )
 
 
 def make_voronoi_mapper_9_3x3():
     mapper_grids = aa.MapperGrids(
-        source_plane_data_grid=make_sub_grid_2d_7x7(),
+        mask=make_mask_2d_7x7(),
+        source_plane_data_grid=make_over_sampler_2d_7x7().over_sampled_grid,
         source_plane_mesh_grid=make_voronoi_mesh_grid_9(),
         image_plane_mesh_grid=aa.Grid2D.uniform(shape_native=(3, 3), pixel_scales=0.1),
         adapt_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
     )
 
     return aa.MapperVoronoiNoInterp(
-        mapper_grids=mapper_grids, regularization=make_regularization_constant()
+        mapper_grids=mapper_grids,
+        over_sampler=make_over_sampler_2d_7x7(),
+        border_relocator=make_border_relocator_2d_7x7(),
+        regularization=make_regularization_constant(),
     )
 
 
 def make_voronoi_mapper_nn_9_3x3():
     mapper_grids = aa.MapperGrids(
-        source_plane_data_grid=make_sub_grid_2d_7x7(),
+        mask=make_mask_2d_7x7(),
+        source_plane_data_grid=make_over_sampler_2d_7x7().over_sampled_grid,
         source_plane_mesh_grid=make_voronoi_mesh_grid_9(),
         image_plane_mesh_grid=aa.Grid2D.uniform(shape_native=(3, 3), pixel_scales=0.1),
         adapt_data=aa.Array2D.ones(shape_native=(3, 3), pixel_scales=0.1),
     )
 
-    return aa.MapperVoronoi(mapper_grids=mapper_grids, regularization=None)
+    return aa.MapperVoronoi(
+        mapper_grids=mapper_grids,
+        over_sampler=make_over_sampler_2d_7x7(),
+        border_relocator=make_border_relocator_2d_7x7(),
+        regularization=None,
+    )
 
 
 def make_rectangular_inversion_7x7_3x3():
     return aa.Inversion(
         dataset=make_masked_imaging_7x7(),
         linear_obj_list=[make_rectangular_mapper_7x7_3x3()],
     )
```

### Comparing `autoarray-2024.1.27.4/autoarray/geometry/abstract_2d.py` & `autoarray-2024.5.16.0/autoarray/geometry/abstract_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/geometry/geometry_1d.py` & `autoarray-2024.5.16.0/autoarray/geometry/geometry_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/geometry/geometry_2d.py` & `autoarray-2024.5.16.0/autoarray/geometry/geometry_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import logging
 from typing import TYPE_CHECKING, Tuple
 
 if TYPE_CHECKING:
     from autoarray.structures.arrays.uniform_2d import Array2D
     from autoarray.structures.grids.uniform_2d import Grid2D
 
+import numpy as np
+
 from autoarray.geometry.abstract_2d import AbstractGeometry2D
 
 from autoarray import type as ty
 from autoarray.geometry import geometry_util
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
@@ -202,15 +204,15 @@
         ----------
         grid_scaled_2d
             A grid of (y,x) coordinates in scaled units.
         """
         from autoarray.structures.grids.uniform_2d import Grid2D
 
         grid_pixels_2d = geometry_util.grid_pixels_2d_slim_from(
-            grid_scaled_2d_slim=grid_scaled_2d,
+            grid_scaled_2d_slim=np.array(grid_scaled_2d),
             shape_native=self.shape_native,
             pixel_scales=self.pixel_scales,
             origin=self.origin,
         )
         return Grid2D(values=grid_pixels_2d, mask=grid_scaled_2d.mask)
 
     def grid_pixel_centres_2d_from(self, grid_scaled_2d: Grid2D) -> Grid2D:
@@ -228,15 +230,15 @@
         ----------
         grid_scaled_2d
             The grid of (y,x) coordinates in scaled units.
         """
         from autoarray.structures.grids.uniform_2d import Grid2D
 
         grid_pixel_centres_1d = geometry_util.grid_pixel_centres_2d_slim_from(
-            grid_scaled_2d_slim=grid_scaled_2d,
+            grid_scaled_2d_slim=np.array(grid_scaled_2d),
             shape_native=self.shape_native,
             pixel_scales=self.pixel_scales,
             origin=self.origin,
         ).astype("int")
 
         return Grid2D(values=grid_pixel_centres_1d, mask=grid_scaled_2d.mask)
 
@@ -261,15 +263,15 @@
         grid_scaled_2d
             The grid of (y,x) coordinates in scaled units.
         """
 
         from autoarray.structures.arrays.uniform_2d import Array2D
 
         grid_pixel_indexes_2d = geometry_util.grid_pixel_indexes_2d_slim_from(
-            grid_scaled_2d_slim=grid_scaled_2d,
+            grid_scaled_2d_slim=np.array(grid_scaled_2d),
             shape_native=self.shape_native,
             pixel_scales=self.pixel_scales,
             origin=self.origin,
         ).astype("int")
 
         return Array2D(values=grid_pixel_indexes_2d, mask=grid_scaled_2d.mask)
 
@@ -287,13 +289,13 @@
         ----------
         grid_pixels_2d
             The grid of (y,x) coordinates in pixels.
         """
         from autoarray.structures.grids.uniform_2d import Grid2D
 
         grid_scaled_1d = geometry_util.grid_scaled_2d_slim_from(
-            grid_pixels_2d_slim=grid_pixels_2d,
+            grid_pixels_2d_slim=np.array(grid_pixels_2d),
             shape_native=self.shape_native,
             pixel_scales=self.pixel_scales,
             origin=self.origin,
         )
         return Grid2D(values=grid_scaled_1d, mask=grid_pixels_2d.mask)
```

### Comparing `autoarray-2024.1.27.4/autoarray/geometry/geometry_2d_irregular.py` & `autoarray-2024.5.16.0/autoarray/geometry/geometry_2d_irregular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/geometry/geometry_util.py` & `autoarray-2024.5.16.0/autoarray/geometry/geometry_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
      2) A rotation of the grid around this new centre, which is performed clockwise from an input angle.
 
     Parameters
     ----------
     grid
         The 2d grid of (y, x) coordinates which are transformed to a new reference frame.
     """
-    shifted_grid_2d = np.subtract(grid_2d, centre)
+    shifted_grid_2d = grid_2d - centre
     radius = np.sqrt(np.sum(shifted_grid_2d**2.0, 1))
     theta_coordinate_to_profile = np.arctan2(
         shifted_grid_2d[:, 0], shifted_grid_2d[:, 1]
     ) - np.radians(angle)
     return np.vstack(
         radius
         * (np.sin(theta_coordinate_to_profile), np.cos(theta_coordinate_to_profile))
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/abstract.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from scipy.sparse import csc_matrix
 from scipy.sparse.linalg import splu
 from typing import Dict, List, Optional, Tuple, Type, Union
 
 from autoconf import cached_property
 from autoarray.numba_util import profile_func
 
+from autoarray.dataset.imaging.dataset import Imaging
+from autoarray.dataset.interferometer.dataset import Interferometer
+from autoarray.inversion.inversion.dataset_interface import DatasetInterface
 from autoarray.inversion.linear_obj.linear_obj import LinearObj
-from autoarray.inversion.linear_obj.func_list import AbstractLinearObjFuncList
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.inversion.regularization.abstract import AbstractRegularization
 from autoarray.inversion.inversion.settings import SettingsInversion
 from autoarray.structures.arrays.uniform_2d import Array2D
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 from autoarray.structures.visibilities import Visibilities
 
@@ -22,16 +24,15 @@
 from autoarray.util import misc_util
 from autoarray.inversion.inversion import inversion_util
 
 
 class AbstractInversion:
     def __init__(
         self,
-        data: Union[Visibilities, Array2D],
-        noise_map: Union[Visibilities, Array2D],
+        dataset: Union[Imaging, Interferometer, DatasetInterface],
         linear_obj_list: List[LinearObj],
         settings: SettingsInversion = SettingsInversion(),
         preloads: Optional["Preloads"] = None,
         run_time_dict: Optional[Dict] = None,
     ):
         """
         An `Inversion` reconstructs an input dataset using a list of linear objects (e.g. a list of analytic functions
@@ -76,35 +77,42 @@
             A dictionary which contains timing of certain functions calls which is used for profiling.
         """
 
         from autoarray.preloads import Preloads
 
         preloads = preloads or Preloads()
 
-        try:
-            import numba
-        except ModuleNotFoundError:
-            raise exc.InversionException(
-                "Inversion functionality (linear light profiles, pixelized reconstructions) is "
-                "disabled if numba is not installed.\n\n"
-                "This is because the run-times without numba are too slow.\n\n"
-                "Please install numba, which is described at the following web page:\n\n"
-                "https://pyautolens.readthedocs.io/en/latest/installation/overview.html"
-            )
+        # try:
+        #     import numba
+        # except ModuleNotFoundError:
+        #     raise exc.InversionException(
+        #         "Inversion functionality (linear light profiles, pixelized reconstructions) is "
+        #         "disabled if numba is not installed.\n\n"
+        #         "This is because the run-times without numba are too slow.\n\n"
+        #         "Please install numba, which is described at the following web page:\n\n"
+        #         "https://pyautolens.readthedocs.io/en/latest/installation/overview.html"
+        #     )
 
-        self.data = data
-        self.noise_map = noise_map
+        self.dataset = dataset
 
         self.linear_obj_list = linear_obj_list
 
         self.settings = settings
 
         self.preloads = preloads
         self.run_time_dict = run_time_dict
 
+    @property
+    def data(self):
+        return self.dataset.data
+
+    @property
+    def noise_map(self):
+        return self.dataset.noise_map
+
     def has(self, cls: Type) -> bool:
         """
         Does this `Inversion` have an attribute which is of type `cls`?
 
         Parameters
         ----------
         dict_values
@@ -842,39 +850,64 @@
 
             magnification_list.append(
                 np.sum(mapped_reconstructed_image) / np.sum(interpolated_reconstruction)
             )
 
         return magnification_list
 
-    @property
-    def brightest_reconstruction_pixel_list(self):
-        brightest_reconstruction_pixel_list = []
+    def brightest_pixel_list_from(
+        self, total_pixels: int = 1, filter_neighbors: bool = False
+    ) -> List[List[int]]:
+        brightest_pixel_list = []
 
         for mapper in self.cls_list_from(cls=AbstractMapper):
-            brightest_reconstruction_pixel_list.append(
-                np.argmax(self.reconstruction_dict[mapper])
+            pixel_list = []
+
+            pixels_ascending_list = list(
+                reversed(np.argsort(self.reconstruction_dict[mapper]))
             )
 
-        return brightest_reconstruction_pixel_list
+            for pixel in range(total_pixels):
+                pixel_index = pixels_ascending_list[pixel]
+
+                add_pixel = True
+
+                if filter_neighbors:
+                    pixel_neighbors = mapper.neighbors[pixel_index]
+                    pixel_neighbors = pixel_neighbors[pixel_neighbors >= 0]
+
+                    brightness = self.reconstruction_dict[mapper][pixel_index]
+                    brightness_neighbors = self.reconstruction_dict[mapper][
+                        pixel_neighbors
+                    ]
+
+                    if brightness < np.max(brightness_neighbors):
+                        add_pixel = False
+
+                if add_pixel:
+                    pixel_list.append(pixel_index)
+
+            brightest_pixel_list.append(pixel_list)
+
+        return brightest_pixel_list
 
     @property
-    def brightest_reconstruction_pixel_centre_list(self):
-        brightest_reconstruction_pixel_centre_list = []
+    def brightest_pixel_centre_list(self):
+        brightest_pixel_centre_list = []
 
         for mapper in self.cls_list_from(cls=AbstractMapper):
             brightest_reconstruction_pixel = np.argmax(self.reconstruction_dict[mapper])
 
             centre = Grid2DIrregular(
                 values=[mapper.source_plane_mesh_grid[brightest_reconstruction_pixel]]
             )
 
-            brightest_reconstruction_pixel_centre_list.append(centre)
+            brightest_pixel_centre_list.append(centre)
 
-        return brightest_reconstruction_pixel_centre_list
+        return brightest_pixel_centre_list
 
     def regularization_weights_from(self, index: int) -> np.ndarray:
         linear_obj = self.linear_obj_list[index]
         regularization = self.regularization_list[index]
 
         if regularization is None:
             pixels = linear_obj.params
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/factory.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 from typing import Dict, List, Optional, Union
 
 from autoarray.dataset.imaging.dataset import Imaging
-from autoarray.dataset.imaging.w_tilde import WTildeImaging
-from autoarray.dataset.interferometer.w_tilde import WTildeInterferometer
-from autoarray.structures.arrays.uniform_2d import Array2D
-from autoarray.structures.visibilities import Visibilities
-from autoarray.structures.visibilities import VisibilitiesNoiseMap
-from autoarray.operators.convolver import Convolver
-from autoarray.operators.transformer import TransformerDFT
-from autoarray.operators.transformer import TransformerNUFFT
-from autoarray.inversion.linear_obj.linear_obj import LinearObj
-from autoarray.inversion.linear_obj.func_list import AbstractLinearObjFuncList
-from autoarray.inversion.inversion.imaging.w_tilde import InversionImagingWTilde
+from autoarray.dataset.interferometer.dataset import Interferometer
 from autoarray.inversion.inversion.imaging.mapping import InversionImagingMapping
 from autoarray.inversion.inversion.interferometer.mapping import (
     InversionInterferometerMapping,
 )
 from autoarray.inversion.inversion.interferometer.w_tilde import (
     InversionInterferometerWTilde,
 )
 from autoarray.inversion.inversion.interferometer.lop import (
     InversionInterferometerMappingPyLops,
 )
+from autoarray.inversion.inversion.dataset_interface import DatasetInterface
+from autoarray.inversion.linear_obj.linear_obj import LinearObj
+from autoarray.inversion.linear_obj.func_list import AbstractLinearObjFuncList
+from autoarray.inversion.inversion.imaging.w_tilde import InversionImagingWTilde
 from autoarray.inversion.inversion.settings import SettingsInversion
+from autoarray.structures.arrays.uniform_2d import Array2D
 from autoarray.preloads import Preloads
 
 
 def inversion_from(
-    dataset,
+    dataset: Union[Imaging, Interferometer, DatasetInterface],
     linear_obj_list: List[LinearObj],
     settings: SettingsInversion = SettingsInversion(),
     preloads: Preloads = Preloads(),
     run_time_dict: Optional[Dict] = None,
 ):
     """
     Factory which given an input dataset and list of linear objects, creates an `Inversion`.
@@ -62,125 +57,33 @@
     run_time_dict
         A dictionary which contains timing of certain functions calls which is used for profiling.
 
     Returns
     -------
     An `Inversion` whose type is determined by the input `dataset` and `settings`.
     """
-    if settings.use_w_tilde:
-        w_tilde = dataset.w_tilde
-    else:
-        w_tilde = None
-
-    if isinstance(dataset, Imaging):
-        return inversion_imaging_unpacked_from(
-            data=dataset.data,
-            noise_map=dataset.noise_map,
-            convolver=dataset.convolver,
-            w_tilde=w_tilde,
+    if isinstance(dataset.data, Array2D):
+        return inversion_imaging_from(
+            dataset=dataset,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
-    return inversion_interferometer_unpacked_from(
-        data=dataset.visibilities,
-        noise_map=dataset.noise_map,
-        transformer=dataset.transformer,
-        w_tilde=w_tilde,
+    return inversion_interferometer_from(
+        dataset=dataset,
         linear_obj_list=linear_obj_list,
         settings=settings,
         run_time_dict=run_time_dict,
     )
 
 
-def inversion_unpacked_from(
+def inversion_imaging_from(
     dataset,
-    data: Union[Array2D, Visibilities],
-    noise_map: Union[Array2D, VisibilitiesNoiseMap],
-    w_tilde: Union[WTildeImaging, WTildeInterferometer],
-    linear_obj_list: List[LinearObj],
-    settings: SettingsInversion = SettingsInversion(),
-    preloads: Preloads = Preloads(),
-    run_time_dict: Optional[Dict] = None,
-):
-    """
-    Factory which given an input dataset and list of linear objects, creates an `Inversion`.
-
-    Unlike the `inversion_from` factory this function takes the `data`, `noise_map` and `w_tilde` objects as separate
-    inputs, which facilitates certain computations where the `dataset` object is unpacked before the `Inversion` is
-    performed (for example if the noise-map is scaled before the inversion to downweight certain regions of the
-    data).
-
-    An `Inversion` reconstructs the input dataset using a list of linear objects (e.g. a list of analytic functions
-    or a pixelized grid). The inversion solves for the values of these linear objects that best reconstruct the
-    dataset, via linear matrix algebra.
-
-    Different `Inversion` objects are used for different dataset types (e.g. `Imaging`, `Interferometer`) and
-    for different linear algebra formalisms (determined via the input `settings`) which solve for the linear object
-    parameters in different ways.
-
-    This factory inspects the type of dataset input and settings of the inversion in order to create the appropriate
-    inversion object.
-
-    Parameters
-    ----------
-    dataset
-        The dataset (e.g. `Imaging`, `Interferometer`) whose data is reconstructed via the `Inversion`.
-    data
-        The data of the dataset (e.g. the `image` of `Imaging` data) which may have been changed.
-    noise_map
-        The noise_map of the noise_mapset (e.g. the `noise_map` of `Imaging` noise_map) which may have been changed.
-    w_tilde
-        Object which uses the dataset's operated (e.g. the PSF of `Imaging`) to perform the `Inversion` using the
-        w-tilde formalism.
-    linear_obj_list
-        The list of linear objects (e.g. analytic functions, a mapper with a pixelized grid) which reconstruct the
-        input dataset's data and whose values are solved for via the inversion.
-    settings
-        Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
-    preloads
-        Preloads in memory certain arrays which may be known beforehand in order to speed up the calculation,
-        for example certain matrices used by the linear algebra could be preloaded.
-    run_time_dict
-        A dictionary which contains timing of certain functions calls which is used for profiling.
-
-    Returns
-    -------
-    An `Inversion` whose type is determined by the input `dataset` and `settings`.
-    """
-    if isinstance(dataset, Imaging):
-        return inversion_imaging_unpacked_from(
-            data=data,
-            noise_map=noise_map,
-            convolver=dataset.convolver,
-            w_tilde=w_tilde,
-            linear_obj_list=linear_obj_list,
-            settings=settings,
-            preloads=preloads,
-            run_time_dict=run_time_dict,
-        )
-
-    return inversion_interferometer_unpacked_from(
-        data=data,
-        noise_map=noise_map,
-        transformer=dataset.transformer,
-        w_tilde=w_tilde,
-        linear_obj_list=linear_obj_list,
-        settings=settings,
-        run_time_dict=run_time_dict,
-    )
-
-
-def inversion_imaging_unpacked_from(
-    data: Array2D,
-    noise_map: Array2D,
-    convolver: Convolver,
-    w_tilde: WTildeImaging,
     linear_obj_list: List[LinearObj],
     settings: SettingsInversion = SettingsInversion(),
     preloads: Preloads = Preloads(),
     run_time_dict: Optional[Dict] = None,
 ):
     """
     Factory which given an input `Imaging` dataset and list of linear objects, creates an `InversionImaging`.
@@ -198,21 +101,16 @@
     input `settings`) which solve for the linear object parameters in different ways.
 
     This factory inspects the type of dataset input and settings of the inversion in order to create the appropriate
     inversion object.
 
     Parameters
     ----------
-    data
-        The `image` data of the `Imaging` dataset which may have been changed.
-    noise_map
-        The noise_map of the `Imaging` dataset which may have been changed.
-    w_tilde
-        Object which uses the `Imaging` dataset's PSF / `Convolver` operateor to perform the `Inversion` using the
-        w-tilde formalism.
+    dataset
+        The dataset (e.g. `Imaging`) whose data is reconstructed via the `Inversion`.
     linear_obj_list
         The list of linear objects (e.g. analytic functions, a mapper with a pixelized grid) which reconstruct the
         input dataset's data and whose values are solved for via the inversion.
     settings
         Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
     preloads
         Preloads in memory certain arrays which may be known beforehand in order to speed up the calculation,
@@ -220,59 +118,53 @@
     run_time_dict
         A dictionary which contains timing of certain functions calls which is used for profiling.
 
     Returns
     -------
     An `Inversion` whose type is determined by the input `dataset` and `settings`.
     """
-
     if all(
         isinstance(linear_obj, AbstractLinearObjFuncList)
         for linear_obj in linear_obj_list
     ):
         use_w_tilde = False
     elif preloads.use_w_tilde is not None:
         use_w_tilde = preloads.use_w_tilde
     else:
         use_w_tilde = settings.use_w_tilde
 
     if not settings.use_w_tilde:
         use_w_tilde = False
 
-    if preloads.w_tilde is not None:
-        w_tilde = preloads.w_tilde
-
     if use_w_tilde:
+        if preloads.w_tilde is not None:
+            w_tilde = preloads.w_tilde
+        else:
+            w_tilde = dataset.w_tilde
+
         return InversionImagingWTilde(
-            data=data,
-            noise_map=noise_map,
-            convolver=convolver,
+            dataset=dataset,
             w_tilde=w_tilde,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
     return InversionImagingMapping(
-        data=data,
-        noise_map=noise_map,
-        convolver=convolver,
+        dataset=dataset,
         linear_obj_list=linear_obj_list,
         settings=settings,
         preloads=preloads,
         run_time_dict=run_time_dict,
     )
 
 
-def inversion_interferometer_unpacked_from(
-    data: Visibilities,
-    noise_map: VisibilitiesNoiseMap,
-    transformer: Union[TransformerDFT, TransformerNUFFT],
-    w_tilde: WTildeInterferometer,
+def inversion_interferometer_from(
+    dataset: Union[Interferometer, DatasetInterface],
     linear_obj_list: List[LinearObj],
     settings: SettingsInversion = SettingsInversion(),
     preloads: Preloads = Preloads(),
     run_time_dict: Optional[Dict] = None,
 ):
     """
     Factory which given an input `Interferometer` dataset and list of linear objects, creates
@@ -291,18 +183,16 @@
     input `settings`) which solve for the linear object parameters in different ways.
 
     This factory inspects the type of dataset input and settings of the inversion in order to create the appropriate
     inversion object.
 
     Parameters
     ----------
-    data
-        The `image` data of the `Imaging` dataset which may have been changed.
-    noise_map
-        The noise_map of the `Imaging` dataset which may have been changed.
+    dataset
+        The dataset (e.g. `Interferometer`) whose data is reconstructed via the `Inversion`.
     w_tilde
         Object which uses the `Imaging` dataset's PSF / `Convolver` operateor to perform the `Inversion` using the
         w-tilde formalism.
     linear_obj_list
         The list of linear objects (e.g. analytic functions, a mapper with a pixelized grid) which reconstruct the
         input dataset's data and whose values are solved for via the inversion.
     settings
@@ -328,39 +218,38 @@
     ):
         use_w_tilde = False
     else:
         use_w_tilde = settings.use_w_tilde
 
     if not settings.use_linear_operators:
         if use_w_tilde:
+            if preloads.w_tilde is not None:
+                w_tilde = preloads.w_tilde
+            else:
+                w_tilde = dataset.w_tilde
+
             return InversionInterferometerWTilde(
-                data=data,
-                noise_map=noise_map,
-                transformer=transformer,
+                dataset=dataset,
                 w_tilde=w_tilde,
                 linear_obj_list=linear_obj_list,
                 settings=settings,
                 preloads=preloads,
                 run_time_dict=run_time_dict,
             )
 
         else:
             return InversionInterferometerMapping(
-                data=data,
-                noise_map=noise_map,
-                transformer=transformer,
+                dataset=dataset,
                 linear_obj_list=linear_obj_list,
                 settings=settings,
                 preloads=preloads,
                 run_time_dict=run_time_dict,
             )
 
     else:
         return InversionInterferometerMappingPyLops(
-            data=data,
-            noise_map=noise_map,
-            transformer=transformer,
+            dataset=dataset,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/imaging/abstract.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/imaging/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import numpy as np
-from typing import Dict, List, Optional, Type
+from typing import Dict, List, Optional, Union, Type
 
 from autoconf import cached_property
 
 from autoarray.numba_util import profile_func
 
+from autoarray.dataset.imaging.dataset import Imaging
+from autoarray.inversion.inversion.dataset_interface import DatasetInterface
 from autoarray.inversion.linear_obj.func_list import AbstractLinearObjFuncList
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.inversion.inversion.abstract import AbstractInversion
 from autoarray.inversion.linear_obj.linear_obj import LinearObj
 from autoarray.inversion.inversion.settings import SettingsInversion
-from autoarray.structures.arrays.uniform_2d import Array2D
-from autoarray.operators.convolver import Convolver
 
 from autoarray.inversion.inversion.imaging import inversion_imaging_util
 
 
 class AbstractInversionImaging(AbstractInversion):
     def __init__(
         self,
-        data: Array2D,
-        noise_map: Array2D,
-        convolver: Convolver,
+        dataset: Union[Imaging, DatasetInterface],
         linear_obj_list: List[LinearObj],
         settings: SettingsInversion = SettingsInversion(),
         preloads=None,
         run_time_dict: Optional[Dict] = None,
     ):
         """
         An `Inversion` reconstructs an input dataset using a list of linear objects (e.g. a list of analytic functions
@@ -74,26 +72,27 @@
             A dictionary which contains timing of certain functions calls which is used for profiling.
         """
 
         from autoarray.preloads import Preloads
 
         preloads = preloads or Preloads()
 
-        self.convolver = convolver
-
         super().__init__(
-            data=data,
-            noise_map=noise_map,
+            dataset=dataset,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
     @property
+    def convolver(self):
+        return self.dataset.convolver
+
+    @property
     def operated_mapping_matrix_list(self) -> List[np.ndarray]:
         """
         The `operated_mapping_matrix` of a linear object describes the mappings between the observed data's values and
         the linear objects model, including a 2D convolution operation.
 
         This is used to construct the simultaneous linear equations which reconstruct the data.
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/imaging/inversion_imaging_util.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/imaging/inversion_imaging_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/imaging/mapping.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/imaging/mapping.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import copy
 import numpy as np
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
 from autoconf import cached_property
 
 from autoarray.numba_util import profile_func
 
+from autoarray.dataset.imaging.dataset import Imaging
+from autoarray.inversion.inversion.dataset_interface import DatasetInterface
 from autoarray.inversion.inversion.imaging.abstract import AbstractInversionImaging
 from autoarray.inversion.linear_obj.linear_obj import LinearObj
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.inversion.inversion.settings import SettingsInversion
 from autoarray.structures.arrays.uniform_2d import Array2D
-from autoarray.operators.convolver import Convolver
 
 from autoarray.inversion.inversion import inversion_util
 from autoarray.inversion.inversion.imaging import inversion_imaging_util
 
 
 class InversionImagingMapping(AbstractInversionImaging):
     def __init__(
         self,
-        data: Array2D,
-        noise_map: Array2D,
-        convolver: Convolver,
+        dataset: Union[Imaging, DatasetInterface],
         linear_obj_list: List[LinearObj],
         settings: SettingsInversion = SettingsInversion(),
         preloads=None,
         run_time_dict: Optional[Dict] = None,
     ):
         """
         Constructs linear equations (via vectors and matrices) which allow for sets of simultaneous linear equations
@@ -49,17 +48,15 @@
             The linear objects used to reconstruct the data's observed values. If multiple linear objects are passed
             the simultaneous linear equations are combined and solved simultaneously.
         run_time_dict
             A dictionary which contains timing of certain functions calls which is used for profiling.
         """
 
         super().__init__(
-            data=data,
-            noise_map=noise_map,
-            convolver=convolver,
+            dataset=dataset,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
     @property
@@ -126,16 +123,16 @@
         if self.preloads.operated_mapping_matrix is not None:
             operated_mapping_matrix = self.preloads.operated_mapping_matrix
         else:
             operated_mapping_matrix = self.operated_mapping_matrix
 
         return inversion_imaging_util.data_vector_via_blurred_mapping_matrix_from(
             blurred_mapping_matrix=operated_mapping_matrix,
-            image=self.data,
-            noise_map=self.noise_map,
+            image=np.array(self.data),
+            noise_map=np.array(self.noise_map),
         )
 
     @property
     @profile_func
     def _curvature_matrix_mapper_diag(self) -> Optional[np.ndarray]:
         """
         Returns the diagonal regions of the `curvature_matrix`, a 2D matrix which uses the mappings between the data
@@ -258,14 +255,13 @@
                 inversion_util.mapped_reconstructed_data_via_mapping_matrix_from(
                     mapping_matrix=operated_mapping_matrix_list[index],
                     reconstruction=reconstruction,
                 )
             )
 
             mapped_reconstructed_image = Array2D(
-                values=mapped_reconstructed_image,
-                mask=self.mask.derive_mask.sub_1,
+                values=mapped_reconstructed_image, mask=self.mask
             )
 
             mapped_reconstructed_data_dict[linear_obj] = mapped_reconstructed_image
 
         return mapped_reconstructed_data_dict
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/imaging/w_tilde.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/imaging/w_tilde.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import copy
 import numpy as np
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
 from autoconf import cached_property
 
 from autoarray.numba_util import profile_func
 
+from autoarray.dataset.imaging.dataset import Imaging
+from autoarray.dataset.imaging.w_tilde import WTildeImaging
+from autoarray.inversion.inversion.dataset_interface import DatasetInterface
 from autoarray.inversion.inversion.imaging.abstract import AbstractInversionImaging
 from autoarray.inversion.linear_obj.linear_obj import LinearObj
 from autoarray.inversion.inversion.settings import SettingsInversion
 from autoarray.inversion.linear_obj.func_list import AbstractLinearObjFuncList
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.preloads import Preloads
 from autoarray.structures.arrays.uniform_2d import Array2D
-from autoarray.operators.convolver import Convolver
-from autoarray.dataset.imaging.w_tilde import WTildeImaging
 
 from autoarray.inversion.inversion import inversion_util
 from autoarray.inversion.inversion.imaging import inversion_imaging_util
 
 
 class InversionImagingWTilde(AbstractInversionImaging):
     def __init__(
         self,
-        data: Array2D,
-        noise_map: Array2D,
-        convolver: Convolver,
+        dataset: Union[Imaging, DatasetInterface],
         w_tilde: WTildeImaging,
         linear_obj_list: List[LinearObj],
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
         run_time_dict: Optional[Dict] = None,
     ):
         """
@@ -44,48 +43,47 @@
         bypassing the construction of a `mapping_matrix`.
 
         Parameters
         ----------
         noise_map
             The noise-map of the observed imaging data which values are solved for.
         convolver
-            The convolver used to include 2D convolution of the mapping matrix with the imaigng data's PSF.
+            The convolver used to perform 2D convolution of the imaigng data's PSF when computing the operated
+            mapping matrix.
         w_tilde
             An object containing matrices that construct the linear equations via the w-tilde formalism which bypasses
             the mapping matrix.
         linear_obj_list
             The linear objects used to reconstruct the data's observed values. If multiple linear objects are passed
             the simultaneous linear equations are combined and solved simultaneously.
         run_time_dict
             A dictionary which contains timing of certain functions calls which is used for profiling.
         """
 
         super().__init__(
-            data=data,
-            noise_map=noise_map,
-            convolver=convolver,
+            dataset=dataset,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
         if self.settings.use_w_tilde:
             self.w_tilde = w_tilde
-            self.w_tilde.check_noise_map(noise_map=noise_map)
+            self.w_tilde.check_noise_map(noise_map=dataset.noise_map)
         else:
             self.w_tilde = None
 
     @cached_property
     @profile_func
     def w_tilde_data(self):
         return inversion_imaging_util.w_tilde_data_imaging_from(
-            image_native=self.data.native,
-            noise_map_native=self.noise_map.native,
-            kernel_native=self.convolver.kernel.native,
+            image_native=np.array(self.data.native),
+            noise_map_native=np.array(self.noise_map.native),
+            kernel_native=np.array(self.convolver.kernel.native),
             native_index_for_slim_index=self.data.mask.derive_indexes.native_for_slim,
         )
 
     @property
     @profile_func
     def _data_vector_mapper(self) -> np.ndarray:
         """
@@ -220,16 +218,16 @@
         ):
             operated_mapping_matrix = self.linear_func_operated_mapping_matrix_dict[
                 linear_func
             ]
 
             diag = inversion_imaging_util.data_vector_via_blurred_mapping_matrix_from(
                 blurred_mapping_matrix=operated_mapping_matrix,
-                image=self.data,
-                noise_map=self.noise_map,
+                image=np.array(self.data),
+                noise_map=np.array(self.noise_map),
             )
 
             param_range = linear_func_param_range[linear_func_index]
 
             data_vector[param_range[0] : param_range[1],] = diag
 
         return data_vector
@@ -566,16 +564,15 @@
                     data_to_pix_unique=linear_obj.unique_mappings.data_to_pix_unique,
                     data_weights=linear_obj.unique_mappings.data_weights,
                     pix_lengths=linear_obj.unique_mappings.pix_lengths,
                     reconstruction=reconstruction,
                 )
 
                 mapped_reconstructed_image = Array2D(
-                    values=mapped_reconstructed_image,
-                    mask=self.mask.derive_mask.sub_1,
+                    values=mapped_reconstructed_image, mask=self.mask
                 )
 
                 mapped_reconstructed_image = self.convolver.convolve_image_no_blurring(
                     image=mapped_reconstructed_image
                 )
 
             else:
@@ -584,14 +581,13 @@
                 ]
 
                 mapped_reconstructed_image = np.sum(
                     reconstruction * operated_mapping_matrix, axis=1
                 )
 
                 mapped_reconstructed_image = Array2D(
-                    values=mapped_reconstructed_image,
-                    mask=self.mask.derive_mask.sub_1,
+                    values=mapped_reconstructed_image, mask=self.mask
                 )
 
             mapped_reconstructed_data_dict[linear_obj] = mapped_reconstructed_image
 
         return mapped_reconstructed_data_dict
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/abstract.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import numpy as np
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
+from autoarray.dataset.interferometer.dataset import Interferometer
+from autoarray.inversion.inversion.dataset_interface import DatasetInterface
 from autoarray.inversion.inversion.abstract import AbstractInversion
 from autoarray.mask.mask_2d import Mask2D
 from autoarray.inversion.linear_obj.linear_obj import LinearObj
 from autoarray.inversion.inversion.settings import SettingsInversion
-from autoarray.operators.transformer import TransformerNUFFT
 from autoarray.preloads import Preloads
 from autoarray.structures.arrays.uniform_2d import Array2D
-from autoarray.structures.visibilities import Visibilities
-from autoarray.structures.visibilities import VisibilitiesNoiseMap
 
 from autoarray.inversion.inversion import inversion_util
 
 from autoarray.numba_util import profile_func
 
 
 class AbstractInversionInterferometer(AbstractInversion):
     def __init__(
         self,
-        data: Visibilities,
-        noise_map: VisibilitiesNoiseMap,
-        transformer: TransformerNUFFT,
+        dataset: Union[Interferometer, DatasetInterface],
         linear_obj_list: List[LinearObj],
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
         run_time_dict: Optional[Dict] = None,
     ):
         """
         Constructs linear equations (via vectors and matrices) which allow for sets of simultaneous linear equations
@@ -47,23 +44,24 @@
             The linear objects used to reconstruct the data's observed values. If multiple linear objects are passed
             the simultaneous linear equations are combined and solved simultaneously.
         run_time_dict
             A dictionary which contains timing of certain functions calls which is used for profiling.
         """
 
         super().__init__(
-            data=data,
-            noise_map=noise_map,
+            dataset=dataset,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
-        self.transformer = transformer
+    @property
+    def transformer(self):
+        return self.dataset.transformer
 
     @property
     def mask(self) -> Mask2D:
         return self.transformer.real_space_mask
 
     @property
     def operated_mapping_matrix_list(self) -> List[np.ndarray]:
@@ -123,14 +121,13 @@
                 inversion_util.mapped_reconstructed_data_via_mapping_matrix_from(
                     mapping_matrix=linear_obj.mapping_matrix,
                     reconstruction=reconstruction,
                 )
             )
 
             mapped_reconstructed_image = Array2D(
-                values=mapped_reconstructed_image,
-                mask=self.mask.derive_mask.sub_1,
+                values=mapped_reconstructed_image, mask=self.mask
             )
 
             mapped_reconstructed_image_dict[linear_obj] = mapped_reconstructed_image
 
         return mapped_reconstructed_image_dict
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/lop.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/lop.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/mapping.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 import numpy as np
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
 from autoconf import cached_property
 
+from autoarray.dataset.interferometer.dataset import Interferometer
+from autoarray.inversion.inversion.dataset_interface import DatasetInterface
 from autoarray.inversion.inversion.interferometer.abstract import (
     AbstractInversionInterferometer,
 )
 from autoarray.inversion.linear_obj.linear_obj import LinearObj
 from autoarray.inversion.inversion.settings import SettingsInversion
-from autoarray.operators.transformer import TransformerNUFFT
 from autoarray.preloads import Preloads
 from autoarray.structures.visibilities import Visibilities
-from autoarray.structures.visibilities import VisibilitiesNoiseMap
 
 from autoarray.inversion.inversion.interferometer import inversion_interferometer_util
 from autoarray.inversion.inversion import inversion_util
 
 from autoarray.numba_util import profile_func
 
 
 class InversionInterferometerMapping(AbstractInversionInterferometer):
     def __init__(
         self,
-        data: Visibilities,
-        noise_map: VisibilitiesNoiseMap,
-        transformer: TransformerNUFFT,
+        dataset: Union[Interferometer, DatasetInterface],
         linear_obj_list: List[LinearObj],
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
         run_time_dict: Optional[Dict] = None,
     ):
         """
         Constructs linear equations (via vectors and matrices) which allow for sets of simultaneous linear equations
@@ -53,25 +51,21 @@
             The linear objects used to reconstruct the data's observed values. If multiple linear objects are passed
             the simultaneous linear equations are combined and solved simultaneously.
         run_time_dict
             A dictionary which contains timing of certain functions calls which is used for profiling.
         """
 
         super().__init__(
-            data=data,
-            noise_map=noise_map,
-            transformer=transformer,
+            dataset=dataset,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
-        self.transformer = transformer
-
     @cached_property
     @profile_func
     def data_vector(self) -> np.ndarray:
         """
         The `data_vector` is a 1D vector whose values are solved for by the simultaneous linear equations constructed
         by this object.
 
@@ -82,16 +76,16 @@
         concatenated ensuring their `data_vector` values are solved for simultaneously.
 
         The calculation is described in more detail in `inversion_util.data_vector_via_transformed_mapping_matrix_from`.
         """
 
         return inversion_interferometer_util.data_vector_via_transformed_mapping_matrix_from(
             transformed_mapping_matrix=self.operated_mapping_matrix,
-            visibilities=self.data,
-            noise_map=self.noise_map,
+            visibilities=np.array(self.data),
+            noise_map=np.array(self.noise_map),
         )
 
     @cached_property
     @profile_func
     def curvature_matrix(self) -> np.ndarray:
         """
         The `curvature_matrix` is a 2D matrix which uses the mappings between the data and the linear objects to
@@ -143,20 +137,14 @@
 
         This function converts an ndarray of a `reconstruction` to a dictionary of ndarrays containing each linear
         object's reconstructed images, where the keys are the instances of each mapper in the inversion.
 
         To perform this mapping the `mapping_matrix` is used, which straightforwardly describes how every value of
         the `reconstruction` maps to pixels in the data-frame after the 2D non-uniform fast Fourier transformer
         operation has been performed.
-
-        Parameters
-        ----------
-        reconstruction
-            The reconstruction (in the source frame) whose values are mapped to a dictionary of values for each
-            individual mapper (in the image-plane).
         """
         mapped_reconstructed_data_dict = {}
 
         reconstruction_dict = self.source_quantity_dict_from(
             source_quantity=self.reconstruction
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/interferometer/w_tilde.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/interferometer/w_tilde.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import numpy as np
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
 from autoconf import cached_property
 
+from autoarray.dataset.interferometer.dataset import Interferometer
+from autoarray.inversion.inversion.dataset_interface import DatasetInterface
 from autoarray.inversion.inversion.interferometer.abstract import (
     AbstractInversionInterferometer,
 )
 from autoarray.dataset.interferometer.w_tilde import WTildeInterferometer
 from autoarray.inversion.linear_obj.linear_obj import LinearObj
 from autoarray.inversion.inversion.settings import SettingsInversion
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.preloads import Preloads
-from autoarray.operators.transformer import TransformerNUFFT
 from autoarray.structures.visibilities import Visibilities
-from autoarray.structures.visibilities import VisibilitiesNoiseMap
 
 from autoarray.inversion.inversion import inversion_util
 
 from autoarray.numba_util import profile_func
 
 
 class InversionInterferometerWTilde(AbstractInversionInterferometer):
     def __init__(
         self,
-        data: Visibilities,
-        noise_map: VisibilitiesNoiseMap,
-        transformer: TransformerNUFFT,
+        dataset: Union[Interferometer, DatasetInterface],
         w_tilde: WTildeInterferometer,
         linear_obj_list: List[LinearObj],
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
         run_time_dict: Optional[Dict] = None,
     ):
         """
@@ -58,20 +56,18 @@
             The linear objects used to reconstruct the data's observed values. If multiple linear objects are passed
             the simultaneous linear equations are combined and solved simultaneously.
         run_time_dict
             A dictionary which contains timing of certain functions calls which is used for profiling.
         """
 
         self.w_tilde = w_tilde
-        self.w_tilde.check_noise_map(noise_map=noise_map)
+        self.w_tilde.check_noise_map(noise_map=dataset.noise_map)
 
         super().__init__(
-            data=data,
-            noise_map=noise_map,
-            transformer=transformer,
+            dataset=dataset,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
         self.settings = settings
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/inversion_util.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/inversion_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/inversion/settings.py` & `autoarray-2024.5.16.0/autoarray/inversion/inversion/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class SettingsInversion:
     def __init__(
         self,
         use_w_tilde: bool = True,
         use_positive_only_solver: Optional[bool] = None,
         positive_only_uses_p_initial: Optional[bool] = None,
-        relocate_pix_border: Optional[bool] = None,
+        use_border_relocator: Optional[bool] = None,
         force_edge_pixels_to_zeros: bool = True,
         force_edge_image_pixels_to_zeros: bool = False,
         image_pixels_source_zero=None,
         no_regularization_add_to_curvature_diag_value: float = None,
         use_w_tilde_numpy: bool = False,
         use_source_loop: bool = False,
         use_linear_operators: bool = False,
@@ -39,15 +39,15 @@
             Whether to use the w-tilde formalism to perform the inversion, which speeds up the construction of the
             simultaneous linear equations (by bypassing the construction of a `mapping_matrix`) for many dataset
             use cases.
         use_positive_only_solver
             Whether to use a positive-only linear system solver, which requires that every reconstructed value is
             positive but is computationally much slower than the default solver (which allows for positive and
             negative values).
-        relocate_pix_border
+        use_border_relocator
             If `True`, all coordinates of all pixelization source mesh grids have pixels outside their border
             relocated to their edge.
         no_regularization_add_to_curvature_diag_value
             If a linear func object does not have a corresponding regularization, this value is added to its
             diagonal entries of the curvature regularization matrix to ensure the matrix is positive-definite.
         use_w_tilde_numpy
             If True, the curvature_matrix is computed via numpy matrix multiplication (as opposed to numba functions
@@ -77,15 +77,15 @@
             For an interferometer inversion using the linear operators method, sets the maximum number of iterations
             of the solver (this input does nothing for dataset data and other interferometer methods).
         """
 
         self.use_w_tilde = use_w_tilde
         self._use_positive_only_solver = use_positive_only_solver
         self._positive_only_uses_p_initial = positive_only_uses_p_initial
-        self._relocate_pix_border = relocate_pix_border
+        self._use_border_relocator = use_border_relocator
         self.use_linear_operators = use_linear_operators
         self.force_edge_pixels_to_zeros = force_edge_pixels_to_zeros
         self.force_edge_image_pixels_to_zeros = force_edge_image_pixels_to_zeros
         self.image_pixels_source_zero = image_pixels_source_zero
         self._no_regularization_add_to_curvature_diag_value = (
             no_regularization_add_to_curvature_diag_value
         )
@@ -114,19 +114,19 @@
     def positive_only_uses_p_initial(self):
         if self._positive_only_uses_p_initial is None:
             return conf.instance["general"]["inversion"]["positive_only_uses_p_initial"]
 
         return self._positive_only_uses_p_initial
 
     @property
-    def relocate_pix_border(self):
-        if self._relocate_pix_border is None:
-            return conf.instance["general"]["inversion"]["relocate_pix_border"]
+    def use_border_relocator(self):
+        if self._use_border_relocator is None:
+            return conf.instance["general"]["inversion"]["use_border_relocator"]
 
-        return self._relocate_pix_border
+        return self._use_border_relocator
 
     @property
     def no_regularization_add_to_curvature_diag_value(self):
         if self._no_regularization_add_to_curvature_diag_value is None:
             return conf.instance["general"]["inversion"][
                 "no_regularization_add_to_curvature_diag_value"
             ]
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/linear_obj/func_list.py` & `autoarray-2024.5.16.0/autoarray/inversion/linear_obj/func_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,15 +92,18 @@
         To perform an `Inversion` efficiently the linear algebra can bypass the calculation of a `mapping_matrix` and
         instead use the w-tilde formalism, which requires these unique mappings for efficient computation. For
         convenience, these mappings and associated metadata are packaged into the class `UniqueMappings`.
 
         For a `LinearObjFuncList` every data pixel's group of sub-pixels maps directly to the linear function.
         """
 
-        sub_size = self.grid.sub_size
+        sub_size = np.max(self.grid.over_sampling.sub_size)
+
+        # TODO : This shape slim is prob unreliable and needs to be divided by sub_size**2
+
         shape_slim = self.grid.mask.shape_slim
 
         data_to_pix_unique = -1.0 * np.ones(shape=(shape_slim, sub_size**2)).astype(
             "int"
         )
         data_weights = np.zeros(shape=(shape_slim, sub_size**2))
         pix_lengths = np.ones(shape=shape_slim).astype("int")
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/linear_obj/linear_obj.py` & `autoarray-2024.5.16.0/autoarray/inversion/linear_obj/linear_obj.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/linear_obj/neighbors.py` & `autoarray-2024.5.16.0/autoarray/inversion/linear_obj/neighbors.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/linear_obj/unique_mappings.py` & `autoarray-2024.5.16.0/autoarray/inversion/linear_obj/unique_mappings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/mock/mock_image_mesh.py` & `autoarray-2024.5.16.0/autoarray/inversion/mock/mock_image_mesh.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 from typing import Optional
 
-from autoarray.structures.grids.uniform_2d import Grid2D
+from autoarray.mask.mask_2d import Mask2D
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 
 from autoarray.inversion.pixelization.image_mesh.abstract import AbstractImageMesh
 
 
 class MockImageMesh(AbstractImageMesh):
     def __init__(self, image_plane_mesh_grid=None):
         super().__init__()
 
         self.image_plane_mesh_grid = image_plane_mesh_grid
 
     def image_plane_mesh_grid_from(
-        self, grid: Grid2D, adapt_data: Optional[np.ndarray], settings=None
+        self, mask: Mask2D, adapt_data: Optional[np.ndarray], settings=None
     ) -> Grid2DIrregular:
         if adapt_data is not None and self.image_plane_mesh_grid is not None:
             return adapt_data * self.image_plane_mesh_grid
 
         return self.image_plane_mesh_grid
 
     @property
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/mock/mock_inversion.py` & `autoarray-2024.5.16.0/autoarray/inversion/mock/mock_inversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from typing import List
 
+from autoarray.inversion.inversion.dataset_interface import DatasetInterface
 from autoarray.inversion.inversion.abstract import AbstractInversion
 from autoarray.inversion.inversion.settings import SettingsInversion
 from autoarray.preloads import Preloads
 
 
 class MockInversion(AbstractInversion):
     def __init__(
@@ -28,17 +29,21 @@
         errors_dict: List[np.ndarray] = None,
         regularization_term=None,
         log_det_curvature_reg_matrix_term=None,
         log_det_regularization_matrix_term=None,
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
     ):
-        super().__init__(
+        dataset = DatasetInterface(
             data=data,
             noise_map=noise_map,
+        )
+
+        super().__init__(
+            dataset=dataset,
             linear_obj_list=linear_obj_list or [],
             settings=settings,
             preloads=preloads,
         )
 
         self._operated_mapping_matrix = operated_mapping_matrix
         self._data_vector = data_vector
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/mock/mock_inversion_imaging.py` & `autoarray-2024.5.16.0/autoarray/inversion/mock/mock_inversion_imaging.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from typing import Dict
 
+from autoarray.inversion.inversion.dataset_interface import DatasetInterface
 from autoarray.inversion.inversion.imaging.mapping import InversionImagingMapping
 from autoarray.inversion.inversion.imaging.w_tilde import InversionImagingWTilde
 from autoarray.inversion.inversion.settings import SettingsInversion
 from autoarray.preloads import Preloads
 
 
 class MockInversionImaging(InversionImagingMapping):
@@ -16,18 +17,22 @@
         linear_obj_list=None,
         operated_mapping_matrix=None,
         linear_func_operated_mapping_matrix_dict=None,
         data_linear_func_matrix_dict=None,
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
     ):
-        super().__init__(
+        dataset = DatasetInterface(
             data=data,
             noise_map=noise_map,
             convolver=convolver,
+        )
+
+        super().__init__(
+            dataset=dataset,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
         )
 
         self._operated_mapping_matrix = operated_mapping_matrix
 
@@ -71,18 +76,22 @@
         convolver=None,
         w_tilde=None,
         linear_obj_list=None,
         curvature_matrix_mapper_diag=None,
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
     ):
-        super().__init__(
+        dataset = DatasetInterface(
             data=data,
             noise_map=noise_map,
             convolver=convolver,
+        )
+
+        super().__init__(
+            dataset=dataset,
             w_tilde=w_tilde or MockWTildeImaging(),
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
         )
 
         self.__curvature_matrix_mapper_diag = curvature_matrix_mapper_diag
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/mock/mock_inversion_interferometer.py` & `autoarray-2024.5.16.0/autoarray/inversion/mock/mock_inversion_interferometer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 
+from autoarray.inversion.inversion.dataset_interface import DatasetInterface
 from autoarray.inversion.inversion.interferometer.mapping import (
     InversionInterferometerMapping,
 )
 from autoarray.inversion.inversion.settings import SettingsInversion
 from autoarray.preloads import Preloads
 
 
@@ -14,18 +15,22 @@
         noise_map=None,
         transformer=None,
         linear_obj_list=None,
         operated_mapping_matrix=None,
         settings: SettingsInversion = SettingsInversion(),
         preloads: Preloads = Preloads(),
     ):
-        super().__init__(
+        dataset = DatasetInterface(
             data=data,
             noise_map=noise_map,
             transformer=transformer,
+        )
+
+        super().__init__(
+            dataset=dataset,
             linear_obj_list=linear_obj_list,
             settings=settings,
             preloads=preloads,
         )
 
         self._operated_mapping_matrix = operated_mapping_matrix
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/mock/mock_linear_obj.py` & `autoarray-2024.5.16.0/autoarray/inversion/mock/mock_linear_obj.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/mock/mock_linear_obj_func_list.py` & `autoarray-2024.5.16.0/autoarray/inversion/mock/mock_linear_obj_func_list.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/mock/mock_mapper.py` & `autoarray-2024.5.16.0/autoarray/inversion/mock/mock_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,33 +4,42 @@
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids
 
 
 class MockMapper(AbstractMapper):
     def __init__(
         self,
+        mask=None,
         source_plane_data_grid=None,
         source_plane_mesh_grid=None,
+        over_sampler=None,
+        border_relocator=None,
         adapt_data=None,
         edge_pixel_list=None,
         regularization=None,
         pix_sub_weights=None,
         pix_sub_weights_split_cross=None,
         mapping_matrix=None,
         pixel_signals=None,
         parameters=None,
         interpolated_array=None,
     ):
         mapper_grids = MapperGrids(
+            mask=mask,
             source_plane_data_grid=source_plane_data_grid,
             source_plane_mesh_grid=source_plane_mesh_grid,
             adapt_data=adapt_data,
         )
 
-        super().__init__(mapper_grids=mapper_grids, regularization=regularization)
+        super().__init__(
+            mapper_grids=mapper_grids,
+            over_sampler=over_sampler,
+            border_relocator=border_relocator,
+            regularization=regularization,
+        )
 
         self._edge_pixel_list = edge_pixel_list
         self._pix_sub_weights = pix_sub_weights
         self._pix_sub_weights_split_cross = pix_sub_weights_split_cross
         self._mapping_matrix = mapping_matrix
         self._parameters = parameters
         self._pixel_signals = pixel_signals
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/mock/mock_mesh.py` & `autoarray-2024.5.16.0/autoarray/inversion/mock/mock_mesh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from typing import Dict, Optional
 
+from autoarray.mask.mask_2d import Mask2D
 from autoarray.inversion.pixelization.mesh.abstract import AbstractMesh
 from autoarray.structures.mesh.abstract_2d import Abstract2DMesh
 from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids
 from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 from autoarray.preloads import Preloads
 
@@ -13,37 +14,39 @@
     def __init__(self, image_plane_mesh_grid=None):
         super().__init__()
 
         self.image_plane_mesh_grid = image_plane_mesh_grid
 
     def mapper_grids_from(
         self,
-        source_plane_data_grid: Grid2D,
+        mask=None,
+        source_plane_data_grid: Grid2D = None,
+        border_relocator=None,
         source_plane_mesh_grid: Optional[Abstract2DMesh] = None,
         image_plane_mesh_grid: Optional[Grid2DIrregular] = None,
         adapt_data: Optional[np.ndarray] = None,
         preloads: Optional[Preloads] = None,
         run_time_dict: Optional[Dict] = None,
     ) -> MapperGrids:
         return MapperGrids(
+            mask=mask,
             source_plane_data_grid=source_plane_data_grid,
+            border_relocator=border_relocator,
             source_plane_mesh_grid=source_plane_mesh_grid,
             image_plane_mesh_grid=self.image_plane_mesh_grid,
             adapt_data=adapt_data,
-            settings=settings,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
 
     def image_plane_mesh_grid_from(
         self,
-        image_plane_data_grid,
+        mask: Mask2D,
         adapt_data,
         settings=None,
-        noise_map: np.ndarray = None,
     ):
         if adapt_data is not None and self.image_plane_mesh_grid is not None:
             return adapt_data * self.image_plane_mesh_grid
 
         return self.image_plane_mesh_grid
 
     @property
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/mock/mock_pixelization.py` & `autoarray-2024.5.16.0/autoarray/inversion/mock/mock_pixelization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 
+from autoarray.mask.mask_2d import Mask2D
 from autoarray.inversion.pixelization.pixelization import Pixelization
 
 
 class MockPixelization(Pixelization):
     def __init__(
         self,
         mesh=None,
@@ -18,28 +19,28 @@
 
         self.mapper = mapper
         self.image_plane_mesh_grid = image_plane_mesh_grid
 
     # noinspection PyUnusedLocal,PyShadowingNames
     def mapper_grids_from(
         self,
+        mask,
         source_plane_data_grid,
         source_plane_mesh_grid,
         image_plane_mesh_grid=None,
         adapt_data=None,
         settings=None,
         preloads=None,
         run_time_dict=None,
     ):
         return self.mapper
 
     def image_plane_mesh_grid_from(
         self,
-        image_plane_data_grid,
+        mask: Mask2D,
         adapt_data,
         settings=None,
-        noise_map: np.ndarray = None,
     ):
         if adapt_data is not None and self.image_plane_mesh_grid is not None:
             return adapt_data * self.image_plane_mesh_grid
 
         return self.image_plane_mesh_grid
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/abstract.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/image_mesh/abstract.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional
 
 import numpy as np
 import os
 
+from autoarray.mask.mask_2d import Mask2D
 from autoarray.structures.arrays.uniform_2d import Array2D
-from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
+from autoarray.inversion.inversion.settings import SettingsInversion
 
 from autoarray.structures.grids import grid_2d_util
 
 from autoarray import exc
 
 
 class AbstractImageMesh:
@@ -21,52 +22,57 @@
         pass
 
     @property
     def uses_adapt_images(self) -> bool:
         raise NotImplementedError
 
     def image_plane_mesh_grid_from(
-        self, grid: Grid2D, adapt_data: Optional[np.ndarray] = None, settings=None
+        self,
+        mask: Mask2D,
+        adapt_data: Optional[np.ndarray] = None,
+        settings: SettingsInversion = None,
     ) -> Grid2DIrregular:
         raise NotImplementedError
 
     def mesh_pixels_per_image_pixels_from(
-        self, grid: Grid2D, mesh_grid: Grid2DIrregular
+        self, mask: Mask2D, mesh_grid: Grid2DIrregular
     ) -> Array2D:
         """
         Returns an array containing the number of mesh pixels in every pixel of the data's mask.
 
         For example, image-mesh adaption may be performed on a 3.0" circular mask of data. The high weight pixels
         may have 3 or more mesh pixels per image pixel, whereas low weight regions may have zero pixels. The array
         returned by this function gives the integer number of pixels in each data pixel.
 
         Parameters
         ----------
-        grid
-            The masked (y,x) grid of the data coordinates, corresponding to the mask applied to the data. The number of
-            mesh pixels mapped inside each of this grid's image-pixels is returned.
+        mask
+            The mask of the dataset being analysed, which the pixelization grid maps too. The number of
+            mesh pixels mapped inside each of this mask's image-pixels is returned.
         mesh_grid
             The image mesh-grid computed by the class which adapts to the data's mask. The number of image mesh pixels
             that fall within each of the data's mask pixels is returned.
 
         Returns
         -------
         An array containing the integer number of image-mesh pixels that fall without each of the data's mask.
         """
 
         mesh_pixels_per_image_pixels = grid_2d_util.grid_pixels_in_mask_pixels_from(
-            grid=mesh_grid,
-            shape_native=grid.shape_native,
-            pixel_scales=grid.pixel_scales,
-            origin=grid.origin,
+            grid=np.array(mesh_grid),
+            shape_native=mask.shape_native,
+            pixel_scales=mask.pixel_scales,
+            origin=mask.origin,
         )
 
-        return Array2D(values=mesh_pixels_per_image_pixels, mask=grid.mask)
+        return Array2D(values=mesh_pixels_per_image_pixels, mask=mask)
 
-    def check_mesh_pixels_per_image_pixels(self, grid, mesh_grid, settings):
+    def check_mesh_pixels_per_image_pixels(
+        self, mask: Mask2D, mesh_grid: Grid2DIrregular, settings: SettingsInversion
+    ):
         """
         Checks the number of mesh pixels in every image pixel and raises an `InversionException` if there are fewer
         mesh pixels inside a certain number of image-pixels than the input settings.
 
         This allows a user to force a model-fit to use image-mesh's which cluster a large number of mesh pixels to
         the brightest regions of the image data (E.g. the highst weighted regions).
 
@@ -80,47 +86,53 @@
            below this value, raise an `InversionException`.
 
         Therefore, by settings `settings.image_mesh_min_mesh_pixels_per_pixel` to a value above 1 the code is forced
         to adapt the image mesh enough to put many mesh pixels in the brightest image pixels.
 
         Parameters
         ----------
-        grid
-            The masked (y,x) grid of the data coordinates, corresponding to the mask applied to the data. The number of
-            mesh pixels mapped inside each of this grid's image-pixels is returned.
+        mask
+            The mask of the dataset being analysed, which the pixelization grid maps too. The number of
+            mesh pixels mapped inside each of this mask's image-pixels is returned.
         mesh_grid
             The image mesh-grid computed by the class which adapts to the data's mask. The number of image mesh pixels
             that fall within each of the data's mask pixels is returned.
         settings
             The inversion settings, which have the criteria dictating if the image-mesh has clustered enough or if
             an exception is raised.
         """
 
         if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
             return
 
         if settings is not None:
             if settings.image_mesh_min_mesh_pixels_per_pixel is not None:
                 mesh_pixels_per_image_pixels = self.mesh_pixels_per_image_pixels_from(
-                    grid=grid, mesh_grid=mesh_grid
+                    mask=mask, mesh_grid=mesh_grid
                 )
 
                 indices_of_highest_values = np.argsort(mesh_pixels_per_image_pixels)[
                     -settings.image_mesh_min_mesh_number :
                 ]
                 lowest_mesh_pixels = np.min(
                     mesh_pixels_per_image_pixels[indices_of_highest_values]
                 )
 
                 if lowest_mesh_pixels < settings.image_mesh_min_mesh_pixels_per_pixel:
                     raise exc.InversionException()
 
         return mesh_grid
 
-    def check_adapt_background_pixels(self, grid, mesh_grid, adapt_data, settings):
+    def check_adapt_background_pixels(
+        self,
+        mask: Mask2D,
+        mesh_grid: Grid2DIrregular,
+        adapt_data: Optional[np.ndarray],
+        settings: SettingsInversion,
+    ):
         """
         Checks the number of mesh pixels in the background of the image-mesh and raises an `InversionException` if
         there are fewer mesh pixels in the background than the input settings.
 
         This allows a user to force a model-fit to use image-mesh's which cluster a minimum number of mesh pixels to
         the faintest regions of the image data (E.g. the lowest weighted regions). This prevents too few image-mesh
         pixels being allocated to the background of the data.
@@ -137,17 +149,17 @@
            of mesh pixels is below this value, meaning the background did not have sufficient mesh pixels in it.
 
         Therefore, by setting `settings.image_mesh_adapt_background_percent_threshold` the code is forced
         to adapt the image mesh in a way that places many mesh pixels in the background regions.
 
         Parameters
         ----------
-        grid
-            The masked (y,x) grid of the data coordinates, corresponding to the mask applied to the data. The number of
-            mesh pixels mapped inside each of this grid's image-pixels is returned.
+        mask
+            The mask of the dataset being analysed, which the pixelization grid maps too. The number of
+            mesh pixels mapped inside each of this mask's image-pixels is returned.
         mesh_grid
             The image mesh-grid computed by the class which adapts to the data's mask. The number of image mesh pixels
             that fall within each of the data's mask pixels is returned.
         adapt_data
             A image which represents one or more components in the masked 2D data in the image-plane.
         settings
             The inversion settings, which have the criteria dictating if the image-mesh has clustered enough or if
@@ -158,23 +170,23 @@
             return
 
         if settings is not None:
             if settings.image_mesh_adapt_background_percent_threshold is not None:
                 pixels = mesh_grid.shape[0]
 
                 pixels_in_background = int(
-                    grid.shape[0] * settings.image_mesh_adapt_background_percent_check
+                    mask.shape_slim * settings.image_mesh_adapt_background_percent_check
                 )
 
                 indices_of_lowest_values = np.argsort(adapt_data)[:pixels_in_background]
                 mask_background = np.zeros_like(adapt_data, dtype=bool)
                 mask_background[indices_of_lowest_values] = True
 
                 mesh_pixels_per_image_pixels = self.mesh_pixels_per_image_pixels_from(
-                    grid=grid, mesh_grid=mesh_grid
+                    mask=mask, mesh_grid=mesh_grid
                 )
 
                 mesh_pixels_in_background = sum(
                     mesh_pixels_per_image_pixels[mask_background]
                 )
 
                 if mesh_pixels_in_background < (
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/hilbert.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/image_mesh/hilbert.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 import numpy as np
 from scipy.interpolate import interp1d, griddata
 from typing import Optional
 
+from autoarray.mask.mask_2d import Mask2D
 from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.mask.mask_2d import Mask2D
 from autoarray.inversion.pixelization.image_mesh.abstract_weighted import (
     AbstractImageMeshWeighted,
 )
+from autoarray.operators.over_sampling.uniform import OverSamplerUniform
 from autoarray.inversion.inversion.settings import SettingsInversion
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 
 from autoarray import exc
 
 
 def gilbert2d(width, height):
@@ -95,26 +97,28 @@
     mask_radius: the circular mask radius. Currently, the code only works with a circular mask.
     sub_scale: oversampling scale for each image pixel.
     """
 
     shape_nnn = np.shape(mask)[0]
 
     grid = Grid2D.uniform(
-        shape_native=(shape_nnn, shape_nnn), pixel_scales=pixel_scales, sub_size=1
+        shape_native=(shape_nnn, shape_nnn),
+        pixel_scales=pixel_scales,
     )
 
     new_mask = Mask2D.circular(
         shape_native=(shape_nnn, shape_nnn),
         pixel_scales=pixel_scales,
-        sub_size=sub_scale,
         centre=mask.origin,
         radius=mask_radius,
     )
 
-    new_grid = Grid2D.from_mask(new_mask)
+    over_sampler = OverSamplerUniform(mask=new_mask, sub_size=sub_scale)
+
+    new_grid = over_sampler.over_sampled_grid
 
     new_img = griddata(
         points=grid, values=img_2d.ravel(), xi=new_grid, fill_value=0.0, method="linear"
     )
 
     return new_img, new_grid
 
@@ -153,18 +157,24 @@
 
 def image_and_grid_from(image, mask, mask_radius, pixel_scales, hilbert_length):
     """
     This code will create a grid in Hilbert space-filling curve order and an interpolated hyper
     image associated to that grid.
     """
 
-    shape_nnn = np.shape(mask)[0]
+    # For multi wavelength fits the input image may be a different resolution than the mask.
+
+    try:
+        shape_nnn = np.shape(image.native)[0]
+    except AttributeError:
+        shape_nnn = np.shape(mask)[0]
 
     grid = Grid2D.uniform(
-        shape_native=(shape_nnn, shape_nnn), pixel_scales=pixel_scales, sub_size=1
+        shape_native=(shape_nnn, shape_nnn),
+        pixel_scales=pixel_scales,
     )
 
     x1d_hb, y1d_hb = grid_hilbert_order_from(
         length=hilbert_length, mask_radius=mask_radius
     )
 
     grid_hb = np.stack((y1d_hb, x1d_hb), axis=-1)
@@ -243,15 +253,15 @@
             pixels=pixels,
             weight_floor=weight_floor,
             weight_power=weight_power,
         )
 
     def image_plane_mesh_grid_from(
         self,
-        grid: Grid2D,
+        mask: Mask2D,
         adapt_data: Optional[np.ndarray],
         settings: SettingsInversion = None,
     ) -> Grid2DIrregular:
         """
         Returns an image mesh by running the Hilbert curve on the weight map.
 
         See the `__init__` docstring for a full description of how this is performed.
@@ -264,28 +274,28 @@
             The weights defining the regions of the image the Hilbert curve adapts to.
 
         Returns
         -------
 
         """
 
-        if not grid.mask.is_circular:
+        if not mask.is_circular:
             raise exc.PixelizationException(
                 """
                 Hilbert image-mesh has been called but the input grid does not use a circular mask.
                 
                 Ensure that analysis is using a circular mask via the Mask2D.circular classmethod.
                 """
             )
 
         adapt_data_hb, grid_hb = image_and_grid_from(
             image=adapt_data,
-            mask=grid.mask,
-            mask_radius=grid.mask.circular_radius,
-            pixel_scales=grid.mask.pixel_scales,
+            mask=mask,
+            mask_radius=mask.circular_radius,
+            pixel_scales=mask.pixel_scales,
             hilbert_length=193,
         )
 
         weight_map = self.weight_map_from(adapt_data=adapt_data_hb)
 
         weight_map /= np.sum(weight_map)
 
@@ -299,15 +309,15 @@
             gridx=grid_hb[:, 1],
             gridy=grid_hb[:, 0],
         )
 
         mesh_grid = Grid2DIrregular(values=np.stack((drawn_y, drawn_x), axis=-1))
 
         self.check_mesh_pixels_per_image_pixels(
-            grid=grid, mesh_grid=mesh_grid, settings=settings
+            mask=mask, mesh_grid=mesh_grid, settings=settings
         )
 
         self.check_adapt_background_pixels(
-            grid=grid, mesh_grid=mesh_grid, adapt_data=adapt_data, settings=settings
+            mask=mask, mesh_grid=mesh_grid, adapt_data=adapt_data, settings=settings
         )
 
         return mesh_grid
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/hilbert_balanced.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/image_mesh/kmeans.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,147 +1,116 @@
-from __future__ import annotations
 import numpy as np
+from sklearn.cluster import KMeans as ScipyKMeans
 from typing import Optional
+import sys
+import warnings
+
+from autoarray.mask.mask_2d import Mask2D
 
-from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.inversion.pixelization.image_mesh.abstract_weighted import (
     AbstractImageMeshWeighted,
 )
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
-
-from autoarray.inversion.pixelization.image_mesh.hilbert import image_and_grid_from
-from autoarray.inversion.pixelization.image_mesh.hilbert import (
-    inverse_transform_sampling_interpolated,
-)
+from autoarray.inversion.inversion.settings import SettingsInversion
 
 from autoarray import exc
 
 
-class HilbertBalanced(AbstractImageMeshWeighted):
+class KMeans(AbstractImageMeshWeighted):
     def __init__(
         self,
         pixels=10.0,
         weight_floor=0.0,
         weight_power=0.0,
-        ratio=0.8,
     ):
         """
-        Computes a balanced image-mesh by computing the Hilbert curve of the adapt data and drawing points from it.
+        Computes an image-mesh by running a weighted KMeans clustering algorithm.
 
-        The standard `Hilbert` image-mesh suffers a systematic where the vast majority of points are drawn from
-        the high weighted reigons. This often leaves few points to reconstruct the lower weight regions, leading to
-        discontinuities in the reconstruction.
-
-        This image-mesh addresses this by drawing half the points from the weight map and the other half from
-        (1 - weight map). This ensures both high and low weighted regions are sampled equally, but still has sufficient
-        flexibility to dedicate many points to the highest weighted regions.
-
-        This requires an adapt-image, which is the image that the Hilbert curve algorithm adapts to in order to compute
-        the image mesh. This could simply be the image itself, or a model fit to the image which removes certain
+        This requires an adapt-image, which is the image that the KMeans algorithm adapts to in order to compute the
+        image mesh. This could simply be the image itself, or a model fit to the image which removes certain
         features or noise.
 
         For example, using the adapt image, the image mesh is computed as follows:
 
         1) Convert the adapt image to a weight map, which is a 2D array of weight values.
 
-        2) Run the Hilbert algorithm on the weight map, such that the image mesh pixels cluster around the weight map
+        2) Run the KMeans algorithm on the weight map, such that the image mesh pixels cluster around the weight map
         values with higher values.
 
         Parameters
         ----------
-        pixels
-            The total number of pixels in the image mesh and drawn from the Hilbert curve.
-        weight_floor
-            The minimum weight value in the weight map, which allows more pixels to be drawn from the lower weight
-            regions of the adapt image.
+        total_pixels
+            The total number of pixels in the image mesh and input into the KMeans algortihm.
         weight_power
-            The power the weight values are raised too, which allows more pixels to be drawn from the higher weight
-            regions of the adapt image.
-        ratio
-            The ratio between the number of pixdels in the image mesh drawn from the weight map and (1 - weight map).
-            For example, if there are 1000 pixels and a ratio of 0.8, 800 pixels are drawn from the weight map
-            and therefore make up the high weighted region of the image mesh.
         """
 
         super().__init__(
             pixels=pixels,
             weight_floor=weight_floor,
             weight_power=weight_power,
         )
 
-        self.ratio = ratio
-
     def image_plane_mesh_grid_from(
-        self, grid: Grid2D, adapt_data: Optional[np.ndarray], settings=None
+        self,
+        mask: Mask2D,
+        adapt_data: Optional[np.ndarray],
+        settings: SettingsInversion = None,
     ) -> Grid2DIrregular:
         """
-        Returns an image mesh by running the balanced Hilbert curve on the weight map.
+        Returns an image mesh by running a KMeans clustering algorithm on the weight map.
 
         See the `__init__` docstring for a full description of how this is performed.
 
         Parameters
         ----------
         grid
-            The grid of (y,x) coordinates of the image data the pixelization fits, which the Hilbert curve adapts to.
+            The grid of (y,x) coordinates of the image data the pixelization fits, which the KMeans algorithm
+            adapts to.
         adapt_data
-            The weights defining the regions of the image the Hilbert curve adapts to.
+            The weights defining the regions of the image the KMeans algorithm adapts to.
 
         Returns
         -------
 
         """
 
-        if not grid.mask.is_circular:
-            raise exc.PixelizationException(
+        if self.pixels > mask.shape_slim:
+            print(
                 """
-                Hilbert image-mesh has been called but the input grid does not use a circular mask.
-
-                Ensure that analysis is using a circular mask via the Mask2D.circular classmethod.
+                The number of pixels passed to the KMeans object exceeds the number of image-pixels in the mask of
+                the data being fitted. This is not allowed by the KMenas algorithm and will cause an error.
+                
+                To fix this, you should reduce the number of pixels in the KMeans object to be less than the number
+                of image-pixels in the mask of the data being fitted.
+                
+                If you are performing model-fitting, you should update the priors to have an upper limit which does
+                not exceed the number of image-pixels in the mask of the data being fitted.
+                
+                For adaptive fitting, the KMeans object has been superseeded by the Hilbert object, which does not
+                have this limitation and performs better in general. You should therefore consider using the Hilbert
+                object instead.
                 """
             )
 
-        adapt_data_hb, grid_hb = image_and_grid_from(
-            image=adapt_data,
-            mask=grid.mask,
-            mask_radius=grid.mask.circular_radius,
-            pixel_scales=grid.mask.pixel_scales,
-            hilbert_length=193,
-        )
-
-        weight_map = self.weight_map_from(adapt_data=adapt_data_hb)
+            sys.exit()
 
-        weight_map_background = 1.0 - weight_map
+        warnings.filterwarnings("ignore")
 
-        weight_map /= np.sum(weight_map)
-        weight_map_background /= np.sum(weight_map_background)
+        weight_map = self.weight_map_from(adapt_data=adapt_data)
 
-        pixels = int(self.pixels * self.ratio)
-
-        (
-            drawn_id,
-            drawn_x,
-            drawn_y,
-        ) = inverse_transform_sampling_interpolated(
-            probabilities=weight_map,
-            n_samples=pixels,
-            gridx=grid_hb[:, 1],
-            gridy=grid_hb[:, 0],
+        kmeans = ScipyKMeans(
+            n_clusters=int(self.pixels),
+            random_state=1,
+            n_init=1,
+            max_iter=5,
         )
 
-        grid = np.stack((drawn_y, drawn_x), axis=-1)
-
-        (
-            drawn_id,
-            drawn_x,
-            drawn_y,
-        ) = inverse_transform_sampling_interpolated(
-            probabilities=weight_map_background,
-            n_samples=(self.pixels - pixels) + 1,
-            gridx=grid_hb[:, 1],
-            gridy=grid_hb[:, 0],
-        )
+        grid = mask.derive_grid.unmasked
 
-        grid_background = np.stack((drawn_y, drawn_x), axis=-1)
+        try:
+            kmeans = kmeans.fit(X=grid, sample_weight=weight_map)
+        except ValueError or OverflowError:
+            raise exc.InversionException()
 
         return Grid2DIrregular(
-            values=np.concatenate((grid, grid_background[1:, :]), axis=0)
+            values=kmeans.cluster_centers_,
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/image_mesh/overlay.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/image_mesh/overlay.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from __future__ import annotations
 import numpy as np
-from typing import Optional, Tuple, TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from autoarray.structures.grids.uniform_2d import Grid2D
+from typing import Optional
 
+from autoarray.mask.mask_2d import Mask2D
 from autoarray.inversion.pixelization.image_mesh.abstract import AbstractImageMesh
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
+from autoarray.inversion.inversion.settings import SettingsInversion
 
 from autoarray.geometry import geometry_util
 from autoarray.structures.grids import grid_2d_util
 from autoarray import numba_util
 
 
 @numba_util.jit()
@@ -181,15 +179,18 @@
         """
 
         super().__init__()
 
         self.shape = (int(shape[0]), int(shape[1]))
 
     def image_plane_mesh_grid_from(
-        self, grid: Grid2D, adapt_data: Optional[np.ndarray] = None, settings=None
+        self,
+        mask: Mask2D,
+        adapt_data: Optional[np.ndarray] = None,
+        settings: SettingsInversion = None,
     ) -> Grid2DIrregular:
         """
         Returns an image-mesh by overlaying a uniform grid of (y,x) coordinates over the masked image that the
         pixelization is fitting.
 
         See the `__init__` docstring for a full description of how this is performed.
 
@@ -198,44 +199,45 @@
         grid
             The grid of (y,x) coordinates of the image data the pixelization fits, which the overlay grid is laid
             over.
         adapt_data
             Not used by this image mesh.
         """
 
-        pixel_scales = grid.mask.pixel_scales
+        pixel_scales = mask.pixel_scales
+
+        grid = mask.derive_grid.unmasked
 
         pixel_scales = (
             (grid.shape_native_scaled_interior[0] + pixel_scales[0]) / (self.shape[0]),
             (grid.shape_native_scaled_interior[1] + pixel_scales[1]) / (self.shape[1]),
         )
 
-        origin = grid.mask.mask_centre
+        origin = mask.mask_centre
 
         unmasked_overlay_grid = grid_2d_util.grid_2d_slim_via_shape_native_from(
             shape_native=self.shape,
             pixel_scales=pixel_scales,
-            sub_size=1,
             origin=origin,
         )
 
         overlaid_centres = geometry_util.grid_pixel_centres_2d_slim_from(
             grid_scaled_2d_slim=unmasked_overlay_grid,
-            shape_native=grid.mask.shape_native,
-            pixel_scales=grid.mask.pixel_scales,
+            shape_native=mask.shape_native,
+            pixel_scales=mask.pixel_scales,
         ).astype("int")
 
         total_pixels = total_pixels_2d_from(
-            mask_2d=grid.mask,
+            mask_2d=mask.array,
             overlaid_centres=overlaid_centres,
         )
 
         overlay_for_mask = overlay_for_mask_from(
             total_pixels=total_pixels,
-            mask=grid.mask,
+            mask=mask.array,
             overlaid_centres=overlaid_centres,
         ).astype("int")
 
         mesh_grid = overlay_via_unmasked_overlaid_from(
             unmasked_overlay_grid=unmasked_overlay_grid,
             overlay_for_mask=overlay_for_mask,
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/abstract.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 
 from autoconf import conf
 from autoconf import cached_property
 
 from autoarray.inversion.linear_obj.linear_obj import LinearObj
 from autoarray.inversion.linear_obj.func_list import UniqueMappings
 from autoarray.inversion.linear_obj.neighbors import Neighbors
+from autoarray.inversion.pixelization.border_relocator import BorderRelocator
 from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids
 from autoarray.inversion.regularization.abstract import AbstractRegularization
+from autoarray.operators.over_sampling.abstract import AbstractOverSampler
 from autoarray.structures.arrays.uniform_2d import Array2D
 from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.structures.mesh.abstract_2d import Abstract2DMesh
 
+
 from autoarray.numba_util import profile_func
 from autoarray.inversion.pixelization.mappers import mapper_util
 
 
 class AbstractMapper(LinearObj):
     def __init__(
         self,
         mapper_grids: MapperGrids,
         regularization: Optional[AbstractRegularization],
+        over_sampler: AbstractOverSampler,
+        border_relocator: BorderRelocator,
         run_time_dict: Optional[Dict] = None,
     ):
         """
         To understand a `Mapper` one must be familiar `Mesh` objects and the `mesh` and `pixelization` packages, where
         the four grids grouped in a `MapperGrids` object are explained (`image_plane_data_grid`, `source_plane_data_grid`,
         `image_plane_mesh_grid`,`source_plane_mesh_grid`)
 
@@ -73,20 +78,28 @@
         ----------
         mapper_grids
             An object containing the data grid and mesh grid in both the data-frame and source-frame used by the
             mapper to map data-points to linear object parameters.
         regularization
             The regularization scheme which may be applied to this linear object in order to smooth its solution,
             which for a mapper smooths neighboring pixels on the mesh.
+        over_sampler
+            Performs over-sampling whereby the masked image pixels are split into sub-pixels, which are all
+            mapped via the mapper with sub-fractional values of flux.
+        border_relocator
+           The border relocator, which relocates coordinates outside the border of the source-plane data grid to its
+           edge.
         run_time_dict
             A dictionary which contains timing of certain functions calls which is used for profiling.
         """
 
         super().__init__(regularization=regularization, run_time_dict=run_time_dict)
 
+        self.over_sampler = over_sampler
+        self.border_relocator = border_relocator
         self.mapper_grids = mapper_grids
 
     @property
     def params(self) -> int:
         return self.source_plane_mesh_grid.pixels
 
     @property
@@ -172,15 +185,15 @@
 
     @property
     def slim_index_for_sub_slim_index(self) -> np.ndarray:
         """
         The mappings between every sub-pixel data point on the sub-gridded data and each data point for a grid which
         does not use sub gridding (e.g. `sub_size=1`).
         """
-        return self.source_plane_data_grid.mask.derive_indexes.slim_for_sub_slim
+        return self.over_sampler.slim_for_sub_slim
 
     @property
     def sub_slim_indexes_for_pix_index(self) -> List[List]:
         """
         Returns the index mappings between each of the pixelization's pixels and the masked data's sub-pixels.
 
         Given that even pixelization pixel maps to multiple data sub-pixels, index mappings are returned as a list of
@@ -240,20 +253,20 @@
         """
 
         (
             data_to_pix_unique,
             data_weights,
             pix_lengths,
         ) = mapper_util.data_slim_to_pixelization_unique_from(
-            data_pixels=self.source_plane_data_grid.shape_slim,
+            data_pixels=self.over_sampler.mask.pixels_in_mask,
             pix_indexes_for_sub_slim_index=self.pix_indexes_for_sub_slim_index,
             pix_sizes_for_sub_slim_index=self.pix_sizes_for_sub_slim_index,
             pix_weights_for_sub_slim_index=self.pix_weights_for_sub_slim_index,
             pix_pixels=self.params,
-            sub_size=self.source_plane_data_grid.sub_size,
+            sub_size=np.array(self.over_sampler.sub_size),
         )
 
         return UniqueMappings(
             data_to_pix_unique=data_to_pix_unique,
             data_weights=data_weights,
             pix_lengths=pix_lengths,
         )
@@ -273,17 +286,17 @@
         detail in the function  `mapper_util.mapping_matrix_from()`.
         """
         return mapper_util.mapping_matrix_from(
             pix_indexes_for_sub_slim_index=self.pix_indexes_for_sub_slim_index,
             pix_size_for_sub_slim_index=self.pix_sizes_for_sub_slim_index,
             pix_weights_for_sub_slim_index=self.pix_weights_for_sub_slim_index,
             pixels=self.pixels,
-            total_mask_pixels=self.source_plane_data_grid.mask.pixels_in_mask,
+            total_mask_pixels=self.over_sampler.mask.pixels_in_mask,
             slim_index_for_sub_slim_index=self.slim_index_for_sub_slim_index,
-            sub_fraction=self.source_plane_data_grid.mask.sub_fraction,
+            sub_fraction=np.array(self.over_sampler.sub_fraction),
         )
 
     def pixel_signals_from(self, signal_scale: float) -> np.ndarray:
         """
         Returns the signal in each pixelization pixel, where this signal is an estimate of the expected signal
         each pixelization pixel contains given the data pixels it maps too.
 
@@ -297,16 +310,16 @@
         """
         return mapper_util.adaptive_pixel_signals_from(
             pixels=self.pixels,
             signal_scale=signal_scale,
             pixel_weights=self.pix_weights_for_sub_slim_index,
             pix_indexes_for_sub_slim_index=self.pix_indexes_for_sub_slim_index,
             pix_size_for_sub_slim_index=self.pix_sizes_for_sub_slim_index,
-            slim_index_for_sub_slim_index=self.source_plane_data_grid.mask.derive_indexes.slim_for_sub_slim,
-            adapt_data=self.adapt_data,
+            slim_index_for_sub_slim_index=self.over_sampler.slim_for_sub_slim,
+            adapt_data=np.array(self.adapt_data),
         )
 
     def pix_indexes_for_slim_indexes(self, pix_indexes: List) -> List[List]:
         """
         Returns the index mappings between every masked data-point (not subgridded) on the data and the mapper
         pixels / parameters that it maps too.
 
@@ -357,15 +370,16 @@
         Parameters
         ----------
         array_slim
             The masked 2D array of values in its slim representation (e.g. the image data) which are mapped to the
             source domain in order to compute their average values.
         """
         return mapper_util.mapped_to_source_via_mapping_matrix_from(
-            mapping_matrix=self.mapping_matrix, array_slim=array.binned.slim
+            mapping_matrix=self.mapping_matrix,
+            array_slim=np.array(array.slim),
         )
 
     def extent_from(
         self, values: np.ndarray = None, zoom_to_brightest: bool = True
     ) -> Tuple[float, float, float, float]:
         if zoom_to_brightest and values is not None:
             zoom_percent = conf.instance["visualize"]["general"]["zoom"][
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/delaunay.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/delaunay.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,68 @@
 import numpy as np
-from typing import Dict, Optional
 
 from autoconf import cached_property
 
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.inversion.pixelization.mappers.abstract import PixSubWeights
-from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids
-from autoarray.inversion.regularization.abstract import AbstractRegularization
 
 from autoarray.numba_util import profile_func
 from autoarray.inversion.pixelization.mappers import mapper_util
 
 
 class MapperDelaunay(AbstractMapper):
-    def __init__(
-        self,
-        mapper_grids: MapperGrids,
-        regularization: Optional[AbstractRegularization],
-        run_time_dict: Optional[Dict] = None,
-    ):
-        """
-        To understand a `Mapper` one must be familiar `Mesh` objects and the `mesh` and `pixelization` packages, where
-        the four grids grouped in a `MapperGrids` object are explained (`image_plane_data_grid`, `source_plane_data_grid`,
-        `image_plane_mesh_grid`,`source_plane_mesh_grid`)
-
-        If you are unfamliar withe above objects, read through the docstrings of the `pixelization`, `mesh` and
-        `mapper_grids` packages.
-
-        A `Mapper` determines the mappings between the masked data grid's pixels (`image_plane_data_grid` and
-        `source_plane_data_grid`) and the pxelization's pixels (`image_plane_mesh_grid` and `source_plane_mesh_grid`).
-
-        The 1D Indexing of each grid is identical in the `data` and `source` frames (e.g. the transformation does not
-        change the indexing, such that `source_plane_data_grid[0]` corresponds to the transformed value
-        of `image_plane_data_grid[0]` and so on).
-
-        A mapper therefore only needs to determine the index mappings between the `grid_slim` and `mesh_grid`,
-        noting that associations are made by pairing `source_plane_mesh_grid` with `source_plane_data_grid`.
-
-        Mappings are represented in the 2D ndarray `pix_indexes_for_sub_slim_index`, whereby the index of
-        a pixel on the `mesh_grid` maps to the index of a pixel on the `grid_slim` as follows:
-
-        - pix_indexes_for_sub_slim_index[0, 0] = 0: the data's 1st sub-pixel maps to the pixelization's 1st pixel.
-        - pix_indexes_for_sub_slim_index[1, 0] = 3: the data's 2nd sub-pixel maps to the pixelization's 4th pixel.
-        - pix_indexes_for_sub_slim_index[2, 0] = 1: the data's 3rd sub-pixel maps to the pixelization's 2nd pixel.
-
-        The second dimension of this array (where all three examples above are 0) is used for cases where a
-        single pixel on the `grid_slim` maps to multiple pixels on the `mesh_grid`. For example, using a
-        `Delaunay` pixelization, where every `grid_slim` pixel maps to three Delaunay pixels (the corners of the
-        triangles):
-
-        - pix_indexes_for_sub_slim_index[0, 0] = 0: the data's 1st sub-pixel maps to the pixelization's 1st pixel.
-        - pix_indexes_for_sub_slim_index[0, 1] = 3: the data's 1st sub-pixel also maps to the pixelization's 4th pixel.
-        - pix_indexes_for_sub_slim_index[0, 2] = 5: the data's 1st sub-pixel also maps to the pixelization's 6th pixel.
-
-        The mapper allows us to create a mapping matrix, which is a matrix representing the mapping between every
-        unmasked data pixel annd the pixels of a pixelization. This matrix is the basis of performing an `Inversion`,
-        which reconstructs the data using the `source_plane_mesh_grid`.
-
-        Parameters
-        ----------
-        mapper_grids
-            An object containing the data grid and mesh grid in both the data-frame and source-frame used by the
-            mapper to map data-points to linear object parameters.
-        regularization
-            The regularization scheme which may be applied to this linear object in order to smooth its solution,
-            which for a mapper smooths neighboring pixels on the mesh.
-        run_time_dict
-            A dictionary which contains timing of certain functions calls which is used for profiling.
-        """
-        super().__init__(
-            mapper_grids=mapper_grids,
-            regularization=regularization,
-            run_time_dict=run_time_dict,
-        )
+    """
+    To understand a `Mapper` one must be familiar `Mesh` objects and the `mesh` and `pixelization` packages, where
+    the four grids grouped in a `MapperGrids` object are explained (`image_plane_data_grid`, `source_plane_data_grid`,
+    `image_plane_mesh_grid`,`source_plane_mesh_grid`)
+
+    If you are unfamliar withe above objects, read through the docstrings of the `pixelization`, `mesh` and
+    `mapper_grids` packages.
+
+    A `Mapper` determines the mappings between the masked data grid's pixels (`image_plane_data_grid` and
+    `source_plane_data_grid`) and the pxelization's pixels (`image_plane_mesh_grid` and `source_plane_mesh_grid`).
+
+    The 1D Indexing of each grid is identical in the `data` and `source` frames (e.g. the transformation does not
+    change the indexing, such that `source_plane_data_grid[0]` corresponds to the transformed value
+    of `image_plane_data_grid[0]` and so on).
+
+    A mapper therefore only needs to determine the index mappings between the `grid_slim` and `mesh_grid`,
+    noting that associations are made by pairing `source_plane_mesh_grid` with `source_plane_data_grid`.
+
+    Mappings are represented in the 2D ndarray `pix_indexes_for_sub_slim_index`, whereby the index of
+    a pixel on the `mesh_grid` maps to the index of a pixel on the `grid_slim` as follows:
+
+    - pix_indexes_for_sub_slim_index[0, 0] = 0: the data's 1st sub-pixel maps to the pixelization's 1st pixel.
+    - pix_indexes_for_sub_slim_index[1, 0] = 3: the data's 2nd sub-pixel maps to the pixelization's 4th pixel.
+    - pix_indexes_for_sub_slim_index[2, 0] = 1: the data's 3rd sub-pixel maps to the pixelization's 2nd pixel.
+
+    The second dimension of this array (where all three examples above are 0) is used for cases where a
+    single pixel on the `grid_slim` maps to multiple pixels on the `mesh_grid`. For example, using a
+    `Delaunay` pixelization, where every `grid_slim` pixel maps to three Delaunay pixels (the corners of the
+    triangles):
+
+    - pix_indexes_for_sub_slim_index[0, 0] = 0: the data's 1st sub-pixel maps to the pixelization's 1st pixel.
+    - pix_indexes_for_sub_slim_index[0, 1] = 3: the data's 1st sub-pixel also maps to the pixelization's 4th pixel.
+    - pix_indexes_for_sub_slim_index[0, 2] = 5: the data's 1st sub-pixel also maps to the pixelization's 6th pixel.
+
+    The mapper allows us to create a mapping matrix, which is a matrix representing the mapping between every
+    unmasked data pixel annd the pixels of a pixelization. This matrix is the basis of performing an `Inversion`,
+    which reconstructs the data using the `source_plane_mesh_grid`.
+
+    Parameters
+    ----------
+    mapper_grids
+        An object containing the data grid and mesh grid in both the data-frame and source-frame used by the
+        mapper to map data-points to linear object parameters.
+    regularization
+        The regularization scheme which may be applied to this linear object in order to smooth its solution,
+        which for a mapper smooths neighboring pixels on the mesh.
+    run_time_dict
+        A dictionary which contains timing of certain functions calls which is used for profiling.
+    """
 
     @property
     def delaunay(self):
         return self.source_plane_mesh_grid.delaunay
 
     @cached_property
     @profile_func
@@ -127,26 +113,26 @@
 
         simplex_index_for_sub_slim_index = delaunay.find_simplex(
             self.source_plane_data_grid
         )
         pix_indexes_for_simplex_index = delaunay.simplices
 
         mappings, sizes = mapper_util.pix_indexes_for_sub_slim_index_delaunay_from(
-            source_plane_data_grid=self.source_plane_data_grid,
+            source_plane_data_grid=np.array(self.source_plane_data_grid),
             simplex_index_for_sub_slim_index=simplex_index_for_sub_slim_index,
             pix_indexes_for_simplex_index=pix_indexes_for_simplex_index,
             delaunay_points=delaunay.points,
         )
 
         mappings = mappings.astype("int")
         sizes = sizes.astype("int")
 
         weights = mapper_util.pixel_weights_delaunay_from(
-            source_plane_data_grid=self.source_plane_data_grid,
-            source_plane_mesh_grid=self.source_plane_mesh_grid,
+            source_plane_data_grid=np.array(self.source_plane_data_grid),
+            source_plane_mesh_grid=np.array(self.source_plane_mesh_grid),
             slim_index_for_sub_slim_index=self.slim_index_for_sub_slim_index,
             pix_indexes_for_sub_slim_index=mappings,
         )
 
         return PixSubWeights(mappings=mappings, sizes=sizes, weights=weights)
 
     @property
@@ -177,15 +163,15 @@
             simplex_index_for_sub_slim_index=splitted_simplex_index_for_sub_slim_index,
             pix_indexes_for_simplex_index=pix_indexes_for_simplex_index,
             delaunay_points=delaunay.points,
         )
 
         splitted_weights = mapper_util.pixel_weights_delaunay_from(
             source_plane_data_grid=self.source_plane_mesh_grid.split_cross,
-            source_plane_mesh_grid=self.source_plane_mesh_grid,
+            source_plane_mesh_grid=np.array(self.source_plane_mesh_grid),
             slim_index_for_sub_slim_index=self.source_plane_mesh_grid.split_cross,
             pix_indexes_for_sub_slim_index=splitted_mappings.astype("int"),
         )
 
         append_line_int = np.zeros((len(splitted_weights), 1), dtype="int") - 1
         append_line_float = np.zeros((len(splitted_weights), 1), dtype="float")
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/factory.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from typing import Dict, Optional
 
 from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids
+from autoarray.inversion.pixelization.border_relocator import BorderRelocator
+from autoarray.operators.over_sampling.abstract import AbstractOverSampler
 from autoarray.inversion.regularization.abstract import AbstractRegularization
 from autoarray.structures.mesh.rectangular_2d import Mesh2DRectangular
 from autoarray.structures.mesh.delaunay_2d import Mesh2DDelaunay
 from autoarray.structures.mesh.voronoi_2d import Mesh2DVoronoi
 
 
 def mapper_from(
     mapper_grids: MapperGrids,
     regularization: Optional[AbstractRegularization],
+    over_sampler: AbstractOverSampler,
+    border_relocator: Optional[BorderRelocator] = None,
     run_time_dict: Optional[Dict] = None,
 ):
     """
     Factory which given input `MapperGrids` and `Regularization` objects creates a `Mapper`.
 
     A `Mapper` determines the mappings between a masked dataset's pixels and pixels of a linear object pixelization.
     The mapper is used in order to fit a dataset via an inversion. Docstrings in the packages `linear_obj`, `mesh`,
@@ -43,29 +47,37 @@
     from autoarray.inversion.pixelization.mappers.delaunay import MapperDelaunay
     from autoarray.inversion.pixelization.mappers.voronoi import MapperVoronoi
     from autoarray.inversion.pixelization.mappers.voronoi import MapperVoronoiNoInterp
 
     if isinstance(mapper_grids.source_plane_mesh_grid, Mesh2DRectangular):
         return MapperRectangularNoInterp(
             mapper_grids=mapper_grids,
+            over_sampler=over_sampler,
+            border_relocator=border_relocator,
             regularization=regularization,
             run_time_dict=run_time_dict,
         )
     elif isinstance(mapper_grids.source_plane_mesh_grid, Mesh2DDelaunay):
         return MapperDelaunay(
             mapper_grids=mapper_grids,
+            over_sampler=over_sampler,
+            border_relocator=border_relocator,
             regularization=regularization,
             run_time_dict=run_time_dict,
         )
     elif isinstance(mapper_grids.source_plane_mesh_grid, Mesh2DVoronoi):
         if mapper_grids.source_plane_mesh_grid.uses_interpolation:
             return MapperVoronoi(
                 mapper_grids=mapper_grids,
+                over_sampler=over_sampler,
+                border_relocator=border_relocator,
                 regularization=regularization,
                 run_time_dict=run_time_dict,
             )
 
         return MapperVoronoiNoInterp(
             mapper_grids=mapper_grids,
+            over_sampler=over_sampler,
+            border_relocator=border_relocator,
             regularization=regularization,
             run_time_dict=run_time_dict,
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/mapper_grids.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/mapper_grids.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 import numpy as np
 from typing import TYPE_CHECKING, Dict, Optional
 
 if TYPE_CHECKING:
     from autoarray import Preloads
 
+from autoarray.mask.mask_2d import Mask2D
 from autoarray.structures.arrays.uniform_2d import Array2D
 from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 from autoarray.structures.mesh.abstract_2d import Abstract2DMesh
 
 from autoarray.structures.grids import grid_2d_util
 
 
 class MapperGrids:
     def __init__(
         self,
+        mask: Mask2D,
         source_plane_data_grid: Grid2D,
         source_plane_mesh_grid: Optional[Abstract2DMesh] = None,
         image_plane_mesh_grid: Optional[Grid2DIrregular] = None,
         adapt_data: Optional[np.ndarray] = None,
         preloads: Optional[Preloads] = None,
         run_time_dict: Optional[Dict] = None,
     ):
@@ -62,31 +64,32 @@
             for example the `source_plane_mesh_grid` could be preloaded.
         run_time_dict
             A dictionary which contains timing of certain functions calls which is used for profiling.
         """
 
         from autoarray.preloads import Preloads
 
+        self.mask = mask
         self.source_plane_data_grid = source_plane_data_grid
         self.source_plane_mesh_grid = source_plane_mesh_grid
         self.image_plane_mesh_grid = image_plane_mesh_grid
         self.adapt_data = adapt_data
         self.preloads = preloads or Preloads()
         self.run_time_dict = run_time_dict
 
     @property
     def image_plane_data_grid(self):
-        return self.source_plane_data_grid.derive_grid.unmasked
+        return self.mask.derive_grid.unmasked
 
     @property
     def mesh_pixels_per_image_pixels(self):
         mesh_pixels_per_image_pixels = grid_2d_util.grid_pixels_in_mask_pixels_from(
-            grid=self.image_plane_mesh_grid,
-            shape_native=self.source_plane_data_grid.mask.shape_native,
-            pixel_scales=self.source_plane_data_grid.mask.pixel_scales,
-            origin=self.source_plane_data_grid.mask.origin,
+            grid=np.array(self.image_plane_mesh_grid),
+            shape_native=self.mask.shape_native,
+            pixel_scales=self.mask.pixel_scales,
+            origin=self.mask.origin,
         )
 
         return Array2D(
             values=mesh_pixels_per_image_pixels,
-            mask=self.source_plane_data_grid.derive_mask.sub_1,
+            mask=self.mask,
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/mapper_util.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/mapper_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 @numba_util.jit()
 def data_slim_to_pixelization_unique_from(
     data_pixels,
     pix_indexes_for_sub_slim_index: np.ndarray,
     pix_sizes_for_sub_slim_index: np.ndarray,
     pix_weights_for_sub_slim_index,
     pix_pixels: int,
-    sub_size: int,
+    sub_size: np.ndarray,
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Create an array describing the unique mappings between the sub-pixels of every slim data pixel and the pixelization
     pixels, which is used to perform efficiently linear algebra calculations.
 
     For example, assuming `sub_size=2`:
 
@@ -99,41 +99,50 @@
         that give the weights and total number of mappings.
     """
 
     sub_fraction = 1.0 / (sub_size**2.0)
 
     max_pix_mappings = int(np.max(pix_sizes_for_sub_slim_index))
 
-    data_to_pix_unique = -1 * np.ones((data_pixels, max_pix_mappings * sub_size**2))
-    data_weights = np.zeros((data_pixels, max_pix_mappings * sub_size**2))
+    # TODO : Work out if we can reduce size from np.max(sub_size) using sub_size of max_pix_mappings.
+
+    data_to_pix_unique = -1 * np.ones(
+        (data_pixels, max_pix_mappings * np.max(sub_size) ** 2)
+    )
+    data_weights = np.zeros((data_pixels, max_pix_mappings * np.max(sub_size) ** 2))
     pix_lengths = np.zeros(data_pixels)
     pix_check = -1 * np.ones(shape=pix_pixels)
 
+    ip_sub_start = 0
+
     for ip in range(data_pixels):
         pix_check[:] = -1
 
         pix_size = 0
 
-        ip_sub_start = ip * sub_size**2
-        ip_sub_end = ip_sub_start + sub_size**2
+        ip_sub_end = ip_sub_start + sub_size[ip] ** 2
 
         for ip_sub in range(ip_sub_start, ip_sub_end):
             for pix_interp_index in range(pix_sizes_for_sub_slim_index[ip_sub]):
                 pix = pix_indexes_for_sub_slim_index[ip_sub, pix_interp_index]
                 pixel_weight = pix_weights_for_sub_slim_index[ip_sub, pix_interp_index]
 
                 if pix_check[pix] > -0.5:
-                    data_weights[ip, int(pix_check[pix])] += sub_fraction * pixel_weight
+                    data_weights[ip, int(pix_check[pix])] += (
+                        sub_fraction[ip] * pixel_weight
+                    )
 
                 else:
                     data_to_pix_unique[ip, pix_size] = pix
-                    data_weights[ip, pix_size] += sub_fraction * pixel_weight
+                    data_weights[ip, pix_size] += sub_fraction[ip] * pixel_weight
                     pix_check[pix] = pix_size
                     pix_size += 1
 
+        ip_sub_start = ip_sub_end
+
         pix_lengths[ip] = pix_size
 
     return data_to_pix_unique, data_weights, pix_lengths
 
 
 @numba_util.jit()
 def pix_indexes_for_sub_slim_index_delaunay_from(
@@ -439,29 +448,29 @@
     (
         pix_weights_for_sub_slim_index,
         pix_indexes_for_sub_slim_index,
     ) = remove_bad_entries_voronoi_nn(
         bad_indexes=bad_indexes,
         pix_weights_for_sub_slim_index=pix_weights_for_sub_slim_index,
         pix_indexes_for_sub_slim_index=pix_indexes_for_sub_slim_index,
-        grid=grid,
-        mesh_grid=mesh_grid,
+        grid=np.array(grid),
+        mesh_grid=np.array(mesh_grid),
     )
 
     bad_indexes = np.argwhere(pix_indexes_for_sub_slim_index[:, 0] == -1)
 
     (
         pix_weights_for_sub_slim_index,
         pix_indexes_for_sub_slim_index,
     ) = remove_bad_entries_voronoi_nn(
         bad_indexes=bad_indexes,
         pix_weights_for_sub_slim_index=pix_weights_for_sub_slim_index,
         pix_indexes_for_sub_slim_index=pix_indexes_for_sub_slim_index,
-        grid=grid,
-        mesh_grid=mesh_grid,
+        grid=np.array(grid),
+        mesh_grid=np.array(mesh_grid),
     )
 
     pix_indexes_for_sub_slim_index_sizes = np.sum(
         pix_indexes_for_sub_slim_index != -1, axis=1
     )
 
     if np.max(pix_indexes_for_sub_slim_index_sizes) > max_nneighbours:
@@ -593,15 +602,15 @@
 def mapping_matrix_from(
     pix_indexes_for_sub_slim_index: np.ndarray,
     pix_size_for_sub_slim_index: np.ndarray,
     pix_weights_for_sub_slim_index: np.ndarray,
     pixels: int,
     total_mask_pixels: int,
     slim_index_for_sub_slim_index: np.ndarray,
-    sub_fraction: float,
+    sub_fraction: np.ndarray,
 ) -> np.ndarray:
     """
     Returns the mapping matrix, which is a matrix representing the mapping between every unmasked sub-pixel of the data
     and the pixels of a pixelization. Non-zero entries signify a mapping, whereas zeros signify no mapping.
 
     For example, if the data has 5 unmasked pixels (with `sub_size=1` so there are not sub-pixels) and the pixelization
     3 pixels, with the following mappings:
@@ -676,15 +685,17 @@
     for sub_slim_index in range(slim_index_for_sub_slim_index.shape[0]):
         slim_index = slim_index_for_sub_slim_index[sub_slim_index]
 
         for pix_count in range(pix_size_for_sub_slim_index[sub_slim_index]):
             pix_index = pix_indexes_for_sub_slim_index[sub_slim_index, pix_count]
             pix_weight = pix_weights_for_sub_slim_index[sub_slim_index, pix_count]
 
-            mapping_matrix[slim_index][pix_index] += sub_fraction * pix_weight
+            mapping_matrix[slim_index][pix_index] += (
+                sub_fraction[slim_index] * pix_weight
+            )
 
     return mapping_matrix
 
 
 @numba_util.jit()
 def mapped_to_source_via_mapping_matrix_from(
     mapping_matrix: np.ndarray, array_slim: np.ndarray
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/rectangular.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/rectangular.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,68 @@
 import numpy as np
-from typing import Dict, Optional, Tuple
+from typing import Tuple
 
 from autoconf import cached_property
 
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.inversion.pixelization.mappers.abstract import PixSubWeights
-from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids
-from autoarray.inversion.regularization.abstract import AbstractRegularization
 
 from autoarray.numba_util import profile_func
 from autoarray.geometry import geometry_util
 
 
 class MapperRectangularNoInterp(AbstractMapper):
-    def __init__(
-        self,
-        mapper_grids: MapperGrids,
-        regularization: Optional[AbstractRegularization],
-        run_time_dict: Optional[Dict] = None,
-    ):
-        """
-         To understand a `Mapper` one must be familiar `Mesh` objects and the `mesh` and `pixelization` packages, where
-         the four grids grouped in a `MapperGrids` object are explained (`image_plane_data_grid`, `source_plane_data_grid`,
-         `image_plane_mesh_grid`,`source_plane_mesh_grid`)
-
-         If you are unfamliar withe above objects, read through the docstrings of the `pixelization`, `mesh` and
-         `mapper_grids` packages.
-
-         A `Mapper` determines the mappings between the masked data grid's pixels (`image_plane_data_grid` and
-         `source_plane_data_grid`) and the mesh's pixels (`image_plane_mesh_grid` and `source_plane_mesh_grid`).
-
-         The 1D Indexing of each grid is identical in the `data` and `source` frames (e.g. the transformation does not
-         change the indexing, such that `source_plane_data_grid[0]` corresponds to the transformed value
-         of `image_plane_data_grid[0]` and so on).
-
-         A mapper therefore only needs to determine the index mappings between the `grid_slim` and `mesh_grid`,
-         noting that associations are made by pairing `source_plane_mesh_grid` with `source_plane_data_grid`.
-
-         Mappings are represented in the 2D ndarray `pix_indexes_for_sub_slim_index`, whereby the index of
-         a pixel on the `mesh_grid` maps to the index of a pixel on the `grid_slim` as follows:
-
-         - pix_indexes_for_sub_slim_index[0, 0] = 0: the data's 1st sub-pixel maps to the mesh's 1st pixel.
-         - pix_indexes_for_sub_slim_index[1, 0] = 3: the data's 2nd sub-pixel maps to the mesh's 4th pixel.
-         - pix_indexes_for_sub_slim_index[2, 0] = 1: the data's 3rd sub-pixel maps to the mesh's 2nd pixel.
-
-         The second dimension of this array (where all three examples above are 0) is used for cases where a
-         single pixel on the `grid_slim` maps to multiple pixels on the `mesh_grid`. For example, a
-         `Delaunay` triangulation, where every `grid_slim` pixel maps to three Delaunay pixels (the corners of the
-         triangles) with varying interpolation weights .
-
-         For a `Rectangular` mesh every pixel in the masked data maps to only one pixel, thus the second
-         dimension of `pix_indexes_for_sub_slim_index` is always of size 1.
-
-         The mapper allows us to create a mapping matrix, which is a matrix representing the mapping between every
-         unmasked data pixel annd the pixels of a mesh. This matrix is the basis of performing an `Inversion`,
-         which reconstructs the data using the `source_plane_mesh_grid`.
-
-         Parameters
-         ----------
-         mapper_grids
-             An object containing the data grid and mesh grid in both the data-frame and source-frame used by the
-             mapper to map data-points to linear object parameters.
-         regularization
-             The regularization scheme which may be applied to this linear object in order to smooth its solution,
-             which for a mapper smooths neighboring pixels on the mesh.
-        relocate_pix_border
-             If `True`, all coordinates of all pixelization source mesh grids have pixels outside their border
-             relocated to their edge.
-         run_time_dict
-             A dictionary which contains timing of certain functions calls which is used for profiling.
-        """
-        super().__init__(
-            mapper_grids=mapper_grids,
-            regularization=regularization,
-            run_time_dict=run_time_dict,
-        )
+    """
+    To understand a `Mapper` one must be familiar `Mesh` objects and the `mesh` and `pixelization` packages, where
+    the four grids grouped in a `MapperGrids` object are explained (`image_plane_data_grid`, `source_plane_data_grid`,
+    `image_plane_mesh_grid`,`source_plane_mesh_grid`)
+
+    If you are unfamliar withe above objects, read through the docstrings of the `pixelization`, `mesh` and
+    `mapper_grids` packages.
+
+    A `Mapper` determines the mappings between the masked data grid's pixels (`image_plane_data_grid` and
+    `source_plane_data_grid`) and the mesh's pixels (`image_plane_mesh_grid` and `source_plane_mesh_grid`).
+
+    The 1D Indexing of each grid is identical in the `data` and `source` frames (e.g. the transformation does not
+    change the indexing, such that `source_plane_data_grid[0]` corresponds to the transformed value
+    of `image_plane_data_grid[0]` and so on).
+
+    A mapper therefore only needs to determine the index mappings between the `grid_slim` and `mesh_grid`,
+    noting that associations are made by pairing `source_plane_mesh_grid` with `source_plane_data_grid`.
+
+    Mappings are represented in the 2D ndarray `pix_indexes_for_sub_slim_index`, whereby the index of
+    a pixel on the `mesh_grid` maps to the index of a pixel on the `grid_slim` as follows:
+
+    - pix_indexes_for_sub_slim_index[0, 0] = 0: the data's 1st sub-pixel maps to the mesh's 1st pixel.
+    - pix_indexes_for_sub_slim_index[1, 0] = 3: the data's 2nd sub-pixel maps to the mesh's 4th pixel.
+    - pix_indexes_for_sub_slim_index[2, 0] = 1: the data's 3rd sub-pixel maps to the mesh's 2nd pixel.
+
+    The second dimension of this array (where all three examples above are 0) is used for cases where a
+    single pixel on the `grid_slim` maps to multiple pixels on the `mesh_grid`. For example, a
+    `Delaunay` triangulation, where every `grid_slim` pixel maps to three Delaunay pixels (the corners of the
+    triangles) with varying interpolation weights .
+
+    For a `Rectangular` mesh every pixel in the masked data maps to only one pixel, thus the second
+    dimension of `pix_indexes_for_sub_slim_index` is always of size 1.
+
+    The mapper allows us to create a mapping matrix, which is a matrix representing the mapping between every
+    unmasked data pixel annd the pixels of a mesh. This matrix is the basis of performing an `Inversion`,
+    which reconstructs the data using the `source_plane_mesh_grid`.
+
+    Parameters
+    ----------
+    mapper_grids
+        An object containing the data grid and mesh grid in both the data-frame and source-frame used by the
+        mapper to map data-points to linear object parameters.
+    regularization
+        The regularization scheme which may be applied to this linear object in order to smooth its solution,
+        which for a mapper smooths neighboring pixels on the mesh.
+    run_time_dict
+        A dictionary which contains timing of certain functions calls which is used for profiling.
+    """
 
     @property
     def shape_native(self) -> Tuple[int, ...]:
         return self.source_plane_mesh_grid.shape_native
 
     @cached_property
     @profile_func
@@ -112,15 +96,15 @@
         are stored in the array `pix_weights_for_sub_slim_index`.
 
         For a Rectangular pixelization each data sub-pixel maps to a single mesh pixel, thus the second
         dimension of the array `pix_indexes_for_sub_slim_index` 1 and all entries in `pix_weights_for_sub_slim_index`
         are equal to 1.0.
         """
         mappings = geometry_util.grid_pixel_indexes_2d_slim_from(
-            grid_scaled_2d_slim=self.source_plane_data_grid,
+            grid_scaled_2d_slim=np.array(self.source_plane_data_grid),
             shape_native=self.source_plane_mesh_grid.shape_native,
             pixel_scales=self.source_plane_mesh_grid.pixel_scales,
             origin=self.source_plane_mesh_grid.origin,
         ).astype("int")
 
         mappings = mappings.reshape((len(mappings), 1))
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mappers/voronoi.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mappers/voronoi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,69 @@
 import numpy as np
-from typing import Dict, Optional, Tuple
+from typing import Optional, Tuple
 
 from autoconf import cached_property
 
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.inversion.pixelization.mappers.abstract import PixSubWeights
-from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids
-from autoarray.inversion.regularization.abstract import AbstractRegularization
 from autoarray.structures.arrays.uniform_2d import Array2D
 
 from autoarray.numba_util import profile_func
 from autoarray.inversion.pixelization.mappers import mapper_util
 
 
 class AbstractMapperVoronoi(AbstractMapper):
-    def __init__(
-        self,
-        mapper_grids: MapperGrids,
-        regularization: Optional[AbstractRegularization],
-        run_time_dict: Optional[Dict] = None,
-    ):
-        """
-        To understand a `Mapper` one must be familiar `Mesh` objects and the `mesh` and `pixelization` packages, where
-        the four grids grouped in a `MapperGrids` object are explained (`image_plane_data_grid`, `source_plane_data_grid`,
-        `image_plane_mesh_grid`,`source_plane_mesh_grid`)
-
-        If you are unfamliar withe above objects, read through the docstrings of the `pixelization`, `mesh` and
-        `mapper_grids` packages.
-
-        A `Mapper` determines the mappings between the masked data grid's pixels (`image_plane_data_grid` and
-        `source_plane_data_grid`) and the pxelization's pixels (`image_plane_mesh_grid` and `source_plane_mesh_grid`).
-
-        The 1D Indexing of each grid is identical in the `data` and `source` frames (e.g. the transformation does not
-        change the indexing, such that `source_plane_data_grid[0]` corresponds to the transformed value
-        of `image_plane_data_grid[0]` and so on).
-
-        A mapper therefore only needs to determine the index mappings between the `grid_slim` and `mesh_grid`,
-        noting that associations are made by pairing `source_plane_mesh_grid` with `source_plane_data_grid`.
-
-        Mappings are represented in the 2D ndarray `pix_indexes_for_sub_slim_index`, whereby the index of
-        a pixel on the `mesh_grid` maps to the index of a pixel on the `grid_slim` as follows:
-
-        - pix_indexes_for_sub_slim_index[0, 0] = 0: the data's 1st sub-pixel maps to the mesh's 1st pixel.
-        - pix_indexes_for_sub_slim_index[1, 0] = 3: the data's 2nd sub-pixel maps to the mesh's 4th pixel.
-        - pix_indexes_for_sub_slim_index[2, 0] = 1: the data's 3rd sub-pixel maps to the mesh's 2nd pixel.
-
-        The second dimension of this array (where all three examples above are 0) is used for cases where a
-        single pixel on the `grid_slim` maps to multiple pixels on the `mesh_grid`. For example, using a
-        `Delaunay` mesh, where every `grid_slim` pixel maps to three Delaunay pixels (the corners of the
-        triangles):
-
-        For a `Voronoi` mesh every pixel in the masked data maps to only one Voronoi pixel, thus the second
-        dimension of `pix_indexes_for_sub_slim_index` is always of size 1.
-
-        The mapper allows us to create a mapping matrix, which is a matrix representing the mapping between every
-        unmasked data pixel annd the pixels of a mesh. This matrix is the basis of performing an `Inversion`,
-        which reconstructs the data using the `source_plane_mesh_grid`.
-
-        Parameters
-        ----------
-        mapper_grids
-            An object containing the data grid and mesh grid in both the data-frame and source-frame used by the
-            mapper to map data-points to linear object parameters.
-        regularization
-            The regularization scheme which may be applied to this linear object in order to smooth its solution,
-            which for a mapper smooths neighboring pixels on the mesh.
-        run_time_dict
-            A dictionary which contains timing of certain functions calls which is used for profiling.
-        """
-        super().__init__(
-            mapper_grids=mapper_grids,
-            regularization=regularization,
-            run_time_dict=run_time_dict,
-        )
+    """
+    To understand a `Mapper` one must be familiar `Mesh` objects and the `mesh` and `pixelization` packages, where
+    the four grids grouped in a `MapperGrids` object are explained (`image_plane_data_grid`, `source_plane_data_grid`,
+    `image_plane_mesh_grid`,`source_plane_mesh_grid`)
+
+    If you are unfamliar withe above objects, read through the docstrings of the `pixelization`, `mesh` and
+    `mapper_grids` packages.
+
+    A `Mapper` determines the mappings between the masked data grid's pixels (`image_plane_data_grid` and
+    `source_plane_data_grid`) and the pxelization's pixels (`image_plane_mesh_grid` and `source_plane_mesh_grid`).
+
+    The 1D Indexing of each grid is identical in the `data` and `source` frames (e.g. the transformation does not
+    change the indexing, such that `source_plane_data_grid[0]` corresponds to the transformed value
+    of `image_plane_data_grid[0]` and so on).
+
+    A mapper therefore only needs to determine the index mappings between the `grid_slim` and `mesh_grid`,
+    noting that associations are made by pairing `source_plane_mesh_grid` with `source_plane_data_grid`.
+
+    Mappings are represented in the 2D ndarray `pix_indexes_for_sub_slim_index`, whereby the index of
+    a pixel on the `mesh_grid` maps to the index of a pixel on the `grid_slim` as follows:
+
+    - pix_indexes_for_sub_slim_index[0, 0] = 0: the data's 1st sub-pixel maps to the mesh's 1st pixel.
+    - pix_indexes_for_sub_slim_index[1, 0] = 3: the data's 2nd sub-pixel maps to the mesh's 4th pixel.
+    - pix_indexes_for_sub_slim_index[2, 0] = 1: the data's 3rd sub-pixel maps to the mesh's 2nd pixel.
+
+    The second dimension of this array (where all three examples above are 0) is used for cases where a
+    single pixel on the `grid_slim` maps to multiple pixels on the `mesh_grid`. For example, using a
+    `Delaunay` mesh, where every `grid_slim` pixel maps to three Delaunay pixels (the corners of the
+    triangles):
+
+    For a `Voronoi` mesh every pixel in the masked data maps to only one Voronoi pixel, thus the second
+    dimension of `pix_indexes_for_sub_slim_index` is always of size 1.
+
+    The mapper allows us to create a mapping matrix, which is a matrix representing the mapping between every
+    unmasked data pixel annd the pixels of a mesh. This matrix is the basis of performing an `Inversion`,
+    which reconstructs the data using the `source_plane_mesh_grid`.
+
+    Parameters
+    ----------
+    mapper_grids
+        An object containing the data grid and mesh grid in both the data-frame and source-frame used by the
+        mapper to map data-points to linear object parameters.
+    regularization
+        The regularization scheme which may be applied to this linear object in order to smooth its solution,
+        which for a mapper smooths neighboring pixels on the mesh.
+    run_time_dict
+        A dictionary which contains timing of certain functions calls which is used for profiling.
+    """
 
     @property
     def voronoi(self):
         return self.source_plane_mesh_grid.voronoi
 
     @property
     def pix_sub_weights_split_cross(self) -> PixSubWeights:
@@ -225,17 +212,17 @@
         For this Voronoi mesh each data sub-pixel maps to a single pixelization pixel, thus the second
         dimension of the array `pix_indexes_for_sub_slim_index` 1 and all entries in `pix_weights_for_sub_slim_index`
         are equal to 1.0.
 
         The weights are used when creating the `mapping_matrix` and `pixel_signals_from`.
         """
         mappings = mapper_util.pix_indexes_for_sub_slim_index_voronoi_from(
-            grid=self.source_plane_data_grid,
-            slim_index_for_sub_slim_index=self.source_plane_data_grid.mask.derive_indexes.slim_for_sub_slim,
-            mesh_grid=self.source_plane_mesh_grid,
+            grid=np.array(self.source_plane_data_grid),
+            slim_index_for_sub_slim_index=self.over_sampler.slim_for_sub_slim,
+            mesh_grid=np.array(self.source_plane_mesh_grid),
             neighbors=self.source_plane_mesh_grid.neighbors,
             neighbors_sizes=self.source_plane_mesh_grid.neighbors.sizes,
         ).astype("int")
 
         return PixSubWeights(
             mappings=mappings,
             sizes=np.ones(self.source_plane_data_grid.shape[0], dtype="int"),
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/abstract.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,111 +1,111 @@
 import numpy as np
 from typing import Dict, Optional
 
 from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids
+from autoarray.inversion.pixelization.border_relocator import BorderRelocator
 from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 from autoarray.preloads import Preloads
 
 from autoarray.numba_util import profile_func
 
 
 class AbstractMesh:
     def __eq__(self, other):
         return self.__dict__ == other.__dict__ and self.__class__ is other.__class__
 
     @profile_func
     def relocated_grid_from(
         self,
+        border_relocator: BorderRelocator,
         source_plane_data_grid: Grid2D,
         preloads: Preloads = Preloads(),
-        relocate_pix_border: bool = False,
     ) -> Grid2D:
         """
-         Relocates all coordinates of the input `source_plane_data_grid` that are outside of a
-         border (which is defined by a grid of (y,x) coordinates) to the edge of this border.
+        Relocates all coordinates of the input `source_plane_data_grid` that are outside of a
+        border (which is defined by a grid of (y,x) coordinates) to the edge of this border.
 
-         The border is determined from the mask of the 2D data in the `data` frame before any transformations of the
-         data's grid are performed. The border is all pixels in this mask that are pixels at its extreme edge. These
-         pixel indexes are used to then determine a grid of (y,x) coordinates from the transformed `source_grid_grid` in
-         the `source` reference frame, whereby points located outside of it are relocated to the border's edge.
-
-         A full description of relocation is given in the method grid_2d.relocated_grid_from()`.
-
-         This is used in the project PyAutoLens to relocate the coordinates that are ray-traced near the centre of mass
-         of galaxies, which are heavily demagnified and may trace to outskirts of the source-plane well beyond the
-         border.
-
-         Parameters
-         ----------
-         source_plane_data_grid
-             A 2D (y,x) grid of coordinates, whose coordinates outside the border are relocated to its edge.
-         preloads
-             Contains quantities which may already be computed and can be preloaded to speed up calculations, in this
-             case the relocated grid.
-        relocate_pix_border
-             If `True`, all coordinates of all pixelization source mesh grids have pixels outside their border
-             relocated to their edge.
+        The border is determined from the mask of the 2D data in the `data` frame before any transformations of the
+        data's grid are performed. The border is all pixels in this mask that are pixels at its extreme edge. These
+        pixel indexes are used to then determine a grid of (y,x) coordinates from the transformed `source_grid_grid` in
+        the `source` reference frame, whereby points located outside of it are relocated to the border's edge.
+
+        A full description of relocation is given in the method grid_2d.relocated_grid_from()`.
+
+        This is used in the project PyAutoLens to relocate the coordinates that are ray-traced near the centre of mass
+        of galaxies, which are heavily demagnified and may trace to outskirts of the source-plane well beyond the
+        border.
+
+        Parameters
+        ----------
+        border_relocator
+           The border relocator, which relocates coordinates outside the border of the source-plane data grid to its
+           edge.
+        source_plane_data_grid
+            A 2D (y,x) grid of coordinates, whose coordinates outside the border are relocated to its edge.
+        preloads
+            Contains quantities which may already be computed and can be preloaded to speed up calculations, in this
+            case the relocated grid.
         """
         if preloads.relocated_grid is None:
-            if relocate_pix_border:
-                return source_plane_data_grid.relocated_grid_from(
-                    grid=source_plane_data_grid
-                )
+            if border_relocator is not None:
+                return border_relocator.relocated_grid_from(grid=source_plane_data_grid)
             return source_plane_data_grid
 
         return preloads.relocated_grid
 
     @profile_func
     def relocated_mesh_grid_from(
         self,
+        border_relocator: Optional[BorderRelocator],
         source_plane_data_grid: Grid2D,
         source_plane_mesh_grid: Grid2DIrregular,
-        relocate_pix_border: bool = False,
     ):
         """
-         Relocates all coordinates of the input `source_plane_mesh_grid` that are outside of a border (which
-         is defined by a grid of (y,x) coordinates) to the edge of this border.
+        Relocates all coordinates of the input `source_plane_mesh_grid` that are outside of a border (which
+        is defined by a grid of (y,x) coordinates) to the edge of this border.
 
-         The border is determined from the mask of the 2D data in the `data` frame before any transformations of the
-         data's grid are performed. The border is all pixels in this mask that are pixels at its extreme edge. These
-         pixel indexes are used to then determine a grid of (y,x) coordinates from the transformed `source_grid_grid` in
-         the `source` reference frame, whereby points located outside of it are relocated to the border's edge.
-
-         A full description of relocation is given in the method grid_2d.relocated_grid_from()`.
-
-         This is used in the project `PyAutoLens` to relocate the coordinates that are ray-traced near the centre of mass
-         of galaxies, which are heavily demagnified and may trace to outskirts of the source-plane well beyond the
-         border.
-
-         Parameters
-         ----------
-         source_plane_data_grid
-             A 2D grid of (y,x) coordinates associated with the unmasked 2D data after it has been transformed to the
-             `source` reference frame.
-         source_plane_mesh_grid
-             The centres of every Voronoi pixel in the `source` frame, which are initially derived by computing a sparse
-             set of (y,x) coordinates computed from the unmasked data in the `data` frame and applying a transformation
-             to this.
-        relocate_pix_border
-             If `True`, all coordinates of all pixelization source mesh grids have pixels outside their border
-             relocated to their edge.
+        The border is determined from the mask of the 2D data in the `data` frame before any transformations of the
+        data's grid are performed. The border is all pixels in this mask that are pixels at its extreme edge. These
+        pixel indexes are used to then determine a grid of (y,x) coordinates from the transformed `source_grid_grid` in
+        the `source` reference frame, whereby points located outside of it are relocated to the border's edge.
+
+        A full description of relocation is given in the method grid_2d.relocated_grid_from()`.
+
+        This is used in the project `PyAutoLens` to relocate the coordinates that are ray-traced near the centre of mass
+        of galaxies, which are heavily demagnified and may trace to outskirts of the source-plane well beyond the
+        border.
+
+        Parameters
+        ----------
+        border_relocator
+           The border relocator, which relocates coordinates outside the border of the source-plane data grid to its
+           edge.
+        source_plane_data_grid
+            A 2D grid of (y,x) coordinates associated with the unmasked 2D data after it has been transformed to the
+            `source` reference frame.
+        source_plane_mesh_grid
+            The centres of every Voronoi pixel in the `source` frame, which are initially derived by computing a sparse
+            set of (y,x) coordinates computed from the unmasked data in the `data` frame and applying a transformation
+            to this.
         """
-        if relocate_pix_border:
-            return source_plane_data_grid.relocated_mesh_grid_from(
-                mesh_grid=source_plane_mesh_grid
+        if border_relocator is not None:
+            return border_relocator.relocated_mesh_grid_from(
+                grid=source_plane_data_grid, mesh_grid=source_plane_mesh_grid
             )
         return source_plane_mesh_grid
 
     def mapper_grids_from(
         self,
+        mask,
         source_plane_data_grid: Grid2D,
+        border_relocator: Optional[BorderRelocator] = None,
         source_plane_mesh_grid: Optional[Grid2DIrregular] = None,
         image_plane_mesh_grid: Optional[Grid2DIrregular] = None,
-        relocate_pix_border: bool = False,
         adapt_data: np.ndarray = None,
         preloads: Preloads = Preloads(),
         run_time_dict: Optional[Dict] = None,
     ) -> MapperGrids:
         raise NotImplementedError
 
     def mesh_grid_from(
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/delaunay.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/delaunay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/mesh_util.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/mesh_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
     simplices = delaunay.simplices
     pixel_points = delaunay.points
 
     interpolated_array = np.zeros(len(interpolation_grid_slim))
 
     for slim_index in range(len(interpolation_grid_slim)):
         simplex_index = simplex_index_for_interpolate_index[slim_index]
-        interpolating_point = interpolation_grid_slim[slim_index]
+        interpolating_point = tuple(interpolation_grid_slim[slim_index])
 
         if simplex_index == -1:
             cloest_pixel_index = np.argmin(
                 np.sum((pixel_points - interpolating_point) ** 2.0, axis=1)
             )
             interpolated_array[slim_index] = pixel_values[cloest_pixel_index]
         else:
@@ -487,15 +487,14 @@
         neighbors[pair1, int(neighbors_index[pair1])] = pair0
         neighbors_index[pair0] += 1
         neighbors_index[pair1] += 1
 
     return neighbors, neighbors_sizes
 
 
-# @numba_util.jit()
 def voronoi_edge_pixels_from(regions: np.ndarray, point_region: np.ndarray) -> List:
     """
     Returns the edge pixels of a Voronoi mesh, where the edge pixels are defined as those pixels which are on the
     edge of the Voronoi diagram.
 
     Parameters
     ----------
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/rectangular.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/rectangular.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 
 from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.structures.mesh.rectangular_2d import Mesh2DRectangular
 from autoarray.preloads import Preloads
 from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids
 from autoarray.inversion.pixelization.mesh.abstract import AbstractMesh
+from autoarray.inversion.pixelization.border_relocator import BorderRelocator
 
 from autoarray import exc
 from autoarray.numba_util import profile_func
 
 
 class Rectangular(AbstractMesh):
     def __init__(self, shape: Tuple[int, int] = (3, 3)):
@@ -58,69 +59,71 @@
         """
         Does this ``Mesh`` object use interpolation when pairing with another 2D grid?
         """
         return False
 
     def mapper_grids_from(
         self,
+        mask,
         source_plane_data_grid: Grid2D,
+        border_relocator: Optional[BorderRelocator] = None,
         source_plane_mesh_grid: Grid2D = None,
         image_plane_mesh_grid: Grid2D = None,
         adapt_data: np.ndarray = None,
-        relocate_pix_border: bool = False,
         preloads: Preloads = Preloads(),
         run_time_dict: Optional[Dict] = None,
     ) -> MapperGrids:
         """
-         Mapper objects describe the mappings between pixels in the masked 2D data and the pixels in a pixelization,
-         in both the `data` and `source` frames.
+        Mapper objects describe the mappings between pixels in the masked 2D data and the pixels in a pixelization,
+        in both the `data` and `source` frames.
 
-         This function returns a `MapperRectangularNoInterp` as follows:
+        This function returns a `MapperRectangularNoInterp` as follows:
 
-         1) If `relocate_pix_border=True`, the border of the input `source_plane_data_grid` is used to relocate all of the
-            grid's (y,x) coordinates beyond the border to the edge of the border.
+        1) If the bordr relocator is input, the border of the input `source_plane_data_grid` is used to relocate all of the
+           grid's (y,x) coordinates beyond the border to the edge of the border.
 
-         2) Determine the (y,x) coordinates of the pixelization's rectangular pixels, by laying this rectangular grid
-            over the 2D grid of relocated (y,x) coordinates computed in step 1 (or the input `source_plane_data_grid` if step 1
-            is bypassed).
-
-         3) Return the `MapperRectangularNoInterp`.
-
-         Parameters
-         ----------
-         source_plane_data_grid
-             A 2D grid of (y,x) coordinates associated with the unmasked 2D data after it has been transformed to the
-             `source` reference frame.
-         source_plane_mesh_grid
-             Not used for a rectangular pixelization, because the pixelization grid in the `source` frame is computed
-             by overlaying the `source_plane_data_grid` with the rectangular pixelization.
-         image_plane_mesh_grid
-             Not used for a rectangular pixelization.
-         adapt_data
-             Not used for a rectangular pixelization.
-        relocate_pix_border
-             If `True`, all coordinates of all pixelization source mesh grids have pixels outside their border
-             relocated to their edge.
-         preloads
-             Object which may contain preloaded arrays of quantities computed in the pixelization, which are passed via
-             this object speed up the calculation.
-         run_time_dict
-             A dictionary which contains timing of certain functions calls which is used for profiling.
+        2) Determine the (y,x) coordinates of the pixelization's rectangular pixels, by laying this rectangular grid
+           over the 2D grid of relocated (y,x) coordinates computed in step 1 (or the input `source_plane_data_grid` if step 1
+           is bypassed).
+
+        3) Return the `MapperRectangularNoInterp`.
+
+        Parameters
+        ----------
+        border_relocator
+           The border relocator, which relocates coordinates outside the border of the source-plane data grid to its
+           edge.
+        source_plane_data_grid
+            A 2D grid of (y,x) coordinates associated with the unmasked 2D data after it has been transformed to the
+            `source` reference frame.
+        source_plane_mesh_grid
+            Not used for a rectangular pixelization, because the pixelization grid in the `source` frame is computed
+            by overlaying the `source_plane_data_grid` with the rectangular pixelization.
+        image_plane_mesh_grid
+            Not used for a rectangular pixelization.
+        adapt_data
+            Not used for a rectangular pixelization.
+        preloads
+            Object which may contain preloaded arrays of quantities computed in the pixelization, which are passed via
+            this object speed up the calculation.
+        run_time_dict
+            A dictionary which contains timing of certain functions calls which is used for profiling.
         """
 
         self.run_time_dict = run_time_dict
 
         relocated_grid = self.relocated_grid_from(
+            border_relocator=border_relocator,
             source_plane_data_grid=source_plane_data_grid,
-            relocate_pix_border=relocate_pix_border,
             preloads=preloads,
         )
         mesh_grid = self.mesh_grid_from(source_plane_data_grid=relocated_grid)
 
         return MapperGrids(
+            mask=mask,
             source_plane_data_grid=relocated_grid,
             source_plane_mesh_grid=mesh_grid,
             image_plane_mesh_grid=image_plane_mesh_grid,
             adapt_data=adapt_data,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/triangulation.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/triangulation.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,97 +2,100 @@
 from typing import Dict, Optional
 
 from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 from autoarray.preloads import Preloads
 from autoarray.inversion.pixelization.mappers.mapper_grids import MapperGrids
 from autoarray.inversion.pixelization.mesh.abstract import AbstractMesh
+from autoarray.inversion.pixelization.border_relocator import BorderRelocator
 
 
 class Triangulation(AbstractMesh):
     def mapper_grids_from(
         self,
+        mask,
         source_plane_data_grid: Grid2D,
+        border_relocator: Optional[BorderRelocator] = None,
         source_plane_mesh_grid: Optional[Grid2DIrregular] = None,
         image_plane_mesh_grid: Optional[Grid2DIrregular] = None,
-        relocate_pix_border: bool = False,
         adapt_data: np.ndarray = None,
         preloads: Preloads = Preloads(),
         run_time_dict: Optional[Dict] = None,
     ) -> MapperGrids:
         """
-         Mapper objects describe the mappings between pixels in the masked 2D data and the pixels in a mesh,
-         in both the `data` and `source` frames.
+        Mapper objects describe the mappings between pixels in the masked 2D data and the pixels in a mesh,
+        in both the `data` and `source` frames.
 
-         This function returns a `MapperVoronoiNoInterp` as follows:
+        This function returns a `MapperVoronoiNoInterp` as follows:
 
-         1) Before this routine is called, a sparse grid of (y,x) coordinates are computed from the 2D masked data,
-            the `image_plane_mesh_grid`, which acts as the Voronoi pixel centres of the mesh and mapper.
+        1) Before this routine is called, a sparse grid of (y,x) coordinates are computed from the 2D masked data,
+           the `image_plane_mesh_grid`, which acts as the Voronoi pixel centres of the mesh and mapper.
 
-         2) Before this routine is called, operations are performed on this `image_plane_mesh_grid` that transform it
-            from a 2D grid which overlaps with the 2D mask of the data in the `data` frame to an irregular grid in
-            the `source` frame, the `source_plane_mesh_grid`.
-
-         3) If `relocate_pix_border=True`, the border of the input `source_plane_data_grid` is used to relocate all of the
-            grid's (y,x) coordinates beyond the border to the edge of the border.
-
-         4) If `relocate_pix_border=True`, the border of the input `source_plane_data_grid` is used to relocate all of the
-            transformed `source_plane_mesh_grid`'s (y,x) coordinates beyond the border to the edge of the border.
-
-         5) Use the transformed `source_plane_mesh_grid`'s (y,x) coordinates as the centres of the Voronoi mesh.
-
-         6) Return the `MapperVoronoiNoInterp`.
-
-         Parameters
-         ----------
-         source_plane_data_grid
-             A 2D grid of (y,x) coordinates associated with the unmasked 2D data after it has been transformed to the
-             `source` reference frame.
-         source_plane_mesh_grid
-             The centres of every Voronoi pixel in the `source` frame, which are initially derived by computing a sparse
-             set of (y,x) coordinates computed from the unmasked data in the `data` frame and applying a transformation
-             to this.
-         image_plane_mesh_grid
-             The sparse set of (y,x) coordinates computed from the unmasked data in the `data` frame. This has a
-             transformation applied to it to create the `source_plane_mesh_grid`.
-         adapt_data
-             Not used for a rectangular mesh.
-        relocate_pix_border
-             If `True`, all coordinates of all pixelization source mesh grids have pixels outside their border
-             relocated to their edge.
-         preloads
-             Object which may contain preloaded arrays of quantities computed in the mesh, which are passed via
-             this object speed up the calculation.
-         run_time_dict
-             A dictionary which contains timing of certain functions calls which is used for profiling.
+        2) Before this routine is called, operations are performed on this `image_plane_mesh_grid` that transform it
+           from a 2D grid which overlaps with the 2D mask of the data in the `data` frame to an irregular grid in
+           the `source` frame, the `source_plane_mesh_grid`.
+
+        3) If the border relocator is input, the border of the input `source_plane_data_grid` is used to relocate all of the
+           grid's (y,x) coordinates beyond the border to the edge of the border.
+
+        4) If the border relocatiro is input, the border of the input `source_plane_data_grid` is used to relocate all of the
+           transformed `source_plane_mesh_grid`'s (y,x) coordinates beyond the border to the edge of the border.
+
+        5) Use the transformed `source_plane_mesh_grid`'s (y,x) coordinates as the centres of the Voronoi mesh.
+
+        6) Return the `MapperVoronoiNoInterp`.
+
+        Parameters
+        ----------
+        border_relocator
+           The border relocator, which relocates coordinates outside the border of the source-plane data grid to its
+           edge.
+        source_plane_data_grid
+            A 2D grid of (y,x) coordinates associated with the unmasked 2D data after it has been transformed to the
+            `source` reference frame.
+        source_plane_mesh_grid
+            The centres of every Voronoi pixel in the `source` frame, which are initially derived by computing a sparse
+            set of (y,x) coordinates computed from the unmasked data in the `data` frame and applying a transformation
+            to this.
+        image_plane_mesh_grid
+            The sparse set of (y,x) coordinates computed from the unmasked data in the `data` frame. This has a
+            transformation applied to it to create the `source_plane_mesh_grid`.
+        adapt_data
+            Not used for a rectangular mesh.
+        preloads
+            Object which may contain preloaded arrays of quantities computed in the mesh, which are passed via
+            this object speed up the calculation.
+        run_time_dict
+            A dictionary which contains timing of certain functions calls which is used for profiling.
         """
 
         self.run_time_dict = run_time_dict
 
         source_plane_data_grid = self.relocated_grid_from(
+            border_relocator=border_relocator,
             source_plane_data_grid=source_plane_data_grid,
-            relocate_pix_border=relocate_pix_border,
             preloads=preloads,
         )
 
         relocated_source_plane_mesh_grid = self.relocated_mesh_grid_from(
+            border_relocator=border_relocator,
             source_plane_data_grid=source_plane_data_grid,
             source_plane_mesh_grid=source_plane_mesh_grid,
-            relocate_pix_border=relocate_pix_border,
         )
 
         try:
             source_plane_mesh_grid = self.mesh_grid_from(
                 source_plane_data_grid=source_plane_data_grid,
                 source_plane_mesh_grid=relocated_source_plane_mesh_grid,
             )
         except ValueError as e:
             raise e
 
         return MapperGrids(
+            mask=mask,
             source_plane_data_grid=source_plane_data_grid,
             source_plane_mesh_grid=source_plane_mesh_grid,
             image_plane_mesh_grid=image_plane_mesh_grid,
             adapt_data=adapt_data,
             preloads=preloads,
             run_time_dict=run_time_dict,
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/voronoi.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/voronoi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from autoarray.structures.mesh.voronoi_2d import Mesh2DVoronoi
 from autoarray.inversion.pixelization.mesh.triangulation import Triangulation
+from autoarray.inversion.pixelization.border_relocator import BorderRelocator
 
 from autoarray.numba_util import profile_func
 
 
 class Voronoi(Triangulation):
     def __init__(self):
         """
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/mesh/voronoi_nn.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/mesh/voronoi_nn.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/pixelization/pixelization.py` & `autoarray-2024.5.16.0/autoarray/inversion/pixelization/pixelization.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/plot/inversion_plotters.py` & `autoarray-2024.5.16.0/autoarray/inversion/plot/inversion_plotters.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 from autoarray.plot.abstract_plotters import Plotter
 from autoarray.plot.visuals.two_d import Visuals2D
 from autoarray.plot.include.two_d import Include2D
 from autoarray.plot.mat_plot.two_d import MatPlot2D
 from autoarray.plot.auto_labels import AutoLabels
+from autoarray.structures.arrays.uniform_2d import Array2D
 from autoarray.inversion.inversion.abstract import AbstractInversion
 from autoarray.inversion.plot.mapper_plotters import MapperPlotter
 
 
 class InversionPlotter(Plotter):
     def __init__(
         self,
@@ -49,17 +50,30 @@
             mat_plot_2d=mat_plot_2d, include_2d=include_2d, visuals_2d=visuals_2d
         )
 
         self.inversion = inversion
         self.residuals_symmetric_cmap = residuals_symmetric_cmap
 
     def get_visuals_2d_for_data(self) -> Visuals2D:
-        return self.get_2d.via_mapper_for_data_from(
-            mapper=self.inversion.cls_list_from(cls=AbstractMapper)[0]
-        )
+        try:
+            mapper = self.inversion.cls_list_from(cls=AbstractMapper)[0]
+
+            visuals = self.get_2d.via_mapper_for_data_from(mapper=mapper)
+
+            if self.visuals_2d.pix_indexes is not None:
+                indexes = mapper.pix_indexes_for_slim_indexes(
+                    pix_indexes=self.visuals_2d.pix_indexes
+                )
+
+                visuals.indexes = indexes
+
+            return visuals
+
+        except (AttributeError, IndexError):
+            return self.visuals_2d
 
     def mapper_plotter_from(self, mapper_index: int) -> MapperPlotter:
         """
         Returns a `MapperPlotter` corresponding to the `Mapper` in the `Inversion`'s `linear_obj_list` given an input
         `mapper_index`.
 
         Parameters
@@ -104,14 +118,15 @@
         self,
         pixelization_index: int = 0,
         data_subtracted: bool = False,
         reconstructed_image: bool = False,
         reconstruction: bool = False,
         errors: bool = False,
         regularization_weights: bool = False,
+        sub_pixels_per_image_pixels: bool = False,
         mesh_pixels_per_image_pixels: bool = False,
         zoom_to_brightest: bool = True,
         interpolate_to_uniform: bool = False,
     ):
         """
         Plots the individual attributes of a specific `Mapper` of the plotter's `Inversion` object in 2D.
 
@@ -124,14 +139,17 @@
             The index of the `Mapper` in the `Inversion`'s `linear_obj_list` that is plotted.
         reconstructed_image
             Whether to make a 2D plot (via `imshow`) of the mapper's reconstructed image data.
         reconstruction
             Whether to make a 2D plot (via `imshow` or `fill`) of the mapper's source-plane reconstruction.
         errors
             Whether to make a 2D plot (via `imshow` or `fill`) of the mapper's source-plane errors.
+        sub_pixels_per_image_pixels
+            Whether to make a 2D plot (via `imshow`) of the number of sub pixels per image pixels in the 2D
+            data's mask.
         mesh_pixels_per_image_pixels
             Whether to make a 2D plot (via `imshow`) of the number of image-mesh pixels per image pixels in the 2D
             data's mask (only valid for pixelizations which use an `image_mesh`, e.g. Hilbert, KMeans).
         zoom_to_brightest
             For images not in the image-plane (e.g. the `plane_image`), whether to automatically zoom the plot to
             the brightest regions of the galaxies being plotted as opposed to the full extent of the grid.
         interpolate_to_uniform
@@ -150,14 +168,15 @@
 
             try:
                 array = self.inversion.data_subtracted_dict[mapper_plotter.mapper]
 
                 self.mat_plot_2d.plot_array(
                     array=array,
                     visuals_2d=self.get_visuals_2d_for_data(),
+                    grid_indexes=mapper_plotter.mapper.over_sampler.over_sampled_grid,
                     auto_labels=AutoLabels(
                         title="Data Subtracted", filename="data_subtracted"
                     ),
                 )
             except AttributeError:
                 pass
 
@@ -165,14 +184,15 @@
             array = self.inversion.mapped_reconstructed_image_dict[
                 mapper_plotter.mapper
             ]
 
             self.mat_plot_2d.plot_array(
                 array=array,
                 visuals_2d=self.get_visuals_2d_for_data(),
+                grid_indexes=mapper_plotter.mapper.over_sampler.over_sampled_grid,
                 auto_labels=AutoLabels(
                     title="Reconstructed Image", filename="reconstructed_image"
                 ),
             )
 
         if reconstruction:
             vmax_custom = False
@@ -210,14 +230,29 @@
                     pixel_values=self.inversion.errors_dict[mapper_plotter.mapper],
                     auto_labels=AutoLabels(title="Errors", filename="errors"),
                 )
 
             except TypeError:
                 pass
 
+        if sub_pixels_per_image_pixels:
+            sub_size = Array2D(
+                values=mapper_plotter.mapper.over_sampler.sub_size,
+                mask=self.inversion.dataset.mask,
+            )
+
+            self.mat_plot_2d.plot_array(
+                array=sub_size,
+                visuals_2d=self.get_visuals_2d_for_data(),
+                auto_labels=AutoLabels(
+                    title="Sub Pixels Per Image Pixels",
+                    filename="sub_pixels_per_image_pixels",
+                ),
+            )
+
         if mesh_pixels_per_image_pixels:
             try:
                 mesh_pixels_per_image_pixels = (
                     mapper_plotter.mapper.mapper_grids.mesh_pixels_per_image_pixels
                 )
 
                 self.mat_plot_2d.plot_array(
@@ -275,19 +310,22 @@
         )
 
         contour_original = self.mat_plot_2d.contour
 
         self.mat_plot_2d.use_log10 = True
         self.mat_plot_2d.contour = False
 
-        self.mat_plot_2d.plot_array(
-            array=self.inversion.data,
-            visuals_2d=self.get_visuals_2d_for_data(),
-            auto_labels=AutoLabels(title=f" Data"),
-        )
+        try:
+            self.mat_plot_2d.plot_array(
+                array=self.inversion.data,
+                visuals_2d=self.get_visuals_2d_for_data(),
+                auto_labels=AutoLabels(title=f" Data"),
+            )
+        except AttributeError:
+            pass
 
         self.figures_2d_of_pixelization(
             pixelization_index=mapper_index, reconstructed_image=True
         )
 
         self.mat_plot_2d.use_log10 = False
 
@@ -330,28 +368,77 @@
         self.include_2d._mapper_image_plane_mesh_grid = False
         self.figures_2d_of_pixelization(
             pixelization_index=mapper_index, mesh_pixels_per_image_pixels=True
         )
 
         self.include_2d._mapper_image_plane_mesh_grid = mapper_image_plane_mesh_grid
 
+        self.figures_2d_of_pixelization(
+            pixelization_index=mapper_index, sub_pixels_per_image_pixels=True
+        )
+
         self.set_title(label="Errors (Unzoomed)")
         self.figures_2d_of_pixelization(
             pixelization_index=mapper_index, errors=True, zoom_to_brightest=False
         )
 
-        self.set_title(label="Regularization Weights (Unzoomed)")
-        try:
-            self.figures_2d_of_pixelization(
-                pixelization_index=mapper_index,
-                regularization_weights=True,
-                zoom_to_brightest=False,
-            )
-        except IndexError:
-            pass
-        self.set_title(label=None)
+        # self.set_title(label="Regularization Weights (Unzoomed)")
+        # try:
+        #     self.figures_2d_of_pixelization(
+        #         pixelization_index=mapper_index,
+        #         regularization_weights=True,
+        #         zoom_to_brightest=False,
+        #     )
+        # except IndexError:
+        #     pass
+        # self.set_title(label=None)
 
         self.mat_plot_2d.output.subplot_to_figure(
             auto_filename=f"{auto_filename}_{mapper_index}"
         )
 
         self.close_subplot_figure()
+
+    def subplot_mappings(
+        self, pixelization_index: int = 0, auto_filename: str = "subplot_mappings"
+    ):
+        self.open_subplot_figure(number_subplots=4)
+
+        self.include_2d._mapper_image_plane_mesh_grid = False
+
+        self.figures_2d_of_pixelization(
+            pixelization_index=pixelization_index, data_subtracted=True
+        )
+
+        total_pixels = conf.instance["visualize"]["general"]["inversion"][
+            "total_mappings_pixels"
+        ]
+
+        pix_indexes = self.inversion.brightest_pixel_list_from(
+            total_pixels=total_pixels, filter_neighbors=True
+        )
+
+        self.visuals_2d.pix_indexes = [
+            [index] for index in pix_indexes[pixelization_index]
+        ]
+
+        self.figures_2d_of_pixelization(
+            pixelization_index=pixelization_index, reconstructed_image=True
+        )
+
+        self.figures_2d_of_pixelization(
+            pixelization_index=pixelization_index, reconstruction=True
+        )
+
+        self.set_title(label="Source Reconstruction (Unzoomed)")
+        self.figures_2d_of_pixelization(
+            pixelization_index=pixelization_index,
+            reconstruction=True,
+            zoom_to_brightest=False,
+        )
+        self.set_title(label=None)
+
+        self.mat_plot_2d.output.subplot_to_figure(
+            auto_filename=f"{auto_filename}_{pixelization_index}"
+        )
+
+        self.close_subplot_figure()
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/plot/mapper_plotters.py` & `autoarray-2024.5.16.0/autoarray/inversion/plot/mapper_plotters.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
         if self.visuals_2d.pix_indexes is not None:
             indexes = self.mapper.pix_indexes_for_slim_indexes(
                 pix_indexes=self.visuals_2d.pix_indexes
             )
 
             self.mat_plot_2d.index_scatter.scatter_grid_indexes(
-                grid=self.mapper.source_plane_data_grid.mask.derive_grid.unmasked,
+                grid=self.mapper.over_sampler.over_sampled_grid,
                 indexes=indexes,
             )
 
         self.figure_2d(interpolate_to_uniform=interpolate_to_uniform)
 
         self.mat_plot_2d.output.subplot_to_figure(
             auto_filename="subplot_image_and_mapper"
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/__init__.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/abstract.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/adaptive_brightness.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/adaptive_brightness.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/adaptive_brightness_split.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/adaptive_brightness_split.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/brightness_zeroth.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/brightness_zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/constant.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/constant.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/constant_split.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/constant_split.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/constant_zeroth.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/constant_zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/exponential_kernel.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/zeroth.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,101 +3,78 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from autoarray.inversion.linear_obj.linear_obj import LinearObj
 
 from autoarray.inversion.regularization.abstract import AbstractRegularization
 
-from autoarray import numba_util
+from autoarray.inversion.regularization import regularization_util
 
 
-@numba_util.jit()
-def exp_cov_matrix_from(
-    scale: float,
-    pixel_points: np.ndarray,
-) -> np.ndarray:
-    """
-    Consutruct the source brightness covariance matrix, which is used to determined the regularization
-    pattern (i.e, how the different  source pixels are smoothed).
-
-    The covariance matrix includes one non-linear parameters, the scale coefficient, which is used to determine
-    the typical scale of the regularization pattern.
-
-    Parameters
-    ----------
-    scale
-        The typical scale of the regularization pattern .
-    pixel_points
-        An 2d array with shape [N_source_pixels, 2], which save the source pixelization coordinates (on source plane).
-        Something like [[y1,x1], [y2,x2], ...]
-
-    Returns
-    -------
-    np.ndarray
-        The source covariance matrix (2d array), shape [N_source_pixels, N_source_pixels].
-    """
-
-    pixels = len(pixel_points)
-    covariance_matrix = np.zeros(shape=(pixels, pixels))
-
-    for i in range(pixels):
-        covariance_matrix[i, i] += 1e-8
-        for j in range(pixels):
-            xi = pixel_points[i, 1]
-            yi = pixel_points[i, 0]
-            xj = pixel_points[j, 1]
-            yj = pixel_points[j, 0]
-            d_ij = np.sqrt(
-                (xi - xj) ** 2 + (yi - yj) ** 2
-            )  # distance between the pixel i and j
-
-            covariance_matrix[i, j] += np.exp(-1.0 * d_ij / scale)
-
-    return covariance_matrix
-
-
-class ExponentialKernel(AbstractRegularization):
-    def __init__(self, coefficient: float = 1.0, scale: float = 1.0):
-        """
-        Regularization which uses an Exponential smoothing kernel to regularize the solution.
-
-        For this regularization scheme, every pixel is regularized with every other pixel. This contrasts many other
-        schemes, where regularization is based on neighboring (e.g. do the pixels share a Voronoi edge?) or computing
-        derivates around the center of the pixel (where nearby pixels are regularization locally in similar ways).
+class Zeroth(AbstractRegularization):
+    def __init__(self, coefficient: float = 1.0):
+        """
+        A zeroth order regularization scheme which zeroth order regularization to pixels with low expected
+        signal values.
+
+        Zeroth order regularization assumes a prior on the solution that its values should be closer to zero,
+        penalizing solutions where they deviate further from zero. This is typically applied to prevent solutions
+        from going to large positive and negative values that alternate.
+
+        For this regularization scheme, there is only 1 regularization coefficient that is applied to
+        all pixels by themselves (e.g. no neighboring scheme is used) For example:
 
-        This makes the regularization matrix fully dense and therefore maybe change the run times of the solution.
-        It also leads to more overall smoothing which can lead to more stable linear inversions.
+        B = [1, 0]  0 -> 0
+            [0, 1]  1 -> 1
 
-        This scheme is introduced by Vernardos et al. (2022): https://arxiv.org/abs/2202.09378
+        A small numerical value of 1.0e-8 is added to all elements in constant regularization matrix, to ensure that
+        it is positive definite.
 
         A full description of regularization and this matrix can be found in the parent `AbstractRegularization` class.
 
         Parameters
         ----------
         coefficient
             The regularization coefficient which controls the degree of smooth of the inversion reconstruction.
-        scale
-            The typical scale of the exponential regularization pattern.
         """
+
         self.coefficient = coefficient
-        self.scale = scale
 
         super().__init__()
 
+    def regularization_weights_from(self, linear_obj: LinearObj) -> np.ndarray:
+        """
+        Returns the regularization weights of this regularization scheme.
+
+        The regularization weights define the level of regularization applied to each parameter in the linear object
+        (e.g. the ``pixels`` in a ``Mapper``).
+
+        For standard regularization (e.g. ``Constant``) are weights are equal, however for adaptive schemes
+        (e.g. ``AdaptiveBrightness``) they vary to adapt to the data being reconstructed.
+
+        Parameters
+        ----------
+        linear_obj
+            The linear object (e.g. a ``Mapper``) which uses these weights when performing regularization.
+
+        Returns
+        -------
+        The regularization weights.
+        """
+        return self.coefficient * np.ones(linear_obj.params)
+
     def regularization_matrix_from(self, linear_obj: LinearObj) -> np.ndarray:
         """
         Returns the regularization matrix with shape [pixels, pixels].
 
         Parameters
         ----------
         linear_obj
             The linear object (e.g. a ``Mapper``) which uses this matrix to perform regularization.
 
         Returns
         -------
         The regularization matrix.
         """
-        covariance_matrix = exp_cov_matrix_from(
-            scale=self.scale, pixel_points=linear_obj.source_plane_mesh_grid
+        return regularization_util.zeroth_regularization_matrix_from(
+            coefficient=self.coefficient, pixels=linear_obj.params
         )
-
-        return self.coefficient * np.linalg.inv(covariance_matrix)
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/gaussian_kernel.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/exponential_kernel.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 
 from autoarray.inversion.regularization.abstract import AbstractRegularization
 
 from autoarray import numba_util
 
 
 @numba_util.jit()
-def gauss_cov_matrix_from(
+def exp_cov_matrix_from(
     scale: float,
     pixel_points: np.ndarray,
 ) -> np.ndarray:
     """
     Consutruct the source brightness covariance matrix, which is used to determined the regularization
-    pattern (i.e, how the different source pixels are smoothed).
+    pattern (i.e, how the different  source pixels are smoothed).
 
-    the covariance matrix includes one non-linear parameters, the scale coefficient, which is used to
-    determine the typical scale of the regularization pattern.
+    The covariance matrix includes one non-linear parameters, the scale coefficient, which is used to determine
+    the typical scale of the regularization pattern.
 
     Parameters
     ----------
     scale
-        the typical scale of the regularization pattern .
+        The typical scale of the regularization pattern .
     pixel_points
         An 2d array with shape [N_source_pixels, 2], which save the source pixelization coordinates (on source plane).
         Something like [[y1,x1], [y2,x2], ...]
 
     Returns
     -------
     np.ndarray
@@ -46,23 +46,23 @@
             yi = pixel_points[i, 0]
             xj = pixel_points[j, 1]
             yj = pixel_points[j, 0]
             d_ij = np.sqrt(
                 (xi - xj) ** 2 + (yi - yj) ** 2
             )  # distance between the pixel i and j
 
-            covariance_matrix[i, j] += np.exp(-1.0 * d_ij**2 / (2 * scale**2))
+            covariance_matrix[i, j] += np.exp(-1.0 * d_ij / scale)
 
     return covariance_matrix
 
 
-class GaussianKernel(AbstractRegularization):
+class ExponentialKernel(AbstractRegularization):
     def __init__(self, coefficient: float = 1.0, scale: float = 1.0):
         """
-        Regularization which uses a Gaussian smoothing kernel to regularize the solution.
+        Regularization which uses an Exponential smoothing kernel to regularize the solution.
 
         For this regularization scheme, every pixel is regularized with every other pixel. This contrasts many other
         schemes, where regularization is based on neighboring (e.g. do the pixels share a Voronoi edge?) or computing
         derivates around the center of the pixel (where nearby pixels are regularization locally in similar ways).
 
         This makes the regularization matrix fully dense and therefore maybe change the run times of the solution.
         It also leads to more overall smoothing which can lead to more stable linear inversions.
@@ -76,27 +76,50 @@
         coefficient
             The regularization coefficient which controls the degree of smooth of the inversion reconstruction.
         scale
             The typical scale of the exponential regularization pattern.
         """
         self.coefficient = coefficient
         self.scale = scale
+
         super().__init__()
 
+    def regularization_weights_from(self, linear_obj: LinearObj) -> np.ndarray:
+        """
+        Returns the regularization weights of this regularization scheme.
+
+        The regularization weights define the level of regularization applied to each parameter in the linear object
+        (e.g. the ``pixels`` in a ``Mapper``).
+
+        For standard regularization (e.g. ``Constant``) are weights are equal, however for adaptive schemes
+        (e.g. ``AdaptiveBrightness``) they vary to adapt to the data being reconstructed.
+
+        Parameters
+        ----------
+        linear_obj
+            The linear object (e.g. a ``Mapper``) which uses these weights when performing regularization.
+
+        Returns
+        -------
+        The regularization weights.
+        """
+        return self.coefficient * np.ones(linear_obj.params)
+
     def regularization_matrix_from(self, linear_obj: LinearObj) -> np.ndarray:
         """
         Returns the regularization matrix with shape [pixels, pixels].
 
         Parameters
         ----------
         linear_obj
             The linear object (e.g. a ``Mapper``) which uses this matrix to perform regularization.
 
         Returns
         -------
         The regularization matrix.
         """
-        covariance_matrix = gauss_cov_matrix_from(
-            scale=self.scale, pixel_points=linear_obj.source_plane_mesh_grid
+        covariance_matrix = exp_cov_matrix_from(
+            scale=self.scale,
+            pixel_points=np.array(linear_obj.source_plane_mesh_grid),
         )
 
         return self.coefficient * np.linalg.inv(covariance_matrix)
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/matern_kernel.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/matern_kernel.py`

 * *Files 14% similar despite different names*

```diff
@@ -135,14 +135,35 @@
             numba_scipy_exception()
 
         self.coefficient = coefficient
         self.scale = float(scale)
         self.nu = float(nu)
         super().__init__()
 
+    def regularization_weights_from(self, linear_obj: LinearObj) -> np.ndarray:
+        """
+        Returns the regularization weights of this regularization scheme.
+
+        The regularization weights define the level of regularization applied to each parameter in the linear object
+        (e.g. the ``pixels`` in a ``Mapper``).
+
+        For standard regularization (e.g. ``Constant``) are weights are equal, however for adaptive schemes
+        (e.g. ``AdaptiveBrightness``) they vary to adapt to the data being reconstructed.
+
+        Parameters
+        ----------
+        linear_obj
+            The linear object (e.g. a ``Mapper``) which uses these weights when performing regularization.
+
+        Returns
+        -------
+        The regularization weights.
+        """
+        return self.coefficient * np.ones(linear_obj.params)
+
     def regularization_matrix_from(self, linear_obj: LinearObj) -> np.ndarray:
         """
         Returns the regularization matrix with shape [pixels, pixels].
 
         Parameters
         ----------
         linear_obj
@@ -150,12 +171,12 @@
 
         Returns
         -------
         The regularization matrix.
         """
         covariance_matrix = matern_cov_matrix_from(
             scale=self.scale,
-            pixel_points=linear_obj.source_plane_mesh_grid,
+            pixel_points=np.array(linear_obj.source_plane_mesh_grid),
             nu=self.nu,
         )
 
         return self.coefficient * np.linalg.inv(covariance_matrix)
```

### Comparing `autoarray-2024.1.27.4/autoarray/inversion/regularization/regularization_util.py` & `autoarray-2024.5.16.0/autoarray/inversion/regularization/regularization_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/layout/layout.py` & `autoarray-2024.5.16.0/autoarray/layout/layout.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/layout/layout_util.py` & `autoarray-2024.5.16.0/autoarray/layout/layout_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/layout/region.py` & `autoarray-2024.5.16.0/autoarray/layout/region.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/mask/abstract_mask.py` & `autoarray-2024.5.16.0/autoarray/mask/abstract_mask.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import ABC
 import logging
 import numpy as np
 from pathlib import Path
 from typing import Dict, Union
 
 from autoarray.abstract_ndarray import AbstractNDArray
@@ -13,31 +15,30 @@
 logger = logging.getLogger(__name__)
 
 
 class Mask(AbstractNDArray, ABC):
     pixel_scales = None
 
     # noinspection PyUnusedLocal
-    def __new__(
-        cls,
+    def __init__(
+        self,
         mask: np.ndarray,
         origin: tuple,
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         *args,
-        **kwargs
+        **kwargs,
     ):
         """
         An abstract class for a mask that represents data structure that can be in 1D, 2D or other shapes.
 
         When applied to data it extracts or masks the unmasked image pixels corresponding to mask entries
         that are (`False` or 0).
 
         The mask also defines the geometry of the data structure it is paired with, for example how its pixels convert
-        to physical units via the pixel_scales and origin parameters and a sub-grid which is used for
+        to physical units via the pixel_scales and origin parameters and a grid which is used for
         perform calculations via super-sampling.
 
         Parameters
         ----------
         mask
             The ndarray containing the bool's representing the mask, where `False` signifies an entry is
             unmasked and used in calculations.
@@ -46,37 +47,38 @@
             converted to a (float, float) structure.
         origin
             The origin of the mask's coordinate system in scaled units.
         """
 
         # noinspection PyArgumentList
         mask = mask.astype("bool")
-        obj = mask.view(cls)
-        obj.sub_size = sub_size
-        obj.pixel_scales = pixel_scales
-        obj.origin = origin
-        return obj
+        super().__init__(mask)
+
+        self.pixel_scales = pixel_scales
+        self.origin = origin
+
+    @property
+    def mask(self):
+        return self._array
 
     def __array_finalize__(self, obj):
         if isinstance(obj, Mask):
-            self.sub_size = obj.sub_size
             self.pixel_scales = obj.pixel_scales
             self.origin = obj.origin
         else:
-            self.sub_size = 1
             self.pixel_scales = None
 
     @property
     def pixel_scale(self) -> float:
         """
         For a mask with dimensions two or above check that are pixel scales are the same, and if so return this
         single value as a float.
         """
         for pixel_scale in self.pixel_scales:
-            if pixel_scale != self.pixel_scales[0]:
+            if abs(pixel_scale - self.pixel_scales[0]) > 1.0e-8:
                 raise exc.MaskException(
                     "Cannot return a pixel_scale for a grid where each dimension has a "
                     "different pixel scale (e.g. pixel_scales[0] != pixel_scales[1])"
                 )
 
         return self.pixel_scales[0]
 
@@ -100,82 +102,39 @@
                 "PIXSCALEX": self.pixel_scales[1],
             }
 
     @property
     def dimensions(self) -> int:
         return len(self.shape)
 
-    @property
-    def sub_length(self) -> int:
-        """
-        The total number of sub-pixels in a give pixel,
-
-        For example, a sub-size of 3x3 means every pixel has 9 sub-pixels.
-        """
-        return int(self.sub_size**self.dimensions)
-
-    @property
-    def sub_fraction(self) -> float:
-        """
-        The fraction of the area of a pixel every sub-pixel contains.
-
-        For example, a sub-size of 3x3 mean every pixel contains 1/9 the area.
-        """
-        return 1.0 / self.sub_length
-
     def output_to_fits(self, file_path: Union[Path, str], overwrite: bool = False):
         """
         Overwrite with method to output the mask to a `.fits` file.
         """
 
     @property
     def pixels_in_mask(self) -> int:
         """
         The total number of unmasked pixels (values are `False`) in the mask.
         """
-        return int(np.size(self) - np.sum(self))
+        return int(np.size(self._array) - np.sum(self._array))
 
     @property
     def is_all_true(self) -> bool:
         """
         Returns `True` if all pixels in a mask are `True`, else returns `False`.
         """
         return self.pixels_in_mask == 0
 
     @property
     def is_all_false(self) -> bool:
         """
         Returns `False` if all pixels in a mask are `False`, else returns `True`.
         """
-        return self.pixels_in_mask == np.size(self)
-
-    @property
-    def sub_pixels_in_mask(self) -> int:
-        """
-        The total number of unmasked sub-pixels (values are `False`) in the mask.
-        """
-        return self.sub_size**self.dimensions * self.pixels_in_mask
+        return self.pixels_in_mask == np.size(self._array)
 
     @property
     def shape_slim(self) -> int:
         """
         The 1D shape of the mask, which is equivalent to the total number of unmasked pixels in the mask.
         """
         return self.pixels_in_mask
-
-    @property
-    def sub_shape_slim(self) -> int:
-        """
-        The 1D shape of the mask's sub-grid, which is equivalent to the total number of unmasked pixels in the mask.
-        """
-        return int(self.pixels_in_mask * self.sub_size**self.dimensions)
-
-    def mask_new_sub_size_from(self, mask, sub_size=1) -> "Mask":
-        """
-        Returns the mask on the same scaled coordinate system but with a sub-grid of an inputsub_size.
-        """
-        return self.__class__(
-            mask=mask,
-            sub_size=sub_size,
-            pixel_scales=self.pixel_scales,
-            origin=self.origin,
-        )
```

### Comparing `autoarray-2024.1.27.4/autoarray/mask/derive/grid_1d.py` & `autoarray-2024.5.16.0/autoarray/mask/derive/grid_1d.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,56 +57,51 @@
             derive_grid_2d = aa.DeriveGrid2D(mask=mask_2d)
 
             print(derive_grid_2d.border)
         """
         self.mask = mask
 
     @property
-    def all_false_sub_1(self) -> Grid1D:
+    def all_false(self) -> Grid1D:
         """
-        Returns a non-subgridded ``Grid1D`` which uses the ``Mask1D``
-        geometry (``shape_native`` / ``sub_size`` / ``pixel_scales`` / ``origin``) and every pixel in the ``Mask2D``
+        Returns a ``Grid1D`` which uses the ``Mask1D``
+        geometry (``shape_native`` / ``pixel_scales`` / ``origin``) and every pixel in the ``Mask2D``
         irrespective of whether pixels are masked or unmasked (given by ``True`` or``False``).
 
         For example, for the following ``Mask2D``:
 
         ::
             mask_2d = aa.Mask1D(
                 mask=[False, False, True,  True]
                 pixel_scales=1.0,
             )
 
-        The ``all_false_sub_1`` ``Grid1D`` (given via ``mask_1d.derive_grid.all_false_sub_1``) is:
+        The ``all_false`` ``Grid1D`` (given via ``mask_1d.derive_grid.all_false``) is:
 
         ::
             [-2.0, -1.0, 1.0, 2.0]
 
         Examples
         --------
 
         .. code-block:: python
 
             import autoarray as aa
 
             mask_1d = aa.Mask2D(
                 mask=[False, False, True,  True],
                 pixel_scales=1.0,
-                sub_size=2
             )
 
             derive_grid_1d = aa.DeriveGrid1D(mask=mask_1d)
 
-            print(derive_grid_1d.all_false_sub_1)
+            print(derive_grid_1d.all_false)
         """
         from autoarray.structures.grids.uniform_1d import Grid1D
 
         grid_slim = grid_1d_util.grid_1d_slim_via_mask_from(
             mask_1d=self.mask,
             pixel_scales=self.mask.pixel_scales,
-            sub_size=1,
             origin=self.mask.origin,
         )
 
-        return Grid1D(
-            values=grid_slim,
-            mask=self.mask.derive_mask.all_false.derive_mask.sub_1,
-        )
+        return Grid1D(values=grid_slim, mask=self.mask.derive_mask.all_false)
```

### Comparing `autoarray-2024.1.27.4/autoarray/mask/derive/grid_2d.py` & `autoarray-2024.5.16.0/autoarray/mask/derive/grid_2d.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 import logging
 from typing import TYPE_CHECKING
+import numpy as np
 
 if TYPE_CHECKING:
     from autoarray.mask.mask_2d import Mask2D
     from autoarray.structures.grids.uniform_2d import Grid2D
 
 from autoarray.structures.grids import grid_2d_util
 
@@ -57,32 +58,32 @@
             derive_grid_2d = aa.DeriveGrid2D(mask=mask_2d)
 
             print(derive_grid_2d.border)
         """
         self.mask = mask
 
     @property
-    def all_false_sub_1(self) -> Grid2D:
+    def all_false(self) -> Grid2D:
         """
-        Returns a non-subgridded ``Grid2D`` which uses the ``Mask2D``
-        geometry (``shape_native`` / ``sub_size`` / ``pixel_scales`` / ``origin``) and every pixel in the ``Mask2D``
+        Returns a ``Grid2D`` which uses the ``Mask2D``
+        geometry (``shape_native`` / ``pixel_scales`` / ``origin``) and every pixel in the ``Mask2D``
         irrespective of whether pixels are masked or unmasked (given by ``True`` or``False``).
 
         For example, for the following ``Mask2D``:
 
         ::
             mask_2d = aa.Mask2D(
                 mask=[
                      [False, False],
                      [ True,  True]
                 ],
                 pixel_scales=1.0,
             )
 
-        The ``all_false_sub_1`` ``Grid2D`` (given via ``mask_2d.derive_grid.all_false_sub_1``) is:
+        The ``all_false`` ``Grid2D`` (given via ``mask_2d.derive_grid.all_false``) is:
 
         ::
             [[ 0.5, -0.5], [ 0.5,  0.5],
              [-0.5, -0.5], [-0.5, -0.5]]
 
         Examples
         --------
@@ -93,169 +94,100 @@
 
             mask_2d = aa.Mask2D(
                 mask=[
                      [False, False],
                      [ True,  True]
                 ],
                 pixel_scales=1.0,
-                sub_size=2
             )
 
             derive_grid_2d = aa.DeriveGrid2D(mask=mask_2d)
 
-            print(derive_grid_2d.all_false_sub_1)
+            print(derive_grid_2d.all_false)
         """
         from autoarray.structures.grids.uniform_2d import Grid2D
 
         grid_slim = grid_2d_util.grid_2d_slim_via_shape_native_from(
             shape_native=self.mask.shape,
             pixel_scales=self.mask.pixel_scales,
-            sub_size=1,
             origin=self.mask.origin,
         )
 
-        return Grid2D(
-            values=grid_slim,
-            mask=self.mask.derive_mask.all_false.derive_mask.sub_1,
-        )
+        return Grid2D(values=grid_slim, mask=self.mask.derive_mask.all_false)
 
     @property
     def unmasked(self) -> Grid2D:
         """
-        Returns a subgridded ``Grid2D`` which uses the ``Mask2D``
-        geometry (``shape_native`` / ``sub_size`` / ``pixel_scales`` / ``origin``) and every unmasked
+        Returns a ``Grid2D`` which uses the ``Mask2D``
+        geometry (``shape_native`` / ``pixel_scales`` / ``origin``) and every unmasked
         pixel (given by ``False``), such that all masked entries (given by ``True``) are removed.
 
         For example, for the following ``Mask2D``:
 
         ::
             mask_2d = aa.Mask2D(
                 mask=[
                      [False, False],
                      [ True,  True]
                 ],
                 pixel_scales=1.0,
-                sub_size=1
             )
 
         The ``masked`` ``Grid2D`` (given via ``mask_2d.derive_grid.unmasked``) is:
 
         ::
             [[0.5, -0.5], [0.5, 0.5]]
 
-        If the ``Mask2D`` has a ``sub_size=2`` then the ``unmasked`` ``Grid2D``  is:
-
-        ::
-            [[ 0.75, -0.75], [ 0.75, -0.25], [ 0.25, -0.75], [ 0.25, -0.25],
-             [ 0.75,  0.25], [ 0.75,  0.75], [ 0.25,  0.25], [ 0.25,  0.75]]
-
         Examples
         --------
 
         .. code-block:: python
 
             import autoarray as aa
 
             mask_2d = aa.Mask2D(
                 mask=[
                      [False, False],
                      [ True,  True]
                 ],
                 pixel_scales=1.0,
-                sub_size=2
             )
 
             derive_grid_2d = aa.DeriveGrid2D(mask=mask_2d)
 
             print(derive_grid_2d.unmasked)
         """
         from autoarray.structures.grids.uniform_2d import Grid2D
 
-        sub_grid_1d = grid_2d_util.grid_2d_slim_via_mask_from(
-            mask_2d=self.mask,
+        grid_1d = grid_2d_util.grid_2d_slim_via_mask_from(
+            mask_2d=np.array(self.mask),
             pixel_scales=self.mask.pixel_scales,
-            sub_size=self.mask.sub_size,
             origin=self.mask.origin,
         )
-        return Grid2D(values=sub_grid_1d, mask=self.mask)
+        return Grid2D(values=grid_1d, mask=self.mask)
 
     @property
-    def unmasked_sub_1(self) -> Grid2D:
+    def edge(self) -> Grid2D:
         """
-        Returns a non-subgridded ``Grid2D`` which uses the ``Mask2D``
-        geometry (``shape_native`` / ``sub_size`` / ``pixel_scales`` / ``origin``) and every unmasked (y,x)
-        coordinate (given by ``False``), where all masked entries (given by ``True``) are removed.
-
-        For example, for the following ``Mask2D``:
-
-        ::
-            mask_2d = aa.Mask2D(
-                mask=[
-                     [False, False],
-                     [ True,  True]
-                ],
-                pixel_scales=1.0,
-                sub_size=2
-            )
-
-        The ``unmasked_sub_1`` ``Grid2D`` (given via ``mask_2d.derive_grid.unmasked_sub_1``) is:
-
-        ::
-            [[0.5, -0.5], [0.5, 0.5]]
-
-        Examples
-        --------
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            mask_2d = aa.Mask2D(
-                mask=[
-                     [False, False],
-                     [ True,  True]
-                ],
-                pixel_scales=1.0,
-                sub_size=2
-            )
-
-            derive_grid_2d = aa.DeriveGrid2D(mask=mask_2d)
-
-            print(derive_grid_2d.unmasked_sub_1)
-        """
-        from autoarray.structures.grids.uniform_2d import Grid2D
-
-        grid_slim = grid_2d_util.grid_2d_slim_via_mask_from(
-            mask_2d=self.mask,
-            pixel_scales=self.mask.pixel_scales,
-            sub_size=1,
-            origin=self.mask.origin,
-        )
-        return Grid2D(values=grid_slim, mask=self.mask.derive_mask.sub_1)
-
-    @property
-    def edge_sub_1(self) -> Grid2D:
-        """
-        Returns a non-subgridded edge ``Grid2D``, which uses all unmasked pixels (given by ``False``) which neighbor
+        Returns an edge ``Grid2D``, which uses all unmasked pixels (given by ``False``) which neighbor
         any masked value (give by ``True``) and therefore are on the edge of the 2D mask.
 
         For example, for the following ``Mask2D``:
 
         ::
             mask_2d = aa.Mask2D(
                 mask=[[True,  True,  True,  True, True],
                       [True, False, False, False, True],
                       [True, False, False, False, True],
                       [True, False, False, False, True],
                       [True,  True,  True,  True, True]]
                 pixel_scales=1.0,
-                sub_size=2
             )
 
-        The ``edge_sub_1`` grid (given via ``mask_2d.derive_grid.edge_sub_1``) is given by:
+        The ``edge`` grid (given via ``mask_2d.derive_grid.edge``) is given by:
 
         ::
               [[1.0, -1.0], [ 1.0, 0.0], [ 1.0,  1.0],
                [0.0, -1.0],              [ 0.0,  1.0],
               [-1.0, -1.0], [-1.0, 0.0], [-1.0, 1.0]]
 
         The central pixel, which does not neighbor a ``True`` value in any one of the eight neighboring directions,
@@ -271,34 +203,33 @@
             mask_2d = aa.Mask2D(
                 mask=[[True,  True,  True,  True, True],
                       [True, False, False, False, True],
                       [True, False, False, False, True],
                       [True, False, False, False, True],
                       [True,  True,  True,  True, True]],
                 pixel_scales=1.0,
-                sub_size=2
             )
 
             derive_grid_2d = aa.DeriveGrid2D(mask=mask_2d)
 
-            print(derive_grid_2d.edge_sub_1)
+            print(derive_grid_2d.edge)
         """
 
         from autoarray.structures.grids.uniform_2d import Grid2D
 
-        edge_grid_1d = self.unmasked_sub_1[self.mask.derive_indexes.edge_slim]
+        edge_grid_1d = self.unmasked[self.mask.derive_indexes.edge_slim]
         return Grid2D(
             values=edge_grid_1d,
-            mask=self.mask.derive_mask.edge.derive_mask.sub_1,
+            mask=self.mask.derive_mask.edge,
         )
 
     @property
     def border(self) -> Grid2D:
         """
-        Returns a subgridded edge ``Grid2D``, which uses all unmasked pixels (given by ``False``) which neighbor
+        Returns a border ``Grid2D``, which uses all unmasked pixels (given by ``False``) which neighbor
         any masked value (give by ``True``) and which are on the extreme exterior of the mask.
 
         For example, for the following ``Mask2D``:
 
         ::
             mask_2d = aa.Mask2D(
                 mask=[[True,  True,  True,  True,  True,  True,  True,  True, True],
@@ -307,34 +238,30 @@
                       [True, False,  True, False, False, False,  True, False, True],
                       [True, False,  True, False,  True, False,  True, False, True],
                       [True, False,  True, False, False, False,  True, False, True],
                       [True, False,  True,  True,  True,  True,  True, False, True],
                       [True, False, False, False, False, False, False, False, True],
                       [True,  True,  True,  True,  True,  True,  True,  True, True]]
                 pixel_scales=1.0,
-                sub_size=1
             )
 
-        The ``edge_sub_1`` grid (given via ``mask_2d.derive_grid.edge_sub_1``) is given by:
+        The ``edge`` grid (given via ``mask_2d.derive_grid.edge``) is given by:
 
         ::
             [[3.0, -3.0],  [3.0, -2.0],  [3.0, -1.0],  [3.0, 0.0],  [3.0, 1.0],  [3.0, 2.0],  [ 3.0, 3.0],
              [ 2.0, -3.0],                                                                    [ 2.0, 3.0],
              [ 1.0, -3.0],                                                                    [ 1.0, 3.0],
              [ 0.0, -3.0],                                                                    [ 0.0, 3.0],
              [-1.0, -3.0],                                                                    [-1.0, 3.0],
              [-2.0, -3.0],                                                                    [-2.0, 3.0],
              [-3.0, -3.0], [-3.0, -2.0], [-3.0, -1.0], [-3.0, 0.0], [-3.0, 1.0], [-3.0, 2.0], [-3.0, 3.0]]
 
         The central group of pixels, which neighbor ``True`` values, are omitted because they are not at an extreme
         edge of the mask.
 
-        The example above assumes ``sub_size=1`` for clairty, but this function generalizes to cases with higher
-        ``sub_size`` values.
-
         Examples
         --------
 
         .. code-block:: python
 
             import autoarray as aa
 
@@ -345,85 +272,20 @@
                       [True, False,  True, False, False, False,  True, False, True],
                       [True, False,  True, False,  True, False,  True, False, True],
                       [True, False,  True, False, False, False,  True, False, True],
                       [True, False,  True,  True,  True,  True,  True, False, True],
                       [True, False, False, False, False, False, False, False, True],
                       [True,  True,  True,  True,  True,  True,  True,  True, True]],
                 pixel_scales=1.0,
-                sub_size=2
             )
 
             derive_grid_2d = aa.DeriveGrid2D(mask=mask_2d)
 
             print(derive_grid_2d.border)
         """
-        return self.unmasked[self.mask.derive_indexes.sub_border_slim]
-
-    @property
-    def border_sub_1(self) -> Grid2D:
-        """
-        Returns a non-subgridded edge ``Grid2D``, which uses all unmasked pixels (given by ``False``) which neighbor
-        any masked value (give by ``True``) and which are on the extreme exterior of the mask.
-
-        For example, for the following ``Mask2D``:
-
-        ::
-            mask_2d = aa.Mask2D(
-                mask=[[True,  True,  True,  True,  True,  True,  True,  True, True],
-                      [True, False, False, False, False, False, False, False, True],
-                      [True, False,  True,  True,  True,  True,  True, False, True],
-                      [True, False,  True, False, False, False,  True, False, True],
-                      [True, False,  True, False,  True, False,  True, False, True],
-                      [True, False,  True, False, False, False,  True, False, True],
-                      [True, False,  True,  True,  True,  True,  True, False, True],
-                      [True, False, False, False, False, False, False, False, True],
-                      [True,  True,  True,  True,  True,  True,  True,  True, True]]
-                pixel_scales=1.0,
-                sub_size=2
-            )
-
-        The ``edge_sub_1`` grid (given via ``mask_2d.derive_grid.edge_sub_1``) is given by:
-
-        ::
-            [[3.0, -3.0],  [3.0, -2.0],  [3.0, -1.0],  [3.0, 0.0],  [3.0, 1.0],  [3.0, 2.0],  [ 3.0, 3.0],
-             [ 2.0, -3.0],                                                                    [ 2.0, 3.0],
-             [ 1.0, -3.0],                                                                    [ 1.0, 3.0],
-             [ 0.0, -3.0],                                                                    [ 0.0, 3.0],
-             [-1.0, -3.0],                                                                    [-1.0, 3.0],
-             [-2.0, -3.0],                                                                    [-2.0, 3.0],
-             [-3.0, -3.0], [-3.0, -2.0], [-3.0, -1.0], [-3.0, 0.0], [-3.0, 1.0], [-3.0, 2.0], [-3.0, 3.0]]
-
-        The central group of pixels, which neighbor ``True`` values, are omitted because they are not at an extreme
-        edge of the mask.
-
-        Examples
-        --------
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            mask_2d = aa.Mask2D(
-                mask=[[True,  True,  True,  True,  True,  True,  True,  True, True],
-                      [True, False, False, False, False, False, False, False, True],
-                      [True, False,  True,  True,  True,  True,  True, False, True],
-                      [True, False,  True, False, False, False,  True, False, True],
-                      [True, False,  True, False,  True, False,  True, False, True],
-                      [True, False,  True, False, False, False,  True, False, True],
-                      [True, False,  True,  True,  True,  True,  True, False, True],
-                      [True, False, False, False, False, False, False, False, True],
-                      [True,  True,  True,  True,  True,  True,  True,  True, True]],
-                pixel_scales=1.0,
-                sub_size=2
-            )
-
-            derive_grid_2d = aa.DeriveGrid2D(mask=mask_2d)
-
-            print(derive_grid_2d.border_sub_1)
-        """
         from autoarray.structures.grids.uniform_2d import Grid2D
 
-        border = self.unmasked_sub_1[self.mask.derive_indexes.border_slim]
+        border = self.unmasked[self.mask.derive_indexes.border_slim]
         return Grid2D(
             values=border,
-            mask=self.mask.derive_mask.border.derive_mask.sub_1,
+            mask=self.mask.derive_mask.border,
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/mask/derive/mask_1d.py` & `autoarray-2024.5.16.0/autoarray/mask/derive/mask_1d.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,66 +46,18 @@
             derive_mask_1d = aa.DeriveMask1D(mask=mask_1d)
 
             print(derive_mask_1d.edge)
         """
         self.mask = mask
 
     @property
-    def sub_1(self) -> Mask1D:
-        """
-        Returns the same ``Mask1D`` but with its geometry and (y,x) Cartesian coordinates reduced to a `sub_size=1`.
-
-        For example, for the following ``Mask1D``:
-
-        ::
-           [True, False, False, False, True]
-
-        The ``sub_1``` mask (given via ``mask_2d.derive_mask.sub_1``) returns the same mask but its ``sub_size``
-        parameter will be reduced to 1 if it was above 1 before.
-
-        ::
-           [True, False, False, False, True]
-
-        Examples
-        --------
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            mask_1d = aa.Mask1D(
-                mask[True, False, False, False, True],
-                pixel_scales=1.0,
-                sub_size=2,
-            )
-
-            derive_mask_1d = aa.DeriveMask1D(mask=mask_1d)
-
-            mask_sub_1 = derive_mask_1d.sub_1
-
-            print(mask_sub_1)
-
-            # The sub_size of the mask is 1.
-            print(mask_sub_1.sub_size)
-        """
-
-        from autoarray.mask.mask_1d import Mask1D
-
-        return Mask1D(
-            mask=self.mask,
-            sub_size=1,
-            pixel_scales=self.mask.pixel_scales,
-            origin=self.mask.origin,
-        )
-
-    @property
     def all_false(self) -> Mask1D:
         """
         Returns a ``Mask1D`` which has the same
-        geometry (``shape_native`` / ``sub_size`` / ``pixel_scales`` / ``origin``) as this ``Mask1D`` but all
+        geometry (``shape_native`` / ``pixel_scales`` / ``origin``) as this ``Mask1D`` but all
         entries are unmasked (given by``False``).
 
         For example, for the following ``Mask1D``:
 
         ::
            [True, False, False, False, True]
 
@@ -120,26 +72,24 @@
         .. code-block:: python
 
             import autoarray as aa
 
             mask_1d = aa.Mask1D(
                 mask[True, False, False, False, True],
                 pixel_scales=1.0,
-                sub_size=2,
             )
 
             derive_mask_1d = aa.DeriveMask1D(mask=mask_1d)
 
             print(derive_mask_1d.all_false)
         """
         from autoarray.mask.mask_1d import Mask1D
 
         return Mask1D.all_false(
             shape_slim=self.mask.shape_slim,
-            sub_size=self.mask.sub_size,
             pixel_scales=self.mask.pixel_scales,
             origin=self.mask.origin,
         )
 
     @property
     def to_mask_2d(self) -> Mask2D:
         """
@@ -164,23 +114,21 @@
         .. code-block:: python
 
             import autoarray as aa
 
             mask_1d = aa.Mask1D(
                 mask[True, False, False, False, True],
                 pixel_scales=1.0,
-                sub_size=2,
             )
 
             derive_mask_1d = aa.DeriveMask1D(mask=mask_1d)
 
             print(derive_mask_1d.to_mask_2d)
         """
 
         from autoarray.mask.mask_2d import Mask2D
 
         return Mask2D(
             [self.mask],
             pixel_scales=(self.mask.pixel_scale, self.mask.pixel_scale),
-            sub_size=self.mask.sub_size,
             origin=(0.0, 0.0),
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/mask/mask_1d.py` & `autoarray-2024.5.16.0/autoarray/mask/mask_1d.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 from __future__ import annotations
+
 from astropy.io import fits
 import logging
 import numpy as np
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Tuple, Union
+from typing import List, Tuple, Union
 
-if TYPE_CHECKING:
-    from autoarray.structures.grids.uniform_1d import Grid1D
-    from autoarray.mask.mask_2d import Mask2D
 
 from autoarray.mask.abstract_mask import Mask
 
 from autoarray.mask.derive.grid_1d import DeriveGrid1D
 from autoarray.mask.derive.mask_1d import DeriveMask1D
 from autoarray.geometry.geometry_1d import Geometry1D
+from autoarray.structures.abstract_structure import Structure
 from autoarray.structures.arrays import array_1d_util
 
 from autoarray import exc
 from autoarray import type as ty
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class Mask1D(Mask):
-    def __new__(
-        cls,
+    def __init__(
+        self,
         mask: Union[np.ndarray, List],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float,] = (0.0,),
         invert: bool = False,
     ):
         """
         A 1D mask, representing 1D data on a uniform line of pixels with equal spacing.
 
         When applied to 1D data it extracts or masks the unmasked image pixels corresponding to mask entries that
         are `False` or 0).
 
         The mask also defines the geometry of the 1D data structure it is paired to, for example how every pixel
         coordinate on the 1D line of data converts to physical units via the `pixel_scales` and `origin`
-        parameters and a sub-grid which is used for performing calculations via super-sampling.
+        parameters and a grid which is used for performing calculations.
 
         Parameters
         ----------
         mask
             The ndarray of shape [total_pixels] containing the bool's representing the mask, where `False`
             signifies an entry is unmasked and used in calculations.
         pixel_scales
@@ -62,31 +60,33 @@
         if type(pixel_scales) is float:
             pixel_scales = (pixel_scales,)
 
         if len(mask.shape) != 1:
             raise exc.MaskException("The input mask is not a one dimensional array")
 
         # noinspection PyArgumentList
-        return Mask.__new__(
-            cls=cls,
+        super().__init__(
             mask=mask,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
     def __array_finalize__(self, obj):
         super().__array_finalize__(obj=obj)
 
         if isinstance(obj, Mask1D):
             pass
         else:
             self.origin = (0.0,)
 
     @property
+    def native(self) -> Structure:
+        raise NotImplemented()
+
+    @property
     def geometry(self) -> Geometry1D:
         """
         Return the 1D geometry of the mask, representing its uniform rectangular grid of (x) coordinates defined by
         its ``shape_native``.
         """
         return Geometry1D(
             shape_native=self.shape_native,
@@ -103,15 +103,14 @@
         return DeriveGrid1D(mask=self)
 
     @classmethod
     def all_false(
         cls,
         shape_slim,
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float] = (0.0,),
         invert: bool = False,
     ) -> "Mask1D":
         """
         Setup a 1D mask where all pixels are unmasked.
 
         Parameters
@@ -121,24 +120,22 @@
         pixel_scales
             The scaled units to pixel units conversion factor of each pixel.
         """
         return cls(
             mask=np.full(shape=shape_slim, fill_value=False),
             pixel_scales=pixel_scales,
             origin=origin,
-            sub_size=sub_size,
             invert=invert,
         )
 
     @classmethod
     def from_fits(
         cls,
         file_path: Union[Path, str],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         hdu: int = 0,
         origin: Tuple[float] = (0.0,),
     ) -> "Mask1D":
         """
         Loads the 1D mask from a .fits file.
 
         Parameters
@@ -150,23 +147,21 @@
         pixel_scales
             The scaled units to pixel units conversion factor of each pixel.
         """
 
         return cls(
             array_1d_util.numpy_array_1d_via_fits_from(file_path=file_path, hdu=hdu),
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
     @classmethod
     def from_primary_hdu(
         cls,
         primary_hdu: fits.PrimaryHDU,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
     ) -> "Mask1D":
         """
         Returns an ``Mask1D`` by from a `PrimaryHDU` object which has been loaded via `astropy.fits`
 
         This assumes that the `header` of the `PrimaryHDU` contains an entry named `PIXSCALE` which gives the
         pixel-scale of the array.
@@ -176,67 +171,42 @@
         the :meth:`Mask1D class API documentation <autoarray.structures.arrays.uniform_1d.AbstractMask1D.__new__>`.
 
         Parameters
         ----------
         primary_hdu
             The `PrimaryHDU` object which has already been loaded from a .fits file via `astropy.fits` and contains
             the array data and the pixel-scale in the header with an entry named `PIXSCALE`.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the coordinate system.
 
         Examples
         --------
 
         .. code-block:: python
 
             from astropy.io import fits
             import autoarray as aa
 
-            # Make Mask1D with sub_size 1.
-
             primary_hdu = fits.open("path/to/file.fits")
 
             array_1d = aa.Mask1D.from_primary_hdu(
                 primary_hdu=primary_hdu,
-                sub_size=1
-            )
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            # Make Mask1D with sub_size 2.
-            # (It is uncommon that a sub-gridded array would be loaded from
-            # a .fits, but the API support its).
-
-             primary_hdu = fits.open("path/to/file.fits")
-
-            array_1d = aa.Mask1D.from_primary_hdu(
-                primary_hdu=primary_hdu,
-                sub_size=2
             )
         """
         return cls(
             mask=primary_hdu.data.astype("bool"),
             pixel_scales=primary_hdu.header["PIXSCALE"],
-            sub_size=sub_size,
             origin=origin,
         )
 
     @property
     def shape_native(self) -> Tuple[int]:
         return self.shape
 
     @property
-    def sub_shape_native(self) -> Tuple[int]:
-        return (self.shape[0] * self.sub_size,)
-
-    @property
     def shape_slim(self) -> Tuple[int]:
         return self.shape
 
     @property
     def hdu_for_output(self) -> fits.PrimaryHDU:
         """
         The mask as a HDU object, which can be output to a .fits file.
```

### Comparing `autoarray-2024.1.27.4/autoarray/mask/mask_1d_util.py` & `autoarray-2024.5.16.0/autoarray/mask/mask_1d_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,86 +34,50 @@
         if not mask_1d[x]:
             total_regular_pixels += 1
 
     return total_regular_pixels
 
 
 @numba_util.jit()
-def total_sub_pixels_1d_from(mask_1d: np.ndarray, sub_size: int) -> int:
-    """
-    Returns the total number of sub-pixels in unmasked pixels in a mask.
-
-    Parameters
-    ----------
-    mask_1d
-        A 2D array of bools, where `False` values are unmasked and included when counting sub pixels.
-    sub_size
-        The size of the sub-grid that each pixel of the 2D mask array is divided into.
-
-    Returns
-    -------
-    int
-        The total number of sub pixels that are unmasked.
-
-    Examples
-    --------
-
-    mask = np.array([[True, False, True],
-                     [False, False, False]
-                     [True, False, True]])
-
-    total_sub_pixels = total_sub_pixels_from(mask=mask, sub_size=2)
-    """
-    return total_pixels_1d_from(mask_1d) * sub_size
-
-
-@numba_util.jit()
 def native_index_for_slim_index_1d_from(
-    mask_1d: np.ndarray, sub_size: int
+    mask_1d: np.ndarray,
 ) -> np.ndarray:
     """
-    Returns an array of shape [total_unmasked_pixels*sub_size] that maps every unmasked sub-pixel to its
+    Returns an array of shape [total_unmasked_pixels] that maps every unmasked pixel to its
     corresponding native 2D pixel using its (y,x) pixel indexes.
 
-    For example, for a sub-grid size of 2x2, if pixel [2,5] corresponds to the first pixel in the masked slim array:
+    For example, for a grid size of 3x3, if pixel [0,1] corresponds to the first pixel in the masked slim array:
 
-    - The first sub-pixel in this pixel on the 1D array is sub_native_index_for_sub_slim_index_2d[4] = [2,5]
-    - The second sub-pixel in this pixel on the 1D array is sub_native_index_for_sub_slim_index_2d[5] = [2,6]
-    - The third sub-pixel in this pixel on the 1D array is sub_native_index_for_sub_slim_index_2d[5] = [3,5]
+    - The first pixel in this pixel on the 1D array is native_index_for_slim_index_2d[0] = [0,1]
 
     Parameters
     ----------
     mask_2d
         A 2D array of bools, where `False` values are unmasked.
-    sub_size
-        The size of the sub-grid in each mask pixel.
 
     Returns
     -------
     ndarray
-        An array that maps pixels from a slimmed array of shape [total_unmasked_pixels*sub_size] to its native array
-        of shape [total_pixels*sub_size, total_pixels*sub_size].
+        An array that maps pixels from a slimmed array of shape [total_unmasked_pixels] to its native array
+        of shape [total_pixels, total_pixels].
 
     Examples
     --------
     mask_2d = np.array([[True, True, True],
                      [True, False, True]
                      [True, True, True]])
 
-    sub_native_index_for_sub_slim_index_2d = sub_native_index_for_sub_slim_index_via_mask_2d_from(mask_2d=mask_2d, sub_size=1)
+    native_index_for_slim_index_1d =  native_index_for_slim_index_1d_from(mask_2d=mask_2d)
 
     """
 
-    total_sub_pixels = total_sub_pixels_1d_from(mask_1d=mask_1d, sub_size=sub_size)
-    sub_native_index_for_sub_slim_index_1d = np.zeros(shape=total_sub_pixels)
+    total_pixels = total_pixels_1d_from(mask_1d=mask_1d)
+    native_index_for_slim_index_1d = np.zeros(shape=total_pixels)
 
-    sub_slim_index = 0
+    slim_index = 0
 
     for x in range(mask_1d.shape[0]):
         if not mask_1d[x]:
-            for x1 in range(sub_size):
-                sub_native_index_for_sub_slim_index_1d[sub_slim_index] = (
-                    x * sub_size
-                ) + x1
-                sub_slim_index += 1
+            native_index_for_slim_index_1d[slim_index] = x
+            slim_index += 1
 
-    return sub_native_index_for_sub_slim_index_1d
+    return native_index_for_slim_index_1d
```

### Comparing `autoarray-2024.1.27.4/autoarray/mask/mask_2d.py` & `autoarray-2024.5.16.0/autoarray/mask/mask_2d.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 from astropy.io import fits
+import copy
 import logging
 import numpy as np
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Tuple, Union
 
+from autoarray.structures.abstract_structure import Structure
+
 if TYPE_CHECKING:
     from autoarray.structures.arrays.uniform_2d import Array2D
 
 from autoconf import cached_property
 
 from autoarray.mask.abstract_mask import Mask
 
@@ -26,19 +29,18 @@
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class Mask2D(Mask):
     # noinspection PyUnusedLocal
-    def __new__(
-        cls,
+    def __init__(
+        self,
         mask: Union[np.ndarray, List],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         invert: bool = False,
         *args,
         **kwargs,
     ):
         """
         A 2D mask, used for masking values which are associated with a a uniform rectangular grid of pixels.
@@ -47,25 +49,23 @@
         unmasked and therefore used in subsequent calculations. .
 
         The ``Mask2D`, has in-built functionality which:
 
         - Maps data structures between two data representations: `slim`` (all unmasked ``False`` values in
           a 1D ``ndarray``) and ``native`` (all unmasked values in a 2D or 3D ``ndarray``).
 
-        - Has a ``Geometry2D`` object (defined by its (y,x) ``pixel scales``, (y,x) ``origin`` and ``sub_size``)
+        - Has a ``Geometry2D`` object (defined by its (y,x) ``pixel scales`` and (y,x) ``origin``)
           which defines how coordinates are converted from pixel units to scaled units.
 
         - Associates Cartesian ``Grid2D`` objects of (y,x) coordinates with the data structure (e.g.
-          a (y,x) grid of all unmasked pixels) via the ``DeriveGrid2D`` object.
-
-        - This includes sub-grids, which perform calculations higher resolutions which are then binned up.
+          a (y,x) grid of all unmasked pixels).
 
         A detailed description of the 2D mask API is provided below.
 
-        **SLIM DATA REPRESENTATION (sub-size=1)**
+        __Slim__
 
         Below is a visual illustration of a ``Mask2D``, where a total of 10 pixels are unmasked (values are ``False``):
 
         ::
 
              x x x x x x x x x x
              x x x x x x x x x x     This is an example ``Mask2D``, where:
@@ -103,18 +103,18 @@
 
         ::
 
             mask[3] = the 4th unmasked pixel's value.
             mask[6] = the 7th unmasked pixel's value.
 
         A Cartesian grid of (y,x) coordinates, corresponding to all ``slim`` values (e.g. unmasked pixels) is given
-        by ``mask.derive_grid.masked.slim``.
+        by:
 
 
-        **NATIVE DATA REPRESENTATION (sub_size=1)**
+        __native__
 
         Masked data represented as an an ``ndarray`` of shape [total_y_values, total_x_values], where all masked
         entries have values of 0.0.
 
         For the following mask:
 
         ::
@@ -159,115 +159,29 @@
             - mask[3,5] = False (not masked)
             - mask[4,5] = False (not masked)
 
         **SLIM TO NATIVE MAPPING**
 
         The ``Mask2D`` has functionality which maps data between the ``slim`` and ``native`` data representations.
 
-        For the example mask above, the 1D ``ndarray`` given by ``mask.derive_indexes.slim_to_native`` is:
+        For the example mask above, the 1D ``ndarray`` given by ``derive_indexes.slim_to_native`` is:
 
         ::
 
             slim_to_native[0] = [3,4]
             slim_to_native[1] = [3,5]
             slim_to_native[2] = [4,3]
             slim_to_native[3] = [4,4]
             slim_to_native[4] = [4,5]
             slim_to_native[5] = [4,6]
             slim_to_native[6] = [5,3]
             slim_to_native[7] = [5,4]
             slim_to_native[8] = [5,5]
             slim_to_native[9] = [5,6]
 
-        **SUB GRIDDING**
-
-        If the ``Mask2D`` ``sub_size`` is > 1, its ``slim`` and ``native`` data representations have entries
-        corresponding to the values at the centre of every sub-pixel of each unmasked pixel.
-
-        The sub-array indexes are ordered such that pixels begin from the first (top-left) sub-pixel in the first
-        unmasked pixel. Indexes then go over the sub-pixels in each unmasked pixel, for every unmasked pixel.
-
-        Therefore, the shapes of the sub-array are as follows:
-
-        - ``slim`` representation: an ``ndarray`` of shape [total_unmasked_pixels*sub_size**2].
-        - ``native`` representation: an ``ndarray`` of shape [total_y_values*sub_size, total_x_values*sub_size].
-
-        Below is a visual illustration of a sub array. Indexing of each sub-pixel goes from the top-left corner. In
-        contrast to the array above, our illustration below restricts the mask to just 2 pixels, to keep the
-        illustration brief.
-
-        ::
-
-             x x x x x x x x x x
-             x x x x x x x x x x     This is an example ``Mask2D``, where:
-             x x x x x x x x x x
-             x x x x x x x x x x     x = `True` (Pixel is masked and excluded from lens)
-             x 0 0 x x x x x x x     O = `False` (Pixel is not masked and included in lens)
-             x x x x x x x x x x
-             x x x x x x x x x x
-             x x x x x x x x x x
-             x x x x x x x x x x
-             x x x x x x x x x x
-
-        If ``sub_size=2``, each unmasked pixel has 4 (2x2) sub-pixel values. For the example above, pixels 0 and 1
-        each have 4 values which map to ``slim`` representation as follows:
-
-        ::
-
-            Pixel 0 - (2x2):
-
-                   slim[0] = value of first sub-pixel in pixel 0.
-             0 1   slim[1] = value of first sub-pixel in pixel 1.
-             2 3   slim[2] = value of first sub-pixel in pixel 2.
-                   slim[3] = value of first sub-pixel in pixel 3.
-
-            Pixel 1 - (2x2):
-
-                   slim[4] = value of first sub-pixel in pixel 0.
-             4 5   slim[5] = value of first sub-pixel in pixel 1.
-             6 7   slim[6] = value of first sub-pixel in pixel 2.
-                   slim[7] = value of first sub-pixel in pixel 3.
-
-        For the ``native`` data representation we get the following mappings:
-
-        ::
-
-            Pixel 0 - (2x2):
-
-                   native[8, 2] = value of first sub-pixel in pixel 0.
-             0 1   native[8, 3] = value of first sub-pixel in pixel 1.
-             2 3   native[9, 2] = value of first sub-pixel in pixel 2.
-                   native[9, 3] = value of first sub-pixel in pixel 3.
-
-            Pixel 1 - (2x2):
-
-                   native[10, 4] = value of first sub-pixel in pixel 0.
-             4 5   native[10, 5] = value of first sub-pixel in pixel 1.
-             6 7   native[11, 4] = value of first sub-pixel in pixel 2.
-                   native[11, 5] = value of first sub-pixel in pixel 3.
-
-            Other entries (all masked sub-pixels are zero):
-
-                   native[0, 0] = 0.0 (it is masked, thus zero)
-                   native[15, 12] = 0.0 (it is masked, thus zero)
-
-        If we used a sub_size of 3, for pixel 0 we we would create a 3x3 sub-array:
-
-        ::
-
-                     slim[0] = value of first sub-pixel in pixel 0.
-                     slim[1] = value of first sub-pixel in pixel 1.
-                     slim[2] = value of first sub-pixel in pixel 2.
-             0 1 2   slim[3] = value of first sub-pixel in pixel 3.
-             3 4 5   slim[4] = value of first sub-pixel in pixel 4.
-             6 7 8   slim[5] = value of first sub-pixel in pixel 5.
-                     slim[6] = value of first sub-pixel in pixel 6.
-                     slim[7] = value of first sub-pixel in pixel 7.
-                     slim[8] = value of first sub-pixel in pixel 8.
-
         Parameters
         ----------
         mask
             The `ndarray` of shape [total_y_pixels, total_x_pixels] containing the `bool`'s representing the
             `mask`, where `False` signifies an entry is unmasked and used in calculations.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
@@ -275,51 +189,56 @@
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         """
 
         if type(mask) is list:
             mask = np.asarray(mask).astype("bool")
 
+        if not isinstance(mask, np.ndarray):
+            mask = mask._array
+
         if invert:
             mask = np.invert(mask)
 
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         if len(mask.shape) != 2:
             raise exc.MaskException("The input mask is not a two dimensional array")
 
-        obj = Mask.__new__(
-            cls=cls,
+        super().__init__(
             mask=mask,
-            pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
+            pixel_scales=pixel_scales,
         )
 
-        return obj
+    __no_flatten__ = ("derive_indexes",)
 
     def __array_finalize__(self, obj):
         super().__array_finalize__(obj=obj)
 
         if not isinstance(obj, Mask2D):
             self.origin = (0.0, 0.0)
 
     @property
+    def native(self) -> Structure:
+        return self
+
+    @property
     def geometry(self) -> Geometry2D:
         """
         Return the 2D geometry of the mask, representing its uniform rectangular grid of (y,x) coordinates defined by
         its ``shape_native``.
         """
         return Geometry2D(
             shape_native=self.shape_native,
             pixel_scales=self.pixel_scales,
             origin=self.origin,
         )
 
-    @cached_property
+    @property
     def derive_indexes(self) -> DeriveIndexes2D:
         return DeriveIndexes2D(mask=self)
 
     @property
     def derive_mask(self) -> DeriveMask2D:
         return DeriveMask2D(mask=self)
 
@@ -328,51 +247,46 @@
         return DeriveGrid2D(mask=self)
 
     @classmethod
     def all_false(
         cls,
         shape_native: Tuple[int, int],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         invert: bool = False,
     ) -> "Mask2D":
         """
         Create a mask where all pixels are `False` and therefore unmasked.
 
         Parameters
         ----------
         shape_native
             The 2D shape of the mask that is created.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) structure.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         invert
             If `True`, the `bool`'s of the input `mask` are inverted, for example `False`'s become `True`
             and visa versa.
         """
         return cls(
             mask=np.full(shape=shape_native, fill_value=False),
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             invert=invert,
         )
 
     @classmethod
     def circular(
         cls,
         shape_native: Tuple[int, int],
         radius: float,
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         centre: Tuple[float, float] = (0.0, 0.0),
         invert: bool = False,
     ) -> "Mask2D":
         """
         Returns a Mask2D (see *Mask2D.__new__*) where all `False` entries are within a circle of input radius.
 
@@ -383,16 +297,14 @@
         shape_native
             The (y,x) shape of the mask in units of pixels.
         radius
             The radius in scaled units of the circle within which pixels are `False` and unmasked.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) structure.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         centre
             The (y,x) scaled units centre of the circle used to mask pixels.
         invert
             If `True`, the `bool`'s of the input `mask` are inverted, for example `False`'s become `True`
             and visa versa.
@@ -406,27 +318,25 @@
             radius=radius,
             centre=centre,
         )
 
         return cls(
             mask=mask,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             invert=invert,
         )
 
     @classmethod
     def circular_annular(
         cls,
         shape_native: Tuple[int, int],
         inner_radius: float,
         outer_radius: float,
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         centre: Tuple[float, float] = (0.0, 0.0),
         invert: bool = False,
     ) -> "Mask2D":
         """
         Returns a Mask2D (see *Mask2D.__new__*) where all `False` entries are within an annulus of input
         inner radius and outer radius.
@@ -440,16 +350,14 @@
         inner_radius
             The inner radius in scaled units of the annulus within which pixels are `False` and unmasked.
         outer_radius
             The outer radius in scaled units of the annulus within which pixels are `False` and unmasked.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) structure.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         centre
             The (y,x) scaled units centre of the annulus used to mask pixels.
         invert
             If `True`, the `bool`'s of the input `mask` are inverted, for example `False`'s become `True`
             and visa versa.
@@ -464,28 +372,26 @@
             outer_radius=outer_radius,
             centre=centre,
         )
 
         return cls(
             mask=mask,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             invert=invert,
         )
 
     @classmethod
     def circular_anti_annular(
         cls,
         shape_native: Tuple[int, int],
         inner_radius: float,
         outer_radius: float,
         outer_radius_2: float,
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         centre: Tuple[float, float] = (0.0, 0.0),
         invert: bool = False,
     ) -> "Mask2D":
         """
         Returns a Mask2D (see *Mask2D.__new__*) where all `False` entries are within an inner circle and second
         outer circle, forming an inverse annulus.
@@ -502,16 +408,14 @@
             The first outer radius in scaled units of the annulus within which pixels are `True` and masked.
         outer_radius_2
             The second outer radius in scaled units of the annulus within which pixels are `False` and unmasked and
             outside of which all entries are `True` and masked.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) structure.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         centre
             The (y,x) scaled units centre of the anti-annulus used to mask pixels.
         invert
             If `True`, the `bool`'s of the input `mask` are inverted, for example `False`'s become `True`
             and visa versa.
@@ -527,28 +431,26 @@
             outer_radius_2_scaled=outer_radius_2,
             centre=centre,
         )
 
         return cls(
             mask=mask,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             invert=invert,
         )
 
     @classmethod
     def elliptical(
         cls,
         shape_native: Tuple[int, int],
         major_axis_radius: float,
         axis_ratio: float,
         angle: float,
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         centre: Tuple[float, float] = (0.0, 0.0),
         invert: bool = False,
     ) -> "Mask2D":
         """
         Returns a Mask2D (see *Mask2D.__new__*) where all `False` entries are within an ellipse.
 
@@ -564,16 +466,14 @@
             The axis-ratio of the ellipse within which pixels are unmasked.
         angle
             The rotation angle of the ellipse within which pixels are unmasked, (counter-clockwise from the positive
              x-axis).
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) structure.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         centre
             The (y,x) scaled units centred of the ellipse used to mask pixels.
         invert
             If `True`, the `bool`'s of the input `mask` are inverted, for example `False`'s become `True`
             and visa versa.
@@ -588,15 +488,14 @@
             angle=angle,
             centre=centre,
         )
 
         return cls(
             mask=mask,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             invert=invert,
         )
 
     @classmethod
     def elliptical_annular(
         cls,
@@ -604,15 +503,14 @@
         inner_major_axis_radius: float,
         inner_axis_ratio: float,
         inner_phi: float,
         outer_major_axis_radius: float,
         outer_axis_ratio: float,
         outer_phi: float,
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         centre: Tuple[float, float] = (0.0, 0.0),
         invert: bool = False,
     ) -> "Mask2D":
         """
         Returns a Mask2D (see *Mask2D.__new__*) where all `False` entries are within an elliptical annulus of input
         inner and outer scaled major-axis and centre.
@@ -635,16 +533,14 @@
         outer_major_axis_radius
             The major-axis in scaled units of the outer ellipse within which pixels are unmasked.
         outer_axis_ratio
             The axis-ratio of the outer ellipse within which pixels are unmasked.
         outer_phi
             The rotation angle of the outer ellipse within which pixels are unmasked, (counter-clockwise from the
             positive x-axis).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         centre
             The (y,x) scaled units centre of the elliptical annuli used to mask pixels.
         invert
             If `True`, the `bool`'s of the input `mask` are inverted, for example `False`'s become `True`
             and visa versa.
@@ -662,26 +558,24 @@
             outer_phi=outer_phi,
             centre=centre,
         )
 
         return cls(
             mask=mask,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             invert=invert,
         )
 
     @classmethod
     def from_pixel_coordinates(
         cls,
         shape_native: Tuple[int, int],
         pixel_coordinates: [[int, int]],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         buffer: int = 0,
         invert: bool = False,
     ) -> "Mask2D":
         """
         Returns a Mask2D (see *Mask2D.__new__*) where all `False` entries are defined from an input list of list of
         pixel coordinates.
@@ -693,16 +587,14 @@
         ----------
         shape_native (int, int)
             The (y,x) shape of the mask in units of pixels.
         pixel_coordinates : [[int, int]]
             The input lists of 2D pixel coordinates where `False` entries are created.
         pixel_scales
             The scaled units to pixel units conversion factor of each pixel.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         buffer
             All input `pixel_coordinates` are buffed with `False` entries in all 8 neighboring directions by this
             amount.
         invert
             If `True`, the `bool`'s of the input `mask` are inverted, for example `False`'s become `True`
@@ -714,66 +606,60 @@
             pixel_coordinates=pixel_coordinates,
             buffer=buffer,
         )
 
         return cls(
             mask=mask,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             invert=invert,
         )
 
     @classmethod
     def from_fits(
         cls,
         file_path: Union[Path, str],
         pixel_scales: ty.PixelScales,
         hdu: int = 0,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         resized_mask_shape: Tuple[int, int] = None,
     ) -> "Mask2D":
         """
         Loads the image from a .fits file.
 
         Parameters
         ----------
         file_path
             The full path of the fits file.
         hdu
             The HDU number in the fits file containing the image image.
         pixel_scales or (float, float)
             The scaled units to pixel units conversion factor of each pixel.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         """
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         mask = Mask2D(
             mask=array_2d_util.numpy_array_2d_via_fits_from(
                 file_path=file_path, hdu=hdu
             ),
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
         if resized_mask_shape is not None:
-            mask = mask.derive_mask.resized_from(new_shape=resized_mask_shape)
+            mask = mask.resized_from(new_shape=resized_mask_shape)
 
         return mask
 
     @classmethod
     def from_primary_hdu(
         cls,
         primary_hdu: fits.PrimaryHDU,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
     ) -> "Mask2D":
         """
         Returns an ``Mask2D`` by from a `PrimaryHDU` object which has been loaded via `astropy.fits`
 
         This assumes that the `header` of the `PrimaryHDU` contains an entry named `PIXSCALE` which gives the
         pixel-scale of the array.
@@ -783,91 +669,62 @@
         the :meth:`Mask2D class API documentation <autoarray.structures.arrays.uniform_2d.AbstractMask2D.__new__>`.
 
         Parameters
         ----------
         primary_hdu
             The `PrimaryHDU` object which has already been loaded from a .fits file via `astropy.fits` and contains
             the array data and the pixel-scale in the header with an entry named `PIXSCALE`.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the coordinate system.
 
         Examples
         --------
 
         .. code-block:: python
 
             from astropy.io import fits
             import autoarray as aa
 
-            # Make Mask2D with sub_size 1.
-
             primary_hdu = fits.open("path/to/file.fits")
 
             array_2d = aa.Mask2D.from_primary_hdu(
                 primary_hdu=primary_hdu,
-                sub_size=1
-            )
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            # Make Mask2D with sub_size 2.
-            # (It is uncommon that a sub-gridded array would be loaded from
-            # a .fits, but the API support its).
-
-             primary_hdu = fits.open("path/to/file.fits")
-
-            array_2d = aa.Mask2D.from_primary_hdu(
-                primary_hdu=primary_hdu,
-                sub_size=2
             )
         """
         return cls(
             mask=cls.flip_hdu_for_ds9(primary_hdu.data.astype("float")),
             pixel_scales=primary_hdu.header["PIXSCALE"],
-            sub_size=sub_size,
             origin=origin,
         )
 
     @property
     def shape_native(self) -> Tuple[int, ...]:
         return self.shape
 
-    @property
-    def sub_shape_native(self) -> Tuple[int, int]:
-        try:
-            return (self.shape[0] * self.sub_size, self.shape[1] * self.sub_size)
-        except AttributeError:
-            print("bleh")
-
     def trimmed_array_from(self, padded_array, image_shape) -> Array2D:
         """
         Map a padded 1D array of values to its original 2D array, trimming all edge values.
 
         Parameters
         ----------
         padded_array
             A 1D array of values which were computed using a padded grid
         """
 
         from autoarray.structures.arrays.uniform_2d import Array2D
 
         pad_size_0 = self.shape[0] - image_shape[0]
         pad_size_1 = self.shape[1] - image_shape[1]
-        trimmed_array = padded_array.binned.native[
+        trimmed_array = padded_array.native[
             pad_size_0 // 2 : self.shape[0] - pad_size_0 // 2,
             pad_size_1 // 2 : self.shape[1] - pad_size_1 // 2,
         ]
         return Array2D.no_mask(
             values=trimmed_array,
             pixel_scales=self.pixel_scales,
-            sub_size=1,
             origin=self.origin,
         )
 
     def unmasked_blurred_array_from(self, padded_array, psf, image_shape) -> Array2D:
         """
         For a padded grid and psf, compute an unmasked blurred image from an unmasked unblurred image.
 
@@ -936,18 +793,22 @@
             file_path=file_path,
             overwrite=overwrite,
             header_dict=self.pixel_scale_header,
         )
 
     @property
     def mask_centre(self) -> Tuple[float, float]:
-        return grid_2d_util.grid_2d_centre_from(
-            grid_2d_slim=self.derive_grid.unmasked_sub_1
+        grid = grid_2d_util.grid_2d_slim_via_mask_from(
+            mask_2d=np.array(self),
+            pixel_scales=self.pixel_scales,
+            origin=self.origin,
         )
 
+        return grid_2d_util.grid_2d_centre_from(grid_2d_slim=grid)
+
     @property
     def shape_native_masked_pixels(self) -> Tuple[int, int]:
         """
         The (y,x) shape corresponding to the extent of unmasked pixels that go vertically and horizontally across the
         mask.
 
         For example, if a mask is primarily surrounded by True entries, and there are 15 False entries going vertically
@@ -956,19 +817,141 @@
 
         where = np.array(np.where(np.invert(self.astype("bool"))))
         y0, x0 = np.amin(where, axis=1)
         y1, x1 = np.amax(where, axis=1)
 
         return (y1 - y0 + 1, x1 - x0 + 1)
 
+    def rescaled_from(self, rescale_factor) -> Mask2D:
+        """
+        Returns the ``Mask2D`` rescaled to a bigger or small shape via input ``rescale_factor``.
+
+        For example, for a ``rescale_factor=2.0`` the following mask:
+
+        ::
+           [[ True,  True],
+            [False, False]]
+
+        Will double in size and become:
+
+        ::
+            [[True,   True,  True,  True],
+             [True,   True,  True,  True],
+             [False, False, False, False],
+             [False, False, False, False]]
+
+        Parameters
+        ----------
+        rescale_factor
+            The factor by which the ``Mask2D`` is rescaled (less than 1.0 produces a smaller mask, greater than 1.0
+            produces a bigger mask).
+
+        Examples
+        --------
+
+        .. code-block:: python
+
+            import autoarray as aa
+
+            mask_2d = aa.Mask2D(
+                mask=[
+                     [ True,  True],
+                     [False, False]
+                ],
+                pixel_scales=1.0,
+            )
+
+            print(mask_2d.rescaled_from(rescale_factor=2.0)
+        """
+        from autoarray.mask.mask_2d import Mask2D
+
+        rescaled_mask = mask_2d_util.rescaled_mask_2d_from(
+            mask_2d=np.array(self),
+            rescale_factor=rescale_factor,
+        )
+
+        return Mask2D(
+            mask=rescaled_mask,
+            pixel_scales=self.pixel_scales,
+            origin=self.origin,
+        )
+
+    def resized_from(self, new_shape, pad_value: int = 0.0) -> Mask2D:
+        """
+        Returns the ``Mask2D`` resized to a small or bigger ``ndarraay``, but with the same distribution of
+         ``False`` and ``True`` entries.
+
+        Resizing which increases the ``Mask2D`` shape pads it with values on its edge.
+
+        Resizing which reduces the ``Mask2D`` shape removes entries on its edge.
+
+        For example, for a ``new_shape=(4,4)`` the following mask:
+
+        ::
+           [[ True,  True],
+            [False, False]]
+
+        Will be padded with zeros (``False`` values) and become:
+
+        ::
+          [[True,  True,  True, True]
+           [True,  True,  True, True],
+           [True, False, False, True],
+           [True,  True,  True, True]]
+
+        Parameters
+        ----------
+        new_shape
+            The new two-dimensional shape of the resized ``Mask2D``.
+        pad_value
+            The value new values are padded using if the resized ``Mask2D`` is bigger.
+
+        Examples
+        --------
+
+        .. code-block:: python
+
+            import autoarray as aa
+
+            mask_2d = aa.Mask2D(
+                mask=[
+                     [ True,  True],
+                     [False, False]
+                ],
+                pixel_scales=1.0,
+            )
+
+            print(mask_2d.resized_from(new_shape=(4,4))
+        """
+
+        resized_mask = array_2d_util.resized_array_2d_from(
+            array_2d=np.array(self),
+            resized_shape=new_shape,
+            pad_value=pad_value,
+        ).astype("bool")
+
+        return Mask2D(
+            mask=resized_mask,
+            pixel_scales=self.pixel_scales,
+            origin=self.origin,
+        )
+
     @property
     def zoom_centre(self) -> Tuple[float, float]:
-        extraction_grid_1d = self.geometry.grid_pixels_2d_from(
-            grid_scaled_2d=self.derive_grid.unmasked_sub_1.slim
+        from autoarray.structures.grids.uniform_2d import Grid2D
+
+        grid = grid_2d_util.grid_2d_slim_via_mask_from(
+            mask_2d=np.array(self),
+            pixel_scales=self.pixel_scales,
+            origin=self.origin,
         )
+
+        grid = Grid2D(values=grid, mask=self)
+
+        extraction_grid_1d = self.geometry.grid_pixels_2d_from(grid_scaled_2d=grid)
         y_pixels_max = np.max(extraction_grid_1d[:, 0])
         y_pixels_min = np.min(extraction_grid_1d[:, 0])
         x_pixels_max = np.max(extraction_grid_1d[:, 1])
         x_pixels_min = np.min(extraction_grid_1d[:, 1])
 
         return (
             ((y_pixels_max + y_pixels_min - 1.0) / 2.0),
@@ -1034,15 +1017,14 @@
         This is defined from the top-left corner, such that the first pixel at location [0, 0] will have a negative x
         value y value in scaled units.
         """
 
         return Mask2D.all_false(
             shape_native=self.zoom_shape_native,
             pixel_scales=self.pixel_scales,
-            sub_size=self.sub_size,
             origin=self.zoom_offset_scaled,
         )
 
     @property
     def is_circular(self) -> bool:
         """
         Returns whether the mask is circular or not.
```

### Comparing `autoarray-2024.1.27.4/autoarray/mask/mask_2d_util.py` & `autoarray-2024.5.16.0/autoarray/mask/mask_2d_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -75,43 +75,14 @@
             if not mask_2d[y, x]:
                 total_regular_pixels += 1
 
     return total_regular_pixels
 
 
 @numba_util.jit()
-def total_sub_pixels_2d_from(mask_2d: np.ndarray, sub_size: int) -> int:
-    """
-    Returns the total number of sub-pixels in unmasked pixels in a mask.
-
-    Parameters
-    ----------
-    mask_2d
-        A 2D array of bools, where `False` values are unmasked and included when counting sub pixels.
-    sub_size
-        The size of the sub-grid that each pixel of the 2D mask array is divided into.
-
-    Returns
-    -------
-    int
-        The total number of sub pixels that are unmasked.
-
-    Examples
-    --------
-
-    mask = np.array([[True, False, True],
-                     [False, False, False]
-                     [True, False, True]])
-
-    total_sub_pixels = total_sub_pixels_from(mask=mask, sub_size=2)
-    """
-    return total_pixels_2d_from(mask_2d) * sub_size**2
-
-
-@numba_util.jit()
 def mask_2d_circular_from(
     shape_native: Tuple[int, int],
     pixel_scales: ty.PixelScales,
     radius: float,
     centre: Tuple[float, float] = (0.0, 0.0),
 ) -> np.ndarray:
     """
@@ -550,15 +521,15 @@
                             0 <= x + x1 <= mask_2d.shape[1] - 1
                             and 0 <= y + y1 <= mask_2d.shape[0] - 1
                         ):
                             if mask_2d[y + y1, x + x1]:
                                 blurring_mask_2d[y + y1, x + x1] = False
                         else:
                             raise exc.MaskException(
-                                "setup_blurring_mask extends beyond the sub_size "
+                                "setup_blurring_mask extends beyond the edge "
                                 "of the mask - pad the datas array before masking"
                             )
 
     return blurring_mask_2d
 
 
 @numba_util.jit()
@@ -607,36 +578,27 @@
 @numba_util.jit()
 def mask_slim_indexes_from(
     mask_2d: np.ndarray, return_masked_indexes: bool = True
 ) -> np.ndarray:
     """
     Returns a 1D array listing all masked (`value=True`) or unmasked pixel indexes (`value=False`) in the mask.
 
-    For example, for the following ``Mask2D`` for ``sub_size=1``:
+    For example, for the following ``Mask2D``:
 
     ::
         [[True,  True,  True, True]
          [True, False, False, True],
          [True, False,  True, True],
          [True,  True,  True, True]]
 
     This has three unmasked (``False`` values) which have the ``slim`` indexes, there ``unmasked_slim`` is:
 
     ::
         [0, 1, 2]
 
-    For a ``Mask2D`` with ``sub_size=2`` each unmasked ``False`` entry is split into a sub-pixel of size 2x2.
-    Therefore the array ``unmasked_slim`` becomes:
-
-    ::
-        [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
-
-    The ``slim`` indexes are by definition the unmasked pixels, therefore this will always return an array of
-    ascending integers with size the total number of unmasked pixels multiplied by the ``sub_size**2``.
-
     Parameters
     ----------
     mask_2d
         The mask for which the 1D unmasked pixel indexes are computed.
     return_masked_indexes
         Whether to return the masked index values (`value=True`) or the unmasked index values (`value=False`).
 
@@ -818,15 +780,15 @@
 
     Parameters
     ----------
     mask_2d
         The mask for which the input pixel is checked if it is a border pixel.
     edge_pixel_slim
         The edge pixel index in 1D that is checked if it is a border pixel (this 1D index is mapped to 2d via the
-        array `sub_native_index_for_sub_slim_index_2d`).
+        array `native_index_for_slim_index_2d`).
     native_to_slim
         An array describing the native 2D array index that every slimmed array index maps too.
 
     Returns
     -------
     bool
         If `True` the pixel on the mask is a border pixel, else a `False` is returned because it is not.
@@ -863,15 +825,15 @@
 
     Parameters
     ----------
     mask_2d
         The mask for which the total number of border pixels is computed.
     edge_pixel_1d
         The edge pixel index in 1D that is checked if it is a border pixel (this 1D index is mapped to 2d via the
-        array `sub_native_index_for_sub_slim_index_2d`).
+        array `native_index_for_slim_index_2d`).
     native_to_slim
         An array describing the 2D array index that every 1D array index maps too.
 
     Returns
     -------
     int
         The total number of border pixels.
@@ -929,101 +891,40 @@
     Returns
     -------
     np.ndarray
         The slimmed indexes of all border pixels on the mask.
     """
 
     edge_pixels = edge_1d_indexes_from(mask_2d=mask_2d)
-    sub_native_index_for_sub_slim_index_2d = native_index_for_slim_index_2d_from(
-        mask_2d=mask_2d, sub_size=1
+    native_index_for_slim_index_2d = native_index_for_slim_index_2d_from(
+        mask_2d=mask_2d,
     )
 
     border_pixel_total = total_border_pixels_from(
         mask_2d=mask_2d,
         edge_pixels=edge_pixels,
-        native_to_slim=sub_native_index_for_sub_slim_index_2d,
+        native_to_slim=native_index_for_slim_index_2d,
     )
 
     border_pixels = np.zeros(border_pixel_total)
 
     border_pixel_index = 0
 
     for edge_pixel_index in range(edge_pixels.shape[0]):
         if check_if_border_pixel(
             mask_2d=mask_2d,
             edge_pixel_slim=edge_pixels[edge_pixel_index],
-            native_to_slim=sub_native_index_for_sub_slim_index_2d,
+            native_to_slim=native_index_for_slim_index_2d,
         ):
             border_pixels[border_pixel_index] = edge_pixels[edge_pixel_index]
             border_pixel_index += 1
 
     return border_pixels
 
 
-def sub_border_pixel_slim_indexes_from(
-    mask_2d: np.ndarray, sub_size: int
-) -> np.ndarray:
-    """
-    Returns a slim array of shape [total_unmasked_border_pixels] listing all sub-borders pixel indexes in
-    the mask.
-
-    A borders pixel is a pixel which:
-
-    1) is not fully surrounding by `False` mask values.
-    2) Can reach the edge of the array without hitting a masked pixel in one of four directions (upwards, downwards,
-       left, right).
-
-    The borders pixels are thus pixels which are on the exterior edge of the mask. For example, the inner ring of
-    edge pixels in an annular mask are edge pixels but not borders pixels.
-
-    A sub-border pixel is, for a border-pixel, the pixel within that border pixel which is furthest from the origin
-    of the mask.
-
-    Parameters
-    ----------
-    mask_2d
-        The mask for which the 1D border pixel indexes are calculated.
-    sub_size
-        The size of the sub-grid in each mask pixel.
-
-    Returns
-    -------
-    np.ndarray
-        The 1D indexes of all border sub-pixels on the mask.
-    """
-
-    border_pixels = border_slim_indexes_from(mask_2d=mask_2d)
-
-    sub_border_pixels = np.zeros(shape=border_pixels.shape[0])
-
-    sub_slim_indexes_for_slim_index = sub_slim_indexes_for_slim_index_via_mask_2d_from(
-        mask_2d=mask_2d, sub_size=sub_size
-    )
-
-    sub_grid_2d_slim = grid_2d_util.grid_2d_slim_via_mask_from(
-        mask_2d=mask_2d, pixel_scales=(1.0, 1.0), sub_size=sub_size, origin=(0.0, 0.0)
-    )
-    mask_centre = grid_2d_util.grid_2d_centre_from(grid_2d_slim=sub_grid_2d_slim)
-
-    for border_1d_index, border_pixel in enumerate(border_pixels):
-        sub_border_pixels_of_border_pixel = sub_slim_indexes_for_slim_index[
-            int(border_pixel)
-        ]
-
-        sub_border_pixels[
-            border_1d_index
-        ] = grid_2d_util.furthest_grid_2d_slim_index_from(
-            grid_2d_slim=sub_grid_2d_slim,
-            slim_indexes=sub_border_pixels_of_border_pixel,
-            coordinate=mask_centre,
-        )
-
-    return sub_border_pixels
-
-
 @numba_util.jit()
 def buffed_mask_2d_from(mask_2d: np.ndarray, buffer: int = 1) -> np.ndarray:
     """
     Returns a buffed mask from an input mask, where the buffed mask is the input mask but all `False` entries in the
     mask are buffed by an integer amount in all 8 surrouning pixels.
 
     Parameters
@@ -1106,171 +1007,22 @@
     rescaled_mask_2d[rescaled_mask_2d.shape[0] - 1, :] = 1
     rescaled_mask_2d[:, 0] = 1
     rescaled_mask_2d[:, rescaled_mask_2d.shape[1] - 1] = 1
     return np.isclose(rescaled_mask_2d, 1)
 
 
 @numba_util.jit()
-def slim_index_for_sub_slim_index_via_mask_2d_from(
-    mask_2d: np.ndarray, sub_size: int
-) -> np.ndarray:
-    """ "
-    For pixels on a native 2D array of shape (total_y_pixels, total_x_pixels), compute a slimmed array which, for
-    every unmasked pixel on the native 2D array, maps the slimmed sub-pixel indexes to their slimmed pixel indexes.
-
-    For example, for a sub-grid size of 2, the following mappings from sub-pixels to 2D array pixels are:
-
-    - slim_index_for_sub_slim_index[0] = 0 -> The first sub-pixel maps to the first unmasked pixel on the native 2D array.
-    - slim_index_for_sub_slim_index[3] = 0 -> The fourth sub-pixel maps to the first unmasked pixel on the native 2D array.
-    - slim_index_for_sub_slim_index[7] = 1 -> The eighth sub-pixel maps to the second unmasked pixel on the native 2D array.
-
-    Parameters
-    ----------
-    mask_2d
-        The mask whose indexes are mapped.
-    sub_size
-        The sub-size of the grid on the mask, so that the sub-mask indexes can be computed correctly.
-
-    Returns
-    -------
-    np.ndarray
-        The array of shape [total_unmasked_pixels] mapping every unmasked pixel on the native 2D mask array to its
-        slimmed index on the sub-mask array.
-
-    Examples
-    --------
-    mask = np.array([[True, False, True]])
-    slim_index_for_sub_slim_index = slim_index_for_sub_slim_index_via_mask_2d_from(mask_2d=mask_2d, sub_size=2)
-    """
-
-    total_sub_pixels = total_sub_pixels_2d_from(mask_2d=mask_2d, sub_size=sub_size)
-
-    slim_index_for_sub_slim_index = np.zeros(shape=total_sub_pixels)
-    slim_index = 0
-    sub_slim_index = 0
-
-    for y in range(mask_2d.shape[0]):
-        for x in range(mask_2d.shape[1]):
-            if not mask_2d[y, x]:
-                for y1 in range(sub_size):
-                    for x1 in range(sub_size):
-                        slim_index_for_sub_slim_index[sub_slim_index] = slim_index
-                        sub_slim_index += 1
-
-                slim_index += 1
-
-    return slim_index_for_sub_slim_index
-
-
-def sub_slim_indexes_for_slim_index_via_mask_2d_from(
-    mask_2d: np.ndarray, sub_size: int
-) -> [list]:
-    """ "
-    For pixels on a native 2D array of shape (total_y_pixels, total_x_pixels), compute a list of lists which, for every
-    unmasked pixel giving its slim pixel indexes of its corresponding sub-pixels.
-
-    For example, for a sub-grid size of 2, the following mappings from sub-pixels to 2D array pixels are:
-
-    - sub_slim_indexes_for_slim_index[0] = [0, 1, 2, 3] -> The first pixel maps to the first 4 subpixels in 1D.
-    - sub_slim_indexes_for_slim_index[1] = [4, 5, 6, 7] -> The seond pixel maps to the next 4 subpixels in 1D.
-
-    Parameters
-    ----------
-    mask_2d
-        The mask whose indexes are mapped.
-    sub_size
-        The sub-size of the grid on the mask, so that the sub-mask indexes can be computed correctly.
-
-    Returns
-    -------
-    [list]
-        The lists of the 1D sub-pixel indexes in every unmasked pixel in the mask.
-    The term 'grid' is used because the grid is defined as the grid of coordinates on the centre of every
-    pixel on the 2D array. Thus, this array maps sub-pixels on a sub-grid to pixels on a grid.
-
-    Examples
-    --------
-    mask = ([[True, False, True]])
-    sub_mask_1d_indexes_for_mask_1d_index = sub_mask_1d_indexes_for_mask_1d_index_from(mask=mask, sub_size=2)
-    """
-
-    total_pixels = total_pixels_2d_from(mask_2d=mask_2d)
-
-    sub_slim_indexes_for_slim_index = [[] for _ in range(total_pixels)]
-
-    slim_index_for_sub_slim_indexes = slim_index_for_sub_slim_index_via_mask_2d_from(
-        mask_2d=mask_2d, sub_size=sub_size
-    ).astype("int")
-
-    for sub_slim_index, slim_index in enumerate(slim_index_for_sub_slim_indexes):
-        sub_slim_indexes_for_slim_index[slim_index].append(sub_slim_index)
-
-    return sub_slim_indexes_for_slim_index
-
-
-@numba_util.jit()
-def sub_slim_index_for_sub_native_index_from(sub_mask_2d: np.ndarray):
-    """
-    Returns a 2D array which maps every `False` entry of a 2D mask to its sub slim mask array. Every
-    True entry is given a value -1.
-
-    This is used as a convenience tool for creating structures util between different grids and structures.
-
-    For example, if we had a 3x4 mask:
-
-    [[False, True, False, False],
-     [False, True, False, False],
-     [False, False, False, True]]]
-
-    The sub_slim_index_for_sub_native_index array would be:
-
-    [[0, -1, 2, 3],
-     [4, -1, 5, 6],
-     [7, 8, 9, -1]]
-
-    Parameters
-    ----------
-    sub_mask_2d
-        The 2D mask that the util array is created for.
-
-    Returns
-    -------
-    ndarray
-        The 2D array mapping 2D mask entries to their 1D masked array indexes.
-
-    Examples
-    --------
-    mask = np.full(fill_value=False, shape=(9,9))
-    sub_two_to_one = mask_to_mask_1d_index_from(mask=mask)
-    """
-
-    sub_slim_index_for_sub_native_index = -1 * np.ones(shape=sub_mask_2d.shape)
-
-    sub_mask_1d_index = 0
-
-    for sub_mask_y in range(sub_mask_2d.shape[0]):
-        for sub_mask_x in range(sub_mask_2d.shape[1]):
-            if sub_mask_2d[sub_mask_y, sub_mask_x] == False:
-                sub_slim_index_for_sub_native_index[
-                    sub_mask_y, sub_mask_x
-                ] = sub_mask_1d_index
-                sub_mask_1d_index += 1
-
-    return sub_slim_index_for_sub_native_index
-
-
-@numba_util.jit()
 def native_index_for_slim_index_2d_from(
-    mask_2d: np.ndarray, sub_size: int
+    mask_2d: np.ndarray,
 ) -> np.ndarray:
     """
-    Returns an array of shape [total_unmasked_pixels*sub_size] that maps every unmasked sub-pixel to its
+    Returns an array of shape [total_unmasked_pixels] that maps every unmasked pixel to its
     corresponding native 2D pixel using its (y,x) pixel indexes.
 
-    For example, for the following ``Mask2D`` for ``sub_size=1``:
+    For example, for the following ``Mask2D``:
 
     ::
         [[True,  True,  True, True]
          [True, False, False, True],
          [True, False,  True, True],
          [True,  True,  True, True]]
 
@@ -1280,137 +1032,38 @@
         [0, 1, 2]
 
     The array ``native_index_for_slim_index_2d`` is therefore:
 
     ::
         [[1,1], [1,2], [2,1]]
 
-    For a ``Mask2D`` with ``sub_size=2`` each unmasked ``False`` entry is split into a sub-pixel of size 2x2 and
-    there are therefore 12 ``slim`` indexes:
-
-    ::
-        [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
-
-    The array ``native_index_for_slim_index_2d`` is therefore:
-
-    ::
-        [[2,2], [2,3], [2,4], [2,5], [3,2], [3,3], [3,4], [3,5], [4,2], [4,3], [5,2], [5,3]]
-
     Parameters
     ----------
     mask_2d
         A 2D array of bools, where `False` values are unmasked.
-    sub_size
-        The size of the sub-grid in each mask pixel.
 
     Returns
     -------
     ndarray
-        An array that maps pixels from a slimmed array of shape [total_unmasked_pixels*sub_size] to its native array
-        of shape [total_pixels*sub_size, total_pixels*sub_size].
+        An array that maps pixels from a slimmed array of shape [total_unmasked_pixels] to its native array
+        of shape [total_pixels, total_pixels].
 
     Examples
     --------
     mask_2d = np.array([[True, True, True],
                      [True, False, True]
                      [True, True, True]])
 
-    sub_native_index_for_sub_slim_index_2d = sub_native_index_for_sub_slim_index_via_mask_2d_from(mask_2d=mask_2d, sub_size=1)
-    """
-
-    total_sub_pixels = total_sub_pixels_2d_from(mask_2d=mask_2d, sub_size=sub_size)
-    sub_native_index_for_sub_slim_index_2d = np.zeros(shape=(total_sub_pixels, 2))
-    sub_slim_index = 0
-
-    for y in range(mask_2d.shape[0]):
-        for x in range(mask_2d.shape[1]):
-            if not mask_2d[y, x]:
-                for y1 in range(sub_size):
-                    for x1 in range(sub_size):
-                        sub_native_index_for_sub_slim_index_2d[sub_slim_index, :] = (
-                            (y * sub_size) + y1,
-                            (x * sub_size) + x1,
-                        )
-                        sub_slim_index += 1
-
-    return sub_native_index_for_sub_slim_index_2d
-
-
-@numba_util.jit()
-def mask_2d_neighbors_from(mask_2d: np.ndarray) -> np.ndarray:
-    """
-    Returns an array of shape [total_unmasked_pixels] that maps every unmasked pixel to the slim index of a
-    neighboring unmasked pixel.
-
-    Neighbors are chosen to the right of every unmasked pixel, and then down, left and up if there is no unmasked pixel
-    in each location.
-
-    Parameters
-    ----------
-    mask_2d
-        A 2D array of bools, where `False` values are unmasked.
-
-    Returns
-    -------
-    ndarray
-        A slimmed array mapping every unmasked pixel to the slimmed index of a neighboring unmasked pixel.
-
-    Examples
-    --------
-    mask = np.array(
-        [
-            [True, True, True, True],
-            [True, False, False, True],
-            [True, False, False, True],
-            [True, True, True, True],
-        ]
-    )
-
-    mask_neighbors = mask_2d_neighbors_from(mask_2d=mask_2d)
-
+    native_index_for_slim_index_2d = native_index_for_slim_index_2d_from(mask_2d=mask_2d)
     """
 
     total_pixels = total_pixels_2d_from(mask_2d=mask_2d)
-
-    mask_neighbors = -1 * np.ones(shape=total_pixels)
-
-    sub_slim_index_for_sub_native_index = sub_slim_index_for_sub_native_index_from(
-        sub_mask_2d=mask_2d
-    )
-
-    mask_index = 0
+    native_index_for_slim_index_2d = np.zeros(shape=(total_pixels, 2))
+    slim_index = 0
 
     for y in range(mask_2d.shape[0]):
         for x in range(mask_2d.shape[1]):
             if not mask_2d[y, x]:
-                flag = True
-
-                if x + 1 < mask_2d.shape[1]:
-                    if not mask_2d[y, x + 1]:
-                        mask_neighbors[
-                            mask_index
-                        ] = sub_slim_index_for_sub_native_index[y, x + 1]
-                        flag = False
-
-                if y + 1 < mask_2d.shape[0] and flag:
-                    if not mask_2d[y + 1, x]:
-                        mask_neighbors[
-                            mask_index
-                        ] = sub_slim_index_for_sub_native_index[y + 1, x]
-                        flag = False
-
-                if x - 1 >= 0 and flag:
-                    if not mask_2d[y, x - 1]:
-                        mask_neighbors[
-                            mask_index
-                        ] = sub_slim_index_for_sub_native_index[y, x - 1]
-                        flag = False
-
-                if y - 1 >= 0 and flag:
-                    if not mask_2d[y - 1, x]:
-                        mask_neighbors[
-                            mask_index
-                        ] = sub_slim_index_for_sub_native_index[y - 1, x]
-
-                mask_index += 1
+                native_index_for_slim_index_2d[slim_index, :] = y, x
+                slim_index += 1
 
-    return mask_neighbors
+    return native_index_for_slim_index_2d
```

### Comparing `autoarray-2024.1.27.4/autoarray/mock.py` & `autoarray-2024.5.16.0/autoarray/mock.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 )
 from autoarray.fit.mock.mock_fit_imaging import MockFitImaging
 from autoarray.fit.mock.mock_fit_interferometer import MockFitInterferometer
 from autoarray.mask.mock.mock_mask import MockMask
 from autoarray.operators.mock.mock_convolver import MockConvolver
 from autoarray.structures.mock.mock_grid import MockGrid2DMesh
 from autoarray.structures.mock.mock_grid import MockMeshGrid
-from autoarray.structures.mock.mock_structure_decorators import MockGridRadialMinimum
-from autoarray.structures.mock.mock_structure_decorators import MockGrid1DLikeObj
-from autoarray.structures.mock.mock_structure_decorators import MockGrid2DLikeObj
-from autoarray.structures.mock.mock_structure_decorators import MockGridLikeIteratorObj
+from autoarray.structures.mock.mock_decorators import MockGridRadialMinimum
+from autoarray.structures.mock.mock_decorators import MockGrid1DLikeObj
+from autoarray.structures.mock.mock_decorators import MockGrid2DLikeObj
+from autoarray.structures.mock.mock_decorators import MockGridLikeIteratorObj
```

### Comparing `autoarray-2024.1.27.4/autoarray/numba_util.py` & `autoarray-2024.5.16.0/autoarray/numba_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from functools import wraps
 import logging
 import time
 from typing import Callable
 
 from autoconf import conf
 
@@ -27,23 +28,27 @@
     parallel = conf.instance["general"]["numba"]["parallel"]
 except Exception:
     nopython = True
     cache = True
     parallel = False
 
 try:
-    import numba
+    if os.environ.get("USE_JAX") == "1":
+        logger.warning("JAX and numba do not work together, so JAX is being used.")
+    else:
+        import numba
 
 except ModuleNotFoundError:
     logger.warning(
         f"\n******************************************************************************\n"
         f"Numba is not being used, either because it is disabled in `config/general.yaml` "
         f"or because it is not installed.\n\n. "
         f"This will lead to slow performance.\n\n. "
         f"Install numba as described at the following webpage for improved performance. \n"
+        f"https://pyautolens.readthedocs.io/en/latest/installation/numba.html \n"
         f"********************************************************************************"
     )
 
 
 def jit(nopython=nopython, cache=cache, parallel=parallel):
     def wrapper(func):
         try:
```

### Comparing `autoarray-2024.1.27.4/autoarray/operators/convolver.py` & `autoarray-2024.5.16.0/autoarray/operators/convolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,31 +207,32 @@
             for y in range(self.mask_index_array.shape[1]):
                 if not mask[x][y]:
                     (
                         image_frame_1d_indexes,
                         image_frame_1d_kernels,
                     ) = self.frame_at_coordinates_jit(
                         coordinates=(x, y),
-                        mask=mask,
+                        mask=np.array(mask),
                         mask_index_array=self.mask_index_array,
-                        kernel_2d=self.kernel.native[:, :],
+                        kernel_2d=np.array(self.kernel.native[:, :]),
                     )
                     self.image_frame_1d_indexes[
                         mask_1d_index, :
                     ] = image_frame_1d_indexes
                     self.image_frame_1d_kernels[
                         mask_1d_index, :
                     ] = image_frame_1d_kernels
                     self.image_frame_1d_lengths[mask_1d_index] = image_frame_1d_indexes[
                         image_frame_1d_indexes >= 0
                     ].shape[0]
                     mask_1d_index += 1
 
         self.blurring_mask = mask_2d_util.blurring_mask_2d_from(
-            mask_2d=mask, kernel_shape_native=kernel.shape_native
+            mask_2d=np.array(mask),
+            kernel_shape_native=kernel.shape_native,
         )
 
         self.pixels_in_blurring_mask = int(
             np.size(self.blurring_mask) - np.sum(self.blurring_mask)
         )
 
         mask_1d_index = 0
@@ -248,17 +249,17 @@
             for y in range(mask.shape[1]):
                 if mask[x][y] and not self.blurring_mask[x, y]:
                     (
                         image_frame_1d_indexes,
                         image_frame_1d_kernels,
                     ) = self.frame_at_coordinates_jit(
                         coordinates=(x, y),
-                        mask=mask,
-                        mask_index_array=self.mask_index_array,
-                        kernel_2d=self.kernel.native,
+                        mask=np.array(mask),
+                        mask_index_array=np.array(self.mask_index_array),
+                        kernel_2d=np.array(self.kernel.native),
                     )
                     self.blurring_frame_1d_indexes[
                         mask_1d_index, :
                     ] = image_frame_1d_indexes
                     self.blurring_frame_1d_kernels[
                         mask_1d_index, :
                     ] = image_frame_1d_kernels
@@ -323,25 +324,25 @@
         if self.blurring_mask is None:
             raise exc.KernelException(
                 "You cannot use the convolve_image function of a Convolver if the Convolver was"
                 "not created with a blurring_mask."
             )
 
         convolved_image = self.convolve_jit(
-            image_1d_array=image.binned.slim,
+            image_1d_array=np.array(image.slim),
             image_frame_1d_indexes=self.image_frame_1d_indexes,
             image_frame_1d_kernels=self.image_frame_1d_kernels,
             image_frame_1d_lengths=self.image_frame_1d_lengths,
-            blurring_1d_array=blurring_image.binned.slim,
+            blurring_1d_array=np.array(blurring_image.slim),
             blurring_frame_1d_indexes=self.blurring_frame_1d_indexes,
             blurring_frame_1d_kernels=self.blurring_frame_1d_kernels,
             blurring_frame_1d_lengths=self.blurring_frame_1d_lengths,
         )
 
-        return Array2D(values=convolved_image, mask=self.mask.derive_mask.sub_1)
+        return Array2D(values=convolved_image, mask=self.mask)
 
     @staticmethod
     @numba_util.jit()
     def convolve_jit(
         image_1d_array,
         image_frame_1d_indexes,
         image_frame_1d_kernels,
@@ -380,46 +381,42 @@
     def convolve_image_no_blurring(self, image):
         """For a given 1D array and blurring array, convolve the two using this convolver.
 
         Parameters
         ----------
         image
             1D array of the values which are to be blurred with the convolver's PSF.
-        blurring_image
-            1D array of the blurring values which blur into the array after PSF convolution.
         """
 
         convolved_image = self.convolve_no_blurring_jit(
-            image_1d_array=image.binned.slim,
+            image_1d_array=np.array(image.slim),
             image_frame_1d_indexes=self.image_frame_1d_indexes,
             image_frame_1d_kernels=self.image_frame_1d_kernels,
             image_frame_1d_lengths=self.image_frame_1d_lengths,
         )
 
-        return Array2D(values=convolved_image, mask=self.mask.derive_mask.sub_1)
+        return Array2D(values=convolved_image, mask=self.mask)
 
     def convolve_image_no_blurring_interpolation(self, image):
         """For a given 1D array and blurring array, convolve the two using this convolver.
 
         Parameters
         ----------
         image
             1D array of the values which are to be blurred with the convolver's PSF.
-        blurring_image
-            1D array of the blurring values which blur into the array after PSF convolution.
         """
 
         convolved_image = self.convolve_no_blurring_jit(
             image_1d_array=image,
             image_frame_1d_indexes=self.image_frame_1d_indexes,
             image_frame_1d_kernels=self.image_frame_1d_kernels,
             image_frame_1d_lengths=self.image_frame_1d_lengths,
         )
 
-        return Array2D(values=convolved_image, mask=self.mask.derive_mask.sub_1)
+        return Array2D(values=convolved_image, mask=self.mask)
 
     @staticmethod
     @numba_util.jit()
     def convolve_no_blurring_jit(
         image_1d_array,
         image_frame_1d_indexes,
         image_frame_1d_kernels,
```

### Comparing `autoarray-2024.1.27.4/autoarray/operators/transformer.py` & `autoarray-2024.5.16.0/autoarray/operators/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,29 +56,31 @@
     def __init__(self, uv_wavelengths, real_space_mask, preload_transform=True):
         if isinstance(self, PyLopsPlaceholder):
             pylops_exception()
 
         super().__init__()
 
         self.uv_wavelengths = uv_wavelengths.astype("float")
-        self.real_space_mask = real_space_mask.derive_mask.sub_1
-        self.grid = self.real_space_mask.derive_grid.unmasked_sub_1.binned.in_radians
+        self.real_space_mask = real_space_mask
+        self.grid = self.real_space_mask.derive_grid.unmasked.in_radians
 
         self.total_visibilities = uv_wavelengths.shape[0]
         self.total_image_pixels = self.real_space_mask.pixels_in_mask
 
         self.preload_transform = preload_transform
 
         if preload_transform:
             self.preload_real_transforms = transformer_util.preload_real_transforms(
-                grid_radians=self.grid, uv_wavelengths=self.uv_wavelengths
+                grid_radians=np.array(self.grid),
+                uv_wavelengths=self.uv_wavelengths,
             )
 
             self.preload_imag_transforms = transformer_util.preload_imag_transforms(
-                grid_radians=self.grid, uv_wavelengths=self.uv_wavelengths
+                grid_radians=np.array(self.grid),
+                uv_wavelengths=self.uv_wavelengths,
             )
 
         self.real_space_pixels = self.real_space_mask.pixels_in_mask
 
         self.shape = (
             int(np.prod(self.total_visibilities)),
             int(np.prod(self.real_space_pixels)),
@@ -90,40 +92,39 @@
         self.adjoint_scaling = (2.0 * self.grid.shape_native[0]) * (
             2.0 * self.grid.shape_native[1]
         )
 
     def visibilities_from(self, image):
         if self.preload_transform:
             visibilities = transformer_util.visibilities_via_preload_jit_from(
-                image_1d=image.binned,
+                image_1d=np.array(image),
                 preloaded_reals=self.preload_real_transforms,
                 preloaded_imags=self.preload_imag_transforms,
             )
 
         else:
             visibilities = transformer_util.visibilities_jit(
-                image_1d=image.binned,
-                grid_radians=self.grid,
+                image_1d=np.array(image.slim),
+                grid_radians=np.array(self.grid),
                 uv_wavelengths=self.uv_wavelengths,
             )
 
         return Visibilities(visibilities=visibilities)
 
     def image_from(self, visibilities, use_adjoint_scaling: bool = False):
         image_slim = transformer_util.image_via_jit_from(
             n_pixels=self.grid.shape[0],
-            grid_radians=self.grid,
+            grid_radians=np.array(self.grid),
             uv_wavelengths=self.uv_wavelengths,
             visibilities=visibilities.in_array,
         )
 
         image_native = array_2d_util.array_2d_native_from(
             array_2d_slim=image_slim,
             mask_2d=self.real_space_mask,
-            sub_size=self.real_space_mask.sub_size,
         )
 
         return Array2D(values=image_native, mask=self.real_space_mask)
 
     def transform_mapping_matrix(self, mapping_matrix):
         if self.preload_transform:
             return transformer_util.transformed_mapping_matrix_via_preload_jit_from(
@@ -131,15 +132,15 @@
                 preloaded_reals=self.preload_real_transforms,
                 preloaded_imags=self.preload_imag_transforms,
             )
 
         else:
             return transformer_util.transformed_mapping_matrix_jit(
                 mapping_matrix=mapping_matrix,
-                grid_radians=self.grid,
+                grid_radians=np.array(self.grid),
                 uv_wavelengths=self.uv_wavelengths,
             )
 
 
 class TransformerNUFFT(NUFFT_cpu, PyLopsOperator):
     def __init__(self, uv_wavelengths, real_space_mask):
         if isinstance(self, NUFFTPlaceholder):
@@ -147,15 +148,15 @@
 
         if isinstance(self, PyLopsPlaceholder):
             pylops_exception()
 
         super(TransformerNUFFT, self).__init__()
 
         self.uv_wavelengths = uv_wavelengths
-        self.real_space_mask = real_space_mask.derive_mask.sub_1
+        self.real_space_mask = real_space_mask
         #        self.grid = self.real_space_mask.unmasked_grid.in_radians
         self.grid = Grid2D.from_mask(mask=self.real_space_mask).in_radians
         self.native_index_for_slim_index = copy.copy(
             real_space_mask.derive_indexes.native_for_slim.astype("int")
         )
 
         # NOTE: The plan need only be initialized once
@@ -227,20 +228,22 @@
         ...
         """
 
         warnings.filterwarnings("ignore")
 
         return Visibilities(
             visibilities=self.forward(
-                image.binned.native[::-1, :]
+                image.native[::-1, :]
             )  # flip due to PyNUFFT internal flip
         )
 
     def image_from(self, visibilities, use_adjoint_scaling: bool = False):
-        image = np.real(self.adjoint(visibilities))[::-1, :]
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            image = np.real(self.adjoint(visibilities))[::-1, :]
 
         if use_adjoint_scaling:
             image *= self.adjoint_scaling
 
         return Array2D(values=image, mask=self.real_space_mask)
 
     def transform_mapping_matrix(self, mapping_matrix):
@@ -248,15 +251,14 @@
             (self.uv_wavelengths.shape[0], mapping_matrix.shape[1])
         )
 
         for source_pixel_1d_index in range(mapping_matrix.shape[1]):
             image_2d = array_2d_util.array_2d_native_from(
                 array_2d_slim=mapping_matrix[:, source_pixel_1d_index],
                 mask_2d=self.grid.mask,
-                sub_size=1,
             )
 
             image = Array2D(values=image_2d, mask=self.grid.mask)
 
             visibilities = self.visibilities_from(image=image)
 
             transformed_mapping_matrix[:, source_pixel_1d_index] = visibilities
@@ -272,15 +274,15 @@
         :rtype: numpy array with the dtype of numpy.complex64
         """
 
         warnings.filterwarnings("ignore")
 
         x2d = array_2d_util.array_2d_native_complex_via_indexes_from(
             array_2d_slim=x,
-            sub_shape_native=self.real_space_mask.shape_native,
+            shape_native=self.real_space_mask.shape_native,
             native_index_for_slim_index_2d=self.native_index_for_slim_index,
         )[::-1, :]
 
         y = self.k2y(self.xx2k(self.x2xx(x2d)))
         return np.concatenate((y.real, y.imag), axis=0)
 
     def adjoint_lop(self, y):
@@ -301,15 +303,16 @@
         y = a_complex_from(
             a_real=y[: int(self.shape[0] / 2.0)], a_imag=y[int(self.shape[0] / 2.0) :]
         )
 
         x2d = np.real(self.xx2x(self.k2xx(self.y2k(y))))
 
         x = array_2d_util.array_2d_slim_complex_from(
-            array_2d_native=x2d[::-1, :], sub_size=1, mask=self.real_space_mask
+            array_2d_native=x2d[::-1, :],
+            mask=np.array(self.real_space_mask),
         )
         x = x.real  # NOTE:
 
         # NOTE:
         x *= self.adjoint_scaling
 
         return x
```

### Comparing `autoarray-2024.1.27.4/autoarray/operators/transformer_util.py` & `autoarray-2024.5.16.0/autoarray/operators/transformer_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/__init__.py` & `autoarray-2024.5.16.0/autoarray/plot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 )
 from autoarray.plot.wrap.two_d.voronoi_drawer import VoronoiDrawer
 from autoarray.plot.wrap.two_d.origin_scatter import OriginScatter
 from autoarray.plot.wrap.two_d.mask_scatter import MaskScatter
 from autoarray.plot.wrap.two_d.border_scatter import BorderScatter
 from autoarray.plot.wrap.two_d.positions_scatter import PositionsScatter
 from autoarray.plot.wrap.two_d.index_scatter import IndexScatter
+from autoarray.plot.wrap.two_d.index_plot import IndexPlot
 from autoarray.plot.wrap.two_d.mesh_grid_scatter import MeshGridScatter
 from autoarray.plot.wrap.two_d.parallel_overscan_plot import ParallelOverscanPlot
 from autoarray.plot.wrap.two_d.serial_prescan_plot import SerialPrescanPlot
 from autoarray.plot.wrap.two_d.serial_overscan_plot import SerialOverscanPlot
 
 from autoarray.plot.get_visuals.one_d import GetVisuals1D
 from autoarray.plot.get_visuals.two_d import GetVisuals2D
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/abstract_plotters.py` & `autoarray-2024.5.16.0/autoarray/plot/abstract_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/get_visuals/abstract.py` & `autoarray-2024.5.16.0/autoarray/plot/get_visuals/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/get_visuals/one_d.py` & `autoarray-2024.5.16.0/autoarray/plot/visuals/abstract.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,53 @@
-from autoarray.plot.get_visuals.abstract import AbstractGetVisuals
-from autoarray.plot.include.one_d import Include1D
-from autoarray.plot.visuals.one_d import Visuals1D
-from autoarray.structures.arrays.uniform_1d import Array1D
+from abc import ABC
 
 
-class GetVisuals1D(AbstractGetVisuals):
-    def __init__(self, include: Include1D, visuals: Visuals1D):
+class AbstractVisuals(ABC):
+    def __add__(self, other):
         """
-        Class which gets 1D attributes and adds them to a `Visuals1D` objects, such that they are plotted on 1D figures.
+        Adds two `Visuals` classes together.
 
-        For a visual to be extracted and added for plotting, it must have a `True` value in its corresponding entry in
-        the `Include1D` object. If this entry is `False`, the `GetVisuals1D.get` method returns a None and the attribute
-        is omitted from the plot.
-
-        The `GetVisuals1D` class adds new visuals to a pre-existing `Visuals1D` object that is passed to its `__init__`
-        method. This only adds a new entry if the visual are not already in this object.
-
-        Parameters
-        ----------
-        include
-            Sets which 1D visuals are included on the figure that is to be plotted (only entries which are `True`
-            are extracted via the `GetVisuals1D` object).
-        visuals
-            The pre-existing visuals of the plotter which new visuals are added too via the `GetVisuals1D` class.
-        """
-        super().__init__(include=include, visuals=visuals)
+        When we perform plotting, the `Include` class is used to create additional `Visuals` class from the data
+        structures that are plotted, for example:
 
-    def via_array_1d_from(self, array_1d: Array1D) -> Visuals1D:
-        """
-        From an `Array1D` get its attributes that can be plotted and return them in a `Visuals1D` object.
+        mask = Mask2D.circular(shape_native=(100, 100), pixel_scales=0.1, radius=3.0)
+        array = Array2D.ones(shape_native=(100, 100), pixel_scales=0.1)
+        masked_array = al.Array2D(values=array, mask=mask)
+        include_2d = Include2D(mask=True)
+        array_plotter = aplt.Array2DPlotter(array=masked_array, include_2d=include_2d)
+        array_plotter.figure()
+
+        Because `mask=True` in `Include2D` the function `figure` extracts the `Mask2D` from the `masked_array`
+        and plots it. It does this by creating a new `Visuals2D` object.
+
+        If the user did not manually input a `Visuals2D` object, the one created in `function_array` is the one used to
+        plot the image
 
-        Only attributes not already in `self.visuals` and with `True` entries in the `Include1D` object are extracted
-        for plotting.
+        However, if the user specifies their own `Visuals2D` object and passed it to the plotter, e.g.:
 
-        From an `Array1D` the following attributes can be extracted for plotting:
+        visuals_2d = Visuals2D(origin=(0.0, 0.0))
+        include_2d = Include2D(mask=True)
+        array_plotter = aplt.Array2DPlotter(array=masked_array, include_2d=include_2d)
 
-        - origin: the (y,x) origin of the 1D array's coordinate system.
-        - mask: the mask of the 1D array.
+        We now wish for the `Plotter` to plot the `origin` in the user's input `Visuals2D` object and the `Mask2d`
+        extracted via the `Include2D`. To achieve this, two `Visuals2D` objects are created: (i) the user's input
+        instance (with an origin) and; (ii) the one created by the `Include2D` object (with a mask).
 
-        Parameters
-        ----------
-        array
-            The 1D array whose attributes are extracted for plotting.
+        This `__add__` override means we can add the two together to make the final `Visuals2D` object that is
+        plotted on the figure containing both the `origin` and `Mask2D`.:
 
-        Returns
-        -------
-        Visuals1D
-            The collection of attributes that are plotted by a `Plotter` object.
+        visuals_2d = visuals_2d_via_user + visuals_2d_via_include
+
+        The ordering of the addition has been specifically chosen to ensure that the `visuals_2d_via_user` does not
+        retain the attributes that are added to it by the `visuals_2d_via_include`. This ensures that if multiple plots
+        are made, the same `visuals_2d_via_user` is used for every plot. If this were not the case, it would
+        permanently inherit attributes from the `Visuals` from the `Include` method and plot them on all figures.
         """
-        return self.visuals + self.visuals.__class__(
-            origin=self.get("origin", array_1d.origin),
-            mask=self.get("mask", array_1d.mask),
-        )
+
+        for attr, value in self.__dict__.items():
+            try:
+                if other.__dict__[attr] is None and self.__dict__[attr] is not None:
+                    other.__dict__[attr] = self.__dict__[attr]
+            except KeyError:
+                pass
+
+        return other
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/get_visuals/two_d.py` & `autoarray-2024.5.16.0/autoarray/plot/get_visuals/two_d.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         Returns
         -------
         Visuals2D
             The collection of attributes that are plotted by a `Plotter` object.
         """
         origin = self.origin_via_mask_from(mask=mask)
         mask_visuals = self.get("mask", mask)
-        border = self.get("border", mask.derive_grid.border_sub_1.binned)
+        border = self.get("border", mask.derive_grid.border)
 
         return self.visuals + self.visuals.__class__(
             origin=origin, mask=mask_visuals, border=border
         )
 
     def via_grid_from(self, grid: Grid2DLike) -> Visuals2D:
         """
@@ -138,15 +138,15 @@
 
         Returns
         -------
         Visuals2D
             The collection of attributes that can be plotted by a `Plotter` object.
         """
 
-        visuals_via_mask = self.via_mask_from(mask=mapper.source_plane_data_grid.mask)
+        visuals_via_mask = self.via_mask_from(mask=mapper.mapper_grids.mask)
 
         mesh_grid = self.get(
             "mesh_grid", mapper.image_plane_mesh_grid, "mapper_image_plane_mesh_grid"
         )
 
         return (
             self.visuals
@@ -187,15 +187,22 @@
             "origin", Grid2DIrregular(values=[mapper.source_plane_mesh_grid.origin])
         )
 
         grid = self.get(
             "grid", mapper.source_plane_data_grid, "mapper_source_plane_data_grid"
         )
 
-        border = self.get("border", mapper.source_plane_data_grid.sub_border_grid)
+        try:
+            border_grid = mapper.mapper_grids.source_plane_data_grid[
+                mapper.border_relocator.sub_border_slim
+            ]
+            border = self.get("border", border_grid)
+
+        except AttributeError:
+            border = None
 
         mesh_grid = self.get(
             "mesh_grid", mapper.source_plane_mesh_grid, "mapper_source_plane_mesh_grid"
         )
 
         return self.visuals + self.visuals.__class__(
             origin=origin, grid=grid, border=border, mesh_grid=mesh_grid
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/include/abstract.py` & `autoarray-2024.5.16.0/autoarray/plot/include/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/include/one_d.py` & `autoarray-2024.5.16.0/autoarray/plot/include/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/include/two_d.py` & `autoarray-2024.5.16.0/autoarray/plot/include/two_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/mat_plot/abstract.py` & `autoarray-2024.5.16.0/autoarray/plot/mat_plot/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,19 @@
 
         self.units = units or wb.Units(is_default=True)
         self.figure = figure or wb.Figure(is_default=True)
         self.axis = axis or wb.Axis(is_default=True)
 
         self.cmap = cmap or wb.Cmap(is_default=True)
 
-        self.colorbar = colorbar or wb.Colorbar(is_default=True)
+        if colorbar is not False:
+            self.colorbar = colorbar or wb.Colorbar(is_default=True)
+        else:
+            self.colorbar = False
+
         self.colorbar_tickparams = colorbar_tickparams or wb.ColorbarTickParams(
             is_default=True
         )
 
         self.tickparams = tickparams or wb.TickParams(is_default=True)
         self.yticks = yticks or wb.YTicks(is_default=True)
         self.xticks = xticks or wb.XTicks(is_default=True)
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/mat_plot/one_d.py` & `autoarray-2024.5.16.0/autoarray/plot/mat_plot/one_d.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
         visuals_1d: Visuals1D,
         auto_labels: AutoLabels,
         x: Optional[Union[np.ndarray, Iterable, List, Array1D]] = None,
         plot_axis_type_override: Optional[str] = None,
         y_errors=None,
         x_errors=None,
         y_extra=None,
+        y_extra_2=None,
         ls_errorbar="",
         should_plot_grid=False,
         should_plot_zero=False,
         text_manual_dict=None,
         text_manual_dict_y=None,
         bypass: bool = False,
     ):
@@ -200,14 +201,15 @@
             y=y,
             x=x,
             label=label,
             plot_axis_type=plot_axis_type,
             y_errors=y_errors,
             x_errors=x_errors,
             y_extra=y_extra,
+            y_extra_2=y_extra_2,
             ls_errorbar=ls_errorbar,
         )
 
         if should_plot_zero:
             plt.plot(x, 1.0e-6 * np.ones(shape=y.shape), c="b", ls="--")
 
         if should_plot_grid:
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/mat_plot/two_d.py` & `autoarray-2024.5.16.0/autoarray/plot/mat_plot/two_d.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         interpolated_reconstruction: Optional[w2d.InterpolatedReconstruction] = None,
         voronoi_drawer: Optional[w2d.VoronoiDrawer] = None,
         origin_scatter: Optional[w2d.OriginScatter] = None,
         mask_scatter: Optional[w2d.MaskScatter] = None,
         border_scatter: Optional[w2d.BorderScatter] = None,
         positions_scatter: Optional[w2d.PositionsScatter] = None,
         index_scatter: Optional[w2d.IndexScatter] = None,
+        index_plot: Optional[w2d.IndexPlot] = None,
         mesh_grid_scatter: Optional[w2d.MeshGridScatter] = None,
         parallel_overscan_plot: Optional[w2d.ParallelOverscanPlot] = None,
         serial_prescan_plot: Optional[w2d.SerialPrescanPlot] = None,
         serial_overscan_plot: Optional[w2d.SerialOverscanPlot] = None,
         use_log10: bool = False,
     ):
         """
@@ -192,14 +193,15 @@
         self.origin_scatter = origin_scatter or w2d.OriginScatter(is_default=True)
         self.mask_scatter = mask_scatter or w2d.MaskScatter(is_default=True)
         self.border_scatter = border_scatter or w2d.BorderScatter(is_default=True)
         self.positions_scatter = positions_scatter or w2d.PositionsScatter(
             is_default=True
         )
         self.index_scatter = index_scatter or w2d.IndexScatter(is_default=True)
+        self.index_plot = index_plot or w2d.IndexPlot(is_default=True)
         self.mesh_grid_scatter = mesh_grid_scatter or w2d.MeshGridScatter(
             is_default=True
         )
 
         self.parallel_overscan_plot = (
             parallel_overscan_plot or w2d.ParallelOverscanPlot(is_default=True)
         )
@@ -215,14 +217,15 @@
         self.is_for_subplot = False
 
     def plot_array(
         self,
         array: Array2D,
         visuals_2d: Visuals2D,
         auto_labels: AutoLabels,
+        grid_indexes=None,
         bypass: bool = False,
     ):
         """
         Plot an `Array2D` data structure as a figure using the matplotlib wrapper objects and tools.
 
         This `Array2D` is plotted using `plt.imshow`.
 
@@ -244,16 +247,14 @@
 
         if array.pixel_scales is None and self.units.use_scaled:
             raise exc.ArrayException(
                 "You cannot plot an array using its scaled unit_label if the input array does not have "
                 "a pixel scales attribute."
             )
 
-        array = array.binned
-
         # Hack being used for BELLSABSORB with Tania, remove later and code up automatic method to make it
         # so that if a mask is irregular and zooming in creates white edges, that instead it doesnt have the eddge.
         # This could just be a matplotlib settings to change the edge color?
 
         #        array = array.resized_from(new_shape=(401, 401))
 
         if array.mask.is_all_false:
@@ -286,20 +287,21 @@
         if not self.is_for_subplot:
             fig, ax = self.figure.open()
         else:
             if not bypass:
                 ax = self.setup_subplot()
 
         aspect = self.figure.aspect_from(shape_native=array.shape_native)
+
         norm = self.cmap.norm_from(array=array, use_log10=self.use_log10)
 
         origin = conf.instance["visualize"]["general"]["general"]["imshow_origin"]
 
         plt.imshow(
-            X=array.native,
+            X=array.native.array,
             aspect=aspect,
             cmap=self.cmap.cmap,
             norm=norm,
             extent=extent,
             origin=origin,
         )
 
@@ -357,20 +359,17 @@
 
         if self.contour is not False:
             try:
                 self.contour.set(array=array, extent=extent, use_log10=self.use_log10)
             except ValueError:
                 pass
 
-        grid_indexes = None
-
-        if visuals_2d.indexes is not None or visuals_2d.pix_indexes is not None:
-            grid_indexes = array.mask.derive_grid.unmasked
-
-        visuals_2d.plot_via_plotter(plotter=self, grid_indexes=grid_indexes)
+        visuals_2d.plot_via_plotter(
+            plotter=self, grid_indexes=grid_indexes, geometry=array.geometry
+        )
 
         if not self.is_for_subplot and not bypass:
             self.output.to_figure(structure=array, auto_filename=auto_labels.filename)
             self.figure.close()
 
     def plot_grid(
         self,
@@ -458,15 +457,17 @@
         if not self.axis.symmetric_around_centre:
             self.yticks.set(min_value=extent[2], max_value=extent[3], units=self.units)
             self.xticks.set(min_value=extent[0], max_value=extent[1], units=self.units)
 
         if self.contour is not False:
             self.contour.set(array=color_array, extent=extent, use_log10=self.use_log10)
 
-        visuals_2d.plot_via_plotter(plotter=self, grid_indexes=grid)
+        visuals_2d.plot_via_plotter(
+            plotter=self, grid_indexes=grid, geometry=grid.geometry
+        )
 
         if not self.is_for_subplot:
             self.output.to_figure(structure=grid, auto_filename=auto_labels.filename)
             self.figure.close()
 
     def plot_mapper(
         self,
@@ -515,20 +516,18 @@
     ):
         if pixel_values is not None:
             solution_array_2d = array_2d_util.array_2d_native_from(
                 array_2d_slim=pixel_values,
                 mask_2d=np.full(
                     fill_value=False, shape=mapper.source_plane_mesh_grid.shape_native
                 ),
-                sub_size=1,
             )
 
             pixel_values = Array2D.no_mask(
                 values=solution_array_2d,
-                sub_size=1,
                 pixel_scales=mapper.source_plane_mesh_grid.pixel_scales,
                 origin=mapper.source_plane_mesh_grid.origin,
             )
 
         extent = self.axis.config_dict.get("extent")
         if extent is None:
             extent = mapper.extent_from(
@@ -572,15 +571,18 @@
 
         self.title.set(auto_title=auto_labels.title)
         self.tickparams.set()
         self.ylabel.set()
         self.xlabel.set()
 
         visuals_2d.plot_via_plotter(
-            plotter=self, grid_indexes=mapper.source_plane_data_grid, mapper=mapper
+            plotter=self,
+            grid_indexes=mapper.source_plane_data_grid,
+            mapper=mapper,
+            geometry=mapper.mapper_grids.mask.geometry,
         )
 
         if not self.is_for_subplot:
             self.output.to_figure(structure=None, auto_filename=auto_labels.filename)
             self.figure.close()
 
     def _plot_delaunay_mapper(
@@ -634,15 +636,18 @@
         )
 
         self.title.set(auto_title=auto_labels.title)
         self.ylabel.set()
         self.xlabel.set()
 
         visuals_2d.plot_via_plotter(
-            plotter=self, grid_indexes=mapper.source_plane_data_grid, mapper=mapper
+            plotter=self,
+            grid_indexes=mapper.source_plane_data_grid,
+            mapper=mapper,
+            geometry=mapper.mapper_grids.mask.geometry,
         )
 
         if not self.is_for_subplot:
             self.output.to_figure(
                 structure=interpolation_array, auto_filename=auto_labels.filename
             )
             self.figure.close()
@@ -714,15 +719,18 @@
             )
 
         self.title.set(auto_title=auto_labels.title)
         self.ylabel.set()
         self.xlabel.set()
 
         visuals_2d.plot_via_plotter(
-            plotter=self, grid_indexes=mapper.source_plane_data_grid, mapper=mapper
+            plotter=self,
+            grid_indexes=mapper.source_plane_data_grid,
+            mapper=mapper,
+            geometry=mapper.mapper_grids.mask.geometry,
         )
 
         if pixel_values is not None:
             interpolation_array = mapper.interpolated_array_from(values=pixel_values)
         else:
             interpolation_array = None
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/multi_plotters.py` & `autoarray-2024.5.16.0/autoarray/plot/multi_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/visuals/one_d.py` & `autoarray-2024.5.16.0/autoarray/plot/visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/visuals/two_d.py` & `autoarray-2024.5.16.0/autoarray/plot/visuals/two_d.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         patches: Optional[List[ptch.Patch]] = None,
         array_overlay: Optional[Array2D] = None,
         parallel_overscan=None,
         serial_prescan=None,
         serial_overscan=None,
         indexes=None,
         pix_indexes=None,
+        indexes_via_scatter=False,
     ):
         self.origin = origin
         self.mask = mask
         self.border = border
         self.lines = lines
         self.positions = positions
         self.grid = grid
@@ -40,25 +41,24 @@
         self.patches = patches
         self.array_overlay = array_overlay
         self.parallel_overscan = parallel_overscan
         self.serial_prescan = serial_prescan
         self.serial_overscan = serial_overscan
         self.indexes = indexes
         self.pix_indexes = pix_indexes
+        self.indexes_via_scatter = indexes_via_scatter
 
-    def plot_via_plotter(self, plotter, grid_indexes=None, mapper=None):
+    def plot_via_plotter(self, plotter, grid_indexes=None, mapper=None, geometry=None):
         if self.origin is not None:
             plotter.origin_scatter.scatter_grid(
                 grid=Grid2DIrregular(values=self.origin)
             )
 
         if self.mask is not None:
-            plotter.mask_scatter.scatter_grid(
-                grid=self.mask.derive_grid.edge_sub_1.binned
-            )
+            plotter.mask_scatter.scatter_grid(grid=self.mask.derive_grid.edge)
 
         if self.border is not None:
             plotter.border_scatter.scatter_grid(grid=self.border)
 
         if self.grid is not None:
             plotter.grid_scatter.scatter_grid(grid=self.grid)
 
@@ -73,18 +73,33 @@
 
         if self.patches is not None:
             plotter.patch_overlay.overlay_patches(patches=self.patches)
 
         if self.lines is not None:
             plotter.grid_plot.plot_grid(grid=self.lines)
 
-        if self.indexes is not None:
-            plotter.index_scatter.scatter_grid_indexes(
-                grid=grid_indexes, indexes=self.indexes
-            )
+        if self.indexes is not None and grid_indexes is not None:
+            if not self.indexes_via_scatter:
+                plotter.index_plot.plot_grid_indexes_multi(
+                    grid=grid_indexes, indexes=self.indexes, geometry=geometry
+                )
+
+            else:
+                plotter.index_scatter.scatter_grid_indexes(
+                    grid=grid_indexes,
+                    indexes=self.indexes,
+                )
 
         if self.pix_indexes is not None and mapper is not None:
             indexes = mapper.pix_indexes_for_slim_indexes(pix_indexes=self.pix_indexes)
 
-            plotter.index_scatter.scatter_grid_indexes(
-                grid=mapper.source_plane_data_grid, indexes=indexes
-            )
+            if not self.indexes_via_scatter:
+                plotter.index_plot.plot_grid_indexes_x1(
+                    grid=grid_indexes,
+                    indexes=indexes,
+                )
+
+            else:
+                plotter.index_scatter.scatter_grid_indexes(
+                    grid=mapper.source_plane_data_grid,
+                    indexes=indexes,
+                )
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/__init__.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,11 +30,12 @@
 )
 from autoarray.plot.wrap.two_d.voronoi_drawer import VoronoiDrawer
 from autoarray.plot.wrap.two_d.origin_scatter import OriginScatter
 from autoarray.plot.wrap.two_d.mask_scatter import MaskScatter
 from autoarray.plot.wrap.two_d.border_scatter import BorderScatter
 from autoarray.plot.wrap.two_d.positions_scatter import PositionsScatter
 from autoarray.plot.wrap.two_d.index_scatter import IndexScatter
+from autoarray.plot.wrap.two_d.index_plot import IndexPlot
 from autoarray.plot.wrap.two_d.mesh_grid_scatter import MeshGridScatter
 from autoarray.plot.wrap.two_d.parallel_overscan_plot import ParallelOverscanPlot
 from autoarray.plot.wrap.two_d.serial_prescan_plot import SerialPrescanPlot
 from autoarray.plot.wrap.two_d.serial_overscan_plot import SerialOverscanPlot
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/annotate.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/annotate.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/axis.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/axis.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/cmap.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/cmap.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,39 +44,29 @@
         cmap = copy.copy(self)
 
         cmap._symmetric = True
         cmap.symmetric_value = symmetric_value
 
         return cmap
 
-    def vmin_from(self, array: np.ndarray):
-        if self.config_dict["vmin"] is None:
-            return np.nanmin(array)
-        return self.config_dict["vmin"]
-
-    def vmax_from(self, array: np.ndarray):
-        if self.config_dict["vmax"] is None:
-            return np.nanmax(array)
-        return self.config_dict["vmax"]
-
     def norm_from(self, array: np.ndarray, use_log10: bool = False) -> object:
         """
         Returns the `Normalization` object which scales of the colormap.
 
         If vmin / vmax are not manually input by the user, the minimum / maximum values of the data being plotted
         are used.
 
         Parameters
         ----------
         array
             The array of data which is to be plotted.
         """
 
-        vmin = self.vmin_from(array=array)
-        vmax = self.vmax_from(array=array)
+        vmin = self.vmin_from(array=array, use_log10=use_log10)
+        vmax = self.vmax_from(array=array, use_log10=use_log10)
 
         if self._symmetric:
             if vmin < 0.0 and vmax > 0.0:
                 if self.symmetric_value is None:
                     if abs(vmin) > abs(vmax):
                         vmax = abs(vmin)
                     else:
@@ -85,16 +75,14 @@
                     vmin = -self.symmetric_value
                     vmax = self.symmetric_value
 
         if isinstance(self.config_dict["norm"], colors.Normalize):
             return self.config_dict["norm"]
 
         if self.config_dict["norm"] in "log" or use_log10:
-            if vmin < self.log10_min_value:
-                vmin = self.log10_min_value
             return colors.LogNorm(vmin=vmin, vmax=vmax)
         elif self.config_dict["norm"] in "linear":
             return colors.Normalize(vmin=vmin, vmax=vmax)
         elif self.config_dict["norm"] in "symmetric_log":
             return colors.SymLogNorm(
                 vmin=vmin,
                 vmax=vmax,
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/colorbar.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/colorbar.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/figure.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/figure.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/label.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/label.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/legend.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/legend.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/output.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/output.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 import matplotlib.pyplot as plt
 from os import path
 import os
 from typing import Union, List, Optional
 
 from autoarray.structures.abstract_structure import Structure
 
+logger = logging.getLogger(__name__)
+
 
 class Output:
     def __init__(
         self,
         path: Optional[str] = None,
         filename: Optional[str] = None,
         prefix: Optional[str] = None,
@@ -93,14 +96,29 @@
             filename = f"{self.prefix}{filename}"
 
         if self.suffix is not None:
             filename = f"{filename}{self.suffix}"
 
         return filename
 
+    def savefig(self, filename: str, output_path: str, format: str):
+        try:
+            plt.savefig(
+                path.join(output_path, f"{filename}.{format}"),
+                bbox_inches=self.bbox_inches,
+            )
+        except ValueError as e:
+            logger.info(
+                f"""
+                Failed to output figure as a .{format} or .fits due to the following error:
+
+                {e}
+            """
+            )
+
     def to_figure(
         self, structure: Optional[Structure], auto_filename: Optional[str] = None
     ):
         """
         Output the figure, by either displaying it on the user's screen or to the hard-disk as a .png or .fits file.
 
         Parameters
@@ -121,24 +139,16 @@
 
             if not self.bypass:
                 if os.environ.get("PYAUTOARRAY_OUTPUT_MODE") == "1":
                     return self.to_figure_output_mode(filename=filename)
 
                 if format == "show":
                     plt.show()
-                elif format == "png":
-                    plt.savefig(
-                        path.join(output_path, f"{filename}.png"),
-                        bbox_inches=self.bbox_inches,
-                    )
-                elif format == "pdf":
-                    plt.savefig(
-                        path.join(output_path, f"{filename}.pdf"),
-                        bbox_inches=self.bbox_inches,
-                    )
+                elif format == "png" or format == "pdf":
+                    self.savefig(filename, output_path, format)
                 elif format == "fits":
                     if structure is not None:
                         structure.output_to_fits(
                             file_path=path.join(output_path, f"{filename}.fits"),
                             overwrite=True,
                         )
 
@@ -161,24 +171,16 @@
                 os.makedirs(output_path, exist_ok=True)
 
             if os.environ.get("PYAUTOARRAY_OUTPUT_MODE") == "1":
                 return self.to_figure_output_mode(filename=filename)
 
             if format == "show":
                 plt.show()
-            elif format == "png":
-                plt.savefig(
-                    path.join(output_path, f"{filename}.png"),
-                    bbox_inches=self.bbox_inches,
-                )
-            elif format == "pdf":
-                plt.savefig(
-                    path.join(output_path, f"{filename}.pdf"),
-                    bbox_inches=self.bbox_inches,
-                )
+            elif format == "png" or format == "pdf":
+                self.savefig(filename, output_path, format)
 
     def to_figure_output_mode(self, filename: str):
         global COUNT
 
         try:
             COUNT += 1
         except NameError:
@@ -187,11 +189,8 @@
         import sys
 
         script_name = path.split(sys.argv[0])[-1].replace(".py", "")
 
         output_path = path.join(os.getcwd(), "output_mode", script_name)
         os.makedirs(output_path, exist_ok=True)
 
-        plt.savefig(
-            path.join(output_path, f"{COUNT}_{filename}.png"),
-            bbox_inches=self.bbox_inches,
-        )
+        self.savefig(f"{COUNT}_{filename}", output_path, "png")
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/text.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/text.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/tickparams.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/tickparams.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/ticks.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/ticks.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/title.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/title.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/base/units.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/base/units.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/abstract.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/avxline.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/avxline.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/fill_between.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/fill_between.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/yx_plot.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/yx_plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         y: Union[np.ndarray, Array1D],
         x: Union[np.ndarray, Array1D],
         label: str = None,
         plot_axis_type=None,
         y_errors=None,
         x_errors=None,
         y_extra=None,
+        y_extra_2=None,
         ls_errorbar="",
     ):
         """
         Plots 1D y-data against 1D x-data using the matplotlib method `plt.plot`, `plt.semilogy`, `plt.loglog`,
         or `plt.scatter`.
 
         Parameters
@@ -83,7 +84,10 @@
 
         if y_extra is not None:
             if isinstance(y_extra, list):
                 for y_extra_ in y_extra:
                     plt.plot(x, y_extra_)
             else:
                 plt.plot(x, y_extra, c="r")
+
+        if y_extra_2 is not None:
+            plt.plot(x, y_extra_2, c="r")
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/one_d/yx_scatter.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/one_d/yx_scatter.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/segmentdata.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/segmentdata.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/__init__.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,11 +10,12 @@
 )
 from .voronoi_drawer import VoronoiDrawer
 from .origin_scatter import OriginScatter
 from .mask_scatter import MaskScatter
 from .border_scatter import BorderScatter
 from .positions_scatter import PositionsScatter
 from .index_scatter import IndexScatter
+from .index_plot import IndexPlot
 from .mesh_grid_scatter import MeshGridScatter
 from .parallel_overscan_plot import ParallelOverscanPlot
 from .serial_prescan_plot import SerialPrescanPlot
 from .serial_overscan_plot import SerialOverscanPlot
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/abstract.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/array_overlay.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/array_overlay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/contour.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/contour.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/grid_errorbar.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/grid_errorbar.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,20 @@
     Parameters
     ----------
     colors : [str]
         The color or list of colors that the grid is plotted using. For plotting indexes or a grid list, a
         list of colors can be specified which the plot cycles through.
     """
 
+    def config_dict_remove_marker(self, config_dict):
+        if config_dict.get("fmt") and config_dict.get("marker"):
+            config_dict.pop("marker")
+
+        return config_dict
+
     def errorbar_grid(
         self,
         grid: Union[np.ndarray, Grid2D],
         y_errors: Optional[Union[np.ndarray, List]] = None,
         x_errors: Optional[Union[np.ndarray, List]] = None,
     ):
         """
@@ -47,14 +53,16 @@
         """
 
         config_dict = self.config_dict
 
         if len(config_dict["c"]) > 1:
             config_dict["c"] = config_dict["c"][0]
 
+        config_dict = self.config_dict_remove_marker(config_dict=config_dict)
+
         try:
             plt.errorbar(
                 y=grid[:, 0], x=grid[:, 1], yerr=y_errors, xerr=x_errors, **config_dict
             )
         except (IndexError, TypeError):
             return self.errorbar_grid_list(grid_list=grid)
 
@@ -80,14 +88,16 @@
         if len(grid_list) == 0:
             return
 
         color = itertools.cycle(self.config_dict["c"])
         config_dict = self.config_dict
         config_dict.pop("c")
 
+        config_dict = self.config_dict_remove_marker(config_dict=config_dict)
+
         try:
             for grid in grid_list:
                 plt.errorbar(
                     y=grid[:, 0],
                     x=grid[:, 1],
                     yerr=np.asarray(y_errors),
                     xerr=np.asarray(x_errors),
@@ -121,15 +131,17 @@
         """
 
         config_dict = self.config_dict
         config_dict.pop("c")
 
         plt.scatter(y=grid[:, 0], x=grid[:, 1], c=color_array, cmap=cmap)
 
+        config_dict = self.config_dict_remove_marker(config_dict=self.config_dict)
+
         plt.errorbar(
             y=grid[:, 0],
             x=grid[:, 1],
             yerr=np.asarray(y_errors),
             xerr=np.asarray(x_errors),
             zorder=0.0,
-            **self.config_dict,
+            **config_dict,
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/grid_plot.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/grid_plot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import itertools
 from typing import List, Union, Tuple
 
+from autoarray.geometry.geometry_2d import Geometry2D
+from autoarray.operators.contour import Grid2DContour
 from autoarray.plot.wrap.two_d.abstract import AbstractMatWrap2D
 from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 
 
 class GridPlot(AbstractMatWrap2D):
     """
@@ -97,7 +99,63 @@
         config_dict.pop("c")
 
         try:
             for grid in grid_list:
                 plt.plot(grid[:, 1], grid[:, 0], c=next(color), **config_dict)
         except IndexError:
             pass
+
+    def plot_grid_indexes_x1(
+        self,
+        grid: Union[np.ndarray, Grid2D, Grid2DIrregular],
+        indexes: np.ndarray,
+    ):
+        color = itertools.cycle(self.config_dict["c"])
+        config_dict = self.config_dict
+        config_dict.pop("c")
+
+        if isinstance(indexes[0], int):
+            indexes = [indexes]
+
+        for index_list in indexes:
+            grid_contour = Grid2DContour(
+                grid=grid[index_list, :],
+                pixel_scales=None,
+                shape_native=None,
+            )
+
+            grid_hull = grid_contour.hull
+
+            if grid_hull is not None:
+                plt.plot(
+                    grid_hull[:, 1], grid_hull[:, 0], color=next(color), **config_dict
+                )
+
+    def plot_grid_indexes_multi(
+        self,
+        grid: Union[np.ndarray, Grid2D, Grid2DIrregular],
+        indexes: np.ndarray,
+        geometry: Geometry2D,
+    ):
+        color = itertools.cycle(self.config_dict["c"])
+        config_dict = self.config_dict
+        config_dict.pop("c")
+
+        if isinstance(indexes[0], int):
+            indexes = [indexes]
+
+        for index_list in indexes:
+            grid_in = grid[index_list, :]
+
+            if isinstance(index_list[0], tuple):
+                grid_in = grid_in[0]
+
+            grid_contour = Grid2DContour(
+                grid=grid_in,
+                pixel_scales=geometry.pixel_scales,
+                shape_native=geometry.shape_native,
+            )
+
+            color_plot = next(color)
+
+            for contour in grid_contour.contour_list:
+                plt.plot(contour[:, 1], contour[:, 0], color=color_plot, **config_dict)
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/grid_scatter.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/grid_scatter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import itertools
+from scipy.spatial import ConvexHull
 from typing import List, Union
 
+
 from autoarray.plot.wrap.two_d.abstract import AbstractMatWrap2D
 from autoarray.structures.grids.uniform_2d import Grid2D
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 
-from autoarray import exc
-
 
 class GridScatter(AbstractMatWrap2D):
     """
     Scatters an input set of grid points, for example (y,x) coordinates or data structures representing 2D (y,x)
     coordinates like a `Grid2D` or `Grid2DIrregular`. List of (y,x) coordinates are plotted with varying colors.
 
     This object wraps the following Matplotlib methods:
@@ -20,16 +20,16 @@
     - plt.scatter: https://matplotlib.org/3.1.1/api/_as_gen/matplotlib.pyplot.scatter.html
 
     There are a number of children of this method in the `mat_obj.py` module that plot specific sets of (y,x)
     points. Each of these objects uses uses their own config file and settings so that each has a unique appearance
     on every figure:
 
     - `OriginScatter`: plots the (y,x) coordinates of the origin of a data structure (e.g. as a black cross).
-    - `MaskScatter`: plots a mask over an image, using the `Mask2d` object's (y,x)  `edge_sub_1` property.
-    - `BorderScatter: plots a border over an image, using the `Mask2d` object's (y,x) `border_sub_1` property.
+    - `MaskScatter`: plots a mask over an image, using the `Mask2d` object's (y,x)  `edge` property.
+    - `BorderScatter: plots a border over an image, using the `Mask2d` object's (y,x) `border` property.
     - `PositionsScatter`: plots the (y,x) coordinates that are input in a plotter via the `positions` input.
     - `IndexScatter`: plots specific (y,x) coordinates of a grid (or grids) via their 1d or 2d indexes.
     - `MeshGridScatter`: plots the grid of a `Mesh` object (see `autoarray.inversion`).
 
     Parameters
     ----------
     colors : [str]
@@ -104,70 +104,35 @@
 
         config_dict = self.config_dict
         config_dict.pop("c")
 
         plt.scatter(y=grid[:, 0], x=grid[:, 1], c=color_array, cmap=cmap, **config_dict)
 
     def scatter_grid_indexes(
-        self, grid: Union[np.ndarray, Grid2D], indexes: np.ndarray
+        self,
+        grid: Union[np.ndarray, Grid2D, Grid2DIrregular],
+        indexes: np.ndarray,
     ):
         """
         Plot specific points of an input grid of (y,x) coordinates, which are specified according to the 1D or 2D
         indexes of the `Grid2D`.
 
         This method allows us to color in points on grids that map between one another.
 
         Parameters
         ----------
         grid : Grid2D
             The grid of (y,x) coordinates that is plotted.
         indexes
             The 1D indexes of the grid that are colored in when plotted.
         """
-        if not isinstance(grid, np.ndarray):
-            raise exc.PlottingException(
-                "The grid passed into scatter_grid_indexes is not a ndarray and thus its"
-                "1D indexes cannot be marked and plotted."
-            )
-
-        if len(grid.shape) != 2:
-            raise exc.PlottingException(
-                "The grid passed into scatter_grid_indexes is not 2D (e.g. a flattened 1D"
-                "grid) and thus its 1D indexes cannot be marked."
-            )
-
-        if isinstance(indexes, list):
-            if not any(isinstance(i, list) for i in indexes):
-                indexes = [indexes]
-
         color = itertools.cycle(self.config_dict["c"])
         config_dict = self.config_dict
         config_dict.pop("c")
 
         for index_list in indexes:
-            if all([isinstance(index, float) for index in index_list]) or all(
-                [isinstance(index, int) for index in index_list]
-            ):
-                plt.scatter(
-                    y=grid[index_list, 0],
-                    x=grid[index_list, 1],
-                    color=next(color),
-                    **config_dict,
-                )
-
-            elif all([isinstance(index, tuple) for index in index_list]) or all(
-                [isinstance(index, list) for index in index_list]
-            ):
-                ys, xs = map(list, zip(*index_list))
-
-                plt.scatter(
-                    y=grid.native[ys, xs, 0],
-                    x=grid.native[ys, xs, 1],
-                    color=next(color),
-                    **config_dict,
-                )
-
-            else:
-                raise exc.PlottingException(
-                    "The indexes input into the grid_scatter_index method do not conform to a "
-                    "useable type"
-                )
+            plt.scatter(
+                y=grid[index_list, 0],
+                x=grid[index_list, 1],
+                color=next(color),
+                **config_dict,
+            )
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/interpolated_reconstruction.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/interpolated_reconstruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,16 @@
         if pixel_values is None:
             return
 
         interpolation_array = mapper.interpolated_array_from(values=pixel_values)
 
         norm = cmap.norm_from(array=interpolation_array, use_log10=use_log10)
 
-        vmin = cmap.vmin_from(array=pixel_values)
-        vmax = cmap.vmax_from(array=pixel_values)
+        vmin = cmap.vmin_from(array=pixel_values, use_log10=use_log10)
+        vmax = cmap.vmax_from(array=pixel_values, use_log10=use_log10)
 
         color_values = np.where(pixel_values > vmax, vmax, pixel_values)
         color_values = np.where(pixel_values < vmin, vmin, color_values)
 
         cmap = plt.get_cmap(cmap.cmap)
 
         if colorbar is not None:
```

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/patch_overlay.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/patch_overlay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/vector_yx_quiver.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/vector_yx_quiver.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/plot/wrap/two_d/voronoi_drawer.py` & `autoarray-2024.5.16.0/autoarray/plot/wrap/two_d/voronoi_drawer.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,16 +63,16 @@
         if pixel_values is not None:
             norm = cmap.norm_from(array=pixel_values, use_log10=use_log10)
 
             if use_log10:
                 pixel_values[pixel_values < 1e-4] = 1e-4
                 pixel_values = np.log10(pixel_values)
 
-            vmin = cmap.vmin_from(array=pixel_values)
-            vmax = cmap.vmax_from(array=pixel_values)
+            vmin = cmap.vmin_from(array=pixel_values, use_log10=use_log10)
+            vmax = cmap.vmax_from(array=pixel_values, use_log10=use_log10)
 
             color_values = np.where(pixel_values > vmax, vmax, pixel_values)
             color_values = np.where(pixel_values < vmin, vmin, color_values)
 
             if vmax != vmin:
                 color_array = (color_values - vmin) / (vmax - vmin)
             else:
```

### Comparing `autoarray-2024.1.27.4/autoarray/preloads.py` & `autoarray-2024.5.16.0/autoarray/preloads.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import numpy as np
 import os
 from typing import List
 
 from autoconf import conf
 
-from autoarray.inversion.inversion.imaging.abstract import AbstractInversionImaging
 from autoarray.inversion.linear_obj.func_list import AbstractLinearObjFuncList
 from autoarray.inversion.pixelization.mappers.abstract import AbstractMapper
 
 from autoarray import exc
 from autoarray.inversion.inversion.imaging import inversion_imaging_util
 
 logger = logging.getLogger(__name__)
@@ -97,17 +96,19 @@
             from autoarray.dataset.imaging.w_tilde import WTildeImaging
 
             (
                 preload,
                 indexes,
                 lengths,
             ) = inversion_imaging_util.w_tilde_curvature_preload_imaging_from(
-                noise_map_native=fit_0.noise_map.native,
-                kernel_native=fit_0.dataset.psf.native,
-                native_index_for_slim_index=fit_0.dataset.mask.derive_indexes.native_for_slim,
+                noise_map_native=np.array(fit_0.noise_map.native),
+                kernel_native=np.array(fit_0.dataset.psf.native),
+                native_index_for_slim_index=np.array(
+                    fit_0.dataset.mask.derive_indexes.native_for_slim
+                ),
             )
 
             self.w_tilde = WTildeImaging(
                 curvature_preload=preload,
                 indexes=indexes.astype("int"),
                 lengths=lengths.astype("int"),
                 noise_map_value=fit_0.noise_map[0],
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/abstract_structure.py` & `autoarray-2024.5.16.0/autoarray/structures/abstract_structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 from abc import ABC
 from abc import abstractmethod
-import numpy as np
-from typing import TYPE_CHECKING, Dict, List, Tuple, Union
+from typing import TYPE_CHECKING, Dict, Tuple, Union
 
 if TYPE_CHECKING:
     from autoarray.structures.grids.uniform_1d import Grid1D
     from autoarray.structures.grids.uniform_2d import Grid2D
 
 from autoarray.abstract_ndarray import AbstractNDArray
 from autoarray.mask.derive.grid_2d import DeriveGrid2D
@@ -45,26 +44,18 @@
         return self.mask.derive_mask
 
     @property
     def shape_slim(self) -> int:
         return self.mask.shape_slim
 
     @property
-    def sub_shape_slim(self) -> int:
-        return self.mask.sub_shape_slim
-
-    @property
     def shape_native(self) -> Tuple[int, ...]:
         return self.mask.shape
 
     @property
-    def sub_shape_native(self) -> Tuple[int, ...]:
-        return self.mask.sub_shape_native
-
-    @property
     def pixel_scales(self) -> Tuple[float, ...]:
         return self.mask.pixel_scales
 
     @property
     def pixel_scale(self) -> float:
         return self.mask.pixel_scale
 
@@ -84,30 +75,20 @@
         return self.total_pixels * self.pixel_area
 
     @property
     def origin(self) -> Tuple[int, ...]:
         return self.mask.origin
 
     @property
-    def sub_size(self) -> int:
-        return self.mask.sub_size
-
-    @property
     def unmasked_grid(self) -> Union[Grid1D, Grid2D]:
-        return self.mask.derive_grid.all_false_sub_1
+        return self.mask.derive_grid.all_false
 
     @property
     def total_pixels(self) -> int:
         return self.shape[0]
 
-    def structure_2d_list_from(self, result_list: list) -> List["Structure"]:
-        raise NotImplementedError
-
-    def structure_2d_from(self, result: np.ndarray) -> "Structure":
-        raise NotImplementedError
-
     def trimmed_after_convolution_from(self, kernel_shape) -> "Structure":
         raise NotImplementedError
 
     @property
     def hdu_for_output(self):
         raise NotImplementedError
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/arrays/array_1d_util.py` & `autoarray-2024.5.16.0/autoarray/structures/arrays/array_1d_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """
     The `manual` classmethods in the `Array2D` object take as input a list or ndarray which is returned as an
     Array2D.
 
     This function performs the following and checks and conversions on the input:
 
     1) If the input is a list, convert it to an ndarray.
-    2) Check that the number of sub-pixels in the array is identical to that of the mask.
+    2) Check that the number of pixels in the array is identical to that of the mask.
     3) Map the input ndarray to its `slim` representation.
 
     For an Array2D, `slim` refers to a 1D NumPy array of shape [total_values] and `native` a 2D NumPy array of shape
     [total_y_values, total_values].
 
     Parameters
     ----------
@@ -40,152 +40,151 @@
     store_native
         If True, the ndarray is stored in its native format [total_y_pixels, total_x_pixels]. This avoids
         mapping large data arrays to and from the slim / native formats, which can be a computational bottleneck.
     """
 
     array_1d = array_2d_util.convert_array(array=array_1d)
 
-    is_native = array_1d.shape[0] == mask_1d.sub_shape_native[0]
+    is_native = array_1d.shape[0] == mask_1d.shape_native[0]
 
     if is_native == store_native:
         return array_1d
     elif not store_native:
         return array_1d_slim_from(
-            array_1d_native=array_1d, mask_1d=mask_1d, sub_size=mask_1d.sub_size
+            array_1d_native=np.array(array_1d),
+            mask_1d=np.array(mask_1d),
         )
 
     return array_1d_native_from(
-        array_1d_slim=array_1d, mask_1d=mask_1d, sub_size=mask_1d.sub_size
+        array_1d_slim=array_1d,
+        mask_1d=np.array(mask_1d),
     )
 
 
 @numba_util.jit()
 def array_1d_slim_from(
-    array_1d_native: np.ndarray, mask_1d: np.ndarray, sub_size: int
+    array_1d_native: np.ndarray,
+    mask_1d: np.ndarray,
 ) -> np.ndarray:
     """
     For a 1D array and mask, map the values of all unmasked pixels to its slimmed 1D array.
 
-    The 1D array has native dimensions corresponding to the array pixels (without masking) multiplied by the
-    sub_size. For example if a native array is shape [total_unmasked_pixels] and the ``sub_size=2``, the array is
-    shape [total_unmasked_x_pixels*sub_size].
+    The 1D array has native dimensions corresponding to the array pixels (without masking), for example a native array
+    may have shape [total_unmasked_pixels].
 
     The pixel coordinate origin is at the left of the 1D array and goes right, with pixels then going right in
-    each pixel. For example, for an array of shape (3,) and a sub-grid size of 2 where all pixels are unmasked:
+    each pixel.
 
-    - pixel[0] of the native 1D array will correspond to index 0 of the slim array (which is the first sub-pixel in
+    For example, for an array of shape (3,) where all pixels are unmasked:
+
+    - pixel[0] of the native 1D array will correspond to index 0 of the slim array (which is the first pixel in
     the array).
-    - pixel[1] of the native 1D array will correspond to index 1 of the slim array (which is the second sub-pixel in
+    - pixel[1] of the native 1D array will correspond to index 1 of the slim array (which is the second pixel in
     the array).
 
     If the native array is masked and the third pixel is masked (e.g. its mask_1d entry is `True`) then:
 
-    - pixels [0], [1], [2] and [3] of the native 1D array will correspond to indexes 0, 1, 2, 3 of the slim array.
-    - pixels [4] and [5] of the native 1D array do not map to the slim array (these sub-pixels are masked).
-    - pixel [6], [7], etc. of the native 1D array will correspond to indexes 4, 5, etc. of the slim array.
+    - pixels [0] and [1] of the native 1D array will correspond to indexes 0, 1 of the slim array.
+    - pixel [3] of the native 1D array do not map to the slim array (the pixels is masked).
 
     Parameters
     ----------
     array_1d_native
         A 1D array of values on the dimensions of the native array.
     mask_1d
         A 1D array of bools, where `False` values mean unmasked and are included in the mapping.
-    sub_size
-        The sub-grid size of the array.
 
     Returns
     -------
     ndarray
         The slimmed 1D array of values mapped from the native 1d array with
-        dimensions [total_unmasked_pixels*sub_size].
+        dimensions [total_unmasked_pixels].
 
     Examples
     --------
 
     array_1d_native = np.array([ 1.0,  2.0,  5.0,  6.0])
 
     mask = np.array([True, False, False, False]])
 
-    array_1d_slim = array_1d_slim_from(array_1d_native, array_2d=array_2d, sub_size=2)
+    array_1d_slim = array_1d_slim_from(array_1d_native, array_2d=array_2d)
     """
 
-    total_sub_pixels = mask_1d_util.total_sub_pixels_1d_from(
-        mask_1d=mask_1d, sub_size=sub_size
+    total_pixels = mask_1d_util.total_pixels_1d_from(
+        mask_1d=mask_1d,
     )
 
-    line_1d_slim = np.zeros(shape=total_sub_pixels)
+    line_1d_slim = np.zeros(shape=total_pixels)
     index = 0
 
     for x in range(mask_1d.shape[0]):
         if not mask_1d[x]:
-            for x1 in range(sub_size):
-                line_1d_slim[index] = array_1d_native[x * sub_size + x1]
-                index += 1
+            line_1d_slim[index] = array_1d_native[x]
+            index += 1
 
     return line_1d_slim
 
 
 def array_1d_native_from(
-    array_1d_slim: np.ndarray, mask_1d: np.ndarray, sub_size: int
+    array_1d_slim: np.ndarray,
+    mask_1d: np.ndarray,
 ) -> np.ndarray:
-    sub_shape = mask_1d.shape[0] * sub_size
+    shape = mask_1d.shape[0]
 
     native_index_for_slim_index_1d = mask_1d_util.native_index_for_slim_index_1d_from(
-        mask_1d=mask_1d, sub_size=sub_size
+        mask_1d=mask_1d,
     ).astype("int")
 
     return array_1d_via_indexes_1d_from(
-        array_1d_slim=array_1d_slim,
-        sub_shape=sub_shape,
+        array_1d_slim=np.array(array_1d_slim),
+        shape=shape,
         native_index_for_slim_index_1d=native_index_for_slim_index_1d,
     )
 
 
 @numba_util.jit()
 def array_1d_via_indexes_1d_from(
     array_1d_slim: np.ndarray,
-    sub_shape: int,
+    shape: int,
     native_index_for_slim_index_1d: np.ndarray,
 ) -> np.ndarray:
     """
-    For a slimmed 1D array with sub-indexes mapping the slimmed array values to their native array indexes,
+    For a slimmed 1D array with indexes mapping the slimmed array values to their native array indexes,
     return the native 1D array.
 
-    The 1D array has dimensions correspond to the size of the 1D array multiplied by the sub_size. For example
-    if an array is shape [total_x_pixels] and the `sub_size=2`, the array is shape [total_x_pixels*sub_size].
+    The pixel coordinate origin is at the left of the 1D array and goes right, with pixels then going right in
+    each pixel.
 
-    The pixel coordinate origin is at the left of the 1D array and goes right, with sub-pixels then going right in
-    each pixel. For example, for an array of shape (3,3) and a sub-grid size of 2 where all pixels are unmasked:
+    For example, for an array of shape (3,3) where all pixels are unmasked:
 
-    - pixel[0] of the native 1D array will correspond to index 0 of the slim array (which is the first sub-pixel in
+    - pixel[0] of the native 1D array will correspond to index 0 of the slim array (which is the first pixel in
     the line).
-    - pixel[1] of the native 1D array will correspond to index 1 of the slim array (which is the second sub-pixel in
+    - pixel[1] of the native 1D array will correspond to index 1 of the slim array (which is the second pixel in
     the line).
 
     If the native line is masked and the third pixel is masked (e.g. its mask_1d entry is `True`) then:
 
-    - pixels [0], [1], [2] and [3] of the native 1D array will correspond to indexes 0, 1, 2, 3 of the slim array.
-    - pixels [4] and [5] of the native 1D array do not map to the slim array (these sub-pixels are masked).
-    - pixel [6], [7], etc. of the native 1D array will correspond to indexes 4, 5, etc. of the slim array.
+    - pixels [0] and [1] of the native 1D array will correspond to indexes 0, 1 of the slim array.
+    - pixels [3] of the native 1D array do not map to the slim array (these pixels are masked).
 
     Parameters
     ----------
     array_1d_slim
-        The slimmed array of shape [total_x_pixels*sub_size] which are mapped to the native array.
-    sub_shape
-        The 1D dimensions of the native 1D sub line.
+        The slimmed array of shape [total_x_pixels] which are mapped to the native array.
+    shape
+        The 1D dimensions of the native 1D line.
     native_index_for_slim_index_1d : np.narray
-        An array of shape [total_x_pixels*sub_size] that maps from the slimmed array to the native array.
+        An array of shape [total_x_pixelss] that maps from the slimmed array to the native array.
 
     Returns
     -------
     ndarray
         The native 1D array of values mapped from the slimmed array with dimensions (total_x_pixels).
     """
-    array_1d_native = np.zeros(sub_shape)
+    array_1d_native = np.zeros(shape)
 
     for slim_index in range(len(native_index_for_slim_index_1d)):
         array_1d_native[native_index_for_slim_index_1d[slim_index]] = array_1d_slim[
             slim_index
         ]
 
     return array_1d_native
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/arrays/array_2d_util.py` & `autoarray-2024.5.16.0/autoarray/structures/arrays/array_2d_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,43 +51,43 @@
     ----------
     array_2d
         The input structure which is converted to its slim representation.
     mask_2d
         The mask of the output Array2D.
     """
     if len(array_2d.shape) == 1:
-        if array_2d.shape[0] != mask_2d.sub_pixels_in_mask:
+        if array_2d.shape[0] != mask_2d.pixels_in_mask:
             raise exc.ArrayException(
                 f"""
-                The input array is a slim 1D array, but it does not have the same number of entries as sub-pixels in
+                The input array is a slim 1D array, but it does not have the same number of entries as pixels in
                 the mask.
 
                 This indicates that the number of unmaksed pixels in the mask  is different to the input slim array 
                 shape.
 
                 The shapes of the two arrays (which this exception is raised because they are different) are as follows:
 
                 Input array_2d_slim.shape = {array_2d.shape[0]}
-                Input mask_2d.sub_pixels_in_mask = {mask_2d.sub_pixels_in_mask}
+                Input mask_2d.pixels_in_mask = {mask_2d.pixels_in_mask}
                 Input mask_2d.shape_native = {mask_2d.shape_native}
                 """
             )
 
     if len(array_2d.shape) == 2:
-        if array_2d.shape != mask_2d.sub_shape_native:
+        if array_2d.shape != mask_2d.shape_native:
             raise exc.ArrayException(
                 f"""
                 The input array is 2D but not the same dimensions as the mask.
     
-                This indicates the mask's shape, multiplied by its `sub_size`, is different to the input array shape.
+                This indicates the mask's shape is different to the input array shape.
     
                 The shapes of the two arrays (which this exception is raised because they are different) are as follows:
     
                 Input array_2d shape = {array_2d.shape}
-                Input mask_2d sub_shape_native = {mask_2d.sub_shape_native}
+                Input mask_2d shape_native = {mask_2d.shape_native}
                 """
             )
 
 
 def convert_array_2d(
     array_2d: Union[np.ndarray, List],
     mask_2d: Mask2D,
@@ -97,15 +97,15 @@
     """
     The `manual` classmethods in the `Array2D` object take as input a list or ndarray which is returned as an
     Array2D.
 
     This function performs the following and checks and conversions on the input:
 
     1) If the input is a list, convert it to an ndarray.
-    2) Check that the number of sub-pixels in the array is identical to that of the mask.
+    2) Check that the number of pixels in the array is identical to that of the mask.
     3) Map the input ndarray to its `slim` representation.
 
     For an Array2D, `slim` refers to a 1D NumPy array of shape [total_values] and `native` a 2D NumPy array of shape
     [total_y_values, total_values].
 
     Parameters
     ----------
@@ -113,32 +113,33 @@
         The input structure which is converted to an ndarray if it is a list.
     mask_2d
         The mask of the output Array2D.
     store_native
         If True, the ndarray is stored in its native format [total_y_pixels, total_x_pixels]. This avoids
         mapping large data arrays to and from the slim / native formats, which can be a computational bottleneck.
     """
-
-    array_2d = convert_array(array=array_2d)
+    array_2d = convert_array(array=array_2d).copy()
 
     check_array_2d_and_mask_2d(array_2d=array_2d, mask_2d=mask_2d)
 
     is_native = len(array_2d.shape) == 2
 
     if is_native and not skip_mask:
-        array_2d *= np.invert(mask_2d.derive_mask.sub)
+        array_2d *= np.invert(mask_2d)
 
     if is_native == store_native:
         return array_2d
     elif not store_native:
         return array_2d_slim_from(
-            array_2d_native=array_2d, mask_2d=mask_2d, sub_size=mask_2d.sub_size
+            array_2d_native=np.array(array_2d),
+            mask_2d=np.array(mask_2d),
         )
     array_2d = array_2d_native_from(
-        array_2d_slim=array_2d, mask_2d=mask_2d, sub_size=mask_2d.sub_size
+        array_2d_slim=array_2d,
+        mask_2d=np.array(mask_2d),
     )
     return array_2d
 
 
 def convert_array_2d_to_slim(array_2d: np.ndarray, mask_2d: Mask2D) -> np.ndarray:
     """
     The `manual` classmethods in the `Array2D` object take as input a list or ndarray which is returned as an
@@ -158,15 +159,16 @@
 
     if len(array_2d.shape) == 1:
         array_2d_slim = array_2d
 
         return array_2d_slim
 
     return array_2d_slim_from(
-        array_2d_native=array_2d, mask_2d=mask_2d, sub_size=mask_2d.sub_size
+        array_2d_native=array_2d,
+        mask_2d=mask_2d,
     )
 
 
 def convert_array_2d_to_native(array_2d: np.ndarray, mask_2d: Mask2D) -> np.ndarray:
     """
     The `manual` classmethods in the `Array2D` object take as input a list or ndarray which is returned as an
     Array2D.
@@ -182,30 +184,31 @@
     mask_2d
         The mask of the output Array2D.
     """
 
     if len(array_2d.shape) == 2:
         array_2d_native = array_2d * np.invert(mask_2d)
 
-        if array_2d.shape != mask_2d.sub_shape_native:
+        if array_2d.shape != mask_2d.shape_native:
             raise exc.ArrayException(
-                "The input array is 2D but not the same dimensions as the sub-mask "
-                "(e.g. the mask 2D shape multipled by its sub size.)"
+                "The input array is 2D but not the same dimensions as the mask "
+                "(e.g. the mask 2D shape.)"
             )
 
         return array_2d_native
 
-    if array_2d.shape[0] != mask_2d.sub_pixels_in_mask:
+    if array_2d.shape[0] != mask_2d.pixels_in_mask:
         raise exc.ArrayException(
-            "The input 1D array does not have the same number of entries as sub-pixels in"
+            "The input 1D array does not have the same number of entries as pixels in"
             "the mask."
         )
 
     return array_2d_native_from(
-        array_2d_slim=array_2d, mask_2d=mask_2d, sub_size=mask_2d.sub_size
+        array_2d_slim=array_2d,
+        mask_2d=mask_2d,
     )
 
 
 @numba_util.jit()
 def extracted_array_2d_from(
     array_2d: np.ndarray, y0: int, y1: int, x0: int, x1: int
 ) -> np.ndarray:
@@ -483,105 +486,96 @@
         )
 
     return index_slim_for_index_native_2d
 
 
 @numba_util.jit()
 def array_2d_slim_from(
-    array_2d_native: np.ndarray, mask_2d: np.ndarray, sub_size: int
+    array_2d_native: np.ndarray,
+    mask_2d: np.ndarray,
 ) -> np.ndarray:
     """
-    For a 2D sub array and mask, map the values of all unmasked pixels to its slimmed 1D sub-array.
+    For a 2D array and mask, map the values of all unmasked pixels to its slimmed 1D array.
+
+    The pixel coordinate origin is at the top left corner of the 2D array and goes right-wards and downwards.
 
-    A sub-array is an array whose native dimensions correspond to the normal array multiplied by the sub_size. For
-    example if an array is shape [total_y_pixels, total_x_pixels] and the ``sub_size=2``, the sub_array is shape
-    [total_y_pixels*sub_size, total_x_pixels*sub_size].
-
-    The pixel coordinate origin is at the top left corner of the 2D array and goes right-wards and downwards,
-    with sub-pixels then going right and downwards in each pixel. For example, for an array of shape (3,3) and a
-    sub-grid size of 2 where all pixels are unmasked:
+    For example, for an array of shape (3,3) where all pixels are unmasked:
 
     - pixel [0,0] of the 2D array will correspond to index 0 of the 1D array.
     - pixel [0,1] of the 2D array will correspond to index 1 of the 1D array.
-    - pixel [1,0] of the 2D array will correspond to index 2 of the 1D array.
-    - pixel [2,0] of the 2D array will correspond to index 4 of the 1D array.
-    - pixel [1,0] of the 2D array will correspond to index 12 of the 1D array.
+    - pixel [1,0] of the 2D array will correspond to index 3 of the 1D array.
+    - pixel [2,0] of the 2D array will correspond to index 6 of the 1D array.
 
     Parameters
     ----------
     array_2d_native
-        A 2D array of values on the dimensions of the sub-grid.
+        A 2D array of values on the dimensions of the grid.
     mask_2d
         A 2D array of bools, where `False` values mean unmasked and are included in the mapping.
     array_2d_native
         The 2D array of values which are mapped to a 1D array.
 
     Returns
     -------
     ndarray
         The slimmed 1D array of values mapped from the native 2D array with dimensions (total_unmasked_pixels).
 
     Examples
     --------
 
-    sub_array_2d = np.array([[ 1.0,  2.0,  5.0,  6.0],
+    array_2d = np.array([[ 1.0,  2.0,  5.0,  6.0],
                              [ 3.0,  4.0,  7.0,  8.0],
                              [ 9.0, 10.0, 13.0, 14.0],
                              [11.0, 12.0, 15.0, 16.0])
 
     mask = np.array([[True, False],
                      [False, False]])
 
-    sub_array_2d_slim = array_2d_slim_from(mask=mask, array_2d=array_2d, sub_size=2)
+    array_2d_slim = array_2d_slim_from(mask=mask, array_2d=array_2d)
     """
 
-    total_sub_pixels = mask_2d_util.total_sub_pixels_2d_from(
-        mask_2d=mask_2d, sub_size=sub_size
+    total_pixels = mask_2d_util.total_pixels_2d_from(
+        mask_2d=mask_2d,
     )
 
-    array_2d_slim = np.zeros(shape=total_sub_pixels)
+    array_2d_slim = np.zeros(shape=total_pixels)
     index = 0
 
     for y in range(mask_2d.shape[0]):
         for x in range(mask_2d.shape[1]):
             if not mask_2d[y, x]:
-                for y1 in range(sub_size):
-                    for x1 in range(sub_size):
-                        array_2d_slim[index] = array_2d_native[
-                            y * sub_size + y1, x * sub_size + x1
-                        ]
-                        index += 1
+                array_2d_slim[index] = array_2d_native[y, x]
+                index += 1
 
     return array_2d_slim
 
 
 def array_2d_native_from(
-    array_2d_slim: np.ndarray, mask_2d: np.ndarray, sub_size: int
+    array_2d_slim: np.ndarray,
+    mask_2d: np.ndarray,
 ) -> np.ndarray:
     """
     For a slimmed 2D array that was computed by mapping unmasked values from a native 2D array of shape
     [total_y_pixels, total_x_pixels], map its values back to the original 2D array where masked values are set to zero.
 
-    This uses the array ``slim_to_native`` where each index gives the 2D sub pixel indexes of the 1D array's
+    This uses the array ``slim_to_native`` where each index gives the 2D pixel indexes of the 1D array's
     unmasked pixels, for example:
 
     - If ``slim_to_native[0] = [0,0]``, the first value of the 1D array maps to the pixel [0,0] of the 2D array.
     - If ``slim_to_native[1] = [0,1]``, the second value of the 1D array maps to the pixel [0,1] of the 2D array.
     - If ``slim_to_native[4] = [1,1]``, the fifth value of the 1D array maps to the pixel [1,1] of the 2D array.
 
-    This example uses an array `sub_slim_to_native` which includes sub-gridding in the mapping.
+    This example uses an array `slim_to_native`.
 
     Parameters
     ----------
     array_2d_slim
         The slimmed array of values which are mapped to a 2D array.
     mask_2d
         A 2D array of bools, where `False` values mean unmasked and are included in the mapping.
-    sub_size
-        The size (sub_size x sub_size) of each unmasked pixels sub-array.
 
     Returns
     -------
     ndarray
         A 2D array of values mapped from the 1D array with dimensions shape.
 
     Examples
@@ -590,161 +584,134 @@
 
     array_1d = np.array([[2.0, 4.0, 5.0, 6.0, 8.0])
 
     array_2d = map_masked_1d_array_to_2d_array_from(
         array_1d=array_1d, shape=(3,3), slim_to_native=slim_to_native)
     """
 
-    sub_shape = (mask_2d.shape[0] * sub_size, mask_2d.shape[1] * sub_size)
+    shape = (mask_2d.shape[0], mask_2d.shape[1])
 
     native_index_for_slim_index_2d = mask_2d_util.native_index_for_slim_index_2d_from(
-        mask_2d=mask_2d, sub_size=sub_size
+        mask_2d=np.array(mask_2d),
     ).astype("int")
 
     return array_2d_via_indexes_from(
         array_2d_slim=array_2d_slim,
-        sub_shape=sub_shape,
+        shape=shape,
         native_index_for_slim_index_2d=native_index_for_slim_index_2d,
     )
 
 
 @numba_util.jit()
 def array_2d_via_indexes_from(
     array_2d_slim: np.ndarray,
-    sub_shape: Tuple[int, int],
+    shape: Tuple[int, int],
     native_index_for_slim_index_2d: np.ndarray,
 ) -> np.ndarray:
     """
-    For a slimmed sub array with sub-indexes mapping the slimmed sub-array values to their native sub-array,
-    return the native 2D sub-array.
+    For a slimmed array with indexes mapping the slimmed array values to their native array, return the native 2D
+    array.
 
-    A sub-array is an array whose dimensions correspond to the normal array multiplied by the sub_size. For example
-    if an array is shape [total_y_pixels, total_x_pixels] and the ``sub_size=2``, the sub_array is shape
-    [total_y_pixels*sub_size, total_x_pixels*sub_size].
-
-    The pixel coordinate origin is at the top left corner of the 2D array and goes right-wards and downwards,
-    with sub-pixels then going right and downwards in each pixel. For example, for an array of shape (3,3) and a
-    sub-grid size of 2 where all pixels are unmasked:
+    The pixel coordinate origin is at the top left corner of the 2D array and goes right-wards and downwards.
+
+    For example, for an array of shape (3,3) and where all pixels are unmasked:
 
     - pixel [0,0] of the native 2D array will correspond to index 0 of the slim array.
     - pixel [0,1] of the native 2D array will correspond to index 1 of the slim array.
-    - pixel [1,0] of the native 2D array will correspond to index 2 of the slim array.
-    - pixel [2,0] of the native 2D array will correspond to index 4 of the slim array.
-    - pixel [1,0] of the native 2D array will correspond to index 12 of the slim array.
+    - pixel [1,0] of the native 2D array will correspond to index 3 of the slim array.
+    - pixel [2,0] of the native 2D array will correspond to index 6 of the slim array.
 
     Parameters
     ----------
     array_2d_slim
         The slimmed array of shape [total_values] which are mapped to the native array..
-    sub_shape
-        The 2D dimensions of the native 2D sub-array.
+    shape
+        The 2D dimensions of the native 2D array.
     native_index_for_slim_index_2d : np.narray
         An array of shape [total_values] that maps from the slimmed array to the native array.
 
     Returns
     -------
     ndarray
         The native 2D array of values mapped from the slimmed array with dimensions (total_values, total_values).
     """
-    sub_array_native_2d = np.zeros(sub_shape)
+    array_native_2d = np.zeros(shape)
 
     for slim_index in range(len(native_index_for_slim_index_2d)):
-        sub_array_native_2d[
+        array_native_2d[
             native_index_for_slim_index_2d[slim_index, 0],
             native_index_for_slim_index_2d[slim_index, 1],
         ] = array_2d_slim[slim_index]
 
-    return sub_array_native_2d
+    return array_native_2d
 
 
 @numba_util.jit()
 def array_2d_slim_complex_from(
-    array_2d_native: np.ndarray, mask: np.ndarray, sub_size: int
+    array_2d_native: np.ndarray,
+    mask: np.ndarray,
 ) -> np.ndarray:
     """
-    For a 2D sub array and mask, map the values of all unmasked pixels to a 1D sub-array.
+    For a 2D array and mask, map the values of all unmasked pixels to a 1D array.
+
+    The pixel coordinate origin is at the top left corner of the 2D array and goes right-wards and downwards.
 
-    A sub-array is an array whose dimensions correspond to the normal array (e.g. used to make the grid)
-    multiplied by the sub_size. E.g., it is an array that would be generated using the sub-grid and not binning
-    up values in sub-pixels back to the grid.
-
-    The pixel coordinate origin is at the top left corner of the 2D array and goes right-wards and downwards,
-    with sub-pixels then going right and downwards in each pixel. For example, for an array of shape (3,3) and a
-    sub-grid size of 2 where all pixels are unmasked:
+    For example, for an array of shape (3,3) and where all pixels are unmasked:
 
     - pixel [0,0] of the 2D array will correspond to index 0 of the 1D array.
     - pixel [0,1] of the 2D array will correspond to index 1 of the 1D array.
-    - pixel [1,0] of the 2D array will correspond to index 2 of the 1D array.
-    - pixel [2,0] of the 2D array will correspond to index 4 of the 1D array.
-    - pixel [1,0] of the 2D array will correspond to index 12 of the 1D array.
+    - pixel [1,0] of the 2D array will correspond to index 3 of the 1D array.
+    - pixel [2,0] of the 2D array will correspond to index 6 of the 1D array.
 
     Parameters
     ----------
     array_2d_native
-        A 2D array of values on the dimensions of the sub-grid.
+        A 2D array of values on the dimensions of the grid.
     mask
         A 2D array of bools, where `False` values mean unmasked and are included in the mapping.
     array_2d
         The 2D array of values which are mapped to a 1D array.
 
     Returns
     -------
     ndarray
         A 1D array of values mapped from the 2D array with dimensions (total_unmasked_pixels).
-
-    Examples
-    --------
-
-    sub_array_2d = np.array([[ 1.0,  2.0,  5.0,  6.0],
-                             [ 3.0,  4.0,  7.0,  8.0],
-                             [ 9.0, 10.0, 13.0, 14.0],
-                             [11.0, 12.0, 15.0, 16.0])
-
-    mask = np.array([[True, False],
-                     [False, False]])
-
-    sub_array_1d = map_sub_array_2d_to_masked_sub_array_1d_from(
-        mask=mask, array_2d=array_2d)
     """
 
-    total_sub_pixels = mask_2d_util.total_sub_pixels_2d_from(
-        mask_2d=mask, sub_size=sub_size
+    total_pixels = mask_2d_util.total_pixels_2d_from(
+        mask_2d=mask,
     )
 
-    sub_array_1d = 0 + 0j * np.zeros(shape=total_sub_pixels)
+    array_1d = 0 + 0j * np.zeros(shape=total_pixels)
     index = 0
 
     for y in range(mask.shape[0]):
         for x in range(mask.shape[1]):
             if not mask[y, x]:
-                for y1 in range(sub_size):
-                    for x1 in range(sub_size):
-                        sub_array_1d[index] = array_2d_native[
-                            y * sub_size + y1, x * sub_size + x1
-                        ]
-                        index += 1
+                array_1d[index] = array_2d_native[y, x]
+                index += 1
 
-    return sub_array_1d
+    return array_1d
 
 
 @numba_util.jit()
 def array_2d_native_complex_via_indexes_from(
     array_2d_slim: np.ndarray,
-    sub_shape_native: Tuple[int, int],
+    shape_native: Tuple[int, int],
     native_index_for_slim_index_2d: np.ndarray,
 ) -> np.ndarray:
-    sub_array_2d = 0 + 0j * np.zeros(sub_shape_native)
+    array_2d = 0 + 0j * np.zeros(shape_native)
 
     for slim_index in range(len(native_index_for_slim_index_2d)):
-        sub_array_2d[
+        array_2d[
             native_index_for_slim_index_2d[slim_index, 0],
             native_index_for_slim_index_2d[slim_index, 1],
         ] = array_2d_slim[slim_index]
 
-    return sub_array_2d
+    return array_2d
 
 
 def hdu_for_output_from(
     array_2d: np.ndarray, header_dict: Optional[dict] = None
 ) -> fits.PrimaryHDU:
     """
     Returns the HDU which can be used to output an array to a .fits file.
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/arrays/kernel_2d.py` & `autoarray-2024.5.16.0/autoarray/structures/arrays/kernel_2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,49 +13,50 @@
 
 from autoarray import exc
 from autoarray import type as ty
 from autoarray.structures.arrays import array_2d_util
 
 
 class Kernel2D(AbstractArray2D):
-    def __new__(
-        cls,
+    def __init__(
+        self,
         values,
         mask,
         header=None,
         normalize: bool = False,
         store_native: bool = False,
         *args,
         **kwargs
     ):
         """
-        An array of values, which are paired to a uniform 2D mask of pixels and sub-pixels. Each entry
-        on the array corresponds to a value at the centre of a sub-pixel in an unmasked pixel. See the ``Array2D`` class
+        An array of values, which are paired to a uniform 2D mask of pixels. Each entry
+        on the array corresponds to a value at the centre of a pixel in an unmasked pixel. See the ``Array2D`` class
         for a full description of how Arrays work.
 
         The ``Kernel2D`` class is an ``Array2D`` but with additioonal methods that allow it to be convolved with data.
 
         Parameters
         ----------
         values
             The values of the array.
         mask
             The 2D mask associated with the array, defining the pixels each array value is paired with and
             originates from.
         normalize
             If True, the Kernel2D's array values are normalized such that they sum to 1.0.
         """
-        obj = super().__new__(
-            cls=cls, values=values, mask=mask, header=header, store_native=store_native
+        super().__init__(
+            values=values,
+            mask=mask,
+            header=header,
+            store_native=store_native,
         )
 
         if normalize:
-            obj[:] = np.divide(obj, np.sum(obj))
-
-        return obj
+            self._array[:] = np.divide(self._array, np.sum(self._array))
 
     @classmethod
     def no_mask(
         cls,
         values: Union[np.ndarray, List],
         pixel_scales: ty.PixelScales,
         shape_native: Tuple[int, int] = None,
@@ -66,23 +67,21 @@
         Create a Kernel2D (see *Kernel2D.__new__*) by inputting the kernel values in 1D or 2D, automatically
         determining whether to use the 'manual_slim' or 'manual_native' methods.
 
         See the manual_slim and manual_native methods for examples.
         Parameters
         ----------
         values
-            The values of the array input as an ndarray of shape [total_unmasked_pixels*(sub_size**2)] or a list of
+            The values of the array input as an ndarray of shape [total_unmasked_pixels] or a list of
             lists.
         shape_native
             The 2D shape of the mask the array is paired with.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         normalize
             If True, the Kernel2D's array values are normalized such that they sum to 1.0.
         """
         values = Array2D.no_mask(
             values=values,
@@ -113,16 +112,14 @@
         fill_value
             The value all array elements are filled with.
         shape_native
             The 2D shape of the mask the array is paired with.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         normalize
             If True, the Kernel2D's array values are normalized such that they sum to 1.0.
         """
         return Kernel2D.no_mask(
             values=np.full(fill_value=fill_value, shape=shape_native),
@@ -149,16 +146,14 @@
         Parameters
         ----------
         shape_native
             The 2D shape of the mask the array is paired with.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         normalize
             If True, the Kernel2D's array values are normalized such that they sum to 1.0.
         """
         return cls.full(
             fill_value=1.0,
@@ -186,16 +181,14 @@
         Parameters
         ----------
         shape_native
             The 2D shape of the mask the array is paired with.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         normalize
             If True, the Kernel2D's array values are normalized such that they sum to 1.0.
         """
         return cls.full(
             fill_value=0.0,
@@ -379,49 +372,29 @@
         the :meth:`Kernel2D class API documentation <autoarray.structures.arrays.uniform_2d.AbstractKernel2D.__new__>`.
 
         Parameters
         ----------
         primary_hdu
             The `PrimaryHDU` object which has already been loaded from a .fits file via `astropy.fits` and contains
             the array data and the pixel-scale in the header with an entry named `PIXSCALE`.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the coordinate system.
 
         Examples
         --------
 
         .. code-block:: python
 
             from astropy.io import fits
             import autoarray as aa
 
-            # Make Kernel2D with sub_size 1.
-
             primary_hdu = fits.open("path/to/file.fits")
 
             array_2d = aa.Kernel2D.from_primary_hdu(
                 primary_hdu=primary_hdu,
-                sub_size=1
-            )
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            # Make Kernel2D with sub_size 2.
-            # (It is uncommon that a sub-gridded array would be loaded from
-            # a .fits, but the API support its).
-
-             primary_hdu = fits.open("path/to/file.fits")
-
-            array_2d = aa.Kernel2D.from_primary_hdu(
-                primary_hdu=primary_hdu,
-                sub_size=2
             )
         """
         return cls.no_mask(
             values=cls.flip_hdu_for_ds9(primary_hdu.data.astype("float")),
             pixel_scales=primary_hdu.header["PIXSCALE"],
             origin=origin,
         )
@@ -453,23 +426,22 @@
 
         try:
             kernel_rescaled = rescale(
                 self.native,
                 rescale_factor,
                 anti_aliasing=False,
                 mode="constant",
-                multichannel=False,
+                channel_axis=None,
             )
         except TypeError:
             kernel_rescaled = rescale(
                 self.native,
                 rescale_factor,
                 anti_aliasing=False,
                 mode="constant",
-                #   multichannel=False,
             )
 
         if kernel_rescaled.shape[0] % 2 == 0 and kernel_rescaled.shape[1] % 2 == 0:
             kernel_rescaled = resize(
                 kernel_rescaled,
                 output_shape=(
                     kernel_rescaled.shape[0] + 1,
@@ -537,25 +509,24 @@
         Raises
         ------
         KernelException if either Kernel2D psf dimension is odd
         """
         if self.mask.shape[0] % 2 == 0 or self.mask.shape[1] % 2 == 0:
             raise exc.KernelException("Kernel2D Kernel2D must be odd")
 
-        array_binned_2d = array.binned.native
+        array_2d = array.native
 
-        convolved_array_2d = scipy.signal.convolve2d(
-            array_binned_2d, self.native, mode="same"
-        )
+        convolved_array_2d = scipy.signal.convolve2d(array_2d, self.native, mode="same")
 
         convolved_array_1d = array_2d_util.array_2d_slim_from(
-            mask_2d=array_binned_2d.mask, array_2d_native=convolved_array_2d, sub_size=1
+            mask_2d=np.array(array_2d.mask),
+            array_2d_native=convolved_array_2d,
         )
 
-        return Array2D(values=convolved_array_1d, mask=array_binned_2d.mask)
+        return Array2D(values=convolved_array_1d, mask=array_2d.mask)
 
     def convolved_array_with_mask_from(self, array: Array2D, mask: Mask2D) -> Array2D:
         """
         Convolve an array with this Kernel2D
 
         Parameters
         ----------
@@ -574,11 +545,12 @@
 
         if self.mask.shape[0] % 2 == 0 or self.mask.shape[1] % 2 == 0:
             raise exc.KernelException("Kernel2D Kernel2D must be odd")
 
         convolved_array_2d = scipy.signal.convolve2d(array, self.native, mode="same")
 
         convolved_array_1d = array_2d_util.array_2d_slim_from(
-            mask_2d=mask, array_2d_native=convolved_array_2d, sub_size=1
+            mask_2d=np.array(mask),
+            array_2d_native=np.array(convolved_array_2d),
         )
 
-        return Array2D(values=convolved_array_1d, mask=mask.derive_mask.sub_1)
+        return Array2D(values=convolved_array_1d, mask=mask)
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/arrays/uniform_1d.py` & `autoarray-2024.5.16.0/autoarray/structures/arrays/uniform_1d.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,53 +12,49 @@
 from autoarray.structures.arrays import array_1d_util
 from autoarray.structures.arrays import array_2d_util
 from autoarray.geometry import geometry_util
 from autoarray import type as ty
 
 
 class Array1D(Structure):
-    def __new__(
-        cls,
+    def __init__(
+        self,
         values: Union[np.ndarray, List],
         mask: Mask1D,
         header: Optional[Header] = None,
         store_native: bool = False,
-        *args,
-        **kwargs
     ):
         values = array_1d_util.convert_array_1d(
-            array_1d=values, mask_1d=mask, store_native=store_native
+            array_1d=values,
+            mask_1d=mask,
+            store_native=store_native,
         )
 
-        obj = values.view(cls)
-        obj.mask = mask
-        obj.header = header
+        self.mask = mask
+        self.header = header
 
-        return obj
+        super().__init__(values)
 
     @classmethod
     def no_mask(
         cls,
         values: Union[np.ndarray, Tuple[float], List[float]],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float] = (0.0,),
         header: Optional[Header] = None,
     ) -> "Array1D":
         """
         Create a Array1D (see `Array1D.__new__`) by inputting the array values in 1D
 
         Parameters
         ----------
         values
-            The values of the array input as an ndarray of shape [total_unmasked_pixels*sub_size] or a list.
+            The values of the array input as an ndarray of shape [total_unmasked_pixels] or a list.
         pixel_scales
             The scaled units to pixel units conversion factor of the array data coordinates (e.g. the x-axis).
-        sub_size
-            The size of each unmasked pixels sub-grid.
         origin
             The origin of the 1D array's mask.
 
         Examples
         --------
 
         .. code-block:: python
@@ -81,29 +77,27 @@
         """
 
         values = array_2d_util.convert_array(values)
 
         pixel_scales = geometry_util.convert_pixel_scales_1d(pixel_scales=pixel_scales)
 
         mask = Mask1D.all_false(
-            shape_slim=values.shape[0] // sub_size,
+            shape_slim=values.shape[0],
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
         return Array1D(values=values, mask=mask, header=header)
 
     @classmethod
     def full(
         cls,
         fill_value: float,
         shape_native: Union[int, Tuple[int]],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float] = (0.0,),
         header: Optional[Header] = None,
     ) -> "Array1D":
         """
         Create an `Array1D` (see `Array1D.__new__`) where all values are filled with an input fill value,
         analogous to the method np.full().
 
@@ -115,38 +109,31 @@
         fill_value
             The value all array elements are filled with.
         shape_native : Tuple[int]
             The 1D shape of the mask the array is paired with.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float,) structure.
-        sub_size
-            The size (sub_size) of each unmasked pixels sub-array.
         origin : (float,)
             The (x) scaled units origin of the mask's coordinate system.
         """
         shape_native = geometry_util.convert_shape_native_1d(shape_native=shape_native)
 
-        if sub_size is not None:
-            shape_native = (shape_native[0] * sub_size,)
-
         return cls.no_mask(
             values=np.full(fill_value=fill_value, shape=shape_native[0]),
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             header=header,
         )
 
     @classmethod
     def zeros(
         cls,
         shape_native: Union[int, Tuple[int]],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float] = (0.0,),
         header: Optional[Header] = None,
     ) -> "Array1D":
         """
         Create an `Array1D` (see `Array1D.__new__`) where all values are filled with zeros, analogous to the
         method np.zeros().
 
@@ -156,34 +143,30 @@
         Parameters
         ----------
         shape_native : Tuple[int]
             The 1D shape of the mask the array is paired with.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float,) structure.
-        sub_size
-            The size (sub_size) of each unmasked pixels sub-array.
         origin : (float,)
             The (x) scaled units origin of the mask's coordinate system.
         """
         return cls.full(
             fill_value=0.0,
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             header=header,
         )
 
     @classmethod
     def ones(
         cls,
         shape_native: Union[int, Tuple[int]],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float] = (0.0,),
         header: Optional[Header] = None,
     ) -> "Array1D":
         """
         Create an `Array1D` (see `Array1D.__new__`) where all values are filled with ones, analogous to the
         method np.ones().
 
@@ -193,35 +176,31 @@
         Parameters
         ----------
         shape_native : Tuple[int]
             The 1D shape of the mask the array is paired with.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float,) structure.
-        sub_size
-            The size (sub_size) of each unmasked pixels sub-array.
         origin : (float,)
             The (x) scaled units origin of the mask's coordinate system.
         """
         return cls.full(
             fill_value=1.0,
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             header=header,
         )
 
     @classmethod
     def from_fits(
         cls,
         file_path: Union[Path, str],
         pixel_scales: ty.PixelScales,
         hdu: int = 0,
-        sub_size: int = 1,
         origin: Tuple[float] = (0.0, 0.0),
     ) -> "Array1D":
         """
         Create an Array1D (see `Array1D.__new__`) by loading the array values from a .fits file.
 
         Parameters
         ----------
@@ -229,16 +208,14 @@
             The path the file is loaded from, including the filename and the `.fits` extension,
             e.g. '/path/to/filename.fits'
         hdu
             The Header-Data Unit of the .fits file the array data is loaded from.
         pixel_scales
             The (x,) scaled units to pixel units conversion factors of every pixel. If this is input as a float,
             it is converted to a (float,) structure.
-        sub_size
-            The sub-size of each unmasked pixels sub-array.
         origin
             The (x,) scaled units origin of the coordinate system.
         """
         array_1d = array_1d_util.numpy_array_1d_via_fits_from(
             file_path=file_path, hdu=hdu
         )
 
@@ -246,24 +223,22 @@
         header_hdu_obj = array_2d_util.header_obj_from(file_path=file_path, hdu=hdu)
 
         return cls.no_mask(
             values=array_1d.astype(
                 "float64"
             ),  # Have to do this due to typing issues in 1D with astorpy fits.
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             header=Header(header_sci_obj=header_sci_obj, header_hdu_obj=header_hdu_obj),
         )
 
     @classmethod
     def from_primary_hdu(
         cls,
         primary_hdu: fits.PrimaryHDU,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
     ) -> "Array1D":
         """
         Returns an ``Array1D`` by from a `PrimaryHDU` object which has been loaded via `astropy.fits`
 
         This assumes that the `header` of the `PrimaryHDU` contains an entry named `PIXSCALE` which gives the
         pixel-scale of the array.
@@ -273,75 +248,54 @@
         the :meth:`Array1D class API documentation <autoarray.structures.arrays.uniform_1d.AbstractArray1D.__new__>`.
 
         Parameters
         ----------
         primary_hdu
             The `PrimaryHDU` object which has already been loaded from a .fits file via `astropy.fits` and contains
             the array data and the pixel-scale in the header with an entry named `PIXSCALE`.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the coordinate system.
 
         Examples
         --------
 
         .. code-block:: python
 
             from astropy.io import fits
             import autoarray as aa
 
-            # Make Array1D with sub_size 1.
-
             primary_hdu = fits.open("path/to/file.fits")
 
             array_1d = aa.Array1D.from_primary_hdu(
                 primary_hdu=primary_hdu,
-                sub_size=1
-            )
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            # Make Array1D with sub_size 2.
-            # (It is uncommon that a sub-gridded array would be loaded from
-            # a .fits, but the API support its).
-
-             primary_hdu = fits.open("path/to/file.fits")
-
-            array_1d = aa.Array1D.from_primary_hdu(
-                primary_hdu=primary_hdu,
-                sub_size=2
             )
         """
         return cls.no_mask(
             values=primary_hdu.data.astype("float"),
             pixel_scales=primary_hdu.header["PIXSCALE"],
-            sub_size=sub_size,
             origin=origin,
             header=Header(header_sci_obj=primary_hdu.header),
         )
 
     @property
     def slim(self) -> "Array1D":
         """
         Return an `Array1D` where the data is stored its `slim` representation, which is an ndarray of shape
-        [total_unmasked_pixels * sub_size].
+        [total_unmasked_pixels].
 
         If it is already stored in its `slim` representation  it is returned as it is. If not, it is  mapped from
         `native` to `slim` and returned as a new `Array1D`.
         """
         return Array1D(values=self, mask=self.mask)
 
     @property
     def native(self) -> "Array1D":
         """
         Return an `Array1D` where the data is stored in its `native` representation, which is an ndarray of shape
-        [total_pixels * sub_size].
+        [total_pixels].
 
         If it is already stored in its `native` representation it is return as it is. If not, it is mapped from
         `slim` to `native` and returned as a new `Array1D`.
         """
         return Array1D(values=self, mask=self.mask, store_native=True)
 
     @property
@@ -352,15 +306,14 @@
         return (0,)
 
     @property
     def grid_radial(self) -> Grid1D:
         return Grid1D.uniform_from_zero(
             shape_native=self.shape_native,
             pixel_scales=self.pixel_scales,
-            sub_size=self.sub_size,
         )
 
     @property
     def hdu_for_output(self) -> fits.PrimaryHDU:
         """
         The array as an HDU object, which can be output to a .fits file.
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/arrays/uniform_2d.py` & `autoarray-2024.5.16.0/autoarray/structures/arrays/uniform_2d.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,52 +14,53 @@
 from autoarray import exc
 from autoarray import type as ty
 
 from autoarray.structures.arrays import array_2d_util
 from autoarray.geometry import geometry_util
 from autoarray.layout import layout_util
 
+
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class AbstractArray2D(Structure):
-    def __new__(
-        cls,
-        values: Union[np.ndarray, List],
+    def __init__(
+        self,
+        values: Union[np.ndarray, List, "AbstractArray2D"],
         mask: Mask2D,
         header: Header = None,
         store_native: bool = False,
         skip_mask: bool = False,
         *args,
         **kwargs,
     ):
         """
-        A uniform 2D array of values, which are paired with a 2D mask of pixels which may be split into sub-pixels.
+        A uniform 2D array of values, which are paired with a 2D mask of pixels.
 
         The ``Array2D`, like all data structures (e.g. ``Grid2D``, ``VectorYX2D``) has in-built functionality which:
 
         - Applies a 2D mask (a ``Mask2D`` object) to the da_ta structure's values.
 
         - Maps the data structure between two data representations: `slim`` (all unmasked values in
           a 1D ``ndarray``) and ``native`` (all unmasked values in a 2D ``ndarray``).
 
         - Associates Cartesian ``Grid2D`` objects of (y,x) coordinates with the data structure (e.g.
           a (y,x) grid of all unmasked pixels).
 
-        - Associates sub-grids with the data structure, which perform calculations higher resolutions which are then
+        - Associates grids with the data structure, which perform calculations higher resolutions which are then
           binned up.
 
-        Each entry of an ``Array2D`` corresponds to a value at the centre of a sub-pixel in its
+        Each entry of an ``Array2D`` corresponds to a value at the centre of a pixel in its
         corresponding ``Mask2D``.  It is ordered such that pixels begin from the top-row of the corresponding mask
         and go right and down. The positive y-axis is upwards and positive x-axis to the right.
 
         A detailed description of the data structure API is provided below.
 
-        **SLIM DATA REPRESENTATION (sub-size=1)**
+        __slim__
 
         Below is a visual illustration of an ``Array2D``'s 2D mask, where a total of 10 pixels are unmasked and are
         included in the array.
 
         ::
 
              x x x x x x x x x x
@@ -101,15 +102,15 @@
             array[3] = the 4th unmasked pixel's value, given by value 40 above.
             array[6] = the 7th unmasked pixel's value, given by value 80 above.
 
         A Cartesian grid of (y,x) coordinates, corresponding to all ``slim`` values (e.g. unmasked pixels) is given
         by ``array_2d.derive_grid.masked.slim``.
 
 
-        **NATIVE DATA REPRESENTATION (sub_size=1)**
+        __native__
 
         The ``Array2D`` above, but represented as an an ``ndarray`` of shape [total_y_values, total_x_values], where
         all masked entries have values of 0.0.
 
         For the following mask:
 
         ::
@@ -169,103 +170,17 @@
             slim_to_native[4] = [4,5]
             slim_to_native[5] = [4,6]
             slim_to_native[6] = [5,3]
             slim_to_native[7] = [5,4]
             slim_to_native[8] = [5,5]
             slim_to_native[9] = [5,6]
 
-        **SUB GRIDDING**
-
-        If the ``Mask2D`` ``sub_size`` is > 1, the array has entries corresponding to the values at the centre of
-        every sub-pixel of each unmasked pixel.
-
-        The sub-array indexes are ordered such that pixels begin from the first (top-left) sub-pixel in the first
-        unmasked pixel. Indexes then go over the sub-pixels in each unmasked pixel, for every unmasked pixel.
-
-        Therefore, the shapes of the sub-array are as follows:
-
-        - ``slim`` representation: an ``ndarray`` of shape [total_unmasked_pixels*sub_size**2].
-        - ``native`` representation: an ``ndarray`` of shape [total_y_values*sub_size, total_x_values*sub_size].
-
-        Below is a visual illustration of a sub array. Indexing of each sub-pixel goes from the top-left corner. In
-        contrast to the array above, our illustration below restricts the mask to just 2 pixels, to keep the
-        illustration brief.
-
-        ::
-
-             x x x x x x x x x x
-             x x x x x x x x x x     This is an example ``Mask2D``, where:
-             x x x x x x x x x x
-             x x x x x x x x x x     x = `True` (Pixel is masked and excluded from lens)
-             x 0 0 x x x x x x x     O = `False` (Pixel is not masked and included in lens)
-             x x x x x x x x x x
-             x x x x x x x x x x
-             x x x x x x x x x x
-             x x x x x x x x x x
-             x x x x x x x x x x
-
-        If ``sub_size=2``, each unmasked pixel has 4 (2x2) sub-pixel values. For the example above, pixels 0 and 1
-        each have 4 values which map to the ``array_2d``'s ``slim`` representation as follows:
-
-        ::
-
-            Pixel 0 - (2x2):
-
-                   array_2d.slim[0] = value of first sub-pixel in pixel 0.
-             0 1   array_2d.slim[1] = value of first sub-pixel in pixel 1.
-             2 3   array_2d.slim[2] = value of first sub-pixel in pixel 2.
-                   array_2d.slim[3] = value of first sub-pixel in pixel 3.
-
-            Pixel 1 - (2x2):
-
-                   array_2d.slim[4] = value of first sub-pixel in pixel 0.
-             4 5   array_2d.slim[5] = value of first sub-pixel in pixel 1.
-             6 7   array_2d.slim[6] = value of first sub-pixel in pixel 2.
-                   array_2d.slim[7] = value of first sub-pixel in pixel 3.
-
-        For the ``native`` data representation we get the following mappings:
-
-        ::
-
-            Pixel 0 - (2x2):
-
-                   array_2d.native[8, 2] = value of first sub-pixel in pixel 0.
-             0 1   array_2d.native[8, 3] = value of first sub-pixel in pixel 1.
-             2 3   array_2d.native[9, 2] = value of first sub-pixel in pixel 2.
-                   array_2d.native[9, 3] = value of first sub-pixel in pixel 3.
-
-            Pixel 1 - (2x2):
-
-                   array_2d.native[10, 4] = value of first sub-pixel in pixel 0.
-             4 5   array_2d.native[10, 5] = value of first sub-pixel in pixel 1.
-             6 7   array_2d.native[11, 4] = value of first sub-pixel in pixel 2.
-                   array_2d.native[11, 5] = value of first sub-pixel in pixel 3.
-
-            Other entries (all masked sub-pixels are zero):
-
-                   array_2d.native[0, 0] = 0.0 (it is masked, thus zero)
-                   array_2d.native[15, 12] = 0.0 (it is masked, thus zero)
-
-        If we used a sub_size of 3, for pixel 0 we we would create a 3x3 sub-array:
-
-        ::
-
-                     array_2d.slim[0] = value of first sub-pixel in pixel 0.
-                     array_2d.slim[1] = value of first sub-pixel in pixel 1.
-                     array_2d.slim[2] = value of first sub-pixel in pixel 2.
-             0 1 2   array_2d.slim[3] = value of first sub-pixel in pixel 3.
-             3 4 5   array_2d.slim[4] = value of first sub-pixel in pixel 4.
-             6 7 8   array_2d.slim[5] = value of first sub-pixel in pixel 5.
-                     array_2d.slim[6] = value of first sub-pixel in pixel 6.
-                     array_2d.slim[7] = value of first sub-pixel in pixel 7.
-                     array_2d.slim[8] = value of first sub-pixel in pixel 8.
-
-        In **PyAutoCTI** all `Array2D` objects are used in their `native` representation without sub-gridding.
-        Significant memory can be saved by only store this format, thus the `native_binned_only` config override
-        can force this behaviour. It is recommended users do not use this option to avoid unexpected behaviour.
+        In **PyAutoCTI** all `Array2D` objects are used in their `native` representation. Significant memory can be
+        saved by only store this format, thus the `native_only` config override can force this behaviour.
+        It is recommended users do not use this option to avoid unexpected behaviour.
 
         Parameters
         ----------
         values
             The values of the array, which can be input in the ``slim`` or ``native`` format.
         mask
             The 2D mask associated with the array, defining the pixels each array value in its ``slim`` representation
@@ -281,216 +196,170 @@
 
         Different methods using different inputs are available and documented throughout this webpage.
 
         .. code-block:: python
 
             import autoarray as aa
 
-            # Make Array2D from input np.ndarray with sub_size 1.
-
             array_2d = aa.Array2D.no_mask(
                 values=np.array([1.0, 2.0, 3.0, 4.0]),
                 shape_native=(2, 2),
                 pixel_scales=1.0,
-                sub_size=1
-            )
-
-            # Make Array2D from input list with different shape_native and sub_size 1.
-
-            array_2d = aa.Array2D.no_mask(
-                values=[1.0, 2.0, 3.0, 4.0, 5.0, 6.0],
-                shape_native=(2, 3),
-                pixel_scales=1.0,
-                sub_size=1
             )
 
         .. code-block:: python
 
             import autoarray as aa
 
-            # Make Array2D with sub_size 2.
-
             array_2d = aa.Array2D.no_mask(
-                values=[1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0],
+                values=[1.0, 2.0, 3.0, 4.0],
                 shape_native=(2, 1),
                 pixel_scales=1.0,
-                sub_size=2,
             )
 
-            # Apply 2D mask to Array2D with sub_size 2, where the
-            # True value masks entries (5.0, 6.0, 7.0, 8.0).
-
             mask = aa.Mask2D(
-                mask=[[False], [True]],
+                mask=[[False, False], [True, True]],
                 pixel_scales=2.0,
-                sub_size=2
             )
 
             array_2d = array_2d.apply_mask(mask=mask)
 
             # Print certain array attributes.
 
-            print(array_2d.slim) # masked 1D data representation on sub-grid.
-            print(array_2d.native) # masked 2D data representation on sub-grid.
-            print(array_2d.slim.binned) # masked 1D data representation binned up from sub-grid.
-            print(array_2d.native.binned) # masked 2D data representation binned up from sub-grid.
+            print(array_2d.slim) # masked 1D data representation.
+            print(array_2d.native) # masked 2D data representation.
 
             # Output array to .fits file.
 
             array_2d.output_to_fits(file_path="/path/for/output")
         """
 
+        try:
+            values = values._array
+        except AttributeError:
+            pass
+
         if conf.instance["general"]["structures"]["native_binned_only"]:
             store_native = True
 
         values = array_2d_util.convert_array_2d(
             array_2d=values,
             mask_2d=mask,
             store_native=store_native,
             skip_mask=skip_mask,
         )
 
-        obj = values.view(cls)
-        obj.mask = mask
-        obj.header = header
+        super().__init__(values)
+        self.mask = mask
+        self.header = header
 
-        return obj
+    @property
+    def values(self):
+        return self._array
 
     def __array_finalize__(self, obj):
         if hasattr(obj, "mask"):
             self.mask = obj.mask
 
         if hasattr(obj, "header"):
             self.header = obj.header
         else:
             self.header = None
 
     @property
     def store_native(self):
-        if len(self.shape) == 1:
-            return False
-        return True
+        return len(self.shape) != 1
 
     def apply_mask(self, mask: Mask2D) -> "Array2D":
         return Array2D(values=self.native, mask=mask, header=self.header)
 
     @property
     def slim(self) -> "Array2D":
         """
         Return an `Array2D` where the data is stored its `slim` representation, which is an ``ndarray`` of shape
-        [total_unmasked_pixels * sub_size**2].
+        [total_unmasked_pixels].
 
         If it is already stored in its `slim` representation it is returned as it is. If not, it is mapped from
         `native` to `slim` and returned as a new `Array2D`.
         """
         return Array2D(values=self, mask=self.mask, header=self.header)
 
     @property
     def native(self) -> "Array2D":
         """
         Return a `Array2D` where the data is stored in its `native` representation, which is an ``ndarray`` of shape
-        [sub_size*total_y_pixels, sub_size*total_x_pixels].
+        [total_y_pixels, total_x_pixels].
 
         If it is already stored in its `native` representation it is return as it is. If not, it is mapped from
         `slim` to `native` and returned as a new `Array2D`.
         """
         return Array2D(
             values=self, mask=self.mask, header=self.header, store_native=True
         )
 
     @property
     def native_skip_mask(self) -> "Array2D":
         """
         Return a `Array2D` where the data is stored in its `native` representation, which is an ``ndarray`` of shape
-        [sub_size*total_y_pixels, sub_size*total_x_pixels].
+        [total_y_pixels, total_x_pixels].
 
         If it is already stored in its `native` representation it is return as it is. If not, it is mapped from
         `slim` to `native` and returned as a new `Array2D`.
         """
         return Array2D(
             values=self,
             mask=self.mask,
             header=self.header,
             store_native=True,
             skip_mask=True,
         )
 
     @property
-    def binned(self) -> "Array2D":
-        """
-        Convenience method to access the binned-up array in its 1D representation, which is a Grid2D stored as an
-        ``ndarray`` of shape [total_unmasked_pixels, 2].
-
-        The binning up process converts a array from (y,x) values where each value is a coordinate on the sub-array to
-        (y,x) values where each coordinate is at the centre of its mask (e.g. a array with a sub_size of 1). This is
-        performed by taking the mean of all (y,x) values in each sub pixel.
-
-        If the array is stored in 1D it is return as is. If it is stored in 2D, it must first be mapped from 2D to 1D.
-
-        In **PyAutoCTI** all `Array2D` objects are used in their `native` representation without sub-gridding.
-        Significant memory can be saved by only store this format, thus the `native_binned_only` config override
-        can force this behaviour. It is recommended users do not use this option to avoid unexpected behaviour.
-        """
-        if conf.instance["general"]["structures"]["native_binned_only"]:
-            return self
-
-        array_2d_slim = self.slim
-
-        binned_array_1d = np.multiply(
-            self.mask.sub_fraction,
-            array_2d_slim.reshape(-1, self.mask.sub_length).sum(axis=1),
-        )
-
-        return Array2D(
-            values=binned_array_1d,
-            mask=self.mask.derive_mask.sub_1,
-            header=self.header,
-        )
-
-    @property
     def in_counts(self) -> "Array2D":
         return self.header.array_eps_to_counts(array_eps=self)
 
     @property
     def in_counts_per_second(self) -> "Array2D":
         return self.header.array_counts_to_counts_per_second(
             array_counts=self.in_counts
         )
 
     @property
     def original_orientation(self) -> Union[np.ndarray, "Array2D"]:
         return layout_util.rotate_array_via_roe_corner_from(
-            array=self, roe_corner=self.header.original_roe_corner
+            array=np.array(self), roe_corner=self.header.original_roe_corner
         )
 
     @property
     def readout_offsets(self) -> Tuple[int, int]:
         if self.header is not None:
             if self.header.readout_offsets is not None:
                 return self.header.readout_offsets
         return (0, 0)
 
     @property
     def binned_across_rows(self) -> Array1D:
         """
         Bins the 2D array up to a 1D array, where each value is the mean of all unmasked values in each row.
         """
-        binned_array = (self.native * np.invert(self.mask)).sum(axis=0) / np.invert(
-            self.mask
-        ).sum(axis=0)
+        binned_array = np.mean(self.native.array, axis=0, where=~self.mask)
+
+        # binned_array = (self.native * np.invert(self.mask)).sum(axis=0) / np.invert(
+        #     self.mask
+        # ).sum(axis=0)
         return Array1D.no_mask(values=binned_array, pixel_scales=self.pixel_scale)
 
     @property
     def binned_across_columns(self) -> Array1D:
         """
         Bins the 2D array up to a 1D array, where each value is the mean of all unmasked values in each column.
         """
-        binned_array = (self.native * np.invert(self.mask)).sum(axis=1) / np.invert(
-            self.mask
-        ).sum(axis=1)
+        binned_array = np.mean(self.native.array, axis=1, where=~self.mask)
+
+        # binned_array = (self.native*np.invert(self.mask)).sum(axis=1)/np.invert(self.mask).sum(axis=1)
         return Array1D.no_mask(values=binned_array, pixel_scales=self.pixel_scale)
 
     def zoomed_around_mask(self, buffer: int = 1) -> "Array2D":
         """
         Extract the 2D region of an array corresponding to the rectangle encompassing all unmasked values.
 
         This is used to extract and visualize only the region of an image that is used in an analysis.
@@ -498,25 +367,24 @@
         Parameters
         ----------
         buffer
             The number pixels around the extracted array used as a buffer.
         """
 
         extracted_array_2d = array_2d_util.extracted_array_2d_from(
-            array_2d=self.native,
+            array_2d=np.array(self.native),
             y0=self.mask.zoom_region[0] - buffer,
             y1=self.mask.zoom_region[1] + buffer,
             x0=self.mask.zoom_region[2] - buffer,
             x1=self.mask.zoom_region[3] + buffer,
         )
 
         mask = Mask2D.all_false(
             shape_native=extracted_array_2d.shape,
             pixel_scales=self.pixel_scales,
-            sub_size=self.sub_size,
             origin=self.mask.mask_centre,
         )
 
         array = array_2d_util.convert_array_2d(
             array_2d=extracted_array_2d, mask_2d=mask
         )
 
@@ -533,25 +401,24 @@
 
         Parameters
         ----------
         buffer
             The number pixels around the extracted array used as a buffer.
         """
         extracted_array_2d = array_2d_util.extracted_array_2d_from(
-            array_2d=self.native,
+            array_2d=np.array(self.native),
             y0=self.mask.zoom_region[0] - buffer,
             y1=self.mask.zoom_region[1] + buffer,
             x0=self.mask.zoom_region[2] - buffer,
             x1=self.mask.zoom_region[3] + buffer,
         )
 
         mask = Mask2D.all_false(
             shape_native=extracted_array_2d.shape,
             pixel_scales=self.pixel_scales,
-            sub_size=self.sub_size,
             origin=self.mask.mask_centre,
         )
 
         return mask.geometry.extent
 
     def resized_from(
         self, new_shape: Tuple[int, int], mask_pad_value: int = 0.0
@@ -568,18 +435,18 @@
         Parameters
         ----------
         new_shape
             The new 2D shape of the array.
         """
 
         resized_array_2d = array_2d_util.resized_array_2d_from(
-            array_2d=self.native, resized_shape=new_shape
+            array_2d=np.array(self.native), resized_shape=new_shape
         )
 
-        resized_mask = self.mask.derive_mask.resized_from(
+        resized_mask = self.mask.resized_from(
             new_shape=new_shape, pad_value=mask_pad_value
         )
 
         array = array_2d_util.convert_array_2d(
             array_2d=resized_array_2d, mask_2d=resized_mask
         )
 
@@ -632,17 +499,15 @@
         psf_cut_x = int(np.ceil(kernel_shape[1] / 2)) - 1
         array_y = int(self.mask.shape[0])
         array_x = int(self.mask.shape[1])
         trimmed_array_2d = self.native[
             psf_cut_y : array_y - psf_cut_y, psf_cut_x : array_x - psf_cut_x
         ]
 
-        resized_mask = self.mask.derive_mask.resized_from(
-            new_shape=trimmed_array_2d.shape
-        )
+        resized_mask = self.mask.resized_from(new_shape=trimmed_array_2d.shape)
 
         array = array_2d_util.convert_array_2d(
             array_2d=trimmed_array_2d, mask_2d=resized_mask
         )
 
         return Array2D(
             values=array,
@@ -662,15 +527,15 @@
         files.
 
         Returns
         -------
         The HDU containing the data and its header which can then be written to .fits.
         """
         return array_2d_util.hdu_for_output_from(
-            array_2d=self.native, header_dict=self.pixel_scale_header
+            array_2d=np.array(self.native), header_dict=self.pixel_scale_header
         )
 
     def output_to_fits(self, file_path: Union[Path, str], overwrite: bool = False):
         """
         Output the array to a .fits file.
 
         The `pixel_scale` is stored in the header as `PIXSCALE`, which is used by the `Array2D.from_primary_hdu`
@@ -680,29 +545,28 @@
         ----------
         file_path
             The output path of the file, including the filename and the `.fits` extension e.g. '/path/to/filename.fits'
         overwrite
             If a file already exists at the path, if overwrite=True it is overwritten else an error is raised.
         """
         array_2d_util.numpy_array_2d_to_fits(
-            array_2d=self.native,
+            array_2d=np.array(self.native),
             file_path=file_path,
             overwrite=overwrite,
             header_dict=self.pixel_scale_header,
         )
 
 
 class Array2D(AbstractArray2D):
     @classmethod
     def no_mask(
         cls,
-        values: Union[np.ndarray, List],
+        values: Union[np.ndarray, List, AbstractArray2D],
         pixel_scales: ty.PixelScales,
         shape_native: Tuple[int, int] = None,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         header: Optional[Header] = None,
     ) -> "Array2D":
         """
         Returns an ``Array2D`` from an array via inputs in its slim or native data representation.
 
         From a ``slim`` 1D input the method cannot determine the 2D shape of the array and its mask. The
@@ -712,54 +576,38 @@
         For a full description of ``Array2D`` objects, including a description of the ``slim`` and ``native`` attribute
         used by the API, see
         the :meth:`Array2D class API documentation <autoarray.structures.arrays.uniform_2d.AbstractArray2D.__new__>`.
 
         Parameters
         ----------
         values
-            The values of the array input with shape [total_unmasked_pixels*(sub_size**2)] or
-            shape [total_y_pixels*sub_size, total_x_pixel*sub_size].
+            The values of the array input with shape [total_unmasked_pixels] or
+            shape [total_y_pixels, total_x_pixels].
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) structure.
         shape_native
             The 2D shape of the array in its ``native`` format, and its 2D mask (only required if input shape is
             in ``slim`` format).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
 
         Examples
         --------
 
         .. code-block:: python
 
             import autoarray as aa
 
-            # Make Array2D from input list, native format with sub_size 1
+            # Make Array2D from input list, native format
             # (This array has shape_native=(2,2)).
 
             array_2d = aa.Array2D.manual(
                 array=np.array([[1.0, 2.0], [3.0, 4.0]]),
                 pixel_scales=1.0.
-                sub_size=1
-            )
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            # Make Array2D from input list, slim format with sub_size 2.
-
-            array_2d = aa.Array2D.no_mask(
-                values=[1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0],
-                shape_native=(2, 1),
-                pixel_scales=1.0,
-                sub_size=2,
             )
         """
 
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         values = array_2d_util.convert_array(array=values)
 
@@ -781,34 +629,32 @@
                     """
                     The input shape_native parameter is not a tuple of type (int, int)
                     """
                 )
 
         else:
             shape_native = (
-                int(values.shape[0] / sub_size),
-                int(values.shape[1] / sub_size),
+                int(values.shape[0]),
+                int(values.shape[1]),
             )
 
         mask = Mask2D.all_false(
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
         return Array2D(values=values, mask=mask, header=header)
 
     @classmethod
     def full(
         cls,
         fill_value: float,
         shape_native: Tuple[int, int],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         header: Optional[Header] = None,
     ) -> "Array2D":
         """
         Returns an ``Array2D`` where all values are filled with an input fill value, analogous to ``np.full()``.
 
         For a full description of ``Array2D`` objects, including a description of the ``slim`` and ``native`` attribute
@@ -824,66 +670,42 @@
         fill_value
             The value all array elements are filled with.
         shape_native
             The 2D shape of the array in its ``native`` format, and its 2D mask.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) structure.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
 
         Examples
         --------
 
         .. code-block:: python
 
             import autoarray as aa
 
-            # Make Array2D with sub_size 1.
-
             array_2d = aa.Array2D.full(
                 fill_value=2.0,
                 shape_native=(2, 2),
                 pixel_scales=1.0,
-                sub_size=1
             )
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            # Make Array2D with sub_size 2.
-
-            array_2d = aa.Array2D.full(
-                fill_value=2.0,
-                shape_native=(2, 2),
-                pixel_scales=1.0,
-                sub_size=2
-            )
-
         """
-        if sub_size is not None:
-            shape_native = (shape_native[0] * sub_size, shape_native[1] * sub_size)
-
         return cls.no_mask(
             values=np.full(fill_value=fill_value, shape=shape_native),
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             header=header,
         )
 
     @classmethod
     def ones(
         cls,
         shape_native: Tuple[int, int],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         header: Header = None,
     ) -> "Array2D":
         """
         Returns an ``Array2D`` where all values are filled with ones, analogous to ``np.ones()``.
 
         For a full description of ``Array2D`` objects, including a description of the ``slim`` and ``native`` attribute
@@ -897,61 +719,42 @@
         Parameters
         ----------
         shape_native
             The 2D shape of the array in its ``native`` format, and its 2D mask.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) structure.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
 
         Examples
         --------
 
         .. code-block:: python
 
             import autoarray as aa
 
-            # Make Array2D with sub_size 1.
-
-            array_2d = aa.Array2D.ones(
-                shape_native=(2, 2),
-                pixel_scales=1.0,
-                sub_size=1
-            )
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            # Make Array2D with sub_size 2.
-
             array_2d = aa.Array2D.ones(
                 shape_native=(2, 2),
                 pixel_scales=1.0,
-                sub_size=2
             )
         """
         return cls.full(
             fill_value=1.0,
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             header=header,
         )
 
     @classmethod
     def zeros(
         cls,
         shape_native: Tuple[int, int],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
         header: Header = None,
     ) -> "Array2D":
         """
         Returns an ``Array2D`` where all values are filled with zeros, analogous to ``np.zeros()``.
 
         For a full description of ``Array2D`` objects, including a description of the ``slim`` and ``native`` attribute
@@ -965,62 +768,43 @@
         Parameters
         ----------
         shape_native
             The 2D shape of the array in its ``native`` format, and its 2D mask.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) structure.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
 
         Examples
         --------
 
         .. code-block:: python
 
             import autoarray as aa
 
-            # Make Array2D with sub_size 1.
-
-            array_2d = aa.Array2D.zeros(
-                shape_native=(2, 2),
-                pixel_scales=1.0,
-                sub_size=1
-            )
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            # Make Array2D with sub_size 2.
-
             array_2d = aa.Array2D.zeros(
                 shape_native=(2, 2),
                 pixel_scales=1.0,
-                sub_size=2
             )
         """
         return cls.full(
             fill_value=0.0,
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             header=header,
         )
 
     @classmethod
     def from_fits(
         cls,
         file_path: Union[Path, str],
         pixel_scales: Optional[ty.PixelScales],
         hdu: int = 0,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
     ) -> "Array2D":
         """
         Returns an ``Array2D`` by loading the array values from a .fits file.
 
         For a full description of ``Array2D`` objects, including a description of the ``slim`` and ``native`` attribute
         used by the API, see
@@ -1032,70 +816,48 @@
             The path the file is loaded from, including the filename and the `.fits` extension,
             e.g. '/path/to/filename.fits'
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) structure.
         hdu
             The Header-Data Unit of the .fits file the array data is loaded from.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the coordinate system.
 
         Examples
         --------
 
         .. code-block:: python
 
             import autoarray as aa
 
-            # Make Array2D with sub_size 1.
-
             array_2d = aa.Array2D.from_fits(
                 file_path="path/to/file.fits",
                 hdu=0,
                 pixel_scales=1.0,
-                sub_size=1
-            )
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            # Make Array2D with sub_size 2.
-            # (It is uncommon that a sub-gridded array would be loaded from
-            # a .fits, but the API support its).
-
-            array_2d = aa.Array2D.from_fits(
-                file_path="path/to/file.fits",
-                hdu=0,
-                pixel_scales=1.0,
-                sub_size=2
             )
         """
         array_2d = array_2d_util.numpy_array_2d_via_fits_from(
             file_path=file_path, hdu=hdu
         )
 
         header_sci_obj = array_2d_util.header_obj_from(file_path=file_path, hdu=0)
         header_hdu_obj = array_2d_util.header_obj_from(file_path=file_path, hdu=hdu)
 
         return cls.no_mask(
             values=array_2d,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
             header=Header(header_sci_obj=header_sci_obj, header_hdu_obj=header_hdu_obj),
         )
 
     @classmethod
     def from_primary_hdu(
         cls,
         primary_hdu: fits.PrimaryHDU,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
     ) -> "Array2D":
         """
         Returns an ``Array2D`` by from a `PrimaryHDU` object which has been loaded via `astropy.fits`
 
         This assumes that the `header` of the `PrimaryHDU` contains an entry named `PIXSCALE` which gives the
         pixel-scale of the array.
@@ -1105,148 +867,107 @@
         the :meth:`Array2D class API documentation <autoarray.structures.arrays.uniform_2d.AbstractArray2D.__new__>`.
 
         Parameters
         ----------
         primary_hdu
             The `PrimaryHDU` object which has already been loaded from a .fits file via `astropy.fits` and contains
             the array data and the pixel-scale in the header with an entry named `PIXSCALE`.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-array.
         origin
             The (y,x) scaled units origin of the coordinate system.
 
         Examples
         --------
 
         .. code-block:: python
 
             from astropy.io import fits
             import autoarray as aa
 
-            # Make Array2D with sub_size 1.
-
             primary_hdu = fits.open("path/to/file.fits")
 
             array_2d = aa.Array2D.from_primary_hdu(
                 primary_hdu=primary_hdu,
-                sub_size=1
-            )
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            # Make Array2D with sub_size 2.
-            # (It is uncommon that a sub-gridded array would be loaded from
-            # a .fits, but the API support its).
-
-             primary_hdu = fits.open("path/to/file.fits")
-
-            array_2d = aa.Array2D.from_primary_hdu(
-                primary_hdu=primary_hdu,
-                sub_size=2
             )
         """
 
         return cls.no_mask(
             values=cls.flip_hdu_for_ds9(primary_hdu.data.astype("float")),
             pixel_scales=primary_hdu.header["PIXSCALE"],
-            sub_size=sub_size,
             origin=origin,
             header=Header(header_sci_obj=primary_hdu.header),
         )
 
     @classmethod
     def from_yx_and_values(
         cls,
         y: Union[np.ndarray, List],
         x: Union[np.ndarray, List],
         values: Union[np.ndarray, List],
         shape_native: Tuple[int, int],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         header: Header = None,
     ) -> "Array2D":
         """
-        Returns an ``Array2D`` by by inputting the y and x pixel values where the array is filled and the values that
+        Returns an ``Array2D`` by inputting the y and x pixel values where the array is filled and the values that
         fill it.
 
         For a full description of ``Array2D`` objects, including a description of the ``slim`` and ``native`` attribute
         used by the API, see
         the :meth:`Array2D class API documentation <autoarray.structures.arrays.uniform_2d.AbstractArray2D.__new__>`.
 
         Parameters
         ----------
         y
-            The y pixel indexes where value are input, with shape [total_unmasked_pixels*sub_size].
+            The y pixel indexes where value are input, with shape [total_unmasked_pixels].
         x
-            The x pixel indexes where value are input, with shape [total_unmasked_pixels*sub_size].
+            The x pixel indexes where value are input, with shape [total_unmasked_pixels].
         values or list
-            The values which are used to fill in the array, with shape [total_unmasked_pixels*sub_size].
+            The values which are used to fill in the array, with shape [total_unmasked_pixel].
         shape_native
             The 2D shape of the array in its ``native`` format, and its 2D mask.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) structure.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
         origin
             The origin of the grid's mask.
 
         Examples
         --------
         .. code-block:: python
 
             import autoarray as aa
 
-            # Make Array2D with sub_size 1.
-
             array_2d = aa.Array2D.from_yx_and_values(
                 y=np.array([0.5, 0.5, -0.5, -0.5]),
                 x=np.array([-0.5, 0.5, -0.5, 0.5]),
                 values=np.array([1.0, 2.0, 3.0, 4.0]),
                 shape_native=(2, 2),
                 pixel_scales=1.0,
-                sub_size=1,
-            )
-
-        .. code-block:: python
-
-            import autoarray as aa
-
-            # Make Array2D with sub_size 2.
-
-            array_2d = aa.Array2D.from_yx_and_values(
-                y=np.array([1.0, 1.0. 0.5, 0.5, -0.5, -0.5, -1.0, -1.0]),
-                x=np.array([-0.5, 0.5, -0.5, 0.5, -0.5, 0.5, -0.5, 0.5]),
-                values=np.array([1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0]),
-                shape_native=(2, 1),
-                pixel_scales=1.0,
-                sub_size=2,
             )
         """
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         from autoarray.structures.grids.uniform_2d import Grid2D
 
         grid = Grid2D.from_yx_1d(
-            y=y, x=x, shape_native=shape_native, pixel_scales=pixel_scales, sub_size=1
+            y=y,
+            x=x,
+            shape_native=shape_native,
+            pixel_scales=pixel_scales,
         )
 
         grid_pixels = geometry_util.grid_pixel_indexes_2d_slim_from(
-            grid_scaled_2d_slim=grid.slim,
+            grid_scaled_2d_slim=np.array(grid.slim),
             shape_native=shape_native,
             pixel_scales=pixel_scales,
         )
 
-        array_1d = np.zeros(shape=shape_native[0] * shape_native[1])
-
-        for i in range(grid_pixels.shape[0]):
-            array_1d[i] = values[int(grid_pixels[i])]
+        array_1d = np.array(
+            [values[int(grid_pixels[i])] for i in range(grid_pixels.shape[0])]
+        )
 
         return cls.no_mask(
             values=array_1d,
             pixel_scales=pixel_scales,
             shape_native=shape_native,
-            sub_size=sub_size,
             header=header,
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/grids/grid_1d_util.py` & `autoarray-2024.5.16.0/autoarray/structures/grids/grid_1d_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ) -> np.ndarray:
     """
     The `manual` classmethods in the Grid2D object take as input a list or ndarray which is returned as a Grid2D.
 
     This function performs the following and checks and conversions on the input:
 
     1: If the input is a list, convert it to an ndarray.
-    2: Check that the number of sub-pixels in the array is identical to that of the mask.
+    2: Check that the number of pixels in the array is identical to that of the mask.
     3) Map the input ndarray to its `slim` representation.
 
     For a Grid2D, `slim` refers to a 2D NumPy array of shape [total_coordinates, 2] and `native` a 3D NumPy array of
     shape [total_y_coordinates, total_x_coordinates, 2]
 
     Parameters
     ----------
@@ -37,143 +37,126 @@
     store_native
         If True, the ndarray is stored in its native format [total_y_pixels, total_x_pixels, 2]. This avoids
         mapping large data arrays to and from the slim / native formats, which can be a computational bottleneck.
     """
 
     grid_1d = grid_2d_util.convert_grid(grid=grid_1d)
 
-    is_native = grid_1d.shape[0] == mask_1d.sub_shape_native[0]
+    is_native = grid_1d.shape[0] == mask_1d.shape_native[0]
 
     if is_native == store_native:
         return grid_1d
     elif not store_native:
         return grid_1d_slim_from(
-            grid_1d_native=grid_1d, mask_1d=mask_1d, sub_size=mask_1d.sub_size
+            grid_1d_native=grid_1d,
+            mask_1d=np.array(mask_1d),
         )
     return grid_1d_native_from(
-        grid_1d_slim=grid_1d, mask_1d=mask_1d, sub_size=mask_1d.sub_size
+        grid_1d_slim=grid_1d,
+        mask_1d=np.array(mask_1d),
     )
 
 
 def grid_1d_slim_via_shape_slim_from(
     shape_slim: Tuple[int],
     pixel_scales: ty.PixelScales,
-    sub_size: int,
     origin: Tuple[float] = (0.0,),
 ) -> np.ndarray:
     """
-    For a sub-grid, every unmasked pixel of its 1D mask with shape (total_pixels,) is divided into a finer uniform
-    grid of shape (total_pixels*sub_size, ). This routine computes the (x) scaled coordinates at the centre of every
-    sub-pixel defined by a 1D shape of the overall grid.
-
-    Grid2D are defined from left to right, where the first unmasked sub-pixel corresponds to index 0. Sub-pixels that
-    are part of the same mask array pixel are indexed next to one another, such that the second
-    sub-pixel in the first pixel has index 1, its next sub-pixel has index 2, and so forth.
+    This routine computes the (x) scaled coordinates at the centre of every pixel defined by a 1D shape of the
+    overall grid.
 
-    The sub-grid is returned on an array of shape (total_unmasked_pixels*sub_size, ).
+    Grid2D are defined from left to right, where the first unmasked pixel corresponds to index 0.
+
+    The grid is returned on an array of shape (total_unmasked_pixels, ).
 
     Parameters
     ----------
     shape_slim
-        The (x) shape of the 1D array the sub-grid of coordinates is computed for.
+        The (x) shape of the 1D array the grid of coordinates is computed for.
     pixel_scales
         The (x) scaled units to pixel units conversion factor of the 1D mask array.
-    sub_size
-        The size of the sub-grid that each pixel of the 1D mask array is divided into.
     origin
-        The (x) origin of the 1D array, which the sub-grid is shifted around.
+        The (x) origin of the 1D array, which the grid is shifted around.
 
     Returns
     -------
     ndarray
-        A sub grid of (x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
-        array. The sub grid array has dimensions (total_unmasked_pixels*sub_size, ).
+        A grid of (x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
+        array. The grid array has dimensions (total_unmasked_pixels, ).
 
     Examples
     --------
-    sub_grid_1d = grid_1d_via_shape_slim_from(mask=mask, pixel_scales=(0.5, 0.5), sub_size=2, origin=(0.0, 0.0))
+    grid_1d = grid_1d_via_shape_slim_from(mask=mask, pixel_scales=(0.5, 0.5), origin=(0.0, 0.0))
     """
     return grid_1d_slim_via_mask_from(
         mask_1d=np.full(fill_value=False, shape=shape_slim),
         pixel_scales=pixel_scales,
-        sub_size=sub_size,
         origin=origin,
     )
 
 
 @numba_util.jit()
 def grid_1d_slim_via_mask_from(
     mask_1d: np.ndarray,
     pixel_scales: ty.PixelScales,
-    sub_size: int,
     origin: Tuple[float] = (0.0,),
 ) -> np.ndarray:
     """
-    For a sub-grid, every unmasked pixel of its 1D mask with shape (total_pixels,) is divided into a finer uniform
-    grid of shape (total_pixels*sub_size, ). This routine computes the (x) scaled coordinates at the centre of every
-    sub-pixel defined by this 1D mask array.
-
-    Grid2D are defined from left to right, where the first unmasked sub-pixel corresponds to index 0. Sub-pixels that
-    are part of the same mask array pixel are indexed next to one another, such that the second
-    sub-pixel in the first pixel has index 1, its next sub-pixel has index 2, and so forth.
+    For a grid, every unmasked pixel of its 1D mask with shape (total_pixels,) is divided into a finer uniform
+    grid of shape (total_pixels, ). This routine computes the (x) scaled coordinates at the centre of every
+    pixel defined by this 1D mask array.
+
+    Grid2D are defined from left to right, where the first unmasked pixel corresponds to index 0.
 
-    The sub-grid is returned on an array of shape (total_unmasked_pixels*sub_size, ).
+    The grid is returned on an array of shape (total_unmasked_pixels, ).
 
     Parameters
     ----------
     mask_1d
         A 1D array of bools, where `False` values are unmasked and therefore included as part of the calculated
-        sub-grid.
+        grid.
     pixel_scales
         The (x) scaled units to pixel units conversion factor of the 2D mask array.
-    sub_size
-        The size of the sub-grid that each pixel of the 2D mask array is divided into.
     origin
-        The (x) origin of the 2D array, which the sub-grid is shifted around.
+        The (x) origin of the 2D array, which the grid is shifted around.
 
     Returns
     -------
     ndarray
-        A sub grid of (x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
-        array. The sub grid array has dimensions (total_unmasked_pixels*sub_size, ).
+        A grid of (x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
+        array. The grid array has dimensions (total_unmasked_pixels, ).
 
     Examples
     --------
     mask = np.array([True, False, True, False, False, False])
-    grid_slim = grid_1d_via_mask_from(mask_1d=mask_1d, pixel_scales=(0.5, 0.5), sub_size=1, origin=(0.0, 0.0))
+    grid_slim = grid_1d_via_mask_from(mask_1d=mask_1d, pixel_scales=(0.5, 0.5), origin=(0.0, 0.0))
     """
 
-    total_sub_pixels = mask_1d_util.total_sub_pixels_1d_from(mask_1d, sub_size)
+    total_pixels = mask_1d_util.total_pixels_1d_from(mask_1d)
 
-    grid_1d = np.zeros(shape=(total_sub_pixels,))
+    grid_1d = np.zeros(shape=(total_pixels,))
 
     centres_scaled = geometry_util.central_scaled_coordinate_1d_from(
         shape_slim=mask_1d.shape, pixel_scales=pixel_scales, origin=origin
     )
 
-    sub_index = 0
-
-    x_sub_half = pixel_scales[0] / 2
-    x_sub_step = pixel_scales[0] / (sub_size)
+    index = 0
 
     for x in range(mask_1d.shape[0]):
         if not mask_1d[x]:
-            x_scaled = (x - centres_scaled[0]) * pixel_scales[0]
-
-            for x1 in range(sub_size):
-                grid_1d[sub_index] = (
-                    x_scaled - x_sub_half + x1 * x_sub_step + (x_sub_step / 2.0)
-                )
-                sub_index += 1
+            grid_1d[index] = (x - centres_scaled[0]) * pixel_scales[0]
+            index += 1
 
     return grid_1d
 
 
 def grid_1d_slim_from(
-    grid_1d_native: np.ndarray, mask_1d: np.ndarray, sub_size: int
+    grid_1d_native: np.ndarray,
+    mask_1d: np.ndarray,
 ) -> np.ndarray:
     """
     For a native 1D grid and mask of shape [total_pixels], map the values of all unmasked pixels to a slimmed grid of
     shape [total_unmasked_pixels].
 
     The pixel coordinate origin is at the left of the native grid and goes right-wards, such
     that for a grid of shape (4,) where pixels 0, 1 and 3 are unmasked:
@@ -184,34 +167,34 @@
 
     Parameters
     ----------
     grid_1d_native : ndarray
         The native grid of (x) values which are mapped to the slimmed grid.
     mask_1d
         A 1D array of bools, where `False` values mean unmasked and are included in the mapping.
-    sub_size
-        The size (sub_size x sub_size) of each unmasked pixels sub-array.
 
     Returns
     -------
     ndarray
         A 1D slim grid of values mapped from the 1D native grid with dimensions (total_unmasked_pixels).
     """
 
     return array_1d_util.array_1d_slim_from(
-        array_1d_native=grid_1d_native, mask_1d=mask_1d, sub_size=sub_size
+        array_1d_native=np.array(grid_1d_native),
+        mask_1d=mask_1d,
     )
 
 
 def grid_1d_native_from(
-    grid_1d_slim: np.ndarray, mask_1d: np.ndarray, sub_size: int
+    grid_1d_slim: np.ndarray,
+    mask_1d: np.ndarray,
 ) -> np.ndarray:
     """
-    For a slimmed 1D grid of shape [total_unmasked_pixels*sub_size], that was computed by extracting the unmasked values
-    from a native 1D grid of shape [total_pixels*sub_size], map the slimmed grid's coordinates back to the native 1D
+    For a slimmed 1D grid of shape [total_unmasked_pixels], that was computed by extracting the unmasked values
+    from a native 1D grid of shape [total_pixels], map the slimmed grid's coordinates back to the native 1D
     grid where masked values are set to zero.
 
     This uses a 1D array 'slim_to_native' where each index gives the 1D pixel indexes of the grid's native unmasked
     pixels, for example:
 
     - If slim_to_native[0] = [0], the first value of the 1D slimmed grid maps to the pixel [0] of the native 1D grid.
     - If slim_to_native[1] = [2], the second value of the 1D slimmed grid maps to the pixel [2] of the native 1D grid.
@@ -219,19 +202,18 @@
 
     Parameters
     ----------
     grid_1d_slim
         The (x) values of the slimmed 1D grid which are mapped to the native 1D grid.
     mask_1d
         A 1D array of bools, where `False` values means unmasked and are included in the mapping.
-    sub_size
-        The size of each unmasked pixels sub-grid.
 
     Returns
     -------
     ndarray
-        A NumPy array of shape [total_pixels*sub_size] corresponding to the (x) values of the native 1D
+        A NumPy array of shape [total_pixels] corresponding to the (x) values of the native 1D
         mapped from the slimmed grid.
     """
     return array_1d_util.array_1d_native_from(
-        array_1d_slim=grid_1d_slim, mask_1d=mask_1d, sub_size=sub_size
+        array_1d_slim=grid_1d_slim,
+        mask_1d=mask_1d,
     )
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/grids/grid_2d_util.py` & `autoarray-2024.5.16.0/autoarray/structures/grids/grid_2d_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,85 +49,85 @@
 
     if 2 < len(grid_2d.shape) > 3:
         raise exc.GridException("The dimensions of the input grid array is not 2 or 3")
 
 
 def check_grid_2d_and_mask_2d(grid_2d: np.ndarray, mask_2d: Mask2D):
     if len(grid_2d.shape) == 2:
-        if grid_2d.shape[0] != mask_2d.sub_pixels_in_mask:
+        if grid_2d.shape[0] != mask_2d.pixels_in_mask:
             raise exc.GridException(
                 f"""
-                The input 2D grid does not have the same number of values as sub-pixels in
+                The input 2D grid does not have the same number of values as pixels in
                 the mask.
                 
                 The shape of the input grid_2d is {grid_2d.shape}.
                 The mask shape_native is {mask_2d.shape_native}.
-                The mask number of sub-pixels is {mask_2d.sub_pixels_in_mask}. 
-                The mask sub size is {mask_2d.sub_size}).
+                The mask number of pixels is {mask_2d.pixels_in_mask}. 
                 """
             )
 
     elif len(grid_2d.shape) == 3:
-        if (grid_2d.shape[0], grid_2d.shape[1]) != mask_2d.sub_shape_native:
+        if (grid_2d.shape[0], grid_2d.shape[1]) != mask_2d.shape_native:
             raise exc.GridException(
                 f"""
-                The input 2D grid is not the same dimensions as the sub-mask
-                (e.g. the mask 2D shape multipled by its sub size.)
+                The input 2D grid is not the same dimensions as the mask
+                (e.g. the mask 2D shape.)
 
                 The shape of the input grid_2d is {grid_2d.shape}.
-                The sub_shape_native of the mask is {mask_2d.sub_shape_native} (the 
-                mask sub size is {mask_2d.sub_size}).
+                The mask shape_native is {mask_2d.shape_native}.
                 """
             )
 
 
 def convert_grid_2d(
     grid_2d: Union[np.ndarray, List], mask_2d: Mask2D, store_native: bool = False
 ) -> np.ndarray:
     """
     The `manual` classmethods in the Grid2D object take as input a list or ndarray which is returned as a Grid2D.
 
     This function performs the following and checks and conversions on the input:
 
     1: If the input is a list, convert it to an ndarray.
-    2: Check that the number of sub-pixels in the array is identical to that of the mask.
+    2: Check that the number of coordinates in the grid is identical to that of the mask.
     3) Map the input ndarray to its `slim` representation.
 
     For a Grid2D, `slim` refers to a 2D NumPy array of shape [total_coordinates, 2] and `native` a 3D NumPy array of
     shape [total_y_coordinates, total_x_coordinates, 2]
 
     Parameters
     ----------
     grid_2d
-        The input (y,x) grid of coordinates which is converted to an ndarray if it is a list.
+        The input (y,x) grid of coordinates which is converted to a ndarray if it is a list.
     mask_2d
         The mask of the output Array2D.
     store_native
         If True, the ndarray is stored in its native format [total_y_pixels, total_x_pixels, 2]. This avoids
         mapping large data arrays to and from the slim / native formats, which can be a computational bottleneck.
     """
 
     grid_2d = convert_grid(grid=grid_2d)
 
     check_grid_2d_and_mask_2d(grid_2d=grid_2d, mask_2d=mask_2d)
 
     is_native = len(grid_2d.shape) == 3
 
     if is_native:
-        grid_2d[:, :, 0] *= np.invert(mask_2d.derive_mask.sub)
-        grid_2d[:, :, 1] *= np.invert(mask_2d.derive_mask.sub)
+        grid_2d[:, :, 0] *= np.invert(mask_2d)
+        grid_2d[:, :, 1] *= np.invert(mask_2d)
 
     if is_native == store_native:
         return grid_2d
     elif not store_native:
         return grid_2d_slim_from(
-            grid_2d_native=grid_2d, mask=mask_2d, sub_size=mask_2d.sub_size
+            grid_2d_native=np.array(grid_2d),
+            mask=np.array(mask_2d),
         )
     return grid_2d_native_from(
-        grid_2d_slim=grid_2d, mask_2d=mask_2d, sub_size=mask_2d.sub_size
+        grid_2d_slim=np.array(grid_2d),
+        mask_2d=np.array(mask_2d),
     )
 
 
 def convert_grid_2d_to_slim(
     grid_2d: Union[np.ndarray, List], mask_2d: Mask2D
 ) -> np.ndarray:
     """
@@ -143,15 +143,16 @@
         The input (y,x) grid of coordinates which is converted to its silm representation.
     mask_2d
         The mask of the output Array2D.
     """
     if len(grid_2d.shape) == 2:
         return grid_2d
     return grid_2d_slim_from(
-        grid_2d_native=grid_2d, mask=mask_2d, sub_size=mask_2d.sub_size
+        grid_2d_native=grid_2d,
+        mask=mask_2d,
     )
 
 
 def convert_grid_2d_to_native(
     grid_2d: Union[np.ndarray, List], mask_2d: Mask2D
 ) -> np.ndarray:
     """
@@ -167,15 +168,16 @@
         The input (y,x) grid of coordinates which is converted to its native representation.
     mask_2d
         The mask of the output Array2D.
     """
     if len(grid_2d.shape) == 3:
         return grid_2d
     return grid_2d_native_from(
-        grid_2d_slim=grid_2d, mask_2d=mask_2d, sub_size=mask_2d.sub_size
+        grid_2d_slim=grid_2d,
+        mask_2d=mask_2d,
     )
 
 
 @numba_util.jit()
 def grid_2d_centre_from(grid_2d_slim: np.ndarray) -> Tuple[float, float]:
     """
     Returns the centre of a grid from a 1D grid.
@@ -195,248 +197,207 @@
     return centre_y, centre_x
 
 
 @numba_util.jit()
 def grid_2d_slim_via_mask_from(
     mask_2d: np.ndarray,
     pixel_scales: ty.PixelScales,
-    sub_size: int,
     origin: Tuple[float, float] = (0.0, 0.0),
 ) -> np.ndarray:
     """
-    For a sub-grid, every unmasked pixel of its 2D mask with shape (total_y_pixels, total_x_pixels) is divided into
-    a finer uniform grid of shape (total_y_pixels*sub_size, total_x_pixels*sub_size). This routine computes the (y,x)
-    scaled coordinates a the centre of every sub-pixel defined by this 2D mask array.
-
-    The sub-grid is returned on an array of shape (total_unmasked_pixels*sub_size**2, 2). y coordinates are
-    stored in the 0 index of the second dimension, x coordinates in the 1 index. Masked coordinates are therefore
-    removed and not included in the slimmed grid.
-
-    Grid2D are defined from the top-left corner, where the first unmasked sub-pixel corresponds to index 0.
-    Sub-pixels that are part of the same mask array pixel are indexed next to one another, such that the second
-    sub-pixel in the first pixel has index 1, its next sub-pixel has index 2, and so forth.
+    For a grid, every unmasked pixel is on a 2D mask with shape (total_y_pixels, total_x_pixels). This routine
+    computes the (y,x) scaled coordinates a the centre of every pixel defined by this 2D mask array.
+
+    The grid is returned on an array of shape (total_unmasked_pixels, 2). y coordinates are stored in the 0 index of
+    the second dimension, x coordinates in the 1 index. Masked coordinates are therefore removed and not included in
+    the slimmed grid.
+
+    Grid2D are defined from the top-left corner, where the first unmasked pixel corresponds to index 0.
 
     Parameters
     ----------
     mask_2d
         A 2D array of bools, where `False` values are unmasked and therefore included as part of the calculated
-        sub-grid.
+        grid.
     pixel_scales
         The (y,x) scaled units to pixel units conversion factor of the 2D mask array.
-    sub_size
-        The size of the sub-grid that each pixel of the 2D mask array is divided into.
     origin
-        The (y,x) origin of the 2D array, which the sub-grid is shifted around.
+        The (y,x) origin of the 2D array, which the grid is shifted around.
 
     Returns
     -------
     ndarray
-        A slimmed sub grid of (y,x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
-        array. The sub grid array has dimensions (total_unmasked_pixels*sub_size**2, 2).
+        A slimmed grid of (y,x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
+        array. The grid array has dimensions (total_unmasked_pixels, 2).
 
     Examples
     --------
     mask = np.array([[True, False, True],
                      [False, False, False]
                      [True, False, True]])
-    grid_slim = grid_2d_slim_via_mask_from(mask=mask, pixel_scales=(0.5, 0.5), sub_size=1, origin=(0.0, 0.0))
+    grid_slim = grid_2d_slim_via_mask_from(mask=mask, pixel_scales=(0.5, 0.5), origin=(0.0, 0.0))
     """
 
-    total_sub_pixels = mask_2d_util.total_sub_pixels_2d_from(mask_2d, sub_size)
+    total_pixels = mask_2d_util.total_pixels_2d_from(mask_2d)
 
-    grid_slim = np.zeros(shape=(total_sub_pixels, 2))
+    grid_slim = np.zeros(shape=(total_pixels, 2))
 
     centres_scaled = geometry_util.central_scaled_coordinate_2d_from(
         shape_native=mask_2d.shape, pixel_scales=pixel_scales, origin=origin
     )
 
-    sub_index = 0
-
-    y_sub_half = pixel_scales[0] / 2
-    y_sub_step = pixel_scales[0] / (sub_size)
-
-    x_sub_half = pixel_scales[1] / 2
-    x_sub_step = pixel_scales[1] / (sub_size)
+    index = 0
 
     for y in range(mask_2d.shape[0]):
         for x in range(mask_2d.shape[1]):
             if not mask_2d[y, x]:
-                y_scaled = (y - centres_scaled[0]) * pixel_scales[0]
-                x_scaled = (x - centres_scaled[1]) * pixel_scales[1]
-
-                for y1 in range(sub_size):
-                    for x1 in range(sub_size):
-                        grid_slim[sub_index, 0] = -(
-                            y_scaled - y_sub_half + y1 * y_sub_step + (y_sub_step / 2.0)
-                        )
-                        grid_slim[sub_index, 1] = (
-                            x_scaled - x_sub_half + x1 * x_sub_step + (x_sub_step / 2.0)
-                        )
-                        sub_index += 1
+                grid_slim[index, 0] = -(y - centres_scaled[0]) * pixel_scales[0]
+                grid_slim[index, 1] = (x - centres_scaled[1]) * pixel_scales[1]
+                index += 1
 
     return grid_slim
 
 
 def grid_2d_via_mask_from(
     mask_2d: np.ndarray,
     pixel_scales: ty.PixelScales,
-    sub_size: int,
     origin: Tuple[float, float] = (0.0, 0.0),
 ) -> np.ndarray:
     """
-    For a sub-grid, every unmasked pixel of its 2D mask with shape (total_y_pixels, total_x_pixels) is divided into a
-    finer uniform grid of shape (total_y_pixels*sub_size, total_x_pixels*sub_size). This routine computes the (y,x)
-    scaled coordinates at the centre of every sub-pixel defined by this 2D mask array.
-
-    The sub-grid is returned in its native dimensions with shape (total_y_pixels*sub_size, total_x_pixels*sub_size).
-    y coordinates are stored in the 0 index of the second dimension, x coordinates in the 1 index. Masked pixels are
-    given values (0.0, 0.0).
-
-    Grids are defined from the top-left corner, where the first unmasked sub-pixel corresponds to index 0.
-    Sub-pixels that are part of the same mask array pixel are indexed next to one another, such that the second
-    sub-pixel in the first pixel has index 1, its next sub-pixel has index 2, and so forth.
+    For a grid, every unmasked pixel is on a 2D mask with shape (total_y_pixels, total_x_pixels). This routine computes
+    the (y,x) scaled coordinates at the centre of every pixel defined by this 2D mask array.
+
+    The grid is returned in its native dimensions with shape (total_y_pixels, total_x_pixels). y coordinates are
+    stored in the 0 index of the second dimension, x coordinates in the 1 index. Masked pixels are given
+    values (0.0, 0.0).
+
+    Grids are defined from the top-left corner, where the first unmasked pixel corresponds to index 0.
 
     Parameters
     ----------
     mask_2d
         A 2D array of bools, where `False` values are unmasked and therefore included as part of the calculated
-        sub-grid.
+        grid.
     pixel_scales
         The (y,x) scaled units to pixel units conversion factor of the 2D mask array.
-    sub_size
-        The size of the sub-grid that each pixel of the 2D mask array is divided into.
     origin
-        The (y,x) origin of the 2D array, which the sub-grid is shifted around.
+        The (y,x) origin of the 2D array, which the grid is shifted around.
 
     Returns
     -------
     ndarray
-        A sub grid of (y,x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
-        array. The sub grid array has dimensions (total_y_pixels*sub_size, total_x_pixels*sub_size).
+        A grid of (y,x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
+        array. The grid array has dimensions (total_y_pixels, total_x_pixels).
 
     Examples
     --------
     mask = np.array([[True, False, True],
                      [False, False, False]
                      [True, False, True]])
-    grid_2d = grid_2d_via_mask_from(mask=mask, pixel_scales=(0.5, 0.5), sub_size=1, origin=(0.0, 0.0))
+    grid_2d = grid_2d_via_mask_from(mask=mask, pixel_scales=(0.5, 0.5), origin=(0.0, 0.0))
     """
 
     grid_2d_slim = grid_2d_slim_via_mask_from(
-        mask_2d=mask_2d, pixel_scales=pixel_scales, sub_size=sub_size, origin=origin
+        mask_2d=mask_2d, pixel_scales=pixel_scales, origin=origin
     )
 
     return grid_2d_native_from(
-        grid_2d_slim=grid_2d_slim, mask_2d=mask_2d, sub_size=sub_size
+        grid_2d_slim=grid_2d_slim,
+        mask_2d=mask_2d,
     )
 
 
 def grid_2d_slim_via_shape_native_from(
     shape_native: Tuple[int, int],
     pixel_scales: ty.PixelScales,
-    sub_size: int,
     origin: Tuple[float, float] = (0.0, 0.0),
 ) -> np.ndarray:
     """
-    For a sub-grid, every unmasked pixel of its 2D mask with shape (total_y_pixels, total_x_pixels) is divided into a
-    finer uniform grid of shape (total_y_pixels*sub_size, total_x_pixels*sub_size). This routine computes the (y,x)
-    scaled coordinates at the centre of every sub-pixel defined by this 2D mask array.
+    For a grid, every unmasked pixel is in a 2D mask with shape (total_y_pixels, total_x_pixels). This routine computes
+    the (y,x) scaled coordinates at the centre of every pixel defined by this 2D mask array.
 
-    The sub-grid is returned in its slimmed dimensions with shape (total_pixels**2*sub_size**2, 2). y coordinates are
+    The grid is returned in its slimmed dimensions with shape (total_pixels, 2). y coordinates are
     stored in the 0 index of the second dimension, x coordinates in the 1 index.
 
-    Grid2D are defined from the top-left corner, where the first sub-pixel corresponds to index [0,0].
-    Sub-pixels that are part of the same mask array pixel are indexed next to one another, such that the second
-    sub-pixel in the first pixel has index 1, its next sub-pixel has index 2, and so forth.
+    Grid2D are defined from the top-left corner, where the first pixel corresponds to index [0,0].
 
     Parameters
     ----------
     shape_native
-        The (y,x) shape of the 2D array the sub-grid of coordinates is computed for.
+        The (y,x) shape of the 2D array the grid of coordinates is computed for.
     pixel_scales
         The (y,x) scaled units to pixel units conversion factor of the 2D mask array.
-    sub_size
-        The size of the sub-grid that each pixel of the 2D mask array is divided into.
     origin
-        The (y,x) origin of the 2D array, which the sub-grid is shifted around.
+        The (y,x) origin of the 2D array, which the grid is shifted around.
 
     Returns
     -------
     ndarray
-        A sub grid of (y,x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
-        array. The sub grid is slimmed and has dimensions (total_unmasked_pixels*sub_size**2, 2).
+        A grid of (y,x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
+        array. The grid is slimmed and has dimensions (total_unmasked_pixels, 2).
 
     Examples
     --------
     mask = np.array([[True, False, True],
                      [False, False, False]
                      [True, False, True]])
-    grid_2d_slim = grid_2d_slim_via_shape_native_from(shape_native=(3,3), pixel_scales=(0.5, 0.5), sub_size=2, origin=(0.0, 0.0))
+    grid_2d_slim = grid_2d_slim_via_shape_native_from(shape_native=(3,3), pixel_scales=(0.5, 0.5), origin=(0.0, 0.0))
     """
     return grid_2d_slim_via_mask_from(
         mask_2d=np.full(fill_value=False, shape=shape_native),
         pixel_scales=pixel_scales,
-        sub_size=sub_size,
         origin=origin,
     )
 
 
 def grid_2d_via_shape_native_from(
     shape_native: Tuple[int, int],
     pixel_scales: ty.PixelScales,
-    sub_size: int,
     origin: Tuple[float, float] = (0.0, 0.0),
 ) -> np.ndarray:
     """
-    For a sub-grid, every unmasked pixel of its 2D mask with shape (total_y_pixels, total_x_pixels) is divided
-    into a finer uniform grid of shape (total_y_pixels*sub_size, total_x_pixels*sub_size). This routine computes
-    the (y,x) scaled coordinates at the centre of every sub-pixel defined by this 2D mask array.
+    For a grid, every unmasked pixel is in a 2D mask with shape (total_y_pixels, total_x_pixels). This routine computes
+    the (y,x) scaled coordinates at the centre of every pixel defined by this 2D mask array.
 
-    The sub-grid is returned in its native dimensions with shape (total_y_pixels*sub_size, total_x_pixels*sub_size).
+    The grid is returned in its native dimensions with shape (total_y_pixels, total_x_pixels).
     y coordinates are stored in the 0 index of the second dimension, x coordinates in the 1 index.
 
-    Grids are defined from the top-left corner, where the first sub-pixel corresponds to index [0,0].
-    Sub-pixels that are part of the same mask array pixel are indexed next to one another, such that the second
-    sub-pixel in the first pixel has index 1, its next sub-pixel has index 2, and so forth.
+    Grids are defined from the top-left corner, where the first pixel corresponds to index [0,0].
 
     Parameters
     ----------
     shape_native
-        The (y,x) shape of the 2D array the sub-grid of coordinates is computed for.
+        The (y,x) shape of the 2D array the grid of coordinates is computed for.
     pixel_scales
         The (y,x) scaled units to pixel units conversion factor of the 2D mask array.
-    sub_size
-        The size of the sub-grid that each pixel of the 2D mask array is divided into.
     origin
-        The (y,x) origin of the 2D array, which the sub-grid is shifted around.
+        The (y,x) origin of the 2D array, which the grid is shifted around.
 
     Returns
     -------
     ndarray
-        A sub grid of (y,x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
-        array. The sub grid array has dimensions (total_y_pixels*sub_size, total_x_pixels*sub_size).
+        A grid of (y,x) scaled coordinates at the centre of every pixel unmasked pixel on the 2D mask
+        array. The grid array has dimensions (total_y_pixels, total_x_pixels).
 
     Examples
     --------
-    grid_2d = grid_2d_via_shape_native_from(shape_native=(3, 3), pixel_scales=(1.0, 1.0), sub_size=2, origin=(0.0, 0.0))
+    grid_2d = grid_2d_via_shape_native_from(shape_native=(3, 3), pixel_scales=(1.0, 1.0), origin=(0.0, 0.0))
     """
     return grid_2d_via_mask_from(
         mask_2d=np.full(fill_value=False, shape=shape_native),
         pixel_scales=pixel_scales,
-        sub_size=sub_size,
         origin=origin,
     )
 
 
 @numba_util.jit()
 def _radial_projected_shape_slim_from(
     extent: np.ndarray,
     centre: Tuple[float, float],
     pixel_scales: ty.PixelScales,
-    sub_size: int,
 ) -> int:
     """
     The function `grid_scaled_2d_slim_radial_projected_from()` determines a projected radial grid of points from a 2D
     region of coordinates defined by an extent [xmin, xmax, ymin, ymax] and with a (y,x) centre.
 
     To do this, the function first performs these 3 steps:
 
@@ -467,16 +428,14 @@
     ----------
     extent
         The extent of the grid the radii grid is computed using, with format [xmin, xmax, ymin, ymax]
     centre : (float, flloat)
         The (y,x) central coordinate which the radial grid is traced outwards from.
     pixel_scales
         The (y,x) scaled units to pixel units conversion factor of the 2D mask array.
-    sub_size
-        The size of the sub-grid that each pixel of the 2D mask array is divided into.
 
     Returns
     -------
     int
         The 1D integer shape of a radial set of points sampling the longest distance from the centre to the edge of the
         extent in along the positive x-axis.
     """
@@ -498,23 +457,22 @@
     if (scaled_distance == distance_to_positive_y) or (
         scaled_distance == distance_to_negative_y
     ):
         pixel_scale = pixel_scales[0]
     else:
         pixel_scale = pixel_scales[1]
 
-    return sub_size * int((scaled_distance / pixel_scale)) + 1
+    return int((scaled_distance / pixel_scale)) + 1
 
 
 @numba_util.jit()
 def grid_scaled_2d_slim_radial_projected_from(
     extent: np.ndarray,
     centre: Tuple[float, float],
     pixel_scales: ty.PixelScales,
-    sub_size: int,
     shape_slim: Optional[int] = 0,
 ) -> np.ndarray:
     """
     Determine a projected radial grid of points from a 2D region of coordinates defined by an
     extent [xmin, xmax, ymin, ymax] and with a (y,x) centre.
 
     This functions operates as follows:
@@ -552,16 +510,14 @@
     ----------
     extent
         The extent of the grid the radii grid is computed using, with format [xmin, xmax, ymin, ymax]
     centre : (float, flloat)
         The (y,x) central coordinate which the radial grid is traced outwards from.
     pixel_scales
         The (y,x) scaled units to pixel units conversion factor of the 2D mask array.
-    sub_size
-        The size of the sub-grid that each pixel of the 2D mask array is divided into.
     shape_slim
         Manually choose the shape of the 1D projected grid that is returned. If 0, the border based on the 2D grid is
         used (due to numba None cannot be used as a default value).
 
     Returns
     -------
     ndarray
@@ -587,25 +543,25 @@
         scaled_distance == distance_to_negative_y
     ):
         pixel_scale = pixel_scales[0]
     else:
         pixel_scale = pixel_scales[1]
 
     if shape_slim == 0:
-        shape_slim = sub_size * int((scaled_distance / pixel_scale)) + 1
+        shape_slim = int((scaled_distance / pixel_scale)) + 1
 
     grid_scaled_2d_slim_radii = np.zeros((shape_slim, 2))
 
     grid_scaled_2d_slim_radii[:, 0] += centre[0]
 
     radii = centre[1]
 
     for slim_index in range(shape_slim):
         grid_scaled_2d_slim_radii[slim_index, 1] = radii
-        radii += pixel_scale / sub_size
+        radii += pixel_scale
 
     return grid_scaled_2d_slim_radii
 
 
 @numba_util.jit()
 def relocated_grid_via_jit_from(grid, border_grid):
     """
@@ -689,15 +645,16 @@
             distance_to_centre = distance_to_centre_new
             furthest_grid_2d_slim_index = slim_index
 
     return furthest_grid_2d_slim_index
 
 
 def grid_2d_slim_from(
-    grid_2d_native: np.ndarray, mask: np.ndarray, sub_size: int
+    grid_2d_native: np.ndarray,
+    mask: np.ndarray,
 ) -> np.ndarray:
     """
     For a native 2D grid and mask of shape [total_y_pixels, total_x_pixels, 2], map the values of all unmasked
     pixels to a slimmed grid of shape [total_unmasked_pixels, 2].
 
     The pixel coordinate origin is at the top left corner of the native grid and goes right-wards and downwards, such
     that for an grid of shape (3,3) where all pixels are unmasked:
@@ -708,36 +665,37 @@
 
     Parameters
     ----------
     grid_2d_native : ndarray
         The native grid of (y,x) values which are mapped to the slimmed grid.
     mask_2d
         A 2D array of bools, where `False` values mean unmasked and are included in the mapping.
-    sub_size
-        The size (sub_size x sub_size) of each unmasked pixels sub-array.
 
     Returns
     -------
     ndarray
         A 1D grid of values mapped from the 2D grid with dimensions (total_unmasked_pixels).
     """
 
     grid_1d_slim_y = array_2d_util.array_2d_slim_from(
-        array_2d_native=grid_2d_native[:, :, 0], mask_2d=mask, sub_size=sub_size
+        array_2d_native=np.array(grid_2d_native[:, :, 0]),
+        mask_2d=np.array(mask),
     )
 
     grid_1d_slim_x = array_2d_util.array_2d_slim_from(
-        array_2d_native=grid_2d_native[:, :, 1], mask_2d=mask, sub_size=sub_size
+        array_2d_native=np.array(grid_2d_native[:, :, 1]),
+        mask_2d=np.array(mask),
     )
 
     return np.stack((grid_1d_slim_y, grid_1d_slim_x), axis=-1)
 
 
 def grid_2d_native_from(
-    grid_2d_slim: np.ndarray, mask_2d: np.ndarray, sub_size: int
+    grid_2d_slim: np.ndarray,
+    mask_2d: np.ndarray,
 ) -> np.ndarray:
     """
     For a slimmed 2D grid of shape [total_unmasked_pixels, 2], that was computed by extracting the unmasked values
     from a native 2D grid of shape [total_y_pixels, total_x_pixels, 2], map the slimmed grid's coordinates back to the
     native 2D grid where masked values are set to zero.
 
     This uses a 1D array 'slim_to_native' where each index gives the 2D pixel indexes of the grid's native unmasked
@@ -749,42 +707,42 @@
 
     Parameters
     ----------
     grid_2d_slim
         The (y,x) values of the slimmed 2D grid which are mapped to the native 2D grid.
     mask_2d
         A 2D array of bools, where `False` values mean unmasked and are included in the mapping.
-    sub_size
-        The size (sub_size x sub_size) of each unmasked pixels sub-array.
 
     Returns
     -------
     ndarray
         A NumPy array of shape [total_y_pixels, total_x_pixels, 2] corresponding to the (y,x) values of the native 2D
         mapped from the slimmed grid.
     """
 
     grid_2d_native_y = array_2d_util.array_2d_native_from(
-        array_2d_slim=grid_2d_slim[:, 0], mask_2d=mask_2d, sub_size=sub_size
+        array_2d_slim=grid_2d_slim[:, 0],
+        mask_2d=mask_2d,
     )
 
     grid_2d_native_x = array_2d_util.array_2d_native_from(
-        array_2d_slim=grid_2d_slim[:, 1], mask_2d=mask_2d, sub_size=sub_size
+        array_2d_slim=grid_2d_slim[:, 1],
+        mask_2d=mask_2d,
     )
 
     return np.stack((grid_2d_native_y, grid_2d_native_x), axis=-1)
 
 
 @numba_util.jit()
 def grid_2d_slim_upscaled_from(
     grid_slim: np.ndarray, upscale_factor: int, pixel_scales: ty.PixelScales
 ) -> np.ndarray:
     """
     From an input slimmed 2D grid, return an upscaled slimmed 2D grid where (y,x) coordinates are added at an
-    upscaled resolution to each grid coordinate, analogous to a sub-grid.
+    upscaled resolution to each grid coordinate.
 
     Parameters
     ----------
     grid_slim
         The slimmed grid of (y,x) coordinates over which a square uniform grid is overlaid.
     upscale_factor
         The upscaled resolution at which the new grid coordinates are computed.
@@ -847,15 +805,15 @@
 def compute_polygon_area(points):
     x = points[:, 1]
     y = points[:, 0]
 
     return 0.5 * np.abs(np.dot(x, np.roll(y, 1)) - np.dot(y, np.roll(x, 1)))
 
 
-# @numba_util.jit()
+@numba_util.jit()
 def grid_pixels_in_mask_pixels_from(
     grid, shape_native, pixel_scales, origin
 ) -> np.ndarray:
     """
     Returns an array containing the number of pixels of one grid in every pixel of another masked grid.
 
     For example, image-mesh adaption may be performed on a 3.0" circular mask of data. The high weight pixels
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/grids/sparse_2d_util.py` & `autoarray-2024.5.16.0/autoarray/structures/grids/sparse_2d_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
     """
 
     from autoarray.structures.grids.uniform_2d import Grid2D
 
     shape_nnn = np.shape(mask)[0]
 
     grid = Grid2D.uniform(
-        shape_native=(shape_nnn, shape_nnn), pixel_scales=pixel_scales, sub_size=1
+        shape_native=(shape_nnn, shape_nnn),
+        pixel_scales=pixel_scales,
     )
 
     x1d_hb, y1d_hb = create_grid_hb_order(length=length_hb, mask_radius=mask_radius)
 
     grid_hb = np.stack((y1d_hb, x1d_hb), axis=-1)
     grid_hb_radius = np.sqrt(grid_hb[:, 0] ** 2.0 + grid_hb[:, 1] ** 2.0)
     new_grid = grid_hb[grid_hb_radius <= mask_radius]
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/grids/uniform_1d.py` & `autoarray-2024.5.16.0/autoarray/operators/over_sampling/uniform.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,480 +1,419 @@
-from __future__ import annotations
 import numpy as np
-from typing import TYPE_CHECKING, List, Union, Tuple
+from typing import Union
 
-if TYPE_CHECKING:
-    from autoarray.structures.arrays.uniform_1d import Array1D
-    from autoarray.structures.grids.uniform_2d import Grid2D
-    from autoarray.structures.grids.transformed_2d import Grid2DTransformed
-    from autoarray.structures.grids.transformed_2d import Grid2DTransformedNumpy
+from autoconf import conf
+from autoconf import cached_property
 
-from autoarray.structures.abstract_structure import Structure
+from autoarray.mask.mask_2d import Mask2D
+from autoarray.operators.over_sampling.abstract import AbstractOverSampling
+from autoarray.operators.over_sampling.abstract import AbstractOverSampler
+from autoarray.structures.arrays.uniform_2d import Array2D
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 
-from autoarray.mask.mask_1d import Mask1D
 
-from autoarray.structures.grids import grid_1d_util
-from autoarray.structures.grids import grid_2d_util
-from autoarray.geometry import geometry_util
-from autoarray import type as ty
+from autoarray.operators.over_sampling import over_sample_util
 
 
-class Grid1D(Structure):
-    def __new__(
-        cls,
-        values: Union[np.ndarray, List],
-        mask: Mask1D,
-        store_native: bool = False,
-        *args,
-        **kwargs,
-    ):
+class OverSamplingUniform(AbstractOverSampling):
+    def __init__(self, sub_size: Union[int, Array2D]):
         """
-        A grid of 1D (x) coordinates, which are paired to a uniform 1D mask of pixels and sub-pixels. Each entry
-        on the grid corresponds to the (x) coordinates at the centre of a sub-pixel of an unmasked pixel.
-
-        A `Grid1D` is ordered such that pixels begin from the left (e.g. index [0]) of the corresponding mask
-        and go right. The positive x-axis is to the right.
-
-        The grid can be stored in two formats:
-
-        - slimmed: all masked entries are removed so the ndarray is shape [total_unmasked_coordinates*sub_size]
-        - native: it retains the original shape of the grid so the ndarray is
-          shape [total_y_coordinates*sub_size, total_x_coordinates*sub_size, 2].
+        Over samples grid calculations using a uniform sub-grid.
 
+        When a 2D grid of (y,x) coordinates is input into a function, the result is evaluated at every coordinate
+        on the grid. When the grid is paired to a 2D image (e.g. an `Array2D`) the solution needs to approximate
+        the 2D integral of that function in each pixel. Over sample objects define how this over-sampling is performed.
 
-        **Case 1 (sub-size=1, slim)**
+        This object inputs a uniform sub-grid, where every image-pixel is split into a uniform grid of sub-pixels. The
+        function is evaluated at every sub-pixel, and the final value in each pixel is computed by summing the
+        contribution from all sub-pixels.
 
-        The Grid1D is an ndarray of shape [total_unmasked_coordinates].
+        This is the simplest over-sampling method, but may not provide precise solutions for functions that vary
+        significantly within a pixel. To achieve precision in these pixels a high `sub_size` is required, which can
+        be computationally expensive as it is applied to every pixel.
 
-        The first element of the ndarray corresponds to the pixel index. For example:
+        **Example**
 
-        - grid[3] = the 4th unmasked pixel's x-coordinate.
-        - grid[6] = the 7th unmasked pixel's x-coordinate.
+        If the mask's `sub_size` is > 1, the grid is defined as a sub-grid where each entry corresponds to the (y,x)
+        coordinates at the centre of each sub-pixel of an unmasked pixel. The Grid2D is therefore stored as an ndarray
+        of shape [total_unmasked_coordinates*sub_size**2, 2]
 
-        Below is a visual illustration of a grid, where a total of 3 pixels are unmasked and are included in the grid.
-
-        .. code-block:: bash
-
-            <--- -ve  x  +ve -->
-
-            x x x O o x O x x x
-
-        This is an example mask.Mask1D, where:
-
-        .. code-block:: bash
-
-            x = `True` (Pixel is masked and excluded from the grid)
-            O = `False` (Pixel is not masked and included in the grid)
-
-        The mask pixel index's will come out like this (and the direction of scaled coordinates is highlighted
-        around the mask.
-
-        .. code-block:: bash
-
-            pixel_scales = 1.0"
-
-            <--- -ve  x  +ve -->
-
-            x x x 0 1 x 2 x x x
-
-            grid[0] = [-1.5]
-            grid[1] = [-0.5]
-            grid[2] = [1.5]
-
-
-        **Case 2 (sub-size>1, slim)
-
-        If the mask's `sub_size` is > 1, the grid is defined as a sub-grid where each entry corresponds to the (x)
-        coordinates at the centre of each sub-pixel of an unmasked pixel. The Grid1D is therefore stored as an ndarray
-        of shape [total_unmasked_coordinates*sub_size].
-
-        The sub-grid indexes are ordered such that pixels begin from the first (leftmost) sub-pixel in the first
+        The sub-grid indexes are ordered such that pixels begin from the first (top-left) sub-pixel in the first
         unmasked pixel. Indexes then go over the sub-pixels in each unmasked pixel, for every unmasked pixel.
-        Therefore, the sub-grid is an ndarray of shape [total_unmasked_coordinates*sub_grid_shape]. For example:
+        Therefore, the sub-grid is an ndarray of shape [total_unmasked_coordinates*(sub_grid_shape)**2, 2].
 
-        - grid[5] - using `sub_size=2`, gives the 3rd unmasked pixel's 2nd sub-pixel x-coordinate.
-        - grid[3] - using `sub_size=3`, gives the 2nd unmasked pixel's 1st sub-pixel x-coordinate.
-        - grid[10] - using `sub_size=3`, gives the 4th unmasked pixel's 1st sub-pixel y-coordinate.
+        For example:
+
+        - grid[9, 1] - using a 2x2 sub-grid, gives the 3rd unmasked pixel's 2nd sub-pixel x-coordinate.
+        - grid[9, 1] - using a 3x3 sub-grid, gives the 2nd unmasked pixel's 1st sub-pixel x-coordinate.
+        - grid[27, 0] - using a 3x3 sub-grid, gives the 4th unmasked pixel's 1st sub-pixel y-coordinate.
 
         Below is a visual illustration of a sub grid. Indexing of each sub-pixel goes from the top-left corner. In
         contrast to the grid above, our illustration below restricts the mask to just 2 pixels, to keep the
         illustration brief.
 
         .. code-block:: bash
 
-            x x x O x O x x x
-
-            This is an example mask.Mask1D, where:
+             x x x x x x x x x x
+             x x x x x x x x x x     This is an example mask.Mask2D, where:
+             x x x x x x x x x x
+             x x x x x x x x x x     x = `True` (Pixel is masked and excluded from lens)
+             x x x x O O x x x x     O = `False` (Pixel is not masked and included in lens)
+             x x x x x x x x x x
+             x x x x x x x x x x
+             x x x x x x x x x x
+             x x x x x x x x x x
+             x x x x x x x x x x
 
-            x = `True` (Pixel is masked and excluded from the grid)
-            O = `False` (Pixel is not masked and included in the grid)
-
-        Our grid with a sub-size=1 looks like it did before:
+        Our grid with a sub-size looks like it did before:
 
         .. code-block:: bash
 
             pixel_scales = 1.0"
 
             <--- -ve  x  +ve -->
 
-             x x x 0 x 1 x x x
+             x x x x x x x x x x  ^
+             x x x x x x x x x x  I
+             x x x x x x x x x x  I                        y     x
+             x x x x x x x x x x +ve  grid[0] = [0.5,  -1.5]
+             x x x x 0 1 x x x x  y   grid[1] = [0.5,  -0.5]
+             x x x x x x x x x x -ve
+             x x x x x x x x x x  I
+             x x x x x x x x x x  I
+             x x x x x x x x x x \/
+             x x x x x x x x x x
 
         However, if the sub-size is 2, we go to each unmasked pixel and allocate sub-pixel coordinates for it. For
-        example, for pixel 0, if `sub_size=2`:
+        example, for pixel 0, if *sub_size=2*, we use a 2x2 sub-grid:
 
         .. code-block:: bash
 
-            grid[0] = [-0.75]
-            grid[1] = [-0.25]
+            Pixel 0 - (2x2):
+                                y      x
+                   grid[0] = [0.66, -1.66]
+            I0I1I  grid[1] = [0.66, -1.33]
+            I2I3I  grid[2] = [0.33, -1.66]
+                   grid[3] = [0.33, -1.33]
 
         If we used a sub_size of 3, for the pixel we we would create a 3x3 sub-grid:
 
         .. code-block:: bash
 
-            grid[0] = [-0.833]
-            grid[1] = [-0.5]
-            grid[2] = [-0.166]
-
+                                  y      x
+                     grid[0] = [0.75, -0.75]
+                     grid[1] = [0.75, -0.5]
+                     grid[2] = [0.75, -0.25]
+            I0I1I2I  grid[3] = [0.5,  -0.75]
+            I3I4I5I  grid[4] = [0.5,  -0.5]
+            I6I7I8I  grid[5] = [0.5,  -0.25]
+                     grid[6] = [0.25, -0.75]
+                     grid[7] = [0.25, -0.5]
+                     grid[8] = [0.25, -0.25]
+
+        All sub-pixels in masked pixels have values (0.0, 0.0).
+
+        __Adaptive Oversampling__
+
+        By default, the sub-grid is the same size in every pixel (e.g. the value of `sub_size` is an integer that
+        defines the size of the sub-grid for every pixel).
+
+        However, the `sub_size` can also be input as an `Array2D`, with varying integer values for each pixel.
+        This is called adaptive over-sampling and is used to adapt the over-sampling to the bright regions of the
+        data, saving computational time.
+
+        __Pixelization__
+
+        For pixelizations performed in the inversion module, over sampling is equally important. Now, the over
+        sampling maps multiple data sub-pixels to pixels in the pixelization, where mappings are performed fractionally
+        based on the sub-grid sizes.
 
-        **Case 3 (sub_size=1 native)**
+        The over sampling class has functions dedicated to mapping between the sub-grid and pixel-grid, for example
+        `sub_mask_native_for_sub_mask_slim` and `slim_for_sub_slim`.
 
-        The Grid2D has the same properties as Case 1, but is stored as an an ndarray of shape [total_x_coordinates].
+        Parameters
+        ----------
+        sub_size
+            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
+        """
 
-        All masked entries on the grid has (y,x) values of (0.0, 0.0).
+        self.sub_size = sub_size
 
-        For the following example mask:
+    @classmethod
+    def from_adapt(
+        cls,
+        data: Array2D,
+        noise_map: Array2D,
+        signal_to_noise_cut: float = 5.0,
+        sub_size_lower: int = 2,
+        sub_size_upper: int = 4,
+    ):
+        """
+        Returns an adaptive sub-grid size based on the signal-to-noise of the data.
 
-        .. code-block:: bash
+        The adaptive sub-grid size is computed as follows:
 
-            x x x O O x O x x x
+        1) The signal-to-noise of every pixel is computed as the data divided by the noise-map.
+        2) For all pixels with signal-to-noise above the signal-to-noise cut, the sub-grid size is set to the upper
+          value. For all other pixels, the sub-grid size is set to the lower value.
 
-            - grid[0] = 0.0 (it is masked, thus zero)
-            - grid[1] = 0.0 (it is masked, thus zero)
-            - grid[2] = 0.0 (it is masked, thus zero)
-            - grid[3] = -1.5
-            - grid[4] = -0.5
-            - grid[5] = 0.0 (it is masked, thus zero)
-            - grid[6] = 0.5
+        This scheme can produce low sub-size values over entire datasets if the data has a low signal-to-noise. However,
+        just because the data has a low signal-to-noise does not mean that the sub-grid size should be low.
 
+        To mitigate this, the signal-to-noise cut is set to the maximum signal-to-noise of the data divided by 2.0 if
+        it this value is below the signal-to-noise cut.
 
-        **Case 4 (sub_size>1 native)**
+        Parameters
+        ----------
+        data
+            The data which is to be fitted via a calculation using this over-sampling sub-grid.
+        noise_map
+            The noise-map of the data.
+        signal_to_noise_cut
+            The signal-to-noise cut which defines whether the sub-grid size is the upper or lower value.
+        sub_size_lower
+            The sub-grid size for pixels with signal-to-noise below the signal-to-noise cut.
+        sub_size_upper
+            The sub-grid size for pixels with signal-to-noise above the signal-to-noise cut.
 
-        The properties of this grid can be derived by combining Case's 2 and 3 above, whereby the grid is stored as
-        an ndarray of shape [total_x_coordinates*sub_size,].
+        Returns
+        -------
+        The adaptive sub-grid sizes.
+        """
+        signal_to_noise = data / noise_map
 
-        All sub-pixels in masked pixels have value 0.0.
+        if np.max(signal_to_noise) < (2.0 * signal_to_noise_cut):
+            signal_to_noise_cut = np.max(signal_to_noise) / 2.0
 
+        sub_size = np.where(
+            signal_to_noise > signal_to_noise_cut, sub_size_upper, sub_size_lower
+        )
 
-        **Grid1D Mapping**
+        sub_size = Array2D(values=sub_size, mask=data.mask)
 
-        Every set of (x) coordinates in a pixel of the sub-grid maps to an unmasked pixel in the mask. For a uniform
-        grid, every x coordinate directly corresponds to the location of its paired unmasked pixel.
+        return cls(sub_size=sub_size)
 
-        It is not a requirement that grid is uniform and that their coordinates align with the mask. The input grid
-        could be an irregular set of x coordinates where the indexing signifies that the x coordinate
-        *originates* or *is paired with* the mask's pixels but has had its value change by some aspect of the
-        calculation.
+    def over_sampler_from(self, mask: Mask2D) -> "OverSamplerUniform":
+        return OverSamplerUniform(
+            mask=mask,
+            sub_size=self.sub_size,
+        )
 
-        This is important for the child project *PyAutoLens*, where grids in the image-plane are ray-traced and
-        deflected to perform lensing calculations. The grid indexing is used to map pixels between the image-plane and
-        source-plane.
 
-        Parameters
-        ----------
-        values
-            The (y,x) coordinates of the grid.
-        mask
-            The 2D mask associated with the grid, defining the pixels each grid coordinate is paired with and
-            originates from.
+class OverSamplerUniform(AbstractOverSampler):
+    def __init__(self, mask: Mask2D, sub_size: Union[int, Array2D]):
         """
+         Over samples grid calculations using a uniform sub-grid.
 
-        values = grid_1d_util.convert_grid_1d(
-            grid_1d=values, mask_1d=mask, store_native=store_native
-        )
-
-        obj = values.view(cls)
-        obj.mask = mask
-
-        return obj
+         See the class `OverSamplingUniform` for a description of how the over-sampling works in full.
 
-    @classmethod
-    def no_mask(
-        cls,
-        values: Union[np.ndarray, List],
-        pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
-        origin: Tuple[float] = (0.0,),
-    ) -> "Grid1D":
-        """
-        Create a Grid1D (see *Grid1D.__new__*) by inputting the grid coordinates in 1D.
+         The class `OverSamplingUniform` is used for the high level API, whereby this is where users input their
+         preferred over-sampling configuration. This class, `OverSamplerUniform`, contains the functionality
+         which actually performs the over-sampling calculations, but is hidden from the user.
 
         Parameters
         ----------
-        values
-            The (y,x) coordinates of the grid input as an ndarray of shape [total_unmasked_pixells*(sub_size**2), 2]
-            or a list of lists.
-        pixel_scales
-            The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
-            it is converted to a (float, float).
+        mask
+            The mask defining the 2D region where the over-sampled grid is computed.
         sub_size
             The size (sub_size x sub_size) of each unmasked pixels sub-grid.
-        origin
-            The origin of the grid's mask.
-
-        Examples
-        --------
-
-        .. code-block:: python
-
-            import autogrid as aa
+        """
+        self.mask = mask
 
-            # Make Grid1D from input np.ndgrid.
+        if isinstance(sub_size, int):
+            sub_size = Array2D(
+                values=np.full(fill_value=sub_size, shape=mask.shape_slim), mask=mask
+            )
 
-            grid_1d = aa.Grid1D.no_mask(grid=np.grid([1.0, 2.0, 3.0, 4.0]), pixel_scales=1.0)
+        self.sub_size = sub_size
 
-            # Make Grid2D from input list.
+    @property
+    def sub_total(self):
+        """
+        The total number of sub-pixels in the entire mask.
+        """
+        return int(np.sum(self.sub_size**2))
 
-            grid_1d = aa.Grid1D.no_mask(grid=[1.0, 2.0, 3.0, 4.0], pixel_scales=1.0)
+    @property
+    def sub_length(self) -> Array2D:
+        """
+        The total number of sub-pixels in a give pixel,
 
-            # Print grid's slim (masked 1D data representation) and
-            # native (masked 1D data representation)
+        For example, a sub-size of 3x3 means every pixel has 9 sub-pixels.
+        """
+        return self.sub_size**self.mask.dimensions
 
-            print(grid_1d.slim)
-            print(grid_1d.native)
+    @property
+    def sub_fraction(self) -> Array2D:
         """
+        The fraction of the area of a pixel every sub-pixel contains.
 
-        pixel_scales = geometry_util.convert_pixel_scales_1d(pixel_scales=pixel_scales)
+        For example, a sub-size of 3x3 mean every pixel contains 1/9 the area.
+        """
 
-        values = grid_2d_util.convert_grid(grid=values)
+        return 1.0 / self.sub_length
 
-        mask = Mask1D.all_false(
-            shape_slim=values.shape[0] // sub_size,
-            pixel_scales=pixel_scales,
-            sub_size=sub_size,
-            origin=origin,
+    @cached_property
+    def over_sampled_grid(self) -> Grid2DIrregular:
+        grid = over_sample_util.grid_2d_slim_over_sampled_via_mask_from(
+            mask_2d=np.array(self.mask),
+            pixel_scales=self.mask.pixel_scales,
+            sub_size=np.array(self.sub_size).astype("int"),
+            origin=self.mask.origin,
         )
 
-        return Grid1D(values=values, mask=mask)
+        return Grid2DIrregular(values=grid)
 
-    @classmethod
-    def from_mask(cls, mask: Mask1D) -> "Grid1D":
+    def binned_array_2d_from(self, array: Array2D) -> "Array2D":
         """
-        Create a Grid1D (see *Grid1D.__new__*) from a mask, where only unmasked pixels are included in the grid (if the
-        grid is represented in its native 1D masked values are 0.0).
+        Convenience method to access the binned-up array in its 1D representation, which is a Grid2D stored as an
+        ``ndarray`` of shape [total_unmasked_pixels, 2].
 
-        The mask's pixel_scales, sub_size and origin properties are used to compute the grid (x) coordinates.
+        The binning up process converts a array from (y,x) values where each value is a coordinate on the sub-array to
+        (y,x) values where each coordinate is at the centre of its mask (e.g. a array with a sub_size of 1). This is
+        performed by taking the mean of all (y,x) values in each sub pixel.
 
-        Parameters
-        ----------
-        mask
-            The mask whose masked pixels are used to setup the sub-pixel grid.
-        """
+        If the array is stored in 1D it is return as is. If it is stored in 2D, it must first be mapped from 2D to 1D.
 
-        sub_grid_1d = grid_1d_util.grid_1d_slim_via_mask_from(
-            mask_1d=mask,
-            pixel_scales=mask.pixel_scales,
-            sub_size=mask.sub_size,
-            origin=mask.origin,
+        In **PyAutoCTI** all `Array2D` objects are used in their `native` representation without sub-gridding.
+        Significant memory can be saved by only store this format, thus the `native_binned_only` config override
+        can force this behaviour. It is recommended users do not use this option to avoid unexpected behaviour.
+        """
+        if conf.instance["general"]["structures"]["native_binned_only"]:
+            return self
+
+        try:
+            array = array.slim
+        except AttributeError:
+            pass
+
+        binned_array_2d = over_sample_util.binned_array_2d_from(
+            array_2d=np.array(array),
+            mask_2d=np.array(self.mask),
+            sub_size=np.array(self.sub_size),
         )
 
-        return Grid1D(values=sub_grid_1d, mask=mask)
-
-    @classmethod
-    def uniform(
-        cls,
-        shape_native: Tuple[int],
-        pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
-        origin: Tuple[float] = (0.0, 0.0),
-    ) -> "Grid1D":
-        """
-        Create a `Grid1D` (see `Grid`D.__new__`) as a uniform grid of (x) values given an input `shape_native` and
-        `pixel_scales` of the grid.
-
-        Parameters
-        ----------
-        shape_native
-            The 1D shape of the uniform grid and the mask that it is paired with.
-        pixel_scales
-            The (x) scaled units to pixel units conversion factor of every pixel. If this is input as a `float`,
-            it is converted to a (float,) tuple.
-        sub_size
-            The size (sub_size) of each unmasked pixels sub-grid.
-        origin
-            The origin of the grid's mask and coordinate system.
-        """
-        pixel_scales = geometry_util.convert_pixel_scales_1d(pixel_scales=pixel_scales)
-
-        grid_slim = grid_1d_util.grid_1d_slim_via_shape_slim_from(
-            shape_slim=shape_native,
-            pixel_scales=pixel_scales,
-            sub_size=sub_size,
-            origin=origin,
+        return Array2D(
+            values=binned_array_2d,
+            mask=self.mask,
         )
 
-        return cls.no_mask(
-            values=grid_slim,
-            pixel_scales=pixel_scales,
-            sub_size=sub_size,
-            origin=origin,
-        )
+    def array_via_func_from(self, func, obj, *args, **kwargs):
+        over_sampled_grid = self.over_sampled_grid
 
-    @classmethod
-    def uniform_from_zero(
-        cls, shape_native: Tuple[int], pixel_scales: ty.PixelScales, sub_size: int = 1
-    ) -> "Grid1D":
-        """
-        Create a `Grid1D` (see `Grid`D.__new__`) as a uniform grid of (x) values given an input `shape_native` and
-        `pixel_scales` of the grid, where the first (x) coordinate of the grid is 0.0 and all other values ascend
-        positively.
+        if obj is not None:
+            values = func(obj, over_sampled_grid, *args, **kwargs)
+        else:
+            values = func(over_sampled_grid, *args, **kwargs)
 
-        Parameters
-        ----------
-        shape_native
-            The 1D shape of the uniform grid and the mask that it is paired with.
-        pixel_scales
-            The (x) scaled units to pixel units conversion factor of every pixel. If this is input as a `float`,
-            it is converted to a (float,) tuple.
-            it is converted to a (float,) tuple.
-        sub_size
-            The size (sub_size) of each unmasked pixels sub-grid.
-        """
-        pixel_scales = geometry_util.convert_pixel_scales_1d(pixel_scales=pixel_scales)
+        return self.binned_array_2d_from(array=values)
 
-        grid_slim = grid_1d_util.grid_1d_slim_via_shape_slim_from(
-            shape_slim=shape_native, pixel_scales=pixel_scales, sub_size=sub_size
-        )
+    @cached_property
+    def sub_mask_native_for_sub_mask_slim(self) -> np.ndarray:
+        """
+        Derives a 1D ``ndarray`` which maps every subgridded 1D ``slim`` index of the ``Mask2D`` to its
+        subgridded 2D ``native`` index.
 
-        grid_slim -= np.min(grid_slim)
+        For example, for the following ``Mask2D`` for ``sub_size=1``:
 
-        return cls.no_mask(
-            values=grid_slim, pixel_scales=pixel_scales, sub_size=sub_size
-        )
+        ::
+            [[True,  True,  True, True]
+             [True, False, False, True],
+             [True, False,  True, True],
+             [True,  True,  True, True]]
 
-    @property
-    def slim(self) -> "Grid1D":
-        """
-        Return a `Grid1D` where the data is stored its `slim` representation, which is an ndarray of shape
-        [total_unmasked_pixels * sub_size, 2].
+        This has three unmasked (``False`` values) which have the ``slim`` indexes:
 
-        If it is already stored in its `slim` representation  the `Grid1D` is returned as it is. If not, it is
-        mapped from  `native` to `slim` and returned as a new `Grid1D`.
-        """
-        return Grid1D(values=self, mask=self.mask)
+        ::
+            [0, 1, 2]
 
-    @property
-    def native(self) -> "Grid1D":
-        """
-        Return a `Grid1D` where the data is stored in its `native` representation, which is an ndarray of shape
-        [sub_size*total_x_pixels, 2].
+        The array ``sub_mask_native_for_sub_mask_slim`` is therefore:
 
-        If it is already stored in its `native` representation it is return as it is. If not, it is mapped from
-        `slim` to `native` and returned as a new `Grid1D`.
-        """
-        return Grid1D(values=self, mask=self.mask, store_native=True)
+        ::
+            [[1,1], [1,2], [2,1]]
 
-    @property
-    def binned(self) -> "Grid1D":
-        """
-        Convenience method to access the binned-up grid in its 1D representation, which is a Grid2D stored as an
-        ndarray of shape [total_unmasked_pixels, 2].
+        For a ``Mask2D`` with ``sub_size=2`` each unmasked ``False`` entry is split into a sub-pixel of size 2x2 and
+        there are therefore 12 ``slim`` indexes:
 
-        The binning up process converts a grid from (y,x) values where each value is a coordinate on the sub-grid to
-        (y,x) values where each coordinate is at the centre of its mask (e.g. a grid with a sub_size of 1). This is
-        performed by taking the mean of all (y,x) values in each sub pixel.
+        ::
+            [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
 
-        If the grid is stored in 1D it is return as is. If it is stored in 2D, it must first be mapped from 2D to 1D.
-        """
+        The array ``native_for_slim`` is therefore:
 
-        grid_1d_slim = self.slim
+        ::
+            [[2,2], [2,3], [2,4], [2,5], [3,2], [3,3], [3,4], [3,5], [4,2], [4,3], [5,2], [5,3]]
 
-        binned_grid_1d_slim = np.multiply(
-            self.mask.sub_fraction,
-            grid_1d_slim.reshape(-1, self.mask.sub_length).sum(axis=1),
-        )
+        Examples
+        --------
 
-        return Grid1D(values=binned_grid_1d_slim, mask=self.mask.derive_mask.sub_1)
+        .. code-block:: python
 
-    def grid_2d_radial_projected_from(self, angle: float = 0.0) -> Grid2DIrregular:
-        """
-        Project the 1D grid of (y,x) coordinates to an irregular 2d grid of (y,x) coordinates. The projection works
-        as follows:
+            import autoarray as aa
 
-        1) Map the 1D (x) coordinates to 2D along the x-axis, such that the x value of every 2D coordinate is the
-        corresponding (x) value in the 1D grid, and every y value is 0.0.
+            mask_2d = aa.Mask2D(
+                mask=[[True,  True,  True, True]
+                      [True, False, False, True],
+                      [True, False,  True, True],
+                      [True,  True,  True, True]]
+                pixel_scales=1.0,
+            )
 
-        2) Rotate this projected 2D grid clockwise by the input angle.
+            derive_indexes_2d = aa.DeriveIndexes2D(mask=mask_2d)
 
-        Parameters
-        ----------
-        angle
-            The angle with which the project 2D grid of coordinates is rotated clockwise.
+            print(derive_indexes_2d.sub_mask_native_for_sub_mask_slim)
+        """
+        return over_sample_util.native_sub_index_for_slim_sub_index_2d_from(
+            mask_2d=self.mask.array, sub_size=np.array(self.sub_size)
+        ).astype("int")
 
-        Returns
-        -------
-        Grid2DIrregular
-            The projected and rotated 2D grid of (y,x) coordinates.
+    @cached_property
+    def slim_for_sub_slim(self) -> np.ndarray:
         """
-        grid = np.zeros((self.sub_shape_slim, 2))
+        Derives a 1D ``ndarray`` which maps every subgridded 1D ``slim`` index of the ``Mask2D`` to its
+        non-subgridded 1D ``slim`` index.
 
-        grid[:, 1] = self.slim
+        For example, for the following ``Mask2D`` for ``sub_size=1``:
 
-        grid = geometry_util.transform_grid_2d_to_reference_frame(
-            grid_2d=grid, centre=(0.0, 0.0), angle=angle
-        )
+        ::
+            [[True,  True,  True, True]
+             [True, False, False, True],
+             [True, False,  True, True],
+             [True,  True,  True, True]]
 
-        return Grid2DIrregular(values=grid)
+        This has three unmasked (``False`` values) which have the ``slim`` indexes:
 
-    def structure_2d_from(
-        self, result: np.ndarray
-    ) -> Union[Array1D, Grid2D, Grid2DTransformed, Grid2DTransformedNumpy]:
-        """
-        Convert a result from an ndarray to an aa.Array2D or aa.Grid2D structure, where the conversion depends on
-        type(result) as follows:
+        ::
+            [0, 1, 2]
 
-        .. code-block:: bash
+        The array ``slim_for_sub_slim`` is therefore:
 
-            - 1D np.ndarray   -> aa.Array2D
-            - 2D np.ndarray   -> aa.Grid2D
+        ::
+            [0, 1, 2]
 
-        This function is used by the grid_2d_to_structure decorator to convert the output result of a function
-        to an autoarray structure when a `Grid2D` instance is passed to the decorated function.
+        For a ``Mask2D`` with ``sub_size=2`` each unmasked ``False`` entry is split into a sub-pixel of size 2x2.
+        Therefore the array ``slim_for_sub_slim`` becomes:
 
-        Parameters
-        ----------
-        result
-            The input result (e.g. of a decorated function) that is converted to a PyAutoArray structure.
-        """
-        from autoarray.structures.arrays.uniform_1d import Array1D
-        from autoarray.structures.grids.transformed_2d import Grid2DTransformed
-        from autoarray.structures.grids.transformed_2d import Grid2DTransformedNumpy
-        from autoarray.structures.grids.uniform_2d import Grid2D
-
-        if len(result.shape) == 1:
-            return Array1D(values=result, mask=self.mask)
-
-        if isinstance(result, Grid2DTransformedNumpy):
-            return Grid2DTransformed(values=result, mask=self.mask)
-        return Grid2D(values=result, mask=self.mask.derive_mask.to_mask_2d)
-
-    def structure_2d_list_from(
-        self, result_list: List
-    ) -> List[Union[Array1D, Grid2D, Grid2DTransformed, Grid2DTransformedNumpy]]:
-        """
-        Convert a result from a list of ndarrays to a list of aa.Array2D or aa.Grid2D structure, where the conversion
-        depends on type(result) as follows:
+        ::
+            [0, 0, 0, 0, 1, 1, 1, 1, 2, 2, 2, 2]
 
-        .. code-block:: bash
+        Examples
+        --------
 
-            - [1D np.ndarray] -> [aa.Array2D]
-            - [2D np.ndarray] -> [aa.Grid2D]
+        .. code-block:: python
 
-        This function is used by the grid_like_list_to_structure-list decorator to convert the output result of a
-        function to a list of autoarray structure when a `Grid2D` instance is passed to the decorated function.
+            import autoarray as aa
 
-        Parameters
-        ----------
-        result_list
-            The input result (e.g. of a decorated function) that is converted to a PyAutoArray structure.
-        """
-        return [self.structure_2d_from(result=result) for result in result_list]
+            mask_2d = aa.Mask2D(
+                mask=[[True,  True,  True, True]
+                      [True, False, False, True],
+                      [True, False,  True, True],
+                      [True,  True,  True, True]]
+                pixel_scales=1.0,
+            )
+
+            derive_indexes_2d = aa.DeriveIndexes2D(mask=mask_2d)
+
+            print(derive_indexes_2d.slim_for_sub_slim)
+        """
+        return over_sample_util.slim_index_for_sub_slim_index_via_mask_2d_from(
+            mask_2d=np.array(self.mask), sub_size=np.array(self.sub_size)
+        ).astype("int")
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/grids/uniform_2d.py` & `autoarray-2024.5.16.0/autoarray/structures/grids/uniform_2d.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,56 @@
+from __future__ import annotations
 import numpy as np
 from pathlib import Path
-from typing import List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, List, Optional, Tuple, Union
+
+if TYPE_CHECKING:
+    from autoarray.operators.over_sampling.abstract import AbstractOverSampling
 
 from autoconf import conf
 from autoconf import cached_property
 
 from autoarray.mask.mask_2d import Mask2D
+from autoarray.operators.over_sampling.abstract import AbstractOverSampler
 from autoarray.structures.abstract_structure import Structure
 from autoarray.structures.arrays.uniform_2d import Array2D
-from autoarray.structures.arrays.irregular import ArrayIrregular
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 
 from autoarray.structures.arrays import array_2d_util
 from autoarray.structures.grids import grid_2d_util
 from autoarray.geometry import geometry_util
 
 from autoarray import type as ty
 
 
 class Grid2D(Structure):
-    def __new__(
-        cls,
+    def __init__(
+        self,
         values: Union[np.ndarray, List],
         mask: Mask2D,
         store_native: bool = False,
+        over_sampling: Optional[AbstractOverSampling] = None,
         *args,
         **kwargs,
     ):
         """
-        A grid of 2D (y,x) coordinates, which are paired to a uniform 2D mask of pixels and sub-pixels. Each entry
-        on the grid corresponds to the (y,x) coordinates at the centre of a sub-pixel of an unmasked pixel.
+        A grid of 2D (y,x) coordinates, which are paired to a uniform 2D mask of pixels. Each entry
+        on the grid corresponds to the (y,x) coordinates at the centre of a pixel of an unmasked pixel.
 
         A `Grid2D` is ordered such that pixels begin from the top-row (e.g. index [0, 0]) of the corresponding mask
         and go right and down. The positive y-axis is upwards and positive x-axis to the right.
 
         The grid can be stored in two formats:
 
-        - slimmed: all masked entries are removed so the ndarray is shape [total_unmasked_coordinates*sub_size**2, 2]
+        - slimmed: all masked entries are removed so the ndarray is shape [total_unmasked_coordinates**2, 2]
         - native: it retains the original shape of the grid so the ndarray is
-          shape [total_y_coordinates*sub_size, total_x_coordinates*sub_size, 2].
+          shape [total_y_coordinates, total_x_coordinates, 2].
 
 
-        **Case 1 (sub-size=1, slim)**
+        __Slim__
 
         The Grid2D is an ndarray of shape [total_unmasked_coordinates, 2], therefore when `slim` the shape of
         the grid is 2, not 1.
 
         The first element of the ndarray corresponds to the pixel index and second element the y or x coordinate value.
 
         For example:
@@ -85,96 +90,15 @@
              x x x 2 3 4 5 x x x  y   grid[4] = [ 0.5,  0.5]
              x x x 6 7 8 9 x x x -ve  grid[5] = [ 0.5,  1.5]
              x x x x x x x x x x  I   grid[6] = [-0.5, -1.5]
              x x x x x x x x x x  I   grid[7] = [-0.5, -0.5]
              x x x x x x x x x x \/   grid[8] = [-0.5,  0.5]
              x x x x x x x x x x      grid[9] = [-0.5,  1.5]
 
-
-        **Case 2 (sub-size>1, slim)**
-
-        If the mask's `sub_size` is > 1, the grid is defined as a sub-grid where each entry corresponds to the (y,x)
-        coordinates at the centre of each sub-pixel of an unmasked pixel. The Grid2D is therefore stored as an ndarray
-        of shape [total_unmasked_coordinates*sub_size**2, 2]
-
-        The sub-grid indexes are ordered such that pixels begin from the first (top-left) sub-pixel in the first
-        unmasked pixel. Indexes then go over the sub-pixels in each unmasked pixel, for every unmasked pixel.
-        Therefore, the sub-grid is an ndarray of shape [total_unmasked_coordinates*(sub_grid_shape)**2, 2].
-
-        For example:
-
-        - grid[9, 1] - using a 2x2 sub-grid, gives the 3rd unmasked pixel's 2nd sub-pixel x-coordinate.
-        - grid[9, 1] - using a 3x3 sub-grid, gives the 2nd unmasked pixel's 1st sub-pixel x-coordinate.
-        - grid[27, 0] - using a 3x3 sub-grid, gives the 4th unmasked pixel's 1st sub-pixel y-coordinate.
-
-        Below is a visual illustration of a sub grid. Indexing of each sub-pixel goes from the top-left corner. In
-        contrast to the grid above, our illustration below restricts the mask to just 2 pixels, to keep the
-        illustration brief.
-
-        .. code-block:: bash
-
-             x x x x x x x x x x
-             x x x x x x x x x x     This is an example mask.Mask2D, where:
-             x x x x x x x x x x
-             x x x x x x x x x x     x = `True` (Pixel is masked and excluded from lens)
-             x x x x O O x x x x     O = `False` (Pixel is not masked and included in lens)
-             x x x x x x x x x x
-             x x x x x x x x x x
-             x x x x x x x x x x
-             x x x x x x x x x x
-             x x x x x x x x x x
-
-        Our grid with a sub-size looks like it did before:
-
-        .. code-block:: bash
-
-            pixel_scales = 1.0"
-
-            <--- -ve  x  +ve -->
-
-             x x x x x x x x x x  ^
-             x x x x x x x x x x  I
-             x x x x x x x x x x  I                        y     x
-             x x x x x x x x x x +ve  grid[0] = [0.5,  -1.5]
-             x x x x 0 1 x x x x  y   grid[1] = [0.5,  -0.5]
-             x x x x x x x x x x -ve
-             x x x x x x x x x x  I
-             x x x x x x x x x x  I
-             x x x x x x x x x x \/
-             x x x x x x x x x x
-
-        However, if the sub-size is 2, we go to each unmasked pixel and allocate sub-pixel coordinates for it. For
-        example, for pixel 0, if *sub_size=2*, we use a 2x2 sub-grid:
-
-        .. code-block:: bash
-
-            Pixel 0 - (2x2):
-                                y      x
-                   grid[0] = [0.66, -1.66]
-            I0I1I  grid[1] = [0.66, -1.33]
-            I2I3I  grid[2] = [0.33, -1.66]
-                   grid[3] = [0.33, -1.33]
-
-        If we used a sub_size of 3, for the pixel we we would create a 3x3 sub-grid:
-
-        .. code-block:: bash
-
-                                  y      x
-                     grid[0] = [0.75, -0.75]
-                     grid[1] = [0.75, -0.5]
-                     grid[2] = [0.75, -0.25]
-            I0I1I2I  grid[3] = [0.5,  -0.75]
-            I3I4I5I  grid[4] = [0.5,  -0.5]
-            I6I7I8I  grid[5] = [0.5,  -0.25]
-                     grid[6] = [0.25, -0.75]
-                     grid[7] = [0.25, -0.5]
-                     grid[8] = [0.25, -0.25]
-
-
-        **Case 3 (sub_size=1, native)**
+        __native__
 
         The Grid2D has the same properties as Case 1, but is stored as an an ndarray of shape
         [total_y_coordinates, total_x_coordinates, 2]. Therefore when `native` the shape of the
         grid is 3, not 2.
 
         All masked entries on the grid has (y,x) values of (0.0, 0.0).
 
@@ -199,25 +123,20 @@
             - grid[0,0,1] = 0.0 (it is masked, thus zero)
             - grid[3,3,0] = 0.0 (it is masked, thus zero)
             - grid[3,3,1] = 0.0 (it is masked, thus zero)
             - grid[3,4,0] = 1.5
             - grid[3,4,1] = -0.5
 
 
-        **Case 4 (sub_size>1 native)**
-
-        The properties of this grid can be derived by combining Case's 2 and 3 above, whereby the grid is stored as
-        an ndarray of shape [total_y_coordinates*sub_size, total_x_coordinates*sub_size, 2].
 
-        All sub-pixels in masked pixels have values (0.0, 0.0).
 
 
         **Grid2D Mapping:**
 
-        Every set of (y,x) coordinates in a pixel of the sub-grid maps to an unmasked pixel in the mask. For a uniform
+        Every set of (y,x) coordinates in a pixel of the grid maps to an unmasked pixel in the mask. For a uniform
         grid, every (y,x) coordinate directly corresponds to the location of its paired unmasked pixel.
 
         It is not a requirement that grid is uniform and that their coordinates align with the mask. The input grid
         could be an irregular set of (y,x) coordinates where the indexing signifies that the (y,x) coordinate
         *originates* or *is paired with* the mask's pixels but has had its value change by some aspect of the
         calculation.
 
@@ -232,92 +151,90 @@
         mask
             The 2D mask associated with the grid, defining the pixels each grid coordinate is paired with and
             originates from.
         store_native
             If True, the ndarray is stored in its native format [total_y_pixels, total_x_pixels, 2]. This avoids
             mapping large data arrays to and from the slim / native formats, which can be a computational bottleneck.
         """
-
         values = grid_2d_util.convert_grid_2d(
-            grid_2d=values, mask_2d=mask, store_native=store_native
+            grid_2d=values,
+            mask_2d=mask,
+            store_native=store_native,
         )
 
-        obj = values.view(cls)
-        obj.mask = mask
+        super().__init__(values)
 
-        grid_2d_util.check_grid_2d(grid_2d=obj)
+        self.mask = mask
 
-        return obj
+        grid_2d_util.check_grid_2d(grid_2d=values)
+
+        self.over_sampling = over_sampling
 
     @classmethod
     def no_mask(
         cls,
         values: Union[np.ndarray, List],
         pixel_scales: ty.PixelScales,
         shape_native: Tuple[int, int] = None,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
+        over_sampling: Optional[AbstractOverSampling] = None,
     ) -> "Grid2D":
         """
         Create a Grid2D (see *Grid2D.__new__*) by inputting the grid coordinates in 1D or 2D, automatically
         determining whether to use the 'manual_slim' or 'manual_native' methods.
 
         From 1D input the method cannot determine the 2D shape of the grid and its mask, thus the shape_native must be
         input into this method. The mask is setup as a unmasked `Mask2D` of shape_native.
 
         The 2D shape of the grid and its mask are determined from the input grid and the mask is setup as an
         unmasked `Mask2D` of shape_native.
 
         Parameters
         ----------
         values
-            The (y,x) coordinates of the grid input as an ndarray of shape [total_unmasked_pixells*(sub_size**2), 2]
+            The (y,x) coordinates of the grid input as an ndarray of shape [total_unmasked_pixels, 2]
             or a list of lists.
         shape_native
             The 2D shape of the mask the grid is paired with.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
         origin
             The origin of the grid's mask.
         """
 
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         values = grid_2d_util.convert_grid(grid=values)
 
         if len(values.shape) == 2:
             grid_2d_util.check_grid_slim(grid=values, shape_native=shape_native)
-
         else:
             shape_native = (
-                int(values.shape[0] / sub_size),
-                int(values.shape[1] / sub_size),
+                int(values.shape[0]),
+                int(values.shape[1]),
             )
 
         mask = Mask2D.all_false(
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
-        return Grid2D(values=values, mask=mask)
+        return Grid2D(values=values, mask=mask, over_sampling=over_sampling)
 
     @classmethod
     def from_yx_1d(
         cls,
         y: Union[np.ndarray, List],
         x: np.ndarray,
         shape_native: Tuple[int, int],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
+        over_sampling: Optional[AbstractOverSampling] = None,
     ) -> "Grid2D":
         """
         Create a Grid2D (see *Grid2D.__new__*) by inputting the grid coordinates as 1D y and x values.
 
         From 1D input the method cannot determine the 2D shape of the grid and its mask, thus the shape_native must be
         input into this method. The mask is setup as a unmasked `Mask2D` of shape_native.
 
@@ -328,16 +245,14 @@
         x or list
             The x coordinates of the grid input as an ndarray of shape [total_coordinates] or list.
         shape_native
             The 2D shape of the mask the grid is paired with.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
         origin
             The origin of the grid's mask.
 
         Examples
         --------
 
         .. code-block:: python
@@ -374,26 +289,26 @@
         if type(x) is list:
             x = np.asarray(x)
 
         return cls.no_mask(
             values=np.stack((y, x), axis=-1),
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
+            over_sampling=over_sampling,
         )
 
     @classmethod
     def from_yx_2d(
         cls,
         y: Union[np.ndarray, List],
         x: Union[np.ndarray, List],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
+        over_sampling: Optional[AbstractOverSampling] = None,
     ) -> "Grid2D":
         """
         Create a Grid2D (see *Grid2D.__new__*) by inputting the grid coordinates as 2D y and x values.
 
         The 2D shape of the grid and its mask are determined from the input grid and the mask is setup as an
         unmasked `Mask2D` of shape_native.
 
@@ -402,16 +317,14 @@
         y or list
             The y coordinates of the grid input as an ndarray of shape [total_coordinates] or list.
         x or list
             The x coordinates of the grid input as an ndarray of shape [total_coordinates] or list.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
         origin
             The origin of the grid's mask.
 
         Examples
         --------
 
         .. code-block:: python
@@ -431,24 +344,24 @@
 
         if type(x) is list:
             x = np.asarray(x)
 
         return cls.no_mask(
             values=np.stack((y, x), axis=-1),
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
+            over_sampling=over_sampling,
         )
 
     @classmethod
     def from_extent(
         cls,
         extent: Tuple[float, float, float, float],
         shape_native: Tuple[int, int],
-        sub_size: int = 1,
+        over_sampling: Optional[AbstractOverSampling] = None,
     ) -> "Grid2D":
         """
         Create a Grid2D (see *Grid2D.__new__*) by inputting the extent of the (y,x) grid coordinates as an input
         (x0, x1, y0, y1) tuple.
 
         The (y,x) `shape_native` in pixels is also input which determines the resolution of the `Grid2D`.
 
@@ -463,91 +376,86 @@
         extent
             The (x0, x1, y0, y1) extent of the grid in scaled coordinates over which the grid is created.
         shape_native
             The 2D shape of the grid that is created within this extent.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
         origin
             The origin of the grid's mask.
         """
 
         x0, x1, y0, y1 = extent
 
-        ys = np.linspace(y1, y0, shape_native[0] * sub_size)
-        xs = np.linspace(x0, x1, shape_native[1] * sub_size)
+        ys = np.linspace(y1, y0, shape_native[0])
+        xs = np.linspace(x0, x1, shape_native[1])
 
         xs_grid, ys_grid = np.meshgrid(xs, ys)
 
         xs_grid_1d = xs_grid.ravel()
         ys_grid_1d = ys_grid.ravel()
 
         grid_2d = np.vstack((ys_grid_1d, xs_grid_1d)).T
 
-        grid_2d = grid_2d.reshape(
-            (shape_native[0] * sub_size, shape_native[1] * sub_size, 2)
-        )
+        grid_2d = grid_2d.reshape((shape_native[0], shape_native[1], 2))
 
         pixel_scales = (
             abs(grid_2d[0, 0, 0] - grid_2d[1, 0, 0]),
             abs(grid_2d[0, 0, 1] - grid_2d[0, 1, 1]),
         )
 
-        return Grid2D.no_mask(values=grid_2d, pixel_scales=pixel_scales)
+        return Grid2D.no_mask(
+            values=grid_2d, pixel_scales=pixel_scales, over_sampling=over_sampling
+        )
 
     @classmethod
     def uniform(
         cls,
         shape_native: Tuple[int, int],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
+        over_sampling: Optional[AbstractOverSampling] = None,
     ) -> "Grid2D":
         """
         Create a `Grid2D` (see *Grid2D.__new__*) as a uniform grid of (y,x) values given an input `shape_native` and
         `pixel_scales` of the grid:
 
         Parameters
         ----------
         shape_native
             The 2D shape of the uniform grid and the mask that it is paired with.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factors of every pixel. If this is input as a `float`,
             it is converted to a (float, float) tuple.
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
         origin
             The origin of the grid's mask.
         """
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         grid_slim = grid_2d_util.grid_2d_slim_via_shape_native_from(
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
         return cls.no_mask(
             values=grid_slim,
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
+            over_sampling=over_sampling,
         )
 
     @classmethod
     def bounding_box(
         cls,
         bounding_box: np.ndarray,
         shape_native: Tuple[int, int],
-        sub_size: int = 1,
         buffer_around_corners: bool = False,
+        over_sampling: Optional[AbstractOverSampling] = None,
     ) -> "Grid2D":
         """
         Create a Grid2D (see *Grid2D.__new__*) from an input bounding box with coordinates [y_min, y_max, x_min, x_max],
         where the shape_native is used to compute the (y,x) grid values within this bounding box.
 
         If buffer_around_corners=True, the grid's (y,x) values fully align with the input bounding box values. This
         means the mask's edge pixels extend beyond the bounding box by pixel_scale/2.0. If buffer_around_corners=False,
@@ -557,16 +465,14 @@
         Parameters
         ----------
         shape_native
             The 2D shape of the uniform grid and the mask that it is paired with.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
         origin
             The origin of the grid's mask.
         buffer_around_corners
             Whether the grid is buffered such that the (y,x) values in the centre of its masks' edge pixels align
             with the input bounding box values.
         """
         y_min, y_max, x_min, x_max = bounding_box
@@ -583,83 +489,85 @@
                 (x_max - x_min) / (shape_native[1] - 1),
             )
         origin = ((y_max + y_min) / 2.0, (x_max + x_min) / 2.0)
 
         return cls.uniform(
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
+            over_sampling=over_sampling,
         )
 
     @classmethod
-    def from_mask(cls, mask: Mask2D) -> "Grid2D":
+    def from_mask(
+        cls, mask: Mask2D, over_sampling: Optional[AbstractOverSampling] = None
+    ) -> "Grid2D":
         """
         Create a Grid2D (see *Grid2D.__new__*) from a mask, where only unmasked pixels are included in the grid (if the
         grid is represented in its native 2D masked values are (0.0, 0.0)).
 
-        The mask's pixel_scales, sub_size and origin properties are used to compute the grid (y,x) coordinates.
+        The mask's pixel_scales and origin properties are used to compute the grid (y,x) coordinates.
 
         Parameters
         ----------
         mask
-            The mask whose masked pixels are used to setup the sub-pixel grid.
+            The mask whose masked pixels are used to setup the grid.
         """
 
-        sub_grid_1d = grid_2d_util.grid_2d_slim_via_mask_from(
-            mask_2d=mask,
+        grid_1d = grid_2d_util.grid_2d_slim_via_mask_from(
+            mask_2d=np.array(mask),
             pixel_scales=mask.pixel_scales,
-            sub_size=mask.sub_size,
             origin=mask.origin,
         )
 
-        return Grid2D(values=sub_grid_1d, mask=mask)
+        return Grid2D(values=grid_1d, mask=mask, over_sampling=over_sampling)
 
     @classmethod
     def from_fits(
         cls,
         file_path: Union[Path, str],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
+        over_sampling: Optional[AbstractOverSampling] = None,
     ) -> "Grid2D":
         """
         Create a Grid2D (see *Grid2D.__new__*) from a mask, where only unmasked pixels are included in the grid (if the
         grid is represented in its native 2D masked values are (0.0, 0.0)).
 
-        The mask's pixel_scales, sub_size and origin properties are used to compute the grid (y,x) coordinates.
+        The mask's pixel_scales and origin properties are used to compute the grid (y,x) coordinates.
 
         Parameters
         ----------
         mask
-            The mask whose masked pixels are used to setup the sub-pixel grid.
+            The mask whose masked pixels are used to setup the grid.
         """
 
-        sub_grid_2d = array_2d_util.numpy_array_2d_via_fits_from(
-            file_path=file_path, hdu=0
-        )
+        grid_2d = array_2d_util.numpy_array_2d_via_fits_from(file_path=file_path, hdu=0)
 
         return Grid2D.no_mask(
-            values=sub_grid_2d,
+            values=grid_2d,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
+            over_sampling=over_sampling,
         )
 
     @classmethod
     def blurring_grid_from(
-        cls, mask: Mask2D, kernel_shape_native: Tuple[int, int]
+        cls,
+        mask: Mask2D,
+        kernel_shape_native: Tuple[int, int],
+        over_sampling: Optional[AbstractOverSampling] = None,
     ) -> "Grid2D":
         """
         Setup a blurring-grid from a mask, where a blurring grid consists of all pixels that are masked (and
         therefore have their values set to (0.0, 0.0)), but are close enough to the unmasked pixels that their values
         will be convolved into the unmasked those pixels. This when computing images from
         light profile objects.
 
-        The mask's pixel_scales, sub_size and origin properties are used to compute the blurring grid's (y,x)
+        The mask's pixel_scales and origin properties are used to compute the blurring grid's (y,x)
         coordinates.
 
         For example, if our mask is as follows:
 
         .. code-block:: bash
 
              x x x x x x x x x xI
@@ -729,80 +637,72 @@
             The 2D shape of the kernel which convolves signal from masked pixels to unmasked pixels.
         """
 
         blurring_mask = mask.derive_mask.blurring_from(
             kernel_shape_native=kernel_shape_native
         )
 
-        return cls.from_mask(mask=blurring_mask)
+        return cls.from_mask(mask=blurring_mask, over_sampling=over_sampling)
+
+    def subtracted_from(self, offset: Tuple[(float, float), np.ndarray]) -> "Grid2D":
+        if offset[0] == 0.0 and offset[1] != 0.0:
+            return self
+
+        mask = Mask2D(
+            mask=self.mask,
+            pixel_scales=self.pixel_scales,
+            origin=(self.origin[0] - offset[0], self.origin[1] - offset[1]),
+        )
+
+        return Grid2D(
+            values=self - np.array(offset), mask=mask, over_sampling=self.over_sampling
+        )
 
     @property
     def slim(self) -> "Grid2D":
         """
         Return a `Grid2D` where the data is stored its `slim` representation, which is an ndarray of shape
-        [total_unmasked_pixels * sub_size**2, 2].
+        [total_unmasked_pixels, 2].
 
         If it is already stored in its `slim` representation  it is returned as it is. If not, it is  mapped from
         `native` to `slim` and returned as a new `Grid2D`.
         """
-        return Grid2D(values=self, mask=self.mask)
+        return Grid2D(values=self, mask=self.mask, over_sampling=self.over_sampling)
 
     @property
     def native(self) -> "Grid2D":
         """
         Return a `Grid2D` where the data is stored in its `native` representation, which has shape
-        [sub_size*total_y_pixels, sub_size*total_x_pixels, 2].
+        [total_y_pixels, total_x_pixels, 2].
 
         If it is already stored in its `native` representation it is return as it is. If not, it is mapped from
         `slim` to `native` and returned as a new `Grid2D`.
 
         This method is used in the child `Grid2D` classes to create their `native` properties.
         """
-        return Grid2D(values=self, mask=self.mask, store_native=True)
-
-    @property
-    def binned(self) -> "Grid2D":
-        """
-        Return a `Grid2D` of the binned-up grid in its 1D representation, which is stored with
-        shape [total_unmasked_pixels, 2].
-
-        The binning up process converts a grid from (y,x) values where each value is a coordinate on the sub-grid to
-        (y,x) values where each coordinate is at the centre of its mask (e.g. a grid with a sub_size of 1). This is
-        performed by taking the mean of all (y,x) values in each sub pixel.
-
-        If the grid is stored in 1D it is return as is. If it is stored in 2D, it must first be mapped from 2D to 1D.
-        """
-
-        grid_2d_slim = self.slim
-
-        grid_2d_slim_binned_y = np.multiply(
-            self.mask.sub_fraction,
-            grid_2d_slim[:, 0].reshape(-1, self.mask.sub_length).sum(axis=1),
-        )
-
-        grid_2d_slim_binned_x = np.multiply(
-            self.mask.sub_fraction,
-            grid_2d_slim[:, 1].reshape(-1, self.mask.sub_length).sum(axis=1),
-        )
-
-        grid_2d_binned = np.stack(
-            (grid_2d_slim_binned_y, grid_2d_slim_binned_x), axis=-1
+        return Grid2D(
+            values=self,
+            mask=self.mask,
+            over_sampling=self.over_sampling,
+            store_native=True,
         )
 
-        return Grid2D(values=grid_2d_binned, mask=self.mask.derive_mask.sub_1)
+    @cached_property
+    def over_sampler(self) -> AbstractOverSampler:
+        return self.over_sampling.over_sampler_from(mask=self.mask)
 
     @property
     def flipped(self) -> "Grid2D":
         """
         Return the grid as an ndarray of shape [total_unmasked_pixels, 2] with flipped values such that coordinates
         are given as (x,y) values.
 
         This is used to interface with Python libraries that require the grid in (x,y) format.
         """
-        return np.fliplr(self)
+        return self.with_new_array(np.fliplr(self.array))
 
     @property
     def in_radians(self) -> "Grid2D":
         """
         Return the grid as an ndarray where all (y,x) values are converted to Radians.
 
         This grid is used by the interferometer module.
@@ -817,15 +717,19 @@
         This is used by PyAutoLens to perform grid ray-tracing.
 
         Parameters
         ----------
         deflection_grid
             The grid of (y,x) coordinates which is subtracted from this grid.
         """
-        return Grid2D(values=self - deflection_grid, mask=self.mask)
+        return Grid2D(
+            values=self - deflection_grid,
+            mask=self.mask,
+            over_sampling=self.over_sampling,
+        )
 
     def blurring_grid_via_kernel_shape_from(
         self, kernel_shape_native: Tuple[int, int]
     ) -> "Grid2D":
         """
         Returns the blurring grid from a grid, via an input 2D kernel shape.
 
@@ -834,15 +738,17 @@
             Parameters
             ----------
             kernel_shape_native
                 The 2D shape of the kernel which convolves signal from masked pixels to unmasked pixels.
         """
 
         return Grid2D.blurring_grid_from(
-            mask=self.mask, kernel_shape_native=kernel_shape_native
+            mask=self.mask,
+            kernel_shape_native=kernel_shape_native,
+            over_sampling=None,
         )
 
     def grid_with_coordinates_within_distance_removed_from(
         self, coordinates: Union[np.ndarray, List], distance: float
     ) -> "Grid2D":
         """Remove all coordinates from this Grid2D which are within a certain distance of an input list of coordinates.
 
@@ -866,72 +772,18 @@
             distances = self.distances_to_coordinate_from(coordinate=coordinate)
 
             distance_mask += distances.native < distance
 
         mask = Mask2D(
             mask=distance_mask,
             pixel_scales=self.pixel_scales,
-            sub_size=self.sub_size,
             origin=self.origin,
         )
 
-        return Grid2D.from_mask(mask=mask)
-
-    def structure_2d_from(self, result: np.ndarray) -> Union[Array2D, "Grid2D"]:
-        """
-        Convert a result from an ndarray to an aa.Array2D or aa.Grid2D structure, where the conversion depends on
-        type(result) as follows:
-
-        - 1D np.ndarray   -> aa.Array2D
-        - 2D np.ndarray   -> aa.Grid2D
-
-        This function is used by the grid_2d_to_structure decorator to convert the output result of a function
-        to an autoarray structure when a `Grid2D` instance is passed to the decorated function.
-
-        Parameters
-        ----------
-        result or [np.ndarray]
-            The input result (e.g. of a decorated function) that is converted to a PyAutoArray structure.
-        """
-        from autoarray.structures.grids.transformed_2d import Grid2DTransformed
-        from autoarray.structures.grids.transformed_2d import Grid2DTransformedNumpy
-
-        if len(result.shape) == 1:
-            return Array2D(values=result, mask=self.mask)
-        else:
-            if isinstance(result, Grid2DTransformedNumpy):
-                return Grid2DTransformed(values=result, mask=self.mask)
-            return Grid2D(values=result, mask=self.mask)
-
-    def structure_2d_list_from(
-        self, result_list: List
-    ) -> List[Union[Array2D, "Grid2D"]]:
-        """
-        Convert a result from a list of ndarrays to a list of aa.Array2D or aa.Grid2D structure, where the conversion
-        depends on type(result) as follows:
-
-        - [1D np.ndarray] -> [aa.Array2D]
-        - [2D np.ndarray] -> [aa.Grid2D]
-
-        This function is used by the grid_like_list_to_structure-list decorator to convert the output result of a
-        function to a list of autoarray structure when a `Grid2D` instance is passed to the decorated function.
-
-        Parameters
-        ----------
-        result_list or [np.ndarray]
-            The input result (e.g. of a decorated function) that is converted to a PyAutoArray structure.
-        """
-        return [self.structure_2d_from(result=result) for result in result_list]
-
-    def values_from(self, array_slim: np.ndarray) -> ArrayIrregular:
-        """
-        Create a *ArrayIrregular* object from a 1D NumPy array of values of shape [total_coordinates]. The
-        *ArrayIrregular* are structured following this `Grid2DIrregular` instance.
-        """
-        return ArrayIrregular(values=array_slim)
+        return Grid2D.from_mask(mask=mask, over_sampling=self.over_sampling)
 
     def squared_distances_to_coordinate_from(
         self, coordinate: Tuple[float, float] = (0.0, 0.0)
     ) -> Array2D:
         """
         Returns the squared distance of every coordinate on the grid from an input coordinate.
 
@@ -1000,36 +852,34 @@
         ----------
         extent
             The extent of the grid the radii grid is computed using, with format [xmin, xmax, ymin, ymax]
         centre : (float, flloat)
             The (y,x) central coordinate which the radial grid is traced outwards from.
         pixel_scales
             The (y,x) scaled units to pixel units conversion factor of the 2D mask array.
-        sub_size
-            The size of the sub-grid that each pixel of the 2D mask array is divided into.
 
         Returns
         -------
         int
             The 1D integer shape of a radial set of points sampling the longest distance from the centre to the edge of the
             extent in along the positive x-axis.
         """
 
         return grid_2d_util._radial_projected_shape_slim_from(
             extent=self.geometry.extent,
             centre=centre,
             pixel_scales=self.mask.pixel_scales,
-            sub_size=self.mask.sub_size,
         )
 
     def grid_2d_radial_projected_from(
         self,
         centre: Tuple[float, float] = (0.0, 0.0),
         angle: float = 0.0,
         shape_slim: Optional[int] = 0,
+        remove_projected_centre: bool = None,
     ) -> Grid2DIrregular:
         """
         Determine a projected radial grid of points from a 2D region of coordinates defined by an
         extent [xmin, xmax, ymin, ymax] and with a (y,x) centre.
 
         This functions operates as follows:
 
@@ -1074,28 +924,32 @@
         """
 
         grid_radial_projected_2d = (
             grid_2d_util.grid_scaled_2d_slim_radial_projected_from(
                 extent=self.geometry.extent,
                 centre=centre,
                 pixel_scales=self.mask.pixel_scales,
-                sub_size=self.mask.sub_size,
                 shape_slim=shape_slim,
             )
         )
 
         grid_radial_projected_2d = geometry_util.transform_grid_2d_to_reference_frame(
             grid_2d=grid_radial_projected_2d, centre=centre, angle=angle
         )
 
         grid_radial_projected_2d = geometry_util.transform_grid_2d_from_reference_frame(
             grid_2d=grid_radial_projected_2d, centre=centre, angle=0.0
         )
 
-        if conf.instance["general"]["grid"]["remove_projected_centre"]:
+        if remove_projected_centre is None:
+            remove_projected_centre = conf.instance["general"]["grid"][
+                "remove_projected_centre"
+            ]
+
+        if remove_projected_centre:
             grid_radial_projected_2d = grid_radial_projected_2d[1:, :]
 
         return Grid2DIrregular(values=grid_radial_projected_2d)
 
     @property
     def shape_native_scaled_interior(self) -> Tuple[float, float]:
         """
@@ -1144,24 +998,14 @@
         return [
             self.scaled_minima[1] - buffer,
             self.scaled_maxima[1] + buffer,
             self.scaled_minima[0] - buffer,
             self.scaled_maxima[0] + buffer,
         ]
 
-    @cached_property
-    def sub_border_grid(self) -> np.ndarray:
-        """
-        The (y,x) grid of all sub-pixels which are at the border of the mask.
-
-        This is NOT all sub-pixels which are in mask pixels at the mask's border, but specifically the sub-pixels
-        within these border pixels which are at the extreme edge of the border.
-        """
-        return self[self.mask.derive_indexes.sub_border_slim]
-
     def padded_grid_from(self, kernel_shape_native: Tuple[int, int]) -> "Grid2D":
         """
         When the edge pixels of a mask are unmasked and a convolution is to occur, the signal of edge pixels will
         be 'missing' if the grid is used to evaluate the signal via an analytic function.
 
         To ensure this signal is included the padded grid is used, which is 'buffed' such that it includes all pixels
         whose signal will be convolved into the unmasked pixels given the 2D kernel shape.
@@ -1178,66 +1022,10 @@
             shape[0] + kernel_shape_native[0] - 1,
             shape[1] + kernel_shape_native[1] - 1,
         )
 
         padded_mask = Mask2D.all_false(
             shape_native=padded_shape,
             pixel_scales=self.mask.pixel_scales,
-            sub_size=self.mask.sub_size,
-        )
-
-        return Grid2D.from_mask(mask=padded_mask)
-
-    def relocated_grid_from(self, grid: "Grid2D") -> "Grid2D":
-        """
-        Relocate the coordinates of a grid to the border of this grid if they are outside the border, where the
-        border is defined as all pixels at the edge of the grid's mask (see *mask._border_1d_indexes*).
-
-        This is performed as follows:
-
-        1: Use the mean value of the grid's y and x coordinates to determine the origin of the grid.
-        2: Compute the radial distance of every grid coordinate from the origin.
-        3: For every coordinate, find its nearest pixel in the border.
-        4: Determine if it is outside the border, by comparing its radial distance from the origin to its paired
-        border pixel's radial distance.
-        5: If its radial distance is larger, use the ratio of radial distances to move the coordinate to the
-        border (if its inside the border, do nothing).
-
-        The method can be used on uniform or irregular grids, however for irregular grids the border of the
-        'image-plane' mask is used to define border pixels.
-
-        Parameters
-        ----------
-        grid : Grid2D
-            The grid (uniform or irregular) whose pixels are to be relocated to the border edge if outside it.
-        """
-
-        if len(self.sub_border_grid) == 0:
-            return grid
-
-        return Grid2D(
-            values=grid_2d_util.relocated_grid_via_jit_from(
-                grid=grid, border_grid=self.sub_border_grid
-            ),
-            mask=grid.mask,
-            sub_size=grid.mask.sub_size,
         )
 
-    def relocated_mesh_grid_from(self, mesh_grid: Grid2DIrregular) -> Grid2DIrregular:
-        """
-        Relocate the coordinates of a pixelization grid to the border of this grid. See the
-        method ``relocated_grid_from()`` for a full description of how this grid relocation works.
-
-        Parameters
-        ----------
-        grid
-            The pixelization grid whose pixels are relocated to the border edge if outside it.
-        """
-
-        if len(self.sub_border_grid) == 0:
-            return mesh_grid
-
-        return Grid2DIrregular(
-            values=grid_2d_util.relocated_grid_via_jit_from(
-                grid=mesh_grid, border_grid=self.sub_border_grid
-            ),
-        )
+        return Grid2D.from_mask(mask=padded_mask, over_sampling=self.over_sampling)
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/header.py` & `autoarray-2024.5.16.0/autoarray/structures/header.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/structures/mesh/abstract_2d.py` & `autoarray-2024.5.16.0/autoarray/structures/mesh/abstract_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/structures/mesh/delaunay_2d.py` & `autoarray-2024.5.16.0/autoarray/structures/mesh/delaunay_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/structures/mesh/rectangular_2d.py` & `autoarray-2024.5.16.0/autoarray/structures/mesh/rectangular_2d.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import numpy as np
 from scipy.interpolate import griddata
 from typing import List, Optional, Tuple
 
-from autoconf import cached_property
-
+from autoarray import type as ty
 from autoarray.inversion.linear_obj.neighbors import Neighbors
+from autoarray.inversion.pixelization.mesh import mesh_util
 from autoarray.mask.mask_2d import Mask2D
+from autoarray.structures.abstract_structure import Structure
 from autoarray.structures.arrays.uniform_2d import Array2D
-from autoarray.structures.mesh.abstract_2d import Abstract2DMesh
-
 from autoarray.structures.grids import grid_2d_util
-from autoarray.inversion.pixelization.mesh import mesh_util
-from autoarray import type as ty
+from autoarray.structures.mesh.abstract_2d import Abstract2DMesh
+from autoconf import cached_property
 
 
 class Mesh2DRectangular(Abstract2DMesh):
-    def __new__(
-        cls,
+    @property
+    def slim(self) -> "Structure":
+        raise NotImplementedError()
+
+    @property
+    def native(self) -> Structure:
+        raise NotImplementedError()
+
+    def __init__(
+        self,
         values: np.ndarray,
         shape_native: Tuple[int, int],
         pixel_scales: ty.PixelScales,
         origin: Tuple[float, float] = (0.0, 0.0),
-        *args,
-        **kwargs
     ):
         """
         A grid of (y,x) coordinates which represent a uniform rectangular pixelization.
 
         A `Mesh2DRectangular` is ordered such pixels begin from the top-row and go rightwards and then downwards.
         It is an ndarray of shape [total_pixels, 2], where the first dimension of the ndarray corresponds to the
         pixelization's pixel index and second element whether it is a y or x arc-second coordinate.
@@ -51,22 +56,20 @@
         origin
             The (y,x) origin of the pixelization.
         """
 
         mask = Mask2D.all_false(
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=1,
             origin=origin,
         )
 
-        obj = values.view(cls)
-        obj.mask = mask
+        self.mask = mask
 
-        return obj
+        super().__init__(array=values)
 
     @classmethod
     def overlay_grid(
         cls, shape_native: Tuple[int, int], grid: np.ndarray, buffer: float = 1e-8
     ) -> "Mesh2DRectangular":
         """
         Creates a `Grid2DRecntagular` by overlaying the rectangular pixelization over an input grid of (y,x)
@@ -100,15 +103,14 @@
         )
 
         origin = ((y_max + y_min) / 2.0, (x_max + x_min) / 2.0)
 
         grid_slim = grid_2d_util.grid_2d_slim_via_shape_native_from(
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=1,
             origin=origin,
         )
 
         return Mesh2DRectangular(
             values=grid_slim,
             shape_native=shape_native,
             pixel_scales=pixel_scales,
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/mesh/triangulation_2d.py` & `autoarray-2024.5.16.0/autoarray/structures/mesh/triangulation_2d.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import numpy as np
 import scipy.spatial
-import scipy.spatial.qhull as qhull
-from typing import Optional, List, Union, Tuple
+from typing import List, Union, Tuple
 
+from autoarray.structures.abstract_structure import Structure
 from autoconf import cached_property
 
 from autoarray.geometry.geometry_2d_irregular import Geometry2DIrregular
 from autoarray.structures.mesh.abstract_2d import Abstract2DMesh
 
 from autoarray import exc
 from autoarray.inversion.pixelization.mesh import mesh_util
 from autoarray.structures.grids import grid_2d_util
 
 
 class Abstract2DMeshTriangulation(Abstract2DMesh):
-    def __new__(
-        cls,
+    @property
+    def slim(self) -> "Structure":
+        raise NotImplementedError()
+
+    @property
+    def native(self) -> Structure:
+        raise NotImplementedError()
+
+    def __init__(
+        self,
         values: Union[np.ndarray, List],
         uses_interpolation: bool = False,
-        *args,
-        **kwargs
     ):
         """
         An irregular 2D grid of (y,x) coordinates which represents both a Delaunay triangulation and Voronoi mesh.
 
         The input irregular `2D` grid represents both of the following quantities:
 
         - The corners of the Delaunay triangulles used to construct a Delaunay triangulation.
@@ -47,18 +53,17 @@
         values
             The grid of (y,x) coordinates corresponding to the Delaunay triangle corners and Voronoi pixel centres.
         """
 
         if type(values) is list:
             values = np.asarray(values)
 
-        obj = values.view(cls)
-        obj.uses_interpolation = uses_interpolation
+        self.uses_interpolation = uses_interpolation
 
-        return obj
+        super().__init__(values)
 
     def __array_finalize__(self, obj: object):
         """
         Ensures that the attribute `uses_interpolation` are retained when numpy array calculations are performed.
         """
 
         if hasattr(obj, "uses_interpolation"):
@@ -201,24 +206,14 @@
 
         region_areas[region_areas == -1] = max_area
         region_areas[region_areas > max_area] = max_area
 
         return region_areas
 
     @property
-    def sub_border_grid(self) -> np.ndarray:
-        """
-        The (y,x) grid of all sub-pixels which are at the border of the mask.
-
-        This is NOT all sub-pixels which are in mask pixels at the mask's border, but specifically the sub-pixels
-        within these border pixels which are at the extreme edge of the border.
-        """
-        return self[self.mask.derive_indexes.sub_border_slim]
-
-    @property
     def origin(self) -> Tuple[float, float]:
         """
         The (y,x) origin of the Voronoi grid, which is fixed to (0.0, 0.0) for simplicity.
         """
         return 0.0, 0.0
 
     @property
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/mesh/voronoi_2d.py` & `autoarray-2024.5.16.0/autoarray/structures/mesh/voronoi_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/structures/mock/mock_grid.py` & `autoarray-2024.5.16.0/autoarray/structures/mock/mock_grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,41 @@
 import numpy as np
-from typing import Tuple
+from typing import Tuple, List
 
 from autoarray.geometry.abstract_2d import AbstractGeometry2D
 from autoarray.inversion.linear_obj.neighbors import Neighbors
+from autoarray.structures.abstract_structure import Structure
 from autoarray.structures.mesh.abstract_2d import Abstract2DMesh
 
 
 class MockGeometry(AbstractGeometry2D):
     def __init__(self, extent):
         self._extent = extent
 
     @property
     def extent(self) -> Tuple[float, float, float, float]:
         return self._extent
 
 
 class MockGrid2DMesh(Abstract2DMesh):
-    def __new__(cls, grid: np.ndarray = None, extent: Tuple[int, int, int, int] = None):
+    @property
+    def pixels(self) -> int:
+        raise NotImplementedError()
+
+    @property
+    def slim(self) -> "Structure":
+        raise NotImplementedError()
+
+    @property
+    def native(self) -> Structure:
+        raise NotImplementedError()
+
+    def __init__(
+        self, grid: np.ndarray = None, extent: Tuple[int, int, int, int] = None
+    ):
         """
         A grid of (y,x) coordinates which represent a uniform rectangular pixelization.
 
         A `Mesh2DRectangular` is ordered such pixels begin from the top-row and go rightwards and then downwards.
         It is an ndarray of shape [total_pixels, 2], where the first dimension of the ndarray corresponds to the
         pixelization's pixel index and second element whether it is a y or x arc-second coordinate.
 
@@ -44,18 +59,17 @@
         origin
             The (y,x) origin of the pixelization.
         """
 
         if grid is None:
             grid = np.ones(shape=(1, 2))
 
-        obj = grid.view(cls)
-        obj._extent = extent
+        self._extent = extent
 
-        return obj
+        super().__init__(grid)
 
     @property
     def geometry(self):
         return MockGeometry(extent=self.extent)
 
     @property
     def extent(self) -> Tuple[float, float, float, float]:
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/mock/mock_structure_decorators.py` & `autoarray-2024.5.16.0/autoarray/structures/mock/mock_decorators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import numpy as np
 
-from autoarray.structures import structure_decorators
+from autoarray.structures import decorators
+from autoarray.operators.over_sampling.decorator import over_sample
 
 
 ### Grids ###
 
 
-def radial_grid_from(grid):
+def radial_grid_from(grid, *args, **kwargs):
     return np.sqrt(np.add(np.square(grid[:, 0]), np.square(grid[:, 1])))
 
 
-def ndarray_1d_from(profile, grid):
+def ndarray_1d_from(profile, grid, *args, **kwargs):
     sersic_constant = (
         (2 * 2.0)
         - (1.0 / 3.0)
         + (4.0 / (405.0 * 2.0))
         + (46.0 / (25515.0 * 2.0**2))
         + (131.0 / (1148175.0 * 2.0**3))
         - (2194697.0 / (30690717750.0 * 2.0**4))
@@ -26,26 +27,34 @@
         np.multiply(
             -sersic_constant,
             np.add(np.power(np.divide(grid_radii, 0.2), 1.0 / 2.0), -1),
         )
     )
 
 
-def angle_to_profile_grid_from(grid_angles):
+def ndarray_1d_zeros_from(profile, grid, *args, **kwargs):
+    return np.zeros(shape=(5, 5))
+
+
+def ndarray_1d_list_from(profile, grid, *args, **kwargs):
+    return [ndarray_1d_from(profile, grid)]
+
+
+def angle_to_profile_grid_from(grid_angles, *args, **kwargs):
     """The angle between each (y,x) coordinate on the grid and the profile, in radians.
 
     Parameters
     ----------
     grid_angles
         The angle theta counter-clockwise from the positive x-axis to each coordinate in radians.
     """
     return np.cos(grid_angles), np.sin(grid_angles)
 
 
-def _cartesian_grid_via_radial_from(grid, radius):
+def _cartesian_grid_via_radial_from(grid, radius, *args, **kwargs):
     """
     Convert a grid of (y,x) coordinates with their specified circular radii to their original (y,x) Cartesian
     coordinates.
 
     Parameters
     ----------
     grid
@@ -54,20 +63,28 @@
         The circular radius of each coordinate from the profile center.
     """
     grid_angles = np.arctan2(grid[:, 0], grid[:, 1])
     cos_theta, sin_theta = angle_to_profile_grid_from(grid_angles=grid_angles)
     return np.multiply(radius[:, None], np.vstack((sin_theta, cos_theta)).T)
 
 
-def ndarray_2d_from(profile, grid):
+def ndarray_2d_from(profile, grid, *args, **kwargs):
     return _cartesian_grid_via_radial_from(
         grid=grid, radius=np.full(grid.shape[0], 2.0)
     )
 
 
+def ndarray_2d_list_from(profile, grid, *args, **kwargs):
+    return [ndarray_2d_from(profile, grid)]
+
+
+def ndarray_2d_yx_from(profile, grid, *args, **kwargs):
+    return 2.0 * grid
+
+
 class MockGridLikeIteratorObj:
     def __init__(self):
         pass
 
     @property
     def sersic_constant(self):
         return (
@@ -104,57 +121,57 @@
         radius
             The circular radius of each coordinate from the profile center.
         """
         grid_angles = np.arctan2(grid[:, 0], grid[:, 1])
         cos_theta, sin_theta = self.angle_to_profile_grid_from(grid_angles=grid_angles)
         return np.multiply(radius[:, None], np.vstack((sin_theta, cos_theta)).T)
 
-    @structure_decorators.grid_2d_to_structure
-    def ndarray_1d_from(self, grid) -> np.ndarray:
+    @over_sample
+    @decorators.to_array
+    def ndarray_1d_from(self, grid, *args, **kwargs) -> np.ndarray:
         """
         Mock function mimicking the behaviour of a class function which given an input 1D grid, returns a 1D ndarray
         of shape [total_masked_grid_pixels].
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         grid_radii = self.radial_grid_from(grid=grid)
         return np.exp(
             np.multiply(
                 -self.sersic_constant,
                 np.add(np.power(np.divide(grid_radii, 0.2), 1.0 / 2.0), -1),
             )
         )
 
-    @structure_decorators.grid_2d_to_structure
-    def ndarray_2d_from(self, grid):
+    @decorators.to_grid
+    def ndarray_2d_from(self, grid, *args, **kwargs):
         """
         Mock function mimicking the behaviour of a class function which given an input grid, returns a 2D ndarray
         of shape [total_masked_grid_pixels, 2].
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         return self._cartesian_grid_via_radial_from(
             grid=grid, radius=np.full(grid.shape[0], 2.0)
         )
 
-    @structure_decorators.grid_2d_to_vector_yx
-    @structure_decorators.grid_2d_to_structure
-    def ndarray_yx_2d_from(self, grid):
+    @decorators.to_vector_yx
+    def ndarray_yx_2d_from(self, grid, *args, **kwargs):
         """
         Mock function mimicking the behaviour of a class function which given an input grid, returns a 2D ndarray
         of shape [total_masked_grid_pixels] which represents a vector field.
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         return self._cartesian_grid_via_radial_from(
             grid=grid, radius=np.full(grid.shape[0], 2.0)
         )
 
-    @structure_decorators.grid_2d_to_structure_list
-    def ndarray_1d_list_from(self, grid):
+    @decorators.to_array
+    def ndarray_1d_list_from(self, grid, *args, **kwargs):
         """
         Mock function mimicking the behaviour of a class function which given an input 1D grid, returns a list of 1D
         ndarrays of shape [total_masked_grid_pixels].
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         grid_radii = self.radial_grid_from(grid=grid)
@@ -163,31 +180,30 @@
                 np.multiply(
                     -self.sersic_constant,
                     np.add(np.power(np.divide(grid_radii, 0.2), 1.0 / 2.0), -1),
                 )
             )
         ]
 
-    @structure_decorators.grid_2d_to_structure_list
-    def ndarray_2d_list_from(self, grid):
+    @decorators.to_grid
+    def ndarray_2d_list_from(self, grid, *args, **kwargs):
         """
         Mock function mimicking the behaviour of a class function which given an input grid, returns a 2D list of
         ndarrays of shape [total_masked_grid_pixels, 2].
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         return [
             self._cartesian_grid_via_radial_from(
                 grid=grid, radius=np.full(grid.shape[0], 2.0)
             )
         ]
 
-    @structure_decorators.grid_2d_to_vector_yx_list
-    @structure_decorators.grid_2d_to_structure_list
-    def ndarray_yx_2d_list_from(self, grid):
+    @decorators.to_vector_yx
+    def ndarray_yx_2d_list_from(self, grid, *args, **kwargs):
         """
         Mock function mimicking the behaviour of a class function which given an input grid, returns a list of 2D
         ndarrays of shape [total_masked_grid_pixels] which represents a vector field.
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         return [
@@ -198,89 +214,77 @@
 
 
 class MockGrid1DLikeObj:
     def __init__(self, centre=(0.0, 0.0), angle=0.0):
         self.centre = centre
         self.angle = angle
 
-    @structure_decorators.grid_1d_to_structure
-    def ndarray_1d_from(self, grid):
+    @over_sample
+    @decorators.project_grid
+    def ndarray_1d_from(self, grid, *args, **kwargs):
         return np.ones(shape=grid.shape[0])
 
-    # @structure_decorators.grid_1d_to_structure
-    # def ndarray_2d_from(self, grid):
-    #     return np.multiply(2.0, grid)
-
-    # @structure_decorators.grid_1d_to_structure_list
-    # def ndarray_1d_list_from(self, grid):
-    #     return [np.ones(shape=grid.shape[0]), 2.0 * np.ones(shape=grid.shape[0])]
-    #
-    # @structure_decorators.grid_1d_to_structure_list
-    # def ndarray_2d_list_from(self, grid):
-    #     return [np.multiply(1.0, grid), np.multiply(2.0, grid)]
-
 
 class MockGrid2DLikeObj:
     def __init__(self):
         pass
 
-    @structure_decorators.grid_2d_to_structure
-    def ndarray_1d_from(self, grid):
+    @over_sample
+    @decorators.to_array
+    def ndarray_1d_from(self, grid, *args, **kwargs):
         """
         Mock function mimicking the behaviour of a class function which given an input 1D grid, returns a 1D ndarray
         of shape [total_masked_grid_pixels].
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         return np.ones(shape=grid.shape[0])
 
-    @structure_decorators.grid_2d_to_structure
-    def ndarray_2d_from(self, grid):
+    @decorators.to_grid
+    def ndarray_2d_from(self, grid, *args, **kwargs):
         """
         Mock function mimicking the behaviour of a class function which given an input grid, returns a 2D ndarray
         of shape [total_masked_grid_pixels, 2].
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         return np.multiply(2.0, grid)
 
-    @structure_decorators.grid_2d_to_vector_yx
-    @structure_decorators.grid_2d_to_structure
-    def ndarray_yx_2d_from(self, grid):
+    @decorators.to_vector_yx
+    def ndarray_yx_2d_from(self, grid, *args, **kwargs):
         """
         Mock function mimicking the behaviour of a class function which given an input grid, returns a 2D ndarray
         of shape [total_masked_grid_pixels] which represents a vector field.
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         return 2.0 * grid
 
-    @structure_decorators.grid_2d_to_structure_list
-    def ndarray_1d_list_from(self, grid):
+    @decorators.to_array
+    def ndarray_1d_list_from(self, grid, *args, **kwargs):
         """
         Mock function mimicking the behaviour of a class function which given an input 1D grid, returns a list of 1D
         ndarrays of shape [total_masked_grid_pixels].
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         return [np.ones(shape=grid.shape[0]), 2.0 * np.ones(shape=grid.shape[0])]
 
-    @structure_decorators.grid_2d_to_structure_list
-    def ndarray_2d_list_from(self, grid):
+    @decorators.to_grid
+    def ndarray_2d_list_from(self, grid, *args, **kwargs):
         """
         Mock function mimicking the behaviour of a class function which given an input grid, returns a 2D list of
         ndarrays of shape [total_masked_grid_pixels, 2].
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         return [np.multiply(1.0, grid), np.multiply(2.0, grid)]
 
-    @structure_decorators.grid_2d_to_vector_yx_list
-    @structure_decorators.grid_2d_to_structure_list
-    def ndarray_yx_2d_list_from(self, grid):
+    @decorators.to_vector_yx
+    def ndarray_yx_2d_list_from(self, grid, *args, **kwargs):
         """
         Mock function mimicking the behaviour of a class function which given an input grid, returns a list of 2D
         ndarrays of shape [total_masked_grid_pixels] which represents a vector field.
 
         Such functions are common in **PyAutoGalaxy** for light and mass profile objects.
         """
         return [np.multiply(1.0, grid), np.multiply(2.0, grid)]
@@ -289,10 +293,10 @@
 class MockGridRadialMinimum:
     def __init__(self):
         pass
 
     def radial_grid_from(self, grid):
         return np.sqrt(np.add(np.square(grid[:, 0]), np.square(grid[:, 1])))
 
-    @structure_decorators.relocate_to_radial_minimum
+    @decorators.relocate_to_radial_minimum
     def deflections_yx_2d_from(self, grid):
         return grid
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/plot/structure_plotters.py` & `autoarray-2024.5.16.0/autoarray/structures/plot/structure_plotters.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
         mat_plot_1d: MatPlot1D = MatPlot1D(),
         visuals_1d: Visuals1D = Visuals1D(),
         include_1d: Include1D = Include1D(),
         should_plot_grid: bool = False,
         should_plot_zero: bool = False,
         plot_axis_type: Optional[str] = None,
         plot_yx_dict=None,
+        auto_labels=AutoLabels(),
     ):
         """
         Plots two 1D objects using the matplotlib method `plot()` (or a similar method) and many other matplotlib
         functions which customize the plot's appearance.
 
         The `mat_plot_1d` attribute wraps matplotlib function calls to make the figure. By default, the settings
         passed to every matplotlib function called are those specified in the `config/visualize/mat_wrap/*.ini` files,
@@ -174,26 +175,27 @@
 
         self.y = y
         self.x = y.grid_radial if x is None else x
         self.should_plot_grid = should_plot_grid
         self.should_plot_zero = should_plot_zero
         self.plot_axis_type = plot_axis_type
         self.plot_yx_dict = plot_yx_dict or {}
+        self.auto_labels = auto_labels
 
     def get_visuals_1d(self) -> Visuals1D:
         return self.get_1d.via_array_1d_from(array_1d=self.x)
 
     def figure_1d(self):
         """
         Plots the plotter's y and x values in 1D.
         """
 
         self.mat_plot_1d.plot_yx(
             y=self.y,
             x=self.x,
             visuals_1d=self.get_visuals_1d(),
-            auto_labels=AutoLabels(),
+            auto_labels=self.auto_labels,
             should_plot_grid=self.should_plot_grid,
             should_plot_zero=self.should_plot_zero,
             plot_axis_type_override=self.plot_axis_type,
             **self.plot_yx_dict
         )
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/vectors/abstract.py` & `autoarray-2024.5.16.0/autoarray/structures/vectors/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/structures/vectors/irregular.py` & `autoarray-2024.5.16.0/autoarray/structures/vectors/irregular.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from autoarray import exc
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class VectorYX2DIrregular(AbstractVectorYX2D):
-    def __new__(
-        cls,
+    def __init__(
+        self,
         values: Union[
             np.ndarray, List[np.ndarray], List[List], List[Tuple[float, float]]
         ],
         grid: Union[Grid2DIrregular, List],
     ):
         """
         A collection of (y,x) vectors which are located on a irregular 2D grid of (y,x) coordinates.
@@ -40,37 +40,37 @@
         ----------
         values
             The 2D (y,x) vectors on an irregular grid that represent the vector-field.
         grid
             The irregular grid of (y,x) coordinates where each vector is located.
         """
 
-        if len(values) == 0:
-            return []
-
         if type(values) is list:
             values = np.asarray(values)
 
-        obj = values.view(cls)
-        obj.grid = Grid2DIrregular(values=grid)
+        self.grid = Grid2DIrregular(values=grid)
 
-        return obj
+        super().__init__(values)
 
     def __array_finalize__(self, obj):
         if hasattr(obj, "grid"):
             self.grid = obj.grid
 
     @property
     def slim(self) -> np.ndarray:
         """
         The vector-field in its 1D representation, an ndarray of shape [total_vectors, 2].
         """
         return self
 
     @property
+    def native(self) -> np.ndarray:
+        return self
+
+    @property
     def in_list(self) -> List[Tuple]:
         """
         The vector-field in its list representation, as list of (y,x) vector tuples in a structure
         [(vector_0_y, vector_0_x), ...].
         """
         return [tuple(vector) for vector in self.slim]
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/vectors/uniform.py` & `autoarray-2024.5.16.0/autoarray/structures/vectors/uniform.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 from autoarray import type as ty
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class VectorYX2D(AbstractVectorYX2D):
-    def __new__(
-        cls,
+    def __init__(
+        self,
         values: Union[np.ndarray, List[Tuple[float, float]]],
         grid: Union[Grid2D, List],
         mask: Mask2D,
         store_native: bool = False,
     ):
         """
         A collection of (y,x) vectors which are located on a regular 2D grid of (y,x) coordinates.
 
-        The vectors are paired to a uniform 2D mask of pixels and sub-pixels. Each vector corresponds to a value at
-        the centre of a sub-pixel in an unmasked pixel.
+        The vectors are paired to a uniform 2D mask of pixels. Each vector corresponds to a value at
+        the centre of a pixel in an unmasked pixel.
 
         The `VectorYX2D` is ordered such that pixels begin from the top-row of the corresponding mask and go right
         and down. The positive y-axis is upwards and positive x-axis to the right.
 
         The (y,x) vectors are stored as a NumPy array which has the `slim` and `native shapes described below.
         Irrespective of this shape, the last dimension of the data structure storing the vectors is always shape 2,
         corresponding to the y and x vectors. [total_vectors, 2].
@@ -46,15 +46,15 @@
         [[vector_0_y, vector_0_x], [vector_1_y, vector_1_x]]
         [(vector_0_y, vector_0_x), (vector_1_y, vector_1_x)]
 
         If your vector field lies on a 2D irregular grid of data the `VectorFieldIrregular2D` data structure should be
         used.
 
 
-        **Case 1 (sub-size=1, slim)**
+        __slim__
 
         The Vector2D is an ndarray of shape [total_unmasked_pixels, 2].
 
         The first element of the ndarray corresponds to the pixel index, for example:
 
         - vector[3, 0:2] = the 4th unmasked pixel's y and x values.
         - vector[6, 0:2] = the 7th unmasked pixel's y and x values.
@@ -88,82 +88,15 @@
          x x x 6 7 8 9 x x x -ve  vector[5, :] = 5
          x x x x x x x x x x  I   vector[6, :] = 6
          x x x x x x x x x x  I   vector[7, :] = 7
          x x x x x x x x x x \/   vector[8, :] = 8
          x x x x x x x x x x      vector[9, :] = 9
 
 
-        **Case 2 (sub-size>1, slim)**
-
-        If the masks's sub size is > 1, the vector is defined as a sub-vector where each entry corresponds to the
-        values at the centre of each sub-pixel of an unmasked pixel.
-
-        The sub-vector indexes are ordered such that pixels begin from the first (top-left) sub-pixel in the first
-        unmasked pixel. Indexes then go over the sub-pixels in each unmasked pixel, for every unmasked pixel.
-        Therefore, the sub-vector is an ndarray of shape [total_unmasked_pixels*(sub_array_shape)**2, 2]. For example:
-
-        - vector[9, 0:2] - using a 2x2 sub-vector, gives the 3rd unmasked pixel's 2nd sub-pixel y and x values.
-        - vector[9, 0:2] - using a 3x3 sub-vector, gives the 2nd unmasked pixel's 1st sub-pixel y and x values.
-        - vector[27, 0:2] - using a 3x3 sub-vector, gives the 4th unmasked pixel's 1st sub-pixel y and x values.
-
-        Below is a visual illustration of a sub vector. Indexing of each sub-pixel goes from the top-left corner. In
-        contrast to the vector above, our illustration below restricts the mask to just 2 pixels, to keep the
-        illustration brief.
-
-         x x x x x x x x x x
-         x x x x x x x x x x     This is an example `Mask2D`, where:
-         x x x x x x x x x x
-         x x x x x x x x x x     x = `True` (Pixel is masked and excluded from lens)
-         x x x x O O x x x x     O = `False` (Pixel is not masked and included in lens)
-         x x x x x x x x x x
-         x x x x x x x x x x
-         x x x x x x x x x x
-         x x x x x x x x x x
-         x x x x x x x x x x
-
-        Our vector with a sub-size looks like it did before:
-
-        <--- -ve  x  +ve -->
-
-         x x x x x x x x x x  ^
-         x x x x x x x x x x  I
-         x x x x x x x x x x  I
-         x x x x x x x x x x +ve
-         x x x 0 1 x x x x x  y
-         x x x x x x x x x x -ve
-         x x x x x x x x x x  I
-         x x x x x x x x x x  I
-         x x x x x x x x x x \/
-         x x x x x x x x x x
-
-        However, if the sub-size is 2,each unmasked pixel has a set of sub-pixels with values. For example, for pixel 0,
-        if `sub_size=2`, it has 4 values on a 2x2 sub-vector:
-
-        Pixel 0 - (2x2):
-
-               vector[0, 0:2] = y and x values of first sub-pixel in pixel 0.
-        I0I1I  vector[1, 0:2] = y and x values of first sub-pixel in pixel 1.
-        I2I3I  vector[2, 0:2] = y and x values of first sub-pixel in pixel 2.
-               vector[3, 0:2] = y and x values of first sub-pixel in pixel 3.
-
-        If we used a sub_size of 3, for the first pixel we we would create a 3x3 sub-vector:
-
-
-                 vector[0] = y and x values of first sub-pixel in pixel 0.
-                 vector[1] = y and x values of first sub-pixel in pixel 1.
-                 vector[2] = y and x values of first sub-pixel in pixel 2.
-        I0I1I2I  vector[3] = y and x values of first sub-pixel in pixel 3.
-        I3I4I5I  vector[4] = y and x values of first sub-pixel in pixel 4.
-        I6I7I8I  vector[5] = y and x values of first sub-pixel in pixel 5.
-                 vector[6] = y and x values of first sub-pixel in pixel 6.
-                 vector[7] = y and x values of first sub-pixel in pixel 7.
-                 vector[8] = y and x values of first sub-pixel in pixel 8.
-
-
-        **Case 3 (sub_size=1, native)**
+        __native__
 
         The Vector2D has the same properties as Case 1, but is stored as an an ndarray of shape
         [total_y_values, total_x_values, 2].
 
         All masked entries on the vector have values of 0.0.
 
         For the following example mask:
@@ -184,70 +117,57 @@
             - vector[0,0, 0:2] = [0.0, 0.0] (it is masked, thus zero)
             - vector[0,0, 0:2] = [0.0, 0.0] (it is masked, thus zero)
             - vector[3,3, 0:2] = [0.0, 0.0] (it is masked, thus zero)
             - vector[3,3, 0:2] = [0.0, 0.0] (it is masked, thus zero)
             - vector[3,4, 0:2] = [0, 0]
             - vector[3,4, 0:2] = [-1, -1]
 
-
-        **Case 4: (sub_size>, native)**
-
-        The properties of this vector can be derived by combining Case's 2 and 3 above, whereby the vector is stored as
-        an ndarray of shape [total_y_values*sub_size, total_x_values*sub_size, 2].
-
-        All sub-pixels in masked pixels have values 0.0.
-
         Parameters
         ----------
         values
             The 2D (y,x) vectors on a regular grid that represent the vector-field.
         grid
             The regular grid of (y,x) coordinates where each vector is located.
         mask
             The 2D mask associated with the array, defining the pixels each array value is paired with and
             originates from.
         store_native
             If True, the ndarray is stored in its native format [total_y_pixels, total_x_pixels, 2]. This avoids
             mapping large data arrays to and from the slim / native formats, which can be a computational bottleneck.
         """
 
-        if len(values) == 0:
-            return []
-
         if type(values) is list:
             values = np.asarray(values)
 
         values = grid_2d_util.convert_grid_2d(
             grid_2d=values, mask_2d=mask, store_native=store_native
         )
 
         grid = grid_2d_util.convert_grid_2d(
             grid_2d=grid, mask_2d=mask, store_native=store_native
         )
 
-        obj = values.view(cls)
-        obj.grid = Grid2D(values=grid, mask=mask)
-        obj.mask = mask
+        self.grid = Grid2D(values=grid, mask=mask)
+        self.mask = mask
 
-        return obj
+        super().__init__(values)
 
     def __array_finalize__(self, obj):
         if hasattr(obj, "mask"):
             self.mask = obj.mask
 
         if hasattr(obj, "grid"):
             self.grid = obj.grid
 
     @classmethod
     def no_mask(
         cls,
         values: Union[np.ndarray, List[List], List[Tuple]],
         pixel_scales: ty.PixelScales,
         shape_native: Optional[Tuple[int, int]] = None,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
     ) -> "VectorYX2D":
         """
         Create a VectorYX2D (see *VectorYX2D.__new__*) by inputting the vector in 1D, for example:
 
         vectors=np.array([[1.0, 1.0], [2.0, 2.0], [3.0, 3.0], [4.0, 4.0]])
         vectors=[[1.0, 1.0], [2.0, 2.0], [3.0, 3.0], [4.0, 4.0]]
@@ -260,22 +180,20 @@
 
         The 2D shape of the grid and its mask are determined from the input grid and the mask is setup as an
         unmasked `Mask2D` of shape_native.
 
         Parameters
         ----------
         values
-            The (y,x) vectors input as an ndarray of shape [total_unmasked_pixells*(sub_size**2), 2] or a list of lists.
+            The (y,x) vectors input as an ndarray of shape [total_unmasked_pixels, 2] or a list of lists.
         shape_native
             The 2D shape of the mask the grid is paired with.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
         origin
             The origin of the grid's mask.
         """
 
         pixel_scales = geometry_util.convert_pixel_scales_2d(pixel_scales=pixel_scales)
 
         values = grid_2d_util.convert_grid(grid=values)
@@ -299,29 +217,27 @@
                     """
                     The input shape_native parameter is not a tuple of type (int, int).
                     """
                 )
 
         else:
             shape_native = (
-                int(values.shape[0] / sub_size),
-                int(values.shape[1] / sub_size),
+                int(values.shape[0]),
+                int(values.shape[1]),
             )
 
         grid = Grid2D.uniform(
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
         mask = Mask2D.all_false(
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
         return cls(values=values, grid=grid, mask=mask)
 
     @classmethod
     def from_mask(cls, values: Union[np.ndarray, List], mask: Mask2D) -> "VectorYX2D":
@@ -331,31 +247,30 @@
 
         mask = Mask2D([[True, False, False, False])
         array=np.array([1.0, 2.0, 3.0])
 
         Parameters
         ----------
         values
-            The values of the array input as an ndarray of shape [total_unmasked_pixels*(sub_size**2)] or a list of
+            The values of the array input as an ndarray of shape [total_unmasked_pixels] or a list of
             lists.
         mask
-            The mask whose masked pixels are used to setup the sub-pixel grid.
+            The mask whose masked pixels are used to setup the pixel grid.
         """
 
         grid = Grid2D.from_mask(mask=mask)
 
         return VectorYX2D(values=values, grid=grid, mask=mask)
 
     @classmethod
     def full(
         cls,
         fill_value: float,
         shape_native: Tuple[int, int],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
     ) -> "VectorYX2D":
         """
         Create a `VectorYX2D` (see `AbstractVectorYX2D.__new__`) where all values are filled with an input fill value,
         analogous to the method np.full().
 
         From 1D input the method cannot determine the 2D shape of the array and its mask, thus the shape_native must be
@@ -364,39 +279,33 @@
         Parameters
         ----------
         fill_value
             The value all array elements are filled with.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
         origin
             The origin of the grid's mask.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         """
-        if sub_size is not None:
-            shape_native = (shape_native[0] * sub_size, shape_native[1] * sub_size)
 
         return cls.no_mask(
             values=np.full(
                 fill_value=fill_value, shape=(shape_native[0], shape_native[1], 2)
             ),
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
     @classmethod
     def ones(
         cls,
         shape_native: Tuple[int, int],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
     ) -> "VectorYX2D":
         """
         Create a `VectorYX2D` (see `AbstractVectorYX2D.__new__`) where all values are filled with 1.0, analogous to
         the method np.ones().
 
         From 1D input the method cannot determine the 2D shape of the array and its mask, thus the shape_native must be
@@ -405,33 +314,29 @@
         Parameters
         ----------
         fill_value
             The value all array elements are filled with.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         """
         return cls.full(
             fill_value=1.0,
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
     @classmethod
     def zeros(
         cls,
         shape_native: Tuple[int, int],
         pixel_scales: ty.PixelScales,
-        sub_size: int = 1,
         origin: Tuple[float, float] = (0.0, 0.0),
     ) -> "VectorYX2D":
         """
         Create a `VectorYX2D` (see `AbstractVectorYX2D.__new__`) where all values are filled with 1.0, analogous to
         the method np.zeros().
 
         From 1D input the method cannot determine the 2D shape of the array and its mask, thus the shape_native must be
@@ -440,84 +345,51 @@
         Parameters
         ----------
         fill_value
             The value all array elements are filled with.
         pixel_scales
             The (y,x) arcsecond-to-pixel units conversion factor of every pixel. If this is input as a `float`,
             it is converted to a (float, float).
-        sub_size
-            The size (sub_size x sub_size) of each unmasked pixels sub-grid.
         origin
             The (y,x) scaled units origin of the mask's coordinate system.
         """
         return cls.full(
             fill_value=0.0,
             shape_native=shape_native,
             pixel_scales=pixel_scales,
-            sub_size=sub_size,
             origin=origin,
         )
 
     @property
     def slim(self) -> "VectorYX2D":
         """
         Return a `VectorYX2D` where the data is stored its `slim` representation, which is an ndarray of shape
-        [total_unmasked_pixels * sub_size**2, 2].
+        [total_unmasked_pixels, 2].
 
         If it is already stored in its `slim` representation it is returned as it is. If not, it is  mapped from
         `native` to `slim` and returned as a new `Array2D`.
         """
         return VectorYX2D(values=self, grid=self.grid.slim, mask=self.mask)
 
     @property
     def native(self) -> "VectorYX2D":
         """
         Return a `VectorYX2D` where the data is stored in its `native` representation, which is an ndarray of shape
-        [sub_size*total_y_pixels, sub_size*total_x_pixels, 2].
+        [total_y_pixels, total_x_pixels, 2].
 
         If it is already stored in its `native` representation it is return as it is. If not, it is mapped from
         `slim` to `native` and returned as a new `Grid2D`.
         """
         return VectorYX2D(
             values=self,
             grid=self.grid.native,
             mask=self.mask,
             store_native=True,
         )
 
-    @property
-    def binned(self) -> "VectorYX2D":
-        """
-        Convenience method to access the binned-up vectors as a Vector2D stored in its `slim` or `native` format.
-
-        The binning up process converts a grid from (y,x) values where each value is a coordinate on the sub-grid to
-        (y,x) values where each coordinate is at the centre of its mask (e.g. a grid with a sub_size of 1). This is
-        performed by taking the mean of all (y,x) values in each sub pixel.
-
-        If the grid is stored in 1D it is return as is. If it is stored in 2D, it must first be mapped from 2D to 1D.
-        """
-
-        vector_2d_slim_binned_y = np.multiply(
-            self.mask.sub_fraction,
-            self.slim[:, 0].reshape(-1, self.mask.sub_length).sum(axis=1),
-        )
-
-        vector_2d_slim_binned_x = np.multiply(
-            self.mask.sub_fraction,
-            self.slim[:, 1].reshape(-1, self.mask.sub_length).sum(axis=1),
-        )
-
-        return VectorYX2D(
-            values=np.stack(
-                (vector_2d_slim_binned_y, vector_2d_slim_binned_x), axis=-1
-            ),
-            grid=self.grid.binned,
-            mask=self.mask.derive_mask.sub_1,
-        )
-
     def apply_mask(self, mask: Mask2D) -> "VectorYX2D":
         return VectorYX2D.from_mask(values=self.native, mask=mask)
 
     @property
     def magnitudes(self) -> Array2D:
         """
         Returns the magnitude of every vector which are computed as sqrt(y**2 + x**2).
```

### Comparing `autoarray-2024.1.27.4/autoarray/structures/visibilities.py` & `autoarray-2024.5.16.0/autoarray/structures/visibilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from abc import ABC
+
 from astropy.io import fits
+
 import logging
 import numpy as np
 from pathlib import Path
 from typing import List, Tuple, Union
 
 from autoconf import cached_property
 
@@ -11,17 +14,17 @@
 
 from autoarray.structures.arrays import array_2d_util
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
-class AbstractVisibilities(Structure):
+class AbstractVisibilities(Structure, ABC):
     # noinspection PyUnusedLocal
-    def __new__(cls, visibilities: Union[np.ndarray, List[complex]], *args, **kwargs):
+    def __init__(self, visibilities: Union[np.ndarray, List[complex]]):
         """
         A collection of (real, imag) visibilities which are used to represent the data in an `Interferometer` dataset.
 
         The (real, imag) visibilities are stored as a 1D complex NumPy array of shape [total_visibilities]. These can
         be mapped to a 2D real NumPy array of shape [total_visibilities, 2] and a `Grid2DIrregular` data structure
         which is used for plotting the visibilities in 2D in the complex plane.
 
@@ -46,31 +49,33 @@
             if visibilities.shape[1] == 2:
                 visibilities = (
                     np.apply_along_axis(lambda args: [complex(*args)], 1, visibilities)
                     .astype("complex128")
                     .ravel()
                 )
 
-        obj = visibilities.view(cls)
-
-        obj.ordered_1d = np.concatenate(
+        self.ordered_1d = np.concatenate(
             (np.real(visibilities), np.imag(visibilities)), axis=0
         )
 
-        return obj
+        super().__init__(array=visibilities)
 
     def __array_finalize__(self, obj):
         if hasattr(obj, "ordered_1d"):
             self.ordered_1d = obj.ordered_1d
 
     @property
     def slim(self) -> "AbstractVisibilities":
         return self
 
     @property
+    def native(self) -> Structure:
+        return self
+
+    @property
     def in_array(self) -> np.ndarray:
         """
         Returns the 1D complex NumPy array of values with shape [total_visibilities] as a NumPy float array of
         shape [total_visibilities, 2].
         """
         return np.stack((np.real(self), np.imag(self)), axis=-1)
 
@@ -222,15 +227,15 @@
             file_path=file_path, hdu=hdu
         )
         return cls(visibilities=visibilities_1d)
 
 
 class VisibilitiesNoiseMap(Visibilities):
     # noinspection PyUnusedLocal
-    def __new__(cls, visibilities: Union[np.ndarray, List[complex]], *args, **kwargs):
+    def __init__(self, visibilities: Union[np.ndarray, List[complex]], *args, **kwargs):
         """
         A collection of (real, imag) visibilities noise-map values which are used to represent the noise-map in
         an `Interferometer` dataset.
 
         This data structure behaves the same as the `Visibilities` structure (see `AbstractVisibilities.__new__`). The
         only difference is that it includes a `WeightOperator` used by `Inversion`'s which use `LinearOperators` and
         the library `PyLops` to fit `Interferometer` data.
@@ -248,29 +253,24 @@
             if visibilities.shape[1] == 2:
                 visibilities = (
                     np.apply_along_axis(lambda args: [complex(*args)], 1, visibilities)
                     .astype("complex128")
                     .ravel()
                 )
 
-        obj = super(VisibilitiesNoiseMap, cls).__new__(
-            cls=cls, visibilities=visibilities
-        )
-
-        obj.ordered_1d = np.concatenate(
+        self.ordered_1d = np.concatenate(
             (np.real(visibilities), np.imag(visibilities)), axis=0
         )
+        super().__init__(visibilities=visibilities)
 
-        weight_list = 1.0 / obj.in_array**2.0
+        weight_list = 1.0 / self.in_array**2.0
 
-        obj.weight_list_ordered_1d = np.concatenate(
+        self.weight_list_ordered_1d = np.concatenate(
             (weight_list[:, 0], weight_list[:, 1]), axis=0
         )
 
-        return obj
-
     def __array_finalize__(self, obj):
         if hasattr(obj, "ordered_1d"):
             self.ordered_1d = obj.ordered_1d
 
         if hasattr(obj, "weight_list_ordered_1d"):
             self.weight_list_ordered_1d = obj.weight_list_ordered_1d
```

### Comparing `autoarray-2024.1.27.4/autoarray/type.py` & `autoarray-2024.5.16.0/autoarray/type.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 from autoarray.structures.arrays.uniform_2d import Array2D
 
 Array1D2DLike = Union[Array1D, Array2D]
 
 
 from autoarray.structures.grids.uniform_1d import Grid1D
 from autoarray.structures.grids.uniform_2d import Grid2D
-from autoarray.structures.grids.iterate_2d import Grid2DIterate
 from autoarray.structures.grids.irregular_2d import Grid2DIrregular
 
-Grid1D2DLike = Union[np.ndarray, Grid1D, Grid2D, Grid2DIterate, Grid2DIrregular]
-Grid2DLike = Union[np.ndarray, Grid2D, Grid2DIterate, Grid2DIrregular]
+Grid1D2DLike = Union[np.ndarray, Grid1D, Grid2D, Grid2DIrregular]
+Grid2DLike = Union[np.ndarray, Grid2D, Grid2DIrregular]
 
 from autoarray.structures.arrays.irregular import ArrayIrregular
 from autoarray.structures.visibilities import Visibilities
 from autoarray.structures.visibilities import VisibilitiesNoiseMap
 
-DataLike = Union[Array1D, Array2D, ArrayIrregular, Visibilities]
-NoiseMapLike = Union[Array1D, Array2D, ArrayIrregular, VisibilitiesNoiseMap]
+DataLike = Union[
+    np.ndarray, Array1D, Array2D, ArrayIrregular, Visibilities, VisibilitiesNoiseMap
+]
 
 from autoarray.operators.transformer import TransformerDFT
 from autoarray.operators.transformer import TransformerNUFFT
 
 Transformer = Union[TransformerDFT, TransformerNUFFT]
```

### Comparing `autoarray-2024.1.27.4/autoarray/util/__init__.py` & `autoarray-2024.5.16.0/autoarray/util/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from autoarray import numba_util as numba
 from autoarray.geometry import geometry_util as geometry
 from autoarray.mask import mask_1d_util as mask_1d
 from autoarray.mask import mask_2d_util as mask_2d
+from autoarray.operators.over_sampling import over_sample_util as over_sample
 from autoarray.structures.arrays import array_1d_util as array_1d
 from autoarray.structures.arrays import array_2d_util as array_2d
 from autoarray.structures.grids import grid_1d_util as grid_1d
 from autoarray.structures.grids import grid_2d_util as grid_2d
 from autoarray.structures.grids import sparse_2d_util as sparse
 from autoarray.layout import layout_util as layout
 from autoarray.fit import fit_util as fit
```

### Comparing `autoarray-2024.1.27.4/autoarray/util/cholesky_funcs.py` & `autoarray-2024.5.16.0/autoarray/util/cholesky_funcs.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/util/fnnls.py` & `autoarray-2024.5.16.0/autoarray/util/fnnls.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/autoarray/util/misc_util.py` & `autoarray-2024.5.16.0/autoarray/util/misc_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2024.1.27.4/setup.py` & `autoarray-2024.5.16.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "1.0.dev0")
+version = environ.get("VERSION", "2024.5.16.0")
 requirements.extend([f"autoconf=={version}"])
 
 
 def config_packages(directory):
     paths = [directory.replace("/", ".")]
     for path, directories, filenames in os.walk(directory):
         for directory in directories:
```

