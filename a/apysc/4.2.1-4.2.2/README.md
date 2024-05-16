# Comparing `tmp/apysc-4.2.1.tar.gz` & `tmp/apysc-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apysc-4.2.1.tar", last modified: Tue May 14 14:18:56 2024, max compression
+gzip compressed data, was "apysc-4.2.2.tar", last modified: Wed May 15 14:36:50 2024, max compression
```

## Comparing `apysc-4.2.1.tar` & `apysc-4.2.2.tar`

### file list

```diff
@@ -1,762 +1,763 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.118780 apysc-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 14:18:39.000000 apysc-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 14:18:39.000000 apysc-4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 14:18:56.118780 apysc-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-14 14:18:39.000000 apysc-4.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.022779 apysc-4.2.1/apysc/
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.026779 apysc-4.2.1/apysc/_animation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_cx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_cy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_finish_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_height_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_height_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_parallel_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_pause_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_play_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_reset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_reverse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_scale_x_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_scale_x_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_scale_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_scale_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_time_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_width.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_width_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_width_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/animation_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_animation/easing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.026779 apysc-4.2.1/apysc/_auto_reloading/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_auto_reloading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_auto_reloading/auto_reloading_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.030779 apysc-4.2.1/apysc/_branch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_branch/_elif.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_branch/_else.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_branch/_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_branch/if_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.030779 apysc-4.2.1/apysc/_callable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_callable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_callable/callable_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.034779 apysc-4.2.1/apysc/_chart/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/add_background_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/add_border_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/axis_label_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/axis_label_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/axis_label_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/axis_label_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/axis_label_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/axis_label_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/axis_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/axis_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/axis_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/background_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/border_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/chart_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/chart_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    22705 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/create_single_column_y_axis_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/initialize_each_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/is_display_axis_label_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/overall_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_background_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_background_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_border_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_border_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_border_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_horizontal_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_matrix_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_vertical_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/set_initial_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/tick_max_num_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/tick_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/tick_text_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/tick_text_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/tick_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/tick_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/tick_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/vertical_bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/x_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/x_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/x_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/x_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/x_axis_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/y_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/y_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/y_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/y_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/y_axis_single_column_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/y_max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_chart/y_min_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.038779 apysc-4.2.1/apysc/_color/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/blue_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/color_copy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/colorless.py
--rw-r--r--   0 runner    (1001) docker     (127)    84071 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/copy_color_if_default_value_specified_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/from_rgb_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/get_colors_members_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/green_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_color/red_color_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.038779 apysc-4.2.1/apysc/_console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_console/_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    32116 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_console/assertion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_console/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.038779 apysc-4.2.1/apysc/_converter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_converter/cast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_converter/to_apysc_val_from_builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_converter/to_builtin_val_from_apysc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.054779 apysc-4.2.1/apysc/_display/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/add_foreign_object_child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/add_to_parent_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/any_display_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/append_fill_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/append_fill_color_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/append_foreign_object_constructor_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/append_line_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/append_line_cap_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/append_line_color_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/append_line_joints_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/append_line_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/append_line_thickness_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/append_x_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/append_y_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/begin_fill_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17462 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/css_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/css_text_align.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/css_text_align_last.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/display_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/ellipse_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/ellipse_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/flip_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/flip_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/flip_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/get_bounds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    49066 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/graphics_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/graphics_clear_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/graphics_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_cap_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_caps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_dash_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_dash_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_joints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_joints_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_round_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    26709 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_style_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/multi_line_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/opacity_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/parent_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    18730 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/points_2d_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/points_var_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/polygon_append_constructor_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/polygon_apply_current_points_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/polygon_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/polygon_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/polygon_x3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/polygon_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/polygon_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/polygon_y3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/polyline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/rotation_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/scale_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/set_lower_scale_limit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/set_overflow_visible_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/skew_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/skew_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/sprite.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_foreign_object_child.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_foreign_object_child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_foreign_object_initialize_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_foreign_object_text_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    23418 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_set_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_set_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_set_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_set_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_set_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_set_font_size_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_set_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_set_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_set_text_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_singleton_for_text_span.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/svg_text_text_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/text_align_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/text_align_last_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/text_bold_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/text_decoration_underline_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/text_fill_color_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/text_font_size_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/text_italic_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/text_line_height_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/visible_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/width_and_height_mixin_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/x_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/y_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_display/y_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.058779 apysc-4.2.1/apysc/_event/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/custom_event_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/custom_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/document_mouse_wheel_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/double_click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/enter_frame_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/enter_frame_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/handler_circular_calling_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/mouse_down_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/mouse_event_binding_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/mouse_event_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/mouse_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/mouse_event_unbinding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/mouse_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/mouse_out_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/mouse_over_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/mouse_up_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/prevent_default_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/set_handler_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/stop_propagation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_event/wheel_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.058779 apysc-4.2.1/apysc/_expression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_expression/event_handler_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_expression/expression_data_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_expression/expression_variables_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_expression/get_last_scope_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_expression/indent_num.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_expression/js_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_expression/last_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    12476 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_expression/var_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.062779 apysc-4.2.1/apysc/_file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_file/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_file/module_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.066779 apysc-4.2.1/apysc/_geom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_close.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_control_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_control_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_control_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_control_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_control_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_control_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_data_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_data_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_dest_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_dest_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/path_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/point2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/rectangle_geom_bottom_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/rectangle_geom_center_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/rectangle_geom_center_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/rectangle_geom_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/rectangle_geom_left_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/rectangle_geom_right_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/rectangle_geom_top_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/rectangle_geom_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_geom/relative_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.066779 apysc-4.2.1/apysc/_html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_html/debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_html/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_html/html_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_html/html_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.066779 apysc-4.2.1/apysc/_jslib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_jslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70264 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_jslib/jquery-3.7.1.slim.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_jslib/jslib_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    78572 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_jslib/svg-3.1.2.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_jslib/underscore-1.12.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.066779 apysc-4.2.1/apysc/_jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_jupyter/jupyter_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.070779 apysc-4.2.1/apysc/_lint_and_doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17625 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/conf_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/docs_keyword_link_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/docs_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/docs_toctree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17282 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/docs_translation_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/docstring_to_markdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    51969 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/docstring_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/document_text_split_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/document_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.070779 apysc-4.2.1/apysc/_lint_and_doc/fixed_translation_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)   245896 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/lint_and_doc_hash_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_lint_and_doc/translation_mapping_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.070779 apysc-4.2.1/apysc/_loop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/_continue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/for_array_indices_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/for_array_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/for_dict_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/for_dict_keys_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/for_dict_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/for_loop_exit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/initialize_with_base_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_loop/loop_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.070779 apysc-4.2.1/apysc/_material_design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_material_design/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.070779 apysc-4.2.1/apysc/_material_design/icon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_material_design/icon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.070779 apysc-4.2.1/apysc/_math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_math/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_math/max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_math/min_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_math/trunc_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.070779 apysc-4.2.1/apysc/_string/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_string/indent_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_string/string_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.074779 apysc-4.2.1/apysc/_testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_testing/e2e_testing_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_testing/testing_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.074779 apysc-4.2.1/apysc/_time/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/datetime_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/day_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/days_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/fps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/hour_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/left_and_right_datetimes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/millisecond_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/minute_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/month_end_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/month_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/now_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/second_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/timedelta_.py
--rw-r--r--   0 runner    (1001) docker     (127)    22600 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/total_seconds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/weekday_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_time/year_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.074779 apysc-4.2.1/apysc/_translation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.106780 apysc-4.2.1/apysc/_translation/jp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/about_handler_options_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/add_child_and_remove_child.py
--rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/add_debug_info_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_base_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_base_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_complete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14477 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_finish.py
--rw-r--r--   0 runner    (1001) docker     (127)   146934 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    11623 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_method_chaining.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_pause_and_play.py
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_return_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    24451 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_width_and_height.py
--rw-r--r--   0 runner    (1001) docker     (127)    13114 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (127)    13134 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/append_js_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    16245 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_append_and_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_clear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_extend_and_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_index_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_insert_and_insert_at.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_last_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_pop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_remove_and_remove_at.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/array_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/assert_defined_and_undefined.py
--rw-r--r--   0 runner    (1001) docker     (127)    16840 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/assert_equal_and_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/assert_greater_and_greater_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    10860 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/assert_less_and_less_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    15946 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/assert_true_and_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/assertion_basic_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)    25610 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/bind_and_trigger_custom_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/blue_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    15004 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    49953 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)    18952 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/color_from_rgb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/colorless.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/contains.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/continue.py
--rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/datetime_day.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/datetime_hour.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/datetime_millisecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/datetime_minute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/datetime_month.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/datetime_now.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/datetime_second.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/datetime_set_month_end.py
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/datetime_year.py
--rw-r--r--   0 runner    (1001) docker     (127)    16601 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/dblclick.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/dictionary_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/dictionary_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/dictionary_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/display_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/display_object_get_and_set_css.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/display_object_mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/display_object_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/display_object_visible.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/display_object_x_and_y.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/display_on_colaboratory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/display_on_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/draw_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    85549 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/easing_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/elif.py
--rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/else.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/enter_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/for_array_indices_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/for_array_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/for_dict_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/for_dict_keys_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/for_dict_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/fps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/fundamental_data_classes_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/get_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/get_child_at.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_flip_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_line_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_scale_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    24463 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_scale_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_base_skew.py
--rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_begin_fill.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_clear.py
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_dashed_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_rect.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_round_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_round_rect.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_draw_triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)    64374 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_line_style.py
--rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/graphics_move_to_and_line_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/green_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/if.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/import_conventions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    18347 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/int_and_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/int_and_number_arithmetic_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/int_and_number_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/int_and_number_to_fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/int_and_number_to_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)    48186 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/material_design_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/math_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/math_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/math_trunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/mouse_event_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    38153 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/mouse_event_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/mousedown_and_mouseup.py
--rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/mousemove.py
--rw-r--r--   0 runner    (1001) docker     (127)    28272 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/mouseover_and_mouseout.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/multi_line_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/num_children.py
--rw-r--r--   0 runner    (1001) docker     (127)    62153 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/path_close.py
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/point2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    50966 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)    53243 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/polyline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/quick_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/range.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/recommended_type_checker_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    54921 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)    25542 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/red_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/remove_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/return.py
--rw-r--r--   0 runner    (1001) docker     (127)    17504 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/save_overall_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/sequential_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/set_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/sprite.py
--rw-r--r--   0 runner    (1001) docker     (127)    31274 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_addition_and_multiplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_lower.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_lstrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_rstrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_strip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_upper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/string_zfill.py
--rw-r--r--   0 runner    (1001) docker     (127)    49504 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    45612 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/text_align.py
--rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/text_align_last.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/text_bold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/text_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/text_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/text_font_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/text_italic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/text_line_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/text_underline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/timedelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/timedelta_days.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/timedelta_total_seconds.py
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/timer_complete.py
--rw-r--r--   0 runner    (1001) docker     (127)    17339 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/timer_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/timer_repeat_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/timer_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/timer_start_and_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/to_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    66343 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/true_and_false.py
--rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/unset_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/variable_name_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)    19570 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/what_apysc_can_do.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.114780 apysc-4.2.1/apysc/_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/_return.py
--rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/any_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    50943 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/attr_linking_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/blank_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/bool_const_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17955 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/copy_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/copy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/deleted_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    24160 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/dictionary_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/expression_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/false.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/hashable_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/initial_substitution_exp_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/initialize_locals_and_globals_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/number.py
--rw-r--r--   0 runner    (1001) docker     (127)    35138 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/number_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/py_builtin_iter_disabling_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/repr_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/revert_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    10223 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/revert_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    28760 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/string_length_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/string_lower_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/string_lstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/string_rstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/string_slice_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/string_split_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/string_strip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/string_upper_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/string_zfill_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/to_fixed_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/to_hex_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/to_number_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/to_string_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/true.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/type_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/value_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/variable_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/variable_name_suffix_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_type/variable_name_suffix_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.118780 apysc-4.2.1/apysc/_validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   119148 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/arg_validation_decos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/bool_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/color_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/display_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/event_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/geom_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/matrix_data_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/number_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/parent_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/path_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/string_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/validation_common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-14 14:18:39.000000 apysc-4.2.1/apysc/_validation/variable_name_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:18:56.022779 apysc-4.2.1/apysc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 14:18:55.000000 apysc-4.2.1/apysc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28630 2024-05-14 14:18:55.000000 apysc-4.2.1/apysc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:18:55.000000 apysc-4.2.1/apysc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 14:18:55.000000 apysc-4.2.1/apysc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 14:18:55.000000 apysc-4.2.1/apysc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:18:56.118780 apysc-4.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.453434 apysc-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 14:36:33.000000 apysc-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 14:36:33.000000 apysc-4.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-15 14:36:50.453434 apysc-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-15 14:36:33.000000 apysc-4.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.369433 apysc-4.2.2/apysc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.373433 apysc-4.2.2/apysc/_animation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_cx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_cy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_finish_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_height_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_height_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_parallel_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_pause_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_play_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_reset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_reverse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_scale_x_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_scale_x_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_scale_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_scale_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_time_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_width.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_width_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_width_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/animation_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_animation/easing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.373433 apysc-4.2.2/apysc/_auto_reloading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_auto_reloading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_auto_reloading/auto_reloading_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.373433 apysc-4.2.2/apysc/_branch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_branch/_elif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_branch/_else.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_branch/_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_branch/if_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.373433 apysc-4.2.2/apysc/_callable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_callable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_callable/callable_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.381433 apysc-4.2.2/apysc/_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/add_background_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/add_border_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/axis_label_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/axis_label_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/axis_label_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/axis_label_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/axis_label_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/axis_label_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/axis_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/axis_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/axis_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/background_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/border_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/chart_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/chart_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22705 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/create_single_column_y_axis_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/initialize_each_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/is_display_axis_label_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/overall_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_background_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_background_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_border_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_border_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_border_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_horizontal_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_matrix_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_vertical_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/set_initial_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/tick_max_num_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/tick_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/tick_text_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/tick_text_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/tick_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/tick_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/tick_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/vertical_bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/x_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/x_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/x_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/x_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/x_axis_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/y_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/y_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/y_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/y_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/y_axis_single_column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/y_max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_chart/y_min_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.381433 apysc-4.2.2/apysc/_color/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/blue_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/color_copy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/colorless.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84071 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/copy_color_if_default_value_specified_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/from_rgb_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/get_colors_members_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/green_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_color/red_color_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.381433 apysc-4.2.2/apysc/_console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_console/_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32116 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_console/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_console/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.385433 apysc-4.2.2/apysc/_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_converter/cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_converter/to_apysc_val_from_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_converter/to_builtin_val_from_apysc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.397433 apysc-4.2.2/apysc/_display/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/add_foreign_object_child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/add_to_parent_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/any_display_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/append_fill_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/append_fill_color_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/append_foreign_object_constructor_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/append_line_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/append_line_cap_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/append_line_color_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/append_line_joints_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/append_line_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/append_line_thickness_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/append_x_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/append_y_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/begin_fill_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17462 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/css_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/css_text_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/css_text_align_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/ellipse_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/ellipse_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/flip_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/flip_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/flip_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/get_bounds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49066 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/graphics_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/graphics_clear_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/graphics_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_cap_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_caps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_dash_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_dash_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_joints_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_round_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26709 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_style_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/multi_line_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/opacity_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/parent_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18730 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/points_2d_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/points_var_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/polygon_append_constructor_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/polygon_apply_current_points_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/polygon_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/polygon_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/polygon_x3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/polygon_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/polygon_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/polygon_y3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/rotation_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/scale_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/set_lower_scale_limit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/set_overflow_visible_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/skew_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/skew_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_foreign_object_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_foreign_object_child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_foreign_object_initialize_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_foreign_object_text_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23418 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_set_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_set_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_set_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_set_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_set_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_set_font_size_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_set_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_set_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_set_text_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_singleton_for_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/svg_text_text_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/text_align_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/text_align_last_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/text_bold_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/text_decoration_underline_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/text_fill_color_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/text_font_size_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/text_italic_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/text_line_height_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/visible_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/width_and_height_mixin_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/x_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/y_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_display/y_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.401434 apysc-4.2.2/apysc/_event/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/custom_event_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/custom_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/document_mouse_wheel_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/double_click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/enter_frame_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/enter_frame_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/handler_circular_calling_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/mouse_down_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/mouse_event_binding_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/mouse_event_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/mouse_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/mouse_event_unbinding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/mouse_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/mouse_out_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/mouse_over_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/mouse_up_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/prevent_default_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/set_handler_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/stop_propagation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_event/wheel_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.401434 apysc-4.2.2/apysc/_expression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_expression/event_handler_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_expression/expression_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_expression/expression_variables_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_expression/get_last_scope_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_expression/indent_num.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_expression/js_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_expression/last_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_expression/var_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.405434 apysc-4.2.2/apysc/_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_file/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_file/module_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.409433 apysc-4.2.2/apysc/_geom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_control_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_control_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_control_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_control_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_control_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_control_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_dest_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_dest_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/path_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/rectangle_geom_bottom_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/rectangle_geom_center_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/rectangle_geom_center_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/rectangle_geom_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/rectangle_geom_left_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/rectangle_geom_right_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/rectangle_geom_top_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/rectangle_geom_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_geom/relative_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.409433 apysc-4.2.2/apysc/_html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_html/debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_html/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_html/html_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_html/html_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.409433 apysc-4.2.2/apysc/_jslib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_jslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70264 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_jslib/jquery-3.7.1.slim.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_jslib/jslib_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78572 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_jslib/svg-3.1.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_jslib/underscore-1.12.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.409433 apysc-4.2.2/apysc/_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_jupyter/jupyter_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.409433 apysc-4.2.2/apysc/_lint_and_doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17625 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/conf_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/docs_keyword_link_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/docs_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/docs_toctree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17282 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/docs_translation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/docstring_to_markdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51969 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/docstring_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/document_text_split_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/document_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.409433 apysc-4.2.2/apysc/_lint_and_doc/fixed_translation_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)   245896 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/lint_and_doc_hash_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_lint_and_doc/translation_mapping_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.413433 apysc-4.2.2/apysc/_loop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/for_array_indices_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/for_dict_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/for_dict_keys_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/for_dict_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/for_loop_exit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/initialize_with_base_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_loop/loop_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.413433 apysc-4.2.2/apysc/_material_design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_material_design/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.413433 apysc-4.2.2/apysc/_material_design/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_material_design/icon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.413433 apysc-4.2.2/apysc/_math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_math/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_math/max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_math/min_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_math/trunc_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.413433 apysc-4.2.2/apysc/_string/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_string/indent_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_string/string_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.413433 apysc-4.2.2/apysc/_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_testing/e2e_testing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_testing/testing_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.417434 apysc-4.2.2/apysc/_time/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/datetime_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/day_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/days_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/fps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/hour_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/left_and_right_datetimes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/millisecond_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/minute_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/month_end_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/month_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/now_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/second_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/timedelta_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22600 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/total_seconds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/weekday_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_time/year_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.417434 apysc-4.2.2/apysc/_translation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.445434 apysc-4.2.2/apysc/_translation/jp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/about_handler_options_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/add_child_and_remove_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/add_debug_info_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_base_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_base_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14477 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_finish.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146934 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11623 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_method_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_pause_and_play.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_return_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24451 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_width_and_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13114 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13134 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/append_js_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16245 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_append_and_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_extend_and_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_index_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_insert_and_insert_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_last_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_pop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_remove_and_remove_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/array_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/assert_defined_and_undefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16840 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/assert_equal_and_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/assert_greater_and_greater_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10860 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/assert_less_and_less_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15946 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/assert_true_and_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/assertion_basic_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25610 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/bind_and_trigger_custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/blue_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15004 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49953 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18952 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/color_from_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/colorless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/contains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/datetime_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/datetime_hour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/datetime_millisecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/datetime_minute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/datetime_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/datetime_now.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/datetime_second.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/datetime_set_month_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/datetime_year.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16601 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/dblclick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/dictionary_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/dictionary_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/dictionary_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/display_object_get_and_set_css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/display_object_mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/display_object_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/display_object_visible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/display_object_x_and_y.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/display_on_colaboratory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/display_on_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/draw_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85549 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/easing_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/elif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/else.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/enter_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/for_array_indices_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/for_dict_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/for_dict_keys_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/for_dict_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/fps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/fundamental_data_classes_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/get_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/get_child_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_flip_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_scale_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24463 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_scale_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_base_skew.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_begin_fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_dashed_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_round_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_round_rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_draw_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64374 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_line_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/graphics_move_to_and_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/green_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/import_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18347 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/int_and_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/int_and_number_arithmetic_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/int_and_number_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/int_and_number_to_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/int_and_number_to_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48186 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/material_design_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/math_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/math_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/math_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/mouse_event_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38153 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/mouse_event_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/mousedown_and_mouseup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/mousemove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28272 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/mouseover_and_mouseout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/multi_line_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/num_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62153 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50966 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53243 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/quick_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/recommended_type_checker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54921 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25542 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/red_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/remove_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/return.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17504 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/save_overall_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/sequential_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/set_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31274 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_addition_and_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_lower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_lstrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_rstrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_strip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_upper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/string_zfill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49504 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45612 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/text_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/text_align_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/text_bold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/text_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/text_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/text_font_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/text_italic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/text_line_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/text_underline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/timedelta_days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/timedelta_total_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/timer_complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17339 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/timer_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/timer_repeat_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/timer_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/timer_start_and_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/to_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66343 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/true_and_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/unset_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/variable_name_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19570 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/what_apysc_can_do.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.453434 apysc-4.2.2/apysc/_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/any_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50943 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/attr_linking_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/blank_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/bool_const_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17955 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/copy_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/copy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/deleted_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24160 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/dictionary_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/expression_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/false.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/hashable_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/initial_substitution_exp_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/initialize_locals_and_globals_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35138 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/number_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/py_builtin_iter_disabling_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/repr_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/revert_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10223 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/revert_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28760 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/string_length_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/string_lower_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/string_lstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/string_rstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/string_slice_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/string_split_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/string_strip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/string_upper_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/string_zfill_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/to_fixed_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/to_hex_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/to_number_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/to_string_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/type_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/value_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/variable_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/variable_name_suffix_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_type/variable_name_suffix_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.453434 apysc-4.2.2/apysc/_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119148 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/arg_validation_decos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/bool_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/color_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/display_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/event_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/geom_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/matrix_data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/number_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/parent_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/path_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/string_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/validation_common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-15 14:36:33.000000 apysc-4.2.2/apysc/_validation/variable_name_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:36:50.369433 apysc-4.2.2/apysc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-15 14:36:50.000000 apysc-4.2.2/apysc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28657 2024-05-15 14:36:50.000000 apysc-4.2.2/apysc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:36:50.000000 apysc-4.2.2/apysc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 14:36:50.000000 apysc-4.2.2/apysc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 14:36:50.000000 apysc-4.2.2/apysc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:36:50.453434 apysc-4.2.2/setup.cfg
```

### Comparing `apysc-4.2.1/LICENSE` & `apysc-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/PKG-INFO` & `apysc-4.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 4.2.1
+Version: 4.2.2
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-4.2.1/README.md` & `apysc-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/__init__.py` & `apysc-4.2.2/apysc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 from apysc._display.path import Path
 from apysc._display.svg_text import SvgText
 from apysc._display.svg_text_align_mixin import SvgTextAlign
 from apysc._display.svg_text_span import SvgTextSpan
 from apysc._display.multi_line_text import MultiLineText
 from apysc._display.css_text_align import CssTextAlign
 from apysc._display.css_text_align_last import CssTextAlignLast
+from apysc._display.svg_icon import SvgIcon
 from apysc._geom.point2d import Point2D
 from apysc._geom.path_label import PathLabel
 from apysc._geom.path_data_base import PathDataBase
 from apysc._geom.path_move_to import PathMoveTo
 from apysc._geom.path_line_to import PathLineTo
 from apysc._geom.path_horizontal import PathHorizontal
 from apysc._geom.path_vertical import PathVertical
@@ -139,8 +140,8 @@
 from apysc._color.colors import Colors
 from apysc._color.colors import MaterialDesignColors
 from apysc._color.colorless import COLORLESS
 
 True_: __True = __True()
 False_: __False = __False()
 
-__version__: str = "4.2.1"
+__version__: str = "4.2.2"
```

### Comparing `apysc-4.2.1/apysc/_animation/animation_base.py` & `apysc-4.2.2/apysc/_animation/animation_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_cx.py` & `apysc-4.2.2/apysc/_animation/animation_cx.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_cx_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_cy.py` & `apysc-4.2.2/apysc/_animation/animation_cy.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_cy_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_fill_alpha.py` & `apysc-4.2.2/apysc/_animation/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_fill_alpha_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_fill_color.py` & `apysc-4.2.2/apysc/_animation/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_fill_color_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_finish_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_finish_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_height.py` & `apysc-4.2.2/apysc/_animation/animation_height.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_height_for_ellipse.py` & `apysc-4.2.2/apysc/_animation/animation_height_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_height_for_ellipse_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_height_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_height_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_line_alpha.py` & `apysc-4.2.2/apysc/_animation/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_line_alpha_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_line_color.py` & `apysc-4.2.2/apysc/_animation/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_line_color_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_line_thickness.py` & `apysc-4.2.2/apysc/_animation/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_line_thickness_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_mixins.py` & `apysc-4.2.2/apysc/_animation/animation_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_move.py` & `apysc-4.2.2/apysc/_animation/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_move_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_parallel.py` & `apysc-4.2.2/apysc/_animation/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_parallel_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_parallel_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_pause_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_pause_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_play_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_play_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_radius.py` & `apysc-4.2.2/apysc/_animation/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_radius_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_reset_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_reset_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_reverse_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_reverse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_rotation_around_center.py` & `apysc-4.2.2/apysc/_animation/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_rotation_around_center_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_rotation_around_point.py` & `apysc-4.2.2/apysc/_animation/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_rotation_around_point_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_scale_x_from_center.py` & `apysc-4.2.2/apysc/_animation/animation_scale_x_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_scale_x_from_center_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_scale_x_from_point.py` & `apysc-4.2.2/apysc/_animation/animation_scale_x_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_scale_x_from_point_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_scale_y_from_center.py` & `apysc-4.2.2/apysc/_animation/animation_scale_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_scale_y_from_center_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_scale_y_from_point.py` & `apysc-4.2.2/apysc/_animation/animation_scale_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_scale_y_from_point_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_time_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_time_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_width.py` & `apysc-4.2.2/apysc/_animation/animation_width.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_width_for_ellipse.py` & `apysc-4.2.2/apysc/_animation/animation_width_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_width_for_ellipse_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_width_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_width_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_x.py` & `apysc-4.2.2/apysc/_animation/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_x_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_y.py` & `apysc-4.2.2/apysc/_animation/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/animation_y_mixin.py` & `apysc-4.2.2/apysc/_animation/animation_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_animation/easing.py` & `apysc-4.2.2/apysc/_animation/easing.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_auto_reloading/auto_reloading_decorator.py` & `apysc-4.2.2/apysc/_auto_reloading/auto_reloading_decorator.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_branch/_elif.py` & `apysc-4.2.2/apysc/_branch/_elif.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_branch/_else.py` & `apysc-4.2.2/apysc/_branch/_else.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_branch/_if.py` & `apysc-4.2.2/apysc/_branch/_if.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_branch/if_base.py` & `apysc-4.2.2/apysc/_branch/if_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_callable/callable_util.py` & `apysc-4.2.2/apysc/_callable/callable_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/add_background_mixin.py` & `apysc-4.2.2/apysc/_chart/add_background_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/add_border_mixin.py` & `apysc-4.2.2/apysc/_chart/add_border_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/axis_label_bold_mixin.py` & `apysc-4.2.2/apysc/_chart/axis_label_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/axis_label_fill_alpha_mixin.py` & `apysc-4.2.2/apysc/_chart/axis_label_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/axis_label_fill_color_mixin.py` & `apysc-4.2.2/apysc/_chart/axis_label_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/axis_label_font_family_mixin.py` & `apysc-4.2.2/apysc/_chart/axis_label_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/axis_label_font_size_mixin.py` & `apysc-4.2.2/apysc/_chart/axis_label_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/axis_label_italic_mixin.py` & `apysc-4.2.2/apysc/_chart/axis_label_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/axis_line_alpha_mixin.py` & `apysc-4.2.2/apysc/_chart/axis_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/axis_line_color_mixin.py` & `apysc-4.2.2/apysc/_chart/axis_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/axis_line_thickness_mixin.py` & `apysc-4.2.2/apysc/_chart/axis_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/background_container_mixin.py` & `apysc-4.2.2/apysc/_chart/background_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/border_container_mixin.py` & `apysc-4.2.2/apysc/_chart/border_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/chart_container_mixin.py` & `apysc-4.2.2/apysc/_chart/chart_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/create_single_column_y_axis_mixin.py` & `apysc-4.2.2/apysc/_chart/create_single_column_y_axis_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/initialize_each_container_mixin.py` & `apysc-4.2.2/apysc/_chart/initialize_each_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/is_display_axis_label_mixin.py` & `apysc-4.2.2/apysc/_chart/is_display_axis_label_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/overall_container_mixin.py` & `apysc-4.2.2/apysc/_chart/overall_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_background_fill_alpha_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_background_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_background_fill_color_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_background_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_border_alpha_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_border_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_border_color_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_border_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_border_thickness_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_border_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_height_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_horizontal_padding_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_horizontal_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_matrix_data_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_matrix_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_overall_container_coordinates_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_overall_container_coordinates_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_vertical_padding_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_vertical_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_width_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_x_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/set_initial_y_mixin.py` & `apysc-4.2.2/apysc/_chart/set_initial_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/tick_max_num_mixin.py` & `apysc-4.2.2/apysc/_chart/tick_max_num_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/tick_text_bold_mixin.py` & `apysc-4.2.2/apysc/_chart/tick_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/tick_text_fill_alpha_mixin.py` & `apysc-4.2.2/apysc/_chart/tick_text_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/tick_text_fill_color_mixin.py` & `apysc-4.2.2/apysc/_chart/tick_text_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/tick_text_font_family_mixin.py` & `apysc-4.2.2/apysc/_chart/tick_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/tick_text_font_size_mixin.py` & `apysc-4.2.2/apysc/_chart/tick_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/tick_text_italic_mixin.py` & `apysc-4.2.2/apysc/_chart/tick_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py` & `apysc-4.2.2/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/vertical_bar_chart.py` & `apysc-4.2.2/apysc/_chart/vertical_bar_chart.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/x_axis_column_name_mixin.py` & `apysc-4.2.2/apysc/_chart/x_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/x_axis_container_mixin.py` & `apysc-4.2.2/apysc/_chart/x_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/x_axis_label_position_mixin.py` & `apysc-4.2.2/apysc/_chart/x_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/x_axis_settings.py` & `apysc-4.2.2/apysc/_chart/x_axis_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/y_axis_column_name_mixin.py` & `apysc-4.2.2/apysc/_chart/y_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/y_axis_container_mixin.py` & `apysc-4.2.2/apysc/_chart/y_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/y_axis_label_position_mixin.py` & `apysc-4.2.2/apysc/_chart/y_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/y_axis_single_column_settings.py` & `apysc-4.2.2/apysc/_chart/y_axis_single_column_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/y_max_mixin.py` & `apysc-4.2.2/apysc/_chart/y_max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_chart/y_min_mixin.py` & `apysc-4.2.2/apysc/_chart/y_min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_color/blue_color_mixin.py` & `apysc-4.2.2/apysc/_color/blue_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_color/color.py` & `apysc-4.2.2/apysc/_color/color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_color/color_copy_mixin.py` & `apysc-4.2.2/apysc/_color/color_copy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_color/color_util.py` & `apysc-4.2.2/apysc/_color/color_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_color/colors.py` & `apysc-4.2.2/apysc/_color/colors.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_color/copy_color_if_default_value_specified_mixin.py` & `apysc-4.2.2/apysc/_color/copy_color_if_default_value_specified_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_color/from_rgb_mixin.py` & `apysc-4.2.2/apysc/_color/from_rgb_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_color/get_colors_members_mixin.py` & `apysc-4.2.2/apysc/_color/get_colors_members_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_color/green_color_mixin.py` & `apysc-4.2.2/apysc/_color/green_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_color/red_color_mixin.py` & `apysc-4.2.2/apysc/_color/red_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_console/_trace.py` & `apysc-4.2.2/apysc/_console/_trace.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_console/assertion.py` & `apysc-4.2.2/apysc/_console/assertion.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_console/loggers.py` & `apysc-4.2.2/apysc/_console/loggers.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_converter/cast.py` & `apysc-4.2.2/apysc/_converter/cast.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_converter/to_apysc_val_from_builtin.py` & `apysc-4.2.2/apysc/_converter/to_apysc_val_from_builtin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_converter/to_builtin_val_from_apysc.py` & `apysc-4.2.2/apysc/_converter/to_builtin_val_from_apysc.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/_document.py` & `apysc-4.2.2/apysc/_display/_document.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/add_foreign_object_child_mixin.py` & `apysc-4.2.2/apysc/_display/add_foreign_object_child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/add_to_parent_mixin.py` & `apysc-4.2.2/apysc/_display/add_to_parent_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/any_display_object.py` & `apysc-4.2.2/apysc/_display/any_display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/append_fill_alpha_attr_expression_mixin.py` & `apysc-4.2.2/apysc/_display/append_fill_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/append_fill_color_expression_mixin.py` & `apysc-4.2.2/apysc/_display/append_fill_color_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/append_foreign_object_constructor_expression_mixin.py` & `apysc-4.2.2/apysc/_display/append_foreign_object_constructor_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/append_line_alpha_attr_expression_mixin.py` & `apysc-4.2.2/apysc/_display/append_line_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/append_line_cap_attr_expression_mixin.py` & `apysc-4.2.2/apysc/_display/append_line_cap_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/append_line_color_attr_expression_mixin.py` & `apysc-4.2.2/apysc/_display/append_line_color_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/append_line_joints_attr_expression_mixin.py` & `apysc-4.2.2/apysc/_display/append_line_joints_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/append_line_point_mixin.py` & `apysc-4.2.2/apysc/_display/append_line_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/append_line_thickness_attr_expression_mixin.py` & `apysc-4.2.2/apysc/_display/append_line_thickness_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/append_x_attr_expression_mixin.py` & `apysc-4.2.2/apysc/_display/append_x_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/append_y_attr_expression_mixin.py` & `apysc-4.2.2/apysc/_display/append_y_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/begin_fill_mixin.py` & `apysc-4.2.2/apysc/_display/begin_fill_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/child_mixin.py` & `apysc-4.2.2/apysc/_display/child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/circle.py` & `apysc-4.2.2/apysc/_display/circle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/css_interface.py` & `apysc-4.2.2/apysc/_display/css_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/css_mixin.py` & `apysc-4.2.2/apysc/_display/css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/cx_mixin.py` & `apysc-4.2.2/apysc/_display/cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/cy_mixin.py` & `apysc-4.2.2/apysc/_display/cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/display_object.py` & `apysc-4.2.2/apysc/_display/display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/ellipse.py` & `apysc-4.2.2/apysc/_display/ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/ellipse_height_mixin.py` & `apysc-4.2.2/apysc/_display/ellipse_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/ellipse_width_mixin.py` & `apysc-4.2.2/apysc/_display/ellipse_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/fill_alpha_mixin.py` & `apysc-4.2.2/apysc/_display/fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/fill_color_mixin.py` & `apysc-4.2.2/apysc/_display/fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/flip_interface_helper.py` & `apysc-4.2.2/apysc/_display/flip_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/flip_x_mixin.py` & `apysc-4.2.2/apysc/_display/flip_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/flip_y_mixin.py` & `apysc-4.2.2/apysc/_display/flip_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/get_bounds_mixin.py` & `apysc-4.2.2/apysc/_display/get_bounds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/graphics.py` & `apysc-4.2.2/apysc/_display/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/graphics_base.py` & `apysc-4.2.2/apysc/_display/graphics_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/graphics_clear_mixin.py` & `apysc-4.2.2/apysc/_display/graphics_clear_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/graphics_expression.py` & `apysc-4.2.2/apysc/_display/graphics_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/height_mixin.py` & `apysc-4.2.2/apysc/_display/height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line.py` & `apysc-4.2.2/apysc/_display/line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_alpha_mixin.py` & `apysc-4.2.2/apysc/_display/line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_cap_mixin.py` & `apysc-4.2.2/apysc/_display/line_cap_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_caps.py` & `apysc-4.2.2/apysc/_display/line_caps.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_color_mixin.py` & `apysc-4.2.2/apysc/_display/line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_dash_dot_setting.py` & `apysc-4.2.2/apysc/_display/line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_dash_dot_setting_mixin.py` & `apysc-4.2.2/apysc/_display/line_dash_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_dash_setting.py` & `apysc-4.2.2/apysc/_display/line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_dash_setting_mixin.py` & `apysc-4.2.2/apysc/_display/line_dash_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_dot_setting.py` & `apysc-4.2.2/apysc/_display/line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_dot_setting_mixin.py` & `apysc-4.2.2/apysc/_display/line_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_joints.py` & `apysc-4.2.2/apysc/_display/line_joints.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_joints_mixin.py` & `apysc-4.2.2/apysc/_display/line_joints_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_round_dot_setting.py` & `apysc-4.2.2/apysc/_display/line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_round_dot_setting_mixin.py` & `apysc-4.2.2/apysc/_display/line_round_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_style_mixin.py` & `apysc-4.2.2/apysc/_display/line_style_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/line_thickness_mixin.py` & `apysc-4.2.2/apysc/_display/line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/multi_line_text.py` & `apysc-4.2.2/apysc/_display/multi_line_text.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/opacity_css_mixin.py` & `apysc-4.2.2/apysc/_display/opacity_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/parent_mixin.py` & `apysc-4.2.2/apysc/_display/parent_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/path.py` & `apysc-4.2.2/apysc/_display/path.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/points_2d_mixin.py` & `apysc-4.2.2/apysc/_display/points_2d_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/polygon.py` & `apysc-4.2.2/apysc/_display/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/polygon_append_constructor_expression_mixin.py` & `apysc-4.2.2/apysc/_display/polygon_append_constructor_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/polygon_apply_current_points_mixin.py` & `apysc-4.2.2/apysc/_display/polygon_apply_current_points_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/polygon_x1_mixin.py` & `apysc-4.2.2/apysc/_display/polygon_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/polygon_x2_mixin.py` & `apysc-4.2.2/apysc/_display/polygon_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/polygon_x3_mixin.py` & `apysc-4.2.2/apysc/_display/polygon_x3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/polygon_y1_mixin.py` & `apysc-4.2.2/apysc/_display/polygon_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/polygon_y2_mixin.py` & `apysc-4.2.2/apysc/_display/polygon_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/polygon_y3_mixin.py` & `apysc-4.2.2/apysc/_display/polygon_y3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/polyline.py` & `apysc-4.2.2/apysc/_display/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/radius_mixin.py` & `apysc-4.2.2/apysc/_display/radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/rectangle.py` & `apysc-4.2.2/apysc/_display/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/rotation_around_center_mixin.py` & `apysc-4.2.2/apysc/_display/rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/rotation_around_point_mixin.py` & `apysc-4.2.2/apysc/_display/rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/rotation_interface_helper.py` & `apysc-4.2.2/apysc/_display/rotation_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/scale_interface_helper.py` & `apysc-4.2.2/apysc/_display/scale_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/scale_x_from_center_mixin.py` & `apysc-4.2.2/apysc/_display/scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/scale_x_from_point_mixin.py` & `apysc-4.2.2/apysc/_display/scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/scale_y_from_center_mixin.py` & `apysc-4.2.2/apysc/_display/scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/scale_y_from_point_mixin.py` & `apysc-4.2.2/apysc/_display/scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/set_lower_scale_limit_mixin.py` & `apysc-4.2.2/apysc/_display/set_lower_scale_limit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/set_overflow_visible_setting_mixin.py` & `apysc-4.2.2/apysc/_display/set_overflow_visible_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/skew_x_mixin.py` & `apysc-4.2.2/apysc/_display/skew_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/skew_y_mixin.py` & `apysc-4.2.2/apysc/_display/skew_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/sprite.py` & `apysc-4.2.2/apysc/_display/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/stage.py` & `apysc-4.2.2/apysc/_display/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_foreign_object_child.py` & `apysc-4.2.2/apysc/_display/svg_foreign_object_child.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_foreign_object_child_mixin.py` & `apysc-4.2.2/apysc/_display/svg_foreign_object_child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_foreign_object_initialize_width_mixin.py` & `apysc-4.2.2/apysc/_display/svg_foreign_object_initialize_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_foreign_object_text_mixin.py` & `apysc-4.2.2/apysc/_display/svg_foreign_object_text_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text.py` & `apysc-4.2.2/apysc/_display/svg_text.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_align_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_bold_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_delta_x_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_delta_y_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_font_family_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_font_size_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_italic_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_leading_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_set_align_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_set_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_set_bold_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_set_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_set_delta_x_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_set_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_set_delta_y_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_set_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_set_font_family_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_set_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_set_font_size_value_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_set_font_size_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_set_italic_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_set_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_set_leading_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_set_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_set_text_value_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_set_text_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_singleton_for_text_span.py` & `apysc-4.2.2/apysc/_display/svg_text_singleton_for_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_span.py` & `apysc-4.2.2/apysc/_display/svg_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/svg_text_text_mixin.py` & `apysc-4.2.2/apysc/_display/svg_text_text_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/text_align_css_mixin.py` & `apysc-4.2.2/apysc/_display/text_align_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/text_align_last_css_mixin.py` & `apysc-4.2.2/apysc/_display/text_align_last_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/text_bold_css_mixin.py` & `apysc-4.2.2/apysc/_display/text_bold_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/text_decoration_underline_css_mixin.py` & `apysc-4.2.2/apysc/_display/text_decoration_underline_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/text_fill_color_css_mixin.py` & `apysc-4.2.2/apysc/_display/text_fill_color_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/text_font_size_css_mixin.py` & `apysc-4.2.2/apysc/_display/text_font_size_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/text_italic_css_mixin.py` & `apysc-4.2.2/apysc/_display/text_italic_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/text_line_height_css_mixin.py` & `apysc-4.2.2/apysc/_display/text_line_height_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/triangle.py` & `apysc-4.2.2/apysc/_display/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/visible_mixin.py` & `apysc-4.2.2/apysc/_display/visible_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/width_and_height_mixin_for_ellipse.py` & `apysc-4.2.2/apysc/_display/width_and_height_mixin_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/width_mixin.py` & `apysc-4.2.2/apysc/_display/width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/x_interface.py` & `apysc-4.2.2/apysc/_display/x_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/x_mixin.py` & `apysc-4.2.2/apysc/_display/x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/y_interface.py` & `apysc-4.2.2/apysc/_display/y_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_display/y_mixin.py` & `apysc-4.2.2/apysc/_display/y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/animation_event.py` & `apysc-4.2.2/apysc/_event/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/click_mixin.py` & `apysc-4.2.2/apysc/_event/click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/custom_event_mixin.py` & `apysc-4.2.2/apysc/_event/custom_event_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/document_mouse_wheel_func.py` & `apysc-4.2.2/apysc/_event/document_mouse_wheel_func.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/double_click_mixin.py` & `apysc-4.2.2/apysc/_event/double_click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/enter_frame_event.py` & `apysc-4.2.2/apysc/_event/enter_frame_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/enter_frame_mixin.py` & `apysc-4.2.2/apysc/_event/enter_frame_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/event.py` & `apysc-4.2.2/apysc/_event/event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/handler.py` & `apysc-4.2.2/apysc/_event/handler.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/handler_circular_calling_util.py` & `apysc-4.2.2/apysc/_event/handler_circular_calling_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/mouse_down_mixin.py` & `apysc-4.2.2/apysc/_event/mouse_down_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/mouse_event.py` & `apysc-4.2.2/apysc/_event/mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/mouse_event_binding_expression_mixin.py` & `apysc-4.2.2/apysc/_event/mouse_event_binding_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/mouse_event_mixins.py` & `apysc-4.2.2/apysc/_event/mouse_event_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/mouse_event_unbinding_mixin.py` & `apysc-4.2.2/apysc/_event/mouse_event_unbinding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/mouse_move_mixin.py` & `apysc-4.2.2/apysc/_event/mouse_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/mouse_out_mixin.py` & `apysc-4.2.2/apysc/_event/mouse_out_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/mouse_over_mixin.py` & `apysc-4.2.2/apysc/_event/mouse_over_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/mouse_up_mixin.py` & `apysc-4.2.2/apysc/_event/mouse_up_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/prevent_default_mixin.py` & `apysc-4.2.2/apysc/_event/prevent_default_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/set_handler_data_mixin.py` & `apysc-4.2.2/apysc/_event/set_handler_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/stop_propagation_mixin.py` & `apysc-4.2.2/apysc/_event/stop_propagation_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/timer_event.py` & `apysc-4.2.2/apysc/_event/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_event/wheel_event.py` & `apysc-4.2.2/apysc/_event/wheel_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_expression/event_handler_scope.py` & `apysc-4.2.2/apysc/_expression/event_handler_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_expression/expression_data_util.py` & `apysc-4.2.2/apysc/_expression/expression_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_expression/expression_variables_util.py` & `apysc-4.2.2/apysc/_expression/expression_variables_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_expression/indent_num.py` & `apysc-4.2.2/apysc/_expression/indent_num.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_expression/js_functions.py` & `apysc-4.2.2/apysc/_expression/js_functions.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_expression/last_scope.py` & `apysc-4.2.2/apysc/_expression/last_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_file/file_util.py` & `apysc-4.2.2/apysc/_file/file_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_file/module_util.py` & `apysc-4.2.2/apysc/_file/module_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_bezier_2d.py` & `apysc-4.2.2/apysc/_geom/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_bezier_2d_continual.py` & `apysc-4.2.2/apysc/_geom/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_bezier_3d.py` & `apysc-4.2.2/apysc/_geom/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_bezier_3d_continual.py` & `apysc-4.2.2/apysc/_geom/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_close.py` & `apysc-4.2.2/apysc/_geom/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_control_x1_mixin.py` & `apysc-4.2.2/apysc/_geom/path_control_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_control_x2_mixin.py` & `apysc-4.2.2/apysc/_geom/path_control_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_control_x_mixin.py` & `apysc-4.2.2/apysc/_geom/path_control_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_control_y1_mixin.py` & `apysc-4.2.2/apysc/_geom/path_control_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_control_y2_mixin.py` & `apysc-4.2.2/apysc/_geom/path_control_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_control_y_mixin.py` & `apysc-4.2.2/apysc/_geom/path_control_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_data.py` & `apysc-4.2.2/apysc/_geom/path_data.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_data_base.py` & `apysc-4.2.2/apysc/_geom/path_data_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_data_util.py` & `apysc-4.2.2/apysc/_geom/path_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_dest_x_mixin.py` & `apysc-4.2.2/apysc/_geom/path_dest_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_dest_y_mixin.py` & `apysc-4.2.2/apysc/_geom/path_dest_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_horizontal.py` & `apysc-4.2.2/apysc/_geom/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_line_to.py` & `apysc-4.2.2/apysc/_geom/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_move_to.py` & `apysc-4.2.2/apysc/_geom/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_vertical.py` & `apysc-4.2.2/apysc/_geom/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_x_mixin.py` & `apysc-4.2.2/apysc/_geom/path_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/path_y_mixin.py` & `apysc-4.2.2/apysc/_geom/path_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/point2d.py` & `apysc-4.2.2/apysc/_geom/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/rectangle_geom.py` & `apysc-4.2.2/apysc/_geom/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/rectangle_geom_bottom_y_mixin.py` & `apysc-4.2.2/apysc/_geom/rectangle_geom_bottom_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/rectangle_geom_center_x_mixin.py` & `apysc-4.2.2/apysc/_geom/rectangle_geom_center_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/rectangle_geom_center_y_mixin.py` & `apysc-4.2.2/apysc/_geom/rectangle_geom_center_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/rectangle_geom_height_mixin.py` & `apysc-4.2.2/apysc/_geom/rectangle_geom_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/rectangle_geom_left_x_mixin.py` & `apysc-4.2.2/apysc/_geom/rectangle_geom_left_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/rectangle_geom_right_x_mixin.py` & `apysc-4.2.2/apysc/_geom/rectangle_geom_right_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/rectangle_geom_top_y_mixin.py` & `apysc-4.2.2/apysc/_geom/rectangle_geom_top_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/rectangle_geom_width_mixin.py` & `apysc-4.2.2/apysc/_geom/rectangle_geom_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_geom/relative_mixin.py` & `apysc-4.2.2/apysc/_geom/relative_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_html/debug_mode.py` & `apysc-4.2.2/apysc/_html/debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_html/exporter.py` & `apysc-4.2.2/apysc/_html/exporter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_html/html_util.py` & `apysc-4.2.2/apysc/_html/html_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_jslib/jquery-3.7.1.slim.min.js` & `apysc-4.2.2/apysc/_jslib/jquery-3.7.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_jslib/jquery.mousewheel-3.1.13.min.js` & `apysc-4.2.2/apysc/_jslib/jquery.mousewheel-3.1.13.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_jslib/jslib_util.py` & `apysc-4.2.2/apysc/_jslib/jslib_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_jslib/svg-3.1.2.min.js` & `apysc-4.2.2/apysc/_jslib/svg-3.1.2.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_jslib/underscore-1.12.0.min.js` & `apysc-4.2.2/apysc/_jslib/underscore-1.12.0.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_jupyter/jupyter_util.py` & `apysc-4.2.2/apysc/_jupyter/jupyter_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py` & `apysc-4.2.2/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/conf_common.py` & `apysc-4.2.2/apysc/_lint_and_doc/conf_common.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/docs_keyword_link_mapping.py` & `apysc-4.2.2/apysc/_lint_and_doc/docs_keyword_link_mapping.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/docs_lang.py` & `apysc-4.2.2/apysc/_lint_and_doc/docs_lang.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/docs_toctree_util.py` & `apysc-4.2.2/apysc/_lint_and_doc/docs_toctree_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/docs_translation_converter.py` & `apysc-4.2.2/apysc/_lint_and_doc/docs_translation_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/docstring_to_markdown_converter.py` & `apysc-4.2.2/apysc/_lint_and_doc/docstring_to_markdown_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/docstring_util.py` & `apysc-4.2.2/apysc/_lint_and_doc/docstring_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/document_text_split_util.py` & `apysc-4.2.2/apysc/_lint_and_doc/document_text_split_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/document_util.py` & `apysc-4.2.2/apysc/_lint_and_doc/document_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py` & `apysc-4.2.2/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/fixed_translation_mapping/jp.py` & `apysc-4.2.2/apysc/_lint_and_doc/fixed_translation_mapping/jp.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/lint_and_doc_hash_util.py` & `apysc-4.2.2/apysc/_lint_and_doc/lint_and_doc_hash_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_lint_and_doc/translation_mapping_utils.py` & `apysc-4.2.2/apysc/_lint_and_doc/translation_mapping_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_loop/_continue.py` & `apysc-4.2.2/apysc/_loop/_continue.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_loop/_range.py` & `apysc-4.2.2/apysc/_loop/_range.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_loop/for_array_indices.py` & `apysc-4.2.2/apysc/_loop/for_array_indices.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_loop/for_array_indices_and_values.py` & `apysc-4.2.2/apysc/_loop/for_array_indices_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_loop/for_array_values.py` & `apysc-4.2.2/apysc/_loop/for_array_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_loop/for_dict_keys.py` & `apysc-4.2.2/apysc/_loop/for_dict_keys.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_loop/for_dict_keys_and_values.py` & `apysc-4.2.2/apysc/_loop/for_dict_keys_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_loop/for_dict_values.py` & `apysc-4.2.2/apysc/_loop/for_dict_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_loop/for_loop_exit_mixin.py` & `apysc-4.2.2/apysc/_loop/for_loop_exit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_loop/loop_count.py` & `apysc-4.2.2/apysc/_loop/loop_count.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_math/max_mixin.py` & `apysc-4.2.2/apysc/_math/max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_math/min_mixin.py` & `apysc-4.2.2/apysc/_math/min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_math/trunc_mixin.py` & `apysc-4.2.2/apysc/_math/trunc_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_string/indent_util.py` & `apysc-4.2.2/apysc/_string/indent_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_string/string_util.py` & `apysc-4.2.2/apysc/_string/string_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_testing/e2e_testing_helper.py` & `apysc-4.2.2/apysc/_testing/e2e_testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_testing/testing_helper.py` & `apysc-4.2.2/apysc/_testing/testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/datetime_.py` & `apysc-4.2.2/apysc/_time/datetime_.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/day_mixin.py` & `apysc-4.2.2/apysc/_time/day_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/days_mixin.py` & `apysc-4.2.2/apysc/_time/days_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/fps.py` & `apysc-4.2.2/apysc/_time/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/hour_mixin.py` & `apysc-4.2.2/apysc/_time/hour_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/left_and_right_datetimes_mixin.py` & `apysc-4.2.2/apysc/_time/left_and_right_datetimes_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/millisecond_mixin.py` & `apysc-4.2.2/apysc/_time/millisecond_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/minute_mixin.py` & `apysc-4.2.2/apysc/_time/minute_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/month_end_mixin.py` & `apysc-4.2.2/apysc/_time/month_end_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/month_mixin.py` & `apysc-4.2.2/apysc/_time/month_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/now_mixin.py` & `apysc-4.2.2/apysc/_time/now_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/second_mixin.py` & `apysc-4.2.2/apysc/_time/second_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/timedelta_.py` & `apysc-4.2.2/apysc/_time/timedelta_.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/timer.py` & `apysc-4.2.2/apysc/_time/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/total_seconds_mixin.py` & `apysc-4.2.2/apysc/_time/total_seconds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/weekday_mixin.py` & `apysc-4.2.2/apysc/_time/weekday_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_time/year_mixin.py` & `apysc-4.2.2/apysc/_time/year_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/about_handler_options_type.py` & `apysc-4.2.2/apysc/_translation/jp/about_handler_options_type.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/add_child_and_remove_child.py` & `apysc-4.2.2/apysc/_translation/jp/add_child_and_remove_child.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/add_debug_info_setting.py` & `apysc-4.2.2/apysc/_translation/jp/add_debug_info_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_base_start.py` & `apysc-4.2.2/apysc/_translation/jp/animation_base_start.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_base_target.py` & `apysc-4.2.2/apysc/_translation/jp/animation_base_target.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_complete.py` & `apysc-4.2.2/apysc/_translation/jp/animation_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_delay.py` & `apysc-4.2.2/apysc/_translation/jp/animation_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_duration.py` & `apysc-4.2.2/apysc/_translation/jp/animation_duration.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_event.py` & `apysc-4.2.2/apysc/_translation/jp/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_fill_alpha.py` & `apysc-4.2.2/apysc/_translation/jp/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_fill_color.py` & `apysc-4.2.2/apysc/_translation/jp/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_finish.py` & `apysc-4.2.2/apysc/_translation/jp/animation_finish.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_interfaces_abstract.py` & `apysc-4.2.2/apysc/_translation/jp/animation_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_line_alpha.py` & `apysc-4.2.2/apysc/_translation/jp/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_line_color.py` & `apysc-4.2.2/apysc/_translation/jp/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_line_thickness.py` & `apysc-4.2.2/apysc/_translation/jp/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_method_chaining.py` & `apysc-4.2.2/apysc/_translation/jp/animation_method_chaining.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_move.py` & `apysc-4.2.2/apysc/_translation/jp/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_parallel.py` & `apysc-4.2.2/apysc/_translation/jp/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_pause_and_play.py` & `apysc-4.2.2/apysc/_translation/jp/animation_pause_and_play.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_radius.py` & `apysc-4.2.2/apysc/_translation/jp/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_reset.py` & `apysc-4.2.2/apysc/_translation/jp/animation_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_return_value.py` & `apysc-4.2.2/apysc/_translation/jp/animation_return_value.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_reverse.py` & `apysc-4.2.2/apysc/_translation/jp/animation_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_rotation_around_center.py` & `apysc-4.2.2/apysc/_translation/jp/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_rotation_around_point.py` & `apysc-4.2.2/apysc/_translation/jp/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_scale_x_and_y_from_center.py` & `apysc-4.2.2/apysc/_translation/jp/animation_scale_x_and_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_scale_x_and_y_from_point.py` & `apysc-4.2.2/apysc/_translation/jp/animation_scale_x_and_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_time.py` & `apysc-4.2.2/apysc/_translation/jp/animation_time.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_width_and_height.py` & `apysc-4.2.2/apysc/_translation/jp/animation_width_and_height.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_x.py` & `apysc-4.2.2/apysc/_translation/jp/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/animation_y.py` & `apysc-4.2.2/apysc/_translation/jp/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/append_js_expression.py` & `apysc-4.2.2/apysc/_translation/jp/append_js_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array.py` & `apysc-4.2.2/apysc/_translation/jp/array.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_append_and_push.py` & `apysc-4.2.2/apysc/_translation/jp/array_append_and_push.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_clear.py` & `apysc-4.2.2/apysc/_translation/jp/array_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_comparison.py` & `apysc-4.2.2/apysc/_translation/jp/array_comparison.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_extend_and_concat.py` & `apysc-4.2.2/apysc/_translation/jp/array_extend_and_concat.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_index_of.py` & `apysc-4.2.2/apysc/_translation/jp/array_index_of.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_insert_and_insert_at.py` & `apysc-4.2.2/apysc/_translation/jp/array_insert_and_insert_at.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_join.py` & `apysc-4.2.2/apysc/_translation/jp/array_join.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_last_value.py` & `apysc-4.2.2/apysc/_translation/jp/array_last_value.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_length.py` & `apysc-4.2.2/apysc/_translation/jp/array_length.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_pop.py` & `apysc-4.2.2/apysc/_translation/jp/array_pop.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_remove_and_remove_at.py` & `apysc-4.2.2/apysc/_translation/jp/array_remove_and_remove_at.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_reverse.py` & `apysc-4.2.2/apysc/_translation/jp/array_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_slice.py` & `apysc-4.2.2/apysc/_translation/jp/array_slice.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/array_sort.py` & `apysc-4.2.2/apysc/_translation/jp/array_sort.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py` & `apysc-4.2.2/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/assert_defined_and_undefined.py` & `apysc-4.2.2/apysc/_translation/jp/assert_defined_and_undefined.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py` & `apysc-4.2.2/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/assert_equal_and_not_equal.py` & `apysc-4.2.2/apysc/_translation/jp/assert_equal_and_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/assert_greater_and_greater_equal.py` & `apysc-4.2.2/apysc/_translation/jp/assert_greater_and_greater_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/assert_less_and_less_equal.py` & `apysc-4.2.2/apysc/_translation/jp/assert_less_and_less_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/assert_true_and_false.py` & `apysc-4.2.2/apysc/_translation/jp/assert_true_and_false.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/assertion_basic_behavior.py` & `apysc-4.2.2/apysc/_translation/jp/assertion_basic_behavior.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/bind_and_trigger_custom_event.py` & `apysc-4.2.2/apysc/_translation/jp/bind_and_trigger_custom_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/blue_color.py` & `apysc-4.2.2/apysc/_translation/jp/blue_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/boolean.py` & `apysc-4.2.2/apysc/_translation/jp/boolean.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py` & `apysc-4.2.2/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/circle.py` & `apysc-4.2.2/apysc/_translation/jp/circle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/click.py` & `apysc-4.2.2/apysc/_translation/jp/click.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/color.py` & `apysc-4.2.2/apysc/_translation/jp/color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/color_from_rgb.py` & `apysc-4.2.2/apysc/_translation/jp/color_from_rgb.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/colorless.py` & `apysc-4.2.2/apysc/_translation/jp/colorless.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/colors.py` & `apysc-4.2.2/apysc/_translation/jp/colors.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/contains.py` & `apysc-4.2.2/apysc/_translation/jp/contains.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/continue.py` & `apysc-4.2.2/apysc/_translation/jp/continue.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/datetime.py` & `apysc-4.2.2/apysc/_translation/jp/datetime.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/datetime_day.py` & `apysc-4.2.2/apysc/_translation/jp/datetime_day.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/datetime_hour.py` & `apysc-4.2.2/apysc/_translation/jp/datetime_hour.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/datetime_millisecond.py` & `apysc-4.2.2/apysc/_translation/jp/datetime_millisecond.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/datetime_minute.py` & `apysc-4.2.2/apysc/_translation/jp/datetime_minute.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/datetime_month.py` & `apysc-4.2.2/apysc/_translation/jp/datetime_month.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/datetime_now.py` & `apysc-4.2.2/apysc/_translation/jp/datetime_now.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/datetime_second.py` & `apysc-4.2.2/apysc/_translation/jp/datetime_second.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/datetime_set_month_end.py` & `apysc-4.2.2/apysc/_translation/jp/datetime_set_month_end.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py` & `apysc-4.2.2/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/datetime_year.py` & `apysc-4.2.2/apysc/_translation/jp/datetime_year.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/dblclick.py` & `apysc-4.2.2/apysc/_translation/jp/dblclick.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/delete.py` & `apysc-4.2.2/apysc/_translation/jp/delete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/dictionary.py` & `apysc-4.2.2/apysc/_translation/jp/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/dictionary_generic.py` & `apysc-4.2.2/apysc/_translation/jp/dictionary_generic.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/dictionary_get.py` & `apysc-4.2.2/apysc/_translation/jp/dictionary_get.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/dictionary_length.py` & `apysc-4.2.2/apysc/_translation/jp/dictionary_length.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/display_object.py` & `apysc-4.2.2/apysc/_translation/jp/display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py` & `apysc-4.2.2/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/display_object_get_and_set_css.py` & `apysc-4.2.2/apysc/_translation/jp/display_object_get_and_set_css.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/display_object_mouse_event.py` & `apysc-4.2.2/apysc/_translation/jp/display_object_mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/display_object_parent.py` & `apysc-4.2.2/apysc/_translation/jp/display_object_parent.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/display_object_visible.py` & `apysc-4.2.2/apysc/_translation/jp/display_object_visible.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/display_object_x_and_y.py` & `apysc-4.2.2/apysc/_translation/jp/display_object_x_and_y.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/display_on_colaboratory.py` & `apysc-4.2.2/apysc/_translation/jp/display_on_colaboratory.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/display_on_jupyter.py` & `apysc-4.2.2/apysc/_translation/jp/display_on_jupyter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/draw_interfaces_abstract.py` & `apysc-4.2.2/apysc/_translation/jp/draw_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/easing_enum.py` & `apysc-4.2.2/apysc/_translation/jp/easing_enum.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/elif.py` & `apysc-4.2.2/apysc/_translation/jp/elif.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/ellipse.py` & `apysc-4.2.2/apysc/_translation/jp/ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/else.py` & `apysc-4.2.2/apysc/_translation/jp/else.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/enter_frame.py` & `apysc-4.2.2/apysc/_translation/jp/enter_frame.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py` & `apysc-4.2.2/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/for_array_indices.py` & `apysc-4.2.2/apysc/_translation/jp/for_array_indices.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/for_array_indices_and_values.py` & `apysc-4.2.2/apysc/_translation/jp/for_array_indices_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/for_array_values.py` & `apysc-4.2.2/apysc/_translation/jp/for_array_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/for_dict_keys.py` & `apysc-4.2.2/apysc/_translation/jp/for_dict_keys.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/for_dict_keys_and_values.py` & `apysc-4.2.2/apysc/_translation/jp/for_dict_keys_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/for_dict_values.py` & `apysc-4.2.2/apysc/_translation/jp/for_dict_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/fps.py` & `apysc-4.2.2/apysc/_translation/jp/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/fundamental_data_classes_value_interface.py` & `apysc-4.2.2/apysc/_translation/jp/fundamental_data_classes_value_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/get_bounds.py` & `apysc-4.2.2/apysc/_translation/jp/get_bounds.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/get_child_at.py` & `apysc-4.2.2/apysc/_translation/jp/get_child_at.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics.py` & `apysc-4.2.2/apysc/_translation/jp/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_fill_alpha.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_fill_color.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_flip_interfaces.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_flip_interfaces.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_line_alpha.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_line_color.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_line_dash_setting.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_line_dot_setting.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_line_round_dot_setting.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_line_thickness.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_rotation_around_center.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_rotation_around_point.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_scale_from_center.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_scale_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_scale_from_point.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_scale_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_base_skew.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_base_skew.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_begin_fill.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_begin_fill.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_clear.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_circle.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_circle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_dash_dotted_line.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_dash_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_dashed_line.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_dashed_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_dotted_line.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_ellipse.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_line.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_path.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_path.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_polygon.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_rect.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_round_dotted_line.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_round_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_round_rect.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_round_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_draw_triangle.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_draw_triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_line_style.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_line_style.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/graphics_move_to_and_line_to.py` & `apysc-4.2.2/apysc/_translation/jp/graphics_move_to_and_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/green_color.py` & `apysc-4.2.2/apysc/_translation/jp/green_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/if.py` & `apysc-4.2.2/apysc/_translation/jp/if.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/import_conventions.py` & `apysc-4.2.2/apysc/_translation/jp/import_conventions.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/index.py` & `apysc-4.2.2/apysc/_translation/jp/index.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/int_and_number.py` & `apysc-4.2.2/apysc/_translation/jp/int_and_number.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/int_and_number_arithmetic_operations.py` & `apysc-4.2.2/apysc/_translation/jp/int_and_number_arithmetic_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/int_and_number_comparison_operations.py` & `apysc-4.2.2/apysc/_translation/jp/int_and_number_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/int_and_number_to_fixed.py` & `apysc-4.2.2/apysc/_translation/jp/int_and_number_to_fixed.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/int_and_number_to_hex.py` & `apysc-4.2.2/apysc/_translation/jp/int_and_number_to_hex.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/line.py` & `apysc-4.2.2/apysc/_translation/jp/line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/material_design_colors.py` & `apysc-4.2.2/apysc/_translation/jp/material_design_colors.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/math_max.py` & `apysc-4.2.2/apysc/_translation/jp/math_max.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/math_min.py` & `apysc-4.2.2/apysc/_translation/jp/math_min.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/math_trunc.py` & `apysc-4.2.2/apysc/_translation/jp/math_trunc.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/mouse_event_abstract.py` & `apysc-4.2.2/apysc/_translation/jp/mouse_event_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/mouse_event_basic.py` & `apysc-4.2.2/apysc/_translation/jp/mouse_event_basic.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/mousedown_and_mouseup.py` & `apysc-4.2.2/apysc/_translation/jp/mousedown_and_mouseup.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/mousemove.py` & `apysc-4.2.2/apysc/_translation/jp/mousemove.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/mouseover_and_mouseout.py` & `apysc-4.2.2/apysc/_translation/jp/mouseover_and_mouseout.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/multi_line_text.py` & `apysc-4.2.2/apysc/_translation/jp/multi_line_text.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/num_children.py` & `apysc-4.2.2/apysc/_translation/jp/num_children.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/path.py` & `apysc-4.2.2/apysc/_translation/jp/path.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/path_bezier_2d.py` & `apysc-4.2.2/apysc/_translation/jp/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/path_bezier_2d_continual.py` & `apysc-4.2.2/apysc/_translation/jp/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/path_bezier_3d.py` & `apysc-4.2.2/apysc/_translation/jp/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/path_bezier_3d_continual.py` & `apysc-4.2.2/apysc/_translation/jp/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/path_close.py` & `apysc-4.2.2/apysc/_translation/jp/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/path_horizontal.py` & `apysc-4.2.2/apysc/_translation/jp/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/path_line_to.py` & `apysc-4.2.2/apysc/_translation/jp/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/path_move_to.py` & `apysc-4.2.2/apysc/_translation/jp/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/path_vertical.py` & `apysc-4.2.2/apysc/_translation/jp/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/point2d.py` & `apysc-4.2.2/apysc/_translation/jp/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/polygon.py` & `apysc-4.2.2/apysc/_translation/jp/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/polyline.py` & `apysc-4.2.2/apysc/_translation/jp/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/quick_start.py` & `apysc-4.2.2/apysc/_translation/jp/quick_start.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/range.py` & `apysc-4.2.2/apysc/_translation/jp/range.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/recommended_type_checker_settings.py` & `apysc-4.2.2/apysc/_translation/jp/recommended_type_checker_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/rectangle.py` & `apysc-4.2.2/apysc/_translation/jp/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/rectangle_geom.py` & `apysc-4.2.2/apysc/_translation/jp/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/red_color.py` & `apysc-4.2.2/apysc/_translation/jp/red_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/remove_children.py` & `apysc-4.2.2/apysc/_translation/jp/remove_children.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/return.py` & `apysc-4.2.2/apysc/_translation/jp/return.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/save_overall_html.py` & `apysc-4.2.2/apysc/_translation/jp/save_overall_html.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/sequential_animation.py` & `apysc-4.2.2/apysc/_translation/jp/sequential_animation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/set_debug_mode.py` & `apysc-4.2.2/apysc/_translation/jp/set_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/sprite.py` & `apysc-4.2.2/apysc/_translation/jp/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/stage.py` & `apysc-4.2.2/apysc/_translation/jp/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string.py` & `apysc-4.2.2/apysc/_translation/jp/string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_addition_and_multiplication.py` & `apysc-4.2.2/apysc/_translation/jp/string_addition_and_multiplication.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py` & `apysc-4.2.2/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_comparison_operations.py` & `apysc-4.2.2/apysc/_translation/jp/string_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_length.py` & `apysc-4.2.2/apysc/_translation/jp/string_length.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_lower.py` & `apysc-4.2.2/apysc/_translation/jp/string_lower.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_lstrip.py` & `apysc-4.2.2/apysc/_translation/jp/string_lstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_rstrip.py` & `apysc-4.2.2/apysc/_translation/jp/string_rstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_slice.py` & `apysc-4.2.2/apysc/_translation/jp/string_slice.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_split.py` & `apysc-4.2.2/apysc/_translation/jp/string_split.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_strip.py` & `apysc-4.2.2/apysc/_translation/jp/string_strip.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_upper.py` & `apysc-4.2.2/apysc/_translation/jp/string_upper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/string_zfill.py` & `apysc-4.2.2/apysc/_translation/jp/string_zfill.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/svg_text.py` & `apysc-4.2.2/apysc/_translation/jp/svg_text.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/svg_text_span.py` & `apysc-4.2.2/apysc/_translation/jp/svg_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/text_align.py` & `apysc-4.2.2/apysc/_translation/jp/text_align.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/text_align_last.py` & `apysc-4.2.2/apysc/_translation/jp/text_align_last.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/text_bold.py` & `apysc-4.2.2/apysc/_translation/jp/text_bold.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/text_fill_alpha.py` & `apysc-4.2.2/apysc/_translation/jp/text_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/text_fill_color.py` & `apysc-4.2.2/apysc/_translation/jp/text_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/text_font_size.py` & `apysc-4.2.2/apysc/_translation/jp/text_font_size.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/text_italic.py` & `apysc-4.2.2/apysc/_translation/jp/text_italic.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/text_line_height.py` & `apysc-4.2.2/apysc/_translation/jp/text_line_height.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/text_underline.py` & `apysc-4.2.2/apysc/_translation/jp/text_underline.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/timedelta.py` & `apysc-4.2.2/apysc/_translation/jp/timedelta.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/timedelta_days.py` & `apysc-4.2.2/apysc/_translation/jp/timedelta_days.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/timedelta_total_seconds.py` & `apysc-4.2.2/apysc/_translation/jp/timedelta_total_seconds.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/timer.py` & `apysc-4.2.2/apysc/_translation/jp/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/timer_complete.py` & `apysc-4.2.2/apysc/_translation/jp/timer_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/timer_delay.py` & `apysc-4.2.2/apysc/_translation/jp/timer_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/timer_event.py` & `apysc-4.2.2/apysc/_translation/jp/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/timer_repeat_count.py` & `apysc-4.2.2/apysc/_translation/jp/timer_repeat_count.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/timer_reset.py` & `apysc-4.2.2/apysc/_translation/jp/timer_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/timer_start_and_stop.py` & `apysc-4.2.2/apysc/_translation/jp/timer_start_and_stop.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/to_string.py` & `apysc-4.2.2/apysc/_translation/jp/to_string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/trace.py` & `apysc-4.2.2/apysc/_translation/jp/trace.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/triangle.py` & `apysc-4.2.2/apysc/_translation/jp/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/true_and_false.py` & `apysc-4.2.2/apysc/_translation/jp/true_and_false.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py` & `apysc-4.2.2/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/unset_debug_mode.py` & `apysc-4.2.2/apysc/_translation/jp/unset_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/variable_name_suffix.py` & `apysc-4.2.2/apysc/_translation/jp/variable_name_suffix.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/what_apysc_can_do.py` & `apysc-4.2.2/apysc/_translation/jp/what_apysc_can_do.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py` & `apysc-4.2.2/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/_delete.py` & `apysc-4.2.2/apysc/_type/_delete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/_return.py` & `apysc-4.2.2/apysc/_type/_return.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/any_value.py` & `apysc-4.2.2/apysc/_type/any_value.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/array.py` & `apysc-4.2.2/apysc/_type/array.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/attr_linking_mixin.py` & `apysc-4.2.2/apysc/_type/attr_linking_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py` & `apysc-4.2.2/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/blank_object_mixin.py` & `apysc-4.2.2/apysc/_type/blank_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/bool_const_mixin.py` & `apysc-4.2.2/apysc/_type/bool_const_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/boolean.py` & `apysc-4.2.2/apysc/_type/boolean.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/copy_mixin.py` & `apysc-4.2.2/apysc/_type/copy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/deleted_object_mixin.py` & `apysc-4.2.2/apysc/_type/deleted_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/dictionary.py` & `apysc-4.2.2/apysc/_type/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/expression_string.py` & `apysc-4.2.2/apysc/_type/expression_string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/false.py` & `apysc-4.2.2/apysc/_type/false.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/initial_substitution_exp_mixin.py` & `apysc-4.2.2/apysc/_type/initial_substitution_exp_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/initialize_locals_and_globals_mixin.py` & `apysc-4.2.2/apysc/_type/initialize_locals_and_globals_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/int.py` & `apysc-4.2.2/apysc/_type/int.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/number.py` & `apysc-4.2.2/apysc/_type/number.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/number_value_mixin.py` & `apysc-4.2.2/apysc/_type/number_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/py_builtin_iter_disabling_mixin.py` & `apysc-4.2.2/apysc/_type/py_builtin_iter_disabling_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/revert_interface.py` & `apysc-4.2.2/apysc/_type/revert_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/revert_mixin.py` & `apysc-4.2.2/apysc/_type/revert_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/string.py` & `apysc-4.2.2/apysc/_type/string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py` & `apysc-4.2.2/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/string_length_mixin.py` & `apysc-4.2.2/apysc/_type/string_length_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/string_lower_mixin.py` & `apysc-4.2.2/apysc/_type/string_lower_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/string_lstrip_mixin.py` & `apysc-4.2.2/apysc/_type/string_lstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/string_rstrip_mixin.py` & `apysc-4.2.2/apysc/_type/string_rstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/string_slice_mixin.py` & `apysc-4.2.2/apysc/_type/string_slice_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/string_split_mixin.py` & `apysc-4.2.2/apysc/_type/string_split_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/string_strip_mixin.py` & `apysc-4.2.2/apysc/_type/string_strip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/string_upper_mixin.py` & `apysc-4.2.2/apysc/_type/string_upper_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/string_zfill_mixin.py` & `apysc-4.2.2/apysc/_type/string_zfill_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/to_fixed_mixin.py` & `apysc-4.2.2/apysc/_type/to_fixed_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/to_hex_mixin.py` & `apysc-4.2.2/apysc/_type/to_hex_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/to_number_mixin.py` & `apysc-4.2.2/apysc/_type/to_number_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/to_string_mixin.py` & `apysc-4.2.2/apysc/_type/to_string_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/true.py` & `apysc-4.2.2/apysc/_type/true.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/type_util.py` & `apysc-4.2.2/apysc/_type/type_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/value_util.py` & `apysc-4.2.2/apysc/_type/value_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/variable_name_mixin.py` & `apysc-4.2.2/apysc/_type/variable_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/variable_name_suffix_attr_or_var_mixin.py` & `apysc-4.2.2/apysc/_type/variable_name_suffix_attr_or_var_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/variable_name_suffix_mixin.py` & `apysc-4.2.2/apysc/_type/variable_name_suffix_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_type/variable_name_suffix_utils.py` & `apysc-4.2.2/apysc/_type/variable_name_suffix_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/arg_validation_decos.py` & `apysc-4.2.2/apysc/_validation/arg_validation_decos.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/bool_validation.py` & `apysc-4.2.2/apysc/_validation/bool_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/color_validation.py` & `apysc-4.2.2/apysc/_validation/color_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/display_validation.py` & `apysc-4.2.2/apysc/_validation/display_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/event_validation.py` & `apysc-4.2.2/apysc/_validation/event_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/geom_validation.py` & `apysc-4.2.2/apysc/_validation/geom_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/handler_validation.py` & `apysc-4.2.2/apysc/_validation/handler_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/matrix_data_validation.py` & `apysc-4.2.2/apysc/_validation/matrix_data_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/number_validation.py` & `apysc-4.2.2/apysc/_validation/number_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/parent_validation.py` & `apysc-4.2.2/apysc/_validation/parent_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/path_validation.py` & `apysc-4.2.2/apysc/_validation/path_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/string_validation.py` & `apysc-4.2.2/apysc/_validation/string_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/validation_common_utils.py` & `apysc-4.2.2/apysc/_validation/validation_common_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc/_validation/variable_name_validation.py` & `apysc-4.2.2/apysc/_validation/variable_name_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.2.1/apysc.egg-info/PKG-INFO` & `apysc-4.2.2/apysc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 4.2.1
+Version: 4.2.2
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-4.2.1/apysc.egg-info/SOURCES.txt` & `apysc-4.2.2/apysc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -234,14 +234,15 @@
 apysc/_display/skew_y_mixin.py
 apysc/_display/sprite.py
 apysc/_display/stage.py
 apysc/_display/svg_foreign_object_child.py
 apysc/_display/svg_foreign_object_child_mixin.py
 apysc/_display/svg_foreign_object_initialize_width_mixin.py
 apysc/_display/svg_foreign_object_text_mixin.py
+apysc/_display/svg_icon.py
 apysc/_display/svg_text.py
 apysc/_display/svg_text_align_mixin.py
 apysc/_display/svg_text_bold_mixin.py
 apysc/_display/svg_text_delta_x_mixin.py
 apysc/_display/svg_text_delta_y_mixin.py
 apysc/_display/svg_text_font_family_mixin.py
 apysc/_display/svg_text_font_size_mixin.py
```

