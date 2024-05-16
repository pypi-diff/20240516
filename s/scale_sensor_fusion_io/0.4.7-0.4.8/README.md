# Comparing `tmp/scale_sensor_fusion_io-0.4.7.tar.gz` & `tmp/scale_sensor_fusion_io-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_sensor_fusion_io-0.4.7.tar", max compression
+gzip compressed data, was "scale_sensor_fusion_io-0.4.8.tar", max compression
```

## Comparing `scale_sensor_fusion_io-0.4.7.tar` & `scale_sensor_fusion_io-0.4.8.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     3072 2024-02-23 02:15:01.231766 scale_sensor_fusion_io-0.4.7/docs/README.md
--rw-r--r--   0        0        0     1021 2024-02-26 20:41:28.193282 scale_sensor_fusion_io-0.4.7/pyproject.toml
--rw-r--r--   0        0        0       98 2024-02-23 02:15:01.232528 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/__init__.py
--rw-r--r--   0        0        0       52 2024-02-23 02:15:01.232630 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/loaders/__init__.py
--rw-r--r--   0        0        0     2885 2024-02-23 02:15:01.232706 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/loaders/bs5_loader.py
--rw-r--r--   0        0        0     3220 2024-02-23 02:15:01.232767 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/loaders/sfs_loader.py
--rw-r--r--   0        0        0       19 2024-02-23 02:15:01.232858 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/model_converters/__init__.py
--rw-r--r--   0        0        0    23359 2024-02-26 21:00:22.477406 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/model_converters/sfs.py
--rw-r--r--   0        0        0     9660 2024-02-23 02:15:01.233117 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/Pose.py
--rw-r--r--   0        0        0      259 2024-02-23 02:15:01.233204 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/__init__.py
--rw-r--r--   0        0        0      456 2024-02-23 02:15:01.238377 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/__init__.py
--rw-r--r--   0        0        0      452 2024-02-26 20:58:32.573632 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/attributes.py
--rw-r--r--   0        0        0      626 2024-02-23 02:15:01.238602 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/box_2d.py
--rw-r--r--   0        0        0     1157 2024-02-26 21:01:08.149317 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/cuboid.py
--rw-r--r--   0        0        0      520 2024-02-23 02:15:01.240358 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/event.py
--rw-r--r--   0        0        0      690 2024-02-23 02:15:01.240451 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/labeled_points.py
--rw-r--r--   0        0        0      924 2024-02-23 02:15:01.240526 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/localization_adjustment.py
--rw-r--r--   0        0        0      425 2024-02-23 02:15:01.240591 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/object.py
--rw-r--r--   0        0        0      638 2024-02-23 02:15:01.240665 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/polygon.py
--rw-r--r--   0        0        0     7252 2024-02-23 02:15:01.240747 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/common.py
--rw-r--r--   0        0        0      213 2024-02-23 02:15:01.240875 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/paths/__init__.py
--rw-r--r--   0        0        0      291 2024-02-23 02:15:01.241371 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/paths/attribute_path.py
--rw-r--r--   0        0        0     5616 2024-02-23 02:15:01.241510 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/paths/cuboid_path.py
--rw-r--r--   0        0        0    13319 2024-02-23 02:15:01.242046 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/paths/pose_path.py
--rw-r--r--   0        0        0     6475 2024-02-23 02:15:01.242125 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/paths/spacial_path.py
--rw-r--r--   0        0        0      543 2024-02-23 02:15:01.242790 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/paths/transformable_path.py
--rw-r--r--   0        0        0      634 2024-02-23 02:15:01.242877 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/scene.py
--rw-r--r--   0        0        0      245 2024-02-23 02:15:01.243608 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/__init__.py
--rw-r--r--   0        0        0       94 2024-02-23 02:15:01.243727 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/camera/__init__.py
--rw-r--r--   0        0        0     7359 2024-02-23 02:15:01.243831 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py
--rw-r--r--   0        0        0      310 2024-02-23 02:15:01.243910 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/camera/camera_intrinsics.py
--rw-r--r--   0        0        0     2709 2024-02-23 02:15:01.243993 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py
--rw-r--r--   0        0        0       27 2024-02-23 02:15:01.244104 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/lidar/__init__.py
--rw-r--r--   0        0        0      931 2024-02-23 02:15:01.244184 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py
--rw-r--r--   0        0        0       30 2024-02-23 02:15:01.244289 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/odometry/__init__.py
--rw-r--r--   0        0        0      347 2024-02-23 02:15:01.244355 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/odometry/odometry_sensor.py
--rw-r--r--   0        0        0       28 2024-02-23 02:15:01.244451 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/points/__init__.py
--rw-r--r--   0        0        0      569 2024-02-23 02:15:01.244510 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/points/points_sensor.py
--rw-r--r--   0        0        0       28 2024-02-23 02:15:01.244609 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/radar/__init__.py
--rw-r--r--   0        0        0      825 2024-02-23 02:15:01.244677 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py
--rw-r--r--   0        0        0        0 2024-02-23 02:15:01.244706 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/py.typed
--rw-r--r--   0        0        0       91 2024-02-23 02:15:01.244827 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/spec/__init__.py
--rw-r--r--   0        0        0       21 2024-02-23 02:15:01.244936 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/spec/sfs/__init__.py
--rw-r--r--   0        0        0    10644 2024-02-26 21:01:03.606264 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/spec/sfs/types.py
--rw-r--r--   0        0        0       21 2024-02-23 02:15:01.245118 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/spec/v5/__init__.py
--rw-r--r--   0        0        0     3835 2024-02-26 20:01:28.137043 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/spec/v5/types.py
--rw-r--r--   0        0        0        0 2024-02-23 02:15:01.245254 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/__init__.py
--rw-r--r--   0        0        0     5471 2024-02-23 02:15:01.245345 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/camera_helpers.py
--rw-r--r--   0        0        0     2005 2024-02-23 02:15:01.245417 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/downsample.py
--rw-r--r--   0        0        0      596 2024-02-23 02:15:01.245487 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/models_common_helpers.py
--rw-r--r--   0        0        0     1984 2024-02-23 02:15:01.245562 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/photocolors.py
--rw-r--r--   0        0        0     3579 2024-02-23 02:15:01.245637 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/pose_helpers.py
--rw-r--r--   0        0        0     5817 2024-02-23 02:15:01.245712 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/pose_path_helpers.py
--rw-r--r--   0        0        0     6616 2024-02-23 02:15:01.245790 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/video_helpers.py
--rw-r--r--   0        0        0      899 2024-02-23 02:15:01.245895 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/__init__.py
--rw-r--r--   0        0        0     1069 2024-02-23 02:15:01.245998 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/LICENSE
--rw-r--r--   0        0        0      297 2024-02-23 02:15:01.246059 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/README.md
--rw-r--r--   0        0        0      135 2024-02-23 02:15:01.246113 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/__init__.py
--rw-r--r--   0        0        0      502 2024-02-23 02:15:01.246173 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/config.py
--rw-r--r--   0        0        0     7388 2024-02-23 02:15:01.246253 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/core.py
--rw-r--r--   0        0        0       90 2024-02-23 02:15:01.246307 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/data.py
--rw-r--r--   0        0        0     1121 2024-02-23 02:15:01.246379 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py
--rw-r--r--   0        0        0     2949 2024-02-23 02:15:01.246457 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py
--rw-r--r--   0        0        0     8189 2024-02-23 02:15:01.246546 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/types.py
--rw-r--r--   0        0        0     2802 2024-02-23 02:15:01.246615 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/error.py
--rw-r--r--   0        0        0      955 2024-02-23 02:15:01.246694 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/helpers.py
--rw-r--r--   0        0        0       19 2024-02-23 02:15:01.246800 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/parser/__init__.py
--rw-r--r--   0        0        0     7525 2024-02-23 02:15:01.246884 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/parser/sfs.py
--rw-r--r--   0        0        0    19071 2024-02-23 02:15:01.246982 scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/validate.py
--rw-r--r--   0        0        0     4104 1970-01-01 00:00:00.000000 scale_sensor_fusion_io-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     3072 2024-02-16 04:29:15.681972 scale_sensor_fusion_io-0.4.8/docs/README.md
+-rw-r--r--   0        0        0     1021 2024-05-16 18:12:23.555416 scale_sensor_fusion_io-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-02-16 04:29:15.682670 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/__init__.py
+-rw-r--r--   0        0        0       52 2024-02-16 04:29:15.682773 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/loaders/__init__.py
+-rw-r--r--   0        0        0     2885 2024-02-16 04:29:15.682857 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/loaders/bs5_loader.py
+-rw-r--r--   0        0        0     3220 2024-02-16 04:29:15.682926 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/loaders/sfs_loader.py
+-rw-r--r--   0        0        0       19 2024-02-16 04:29:15.683048 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/model_converters/__init__.py
+-rw-r--r--   0        0        0    23359 2024-03-03 19:33:08.796957 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/model_converters/sfs.py
+-rw-r--r--   0        0        0     9660 2024-02-16 04:29:15.683298 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/Pose.py
+-rw-r--r--   0        0        0      259 2024-02-16 04:29:15.683367 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/__init__.py
+-rw-r--r--   0        0        0      456 2024-02-16 04:29:15.683470 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/__init__.py
+-rw-r--r--   0        0        0      452 2024-03-03 19:33:08.797329 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/attributes.py
+-rw-r--r--   0        0        0      626 2024-02-16 04:29:15.683642 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/box_2d.py
+-rw-r--r--   0        0        0     1157 2024-03-03 19:33:08.797570 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/cuboid.py
+-rw-r--r--   0        0        0      520 2024-02-16 04:29:15.683783 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/event.py
+-rw-r--r--   0        0        0      690 2024-02-16 04:29:15.683875 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/labeled_points.py
+-rw-r--r--   0        0        0      924 2024-02-16 04:29:15.683978 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/localization_adjustment.py
+-rw-r--r--   0        0        0      425 2024-02-16 04:29:15.684059 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/object.py
+-rw-r--r--   0        0        0      638 2024-02-16 04:29:15.684121 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/polygon.py
+-rw-r--r--   0        0        0     7252 2024-02-16 04:29:15.684217 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/common.py
+-rw-r--r--   0        0        0      213 2024-02-16 04:29:15.684352 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/paths/__init__.py
+-rw-r--r--   0        0        0      291 2024-02-16 04:29:15.684424 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/paths/attribute_path.py
+-rw-r--r--   0        0        0     5616 2024-02-16 04:29:15.684556 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/paths/cuboid_path.py
+-rw-r--r--   0        0        0    13319 2024-02-16 04:29:15.684641 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/paths/pose_path.py
+-rw-r--r--   0        0        0     6475 2024-02-16 04:29:15.684725 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/paths/spacial_path.py
+-rw-r--r--   0        0        0      543 2024-02-16 04:29:15.684796 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/paths/transformable_path.py
+-rw-r--r--   0        0        0      634 2024-02-16 04:29:15.684876 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/scene.py
+-rw-r--r--   0        0        0      245 2024-02-16 04:29:15.684988 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/__init__.py
+-rw-r--r--   0        0        0       94 2024-02-16 04:29:15.685085 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/camera/__init__.py
+-rw-r--r--   0        0        0     7359 2024-02-16 04:29:15.685172 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py
+-rw-r--r--   0        0        0      310 2024-02-16 04:29:15.685239 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/camera/camera_intrinsics.py
+-rw-r--r--   0        0        0     2760 2024-03-25 21:50:09.870304 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py
+-rw-r--r--   0        0        0       27 2024-02-16 04:29:15.685414 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/lidar/__init__.py
+-rw-r--r--   0        0        0      931 2024-02-16 04:29:15.685531 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py
+-rw-r--r--   0        0        0       30 2024-02-16 04:29:15.685658 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/odometry/__init__.py
+-rw-r--r--   0        0        0      347 2024-02-16 04:29:15.685732 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/odometry/odometry_sensor.py
+-rw-r--r--   0        0        0       28 2024-02-16 04:29:15.685843 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/points/__init__.py
+-rw-r--r--   0        0        0      569 2024-02-16 04:29:15.685911 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/points/points_sensor.py
+-rw-r--r--   0        0        0       28 2024-02-16 04:29:15.686006 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/radar/__init__.py
+-rw-r--r--   0        0        0      825 2024-02-16 04:29:15.686084 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py
+-rw-r--r--   0        0        0        0 2024-02-16 04:29:15.686122 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/py.typed
+-rw-r--r--   0        0        0       91 2024-02-16 04:29:15.686253 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/spec/__init__.py
+-rw-r--r--   0        0        0       21 2024-02-16 04:29:15.686373 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/spec/sfs/__init__.py
+-rw-r--r--   0        0        0    10644 2024-03-03 19:33:08.797871 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/spec/sfs/types.py
+-rw-r--r--   0        0        0       21 2024-02-16 04:29:15.686575 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/spec/v5/__init__.py
+-rw-r--r--   0        0        0     3835 2024-03-03 19:33:08.798121 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/spec/v5/types.py
+-rw-r--r--   0        0        0        0 2024-02-16 04:29:15.686698 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/__init__.py
+-rw-r--r--   0        0        0     5471 2024-02-16 04:29:15.686792 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/camera_helpers.py
+-rw-r--r--   0        0        0     2005 2024-02-16 04:29:15.686862 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/downsample.py
+-rw-r--r--   0        0        0      596 2024-02-16 04:29:15.686928 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/models_common_helpers.py
+-rw-r--r--   0        0        0     1984 2024-02-16 04:29:15.687012 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/photocolors.py
+-rw-r--r--   0        0        0     3579 2024-02-16 04:29:15.687089 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/pose_helpers.py
+-rw-r--r--   0        0        0     5817 2024-02-16 04:29:15.687195 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/pose_path_helpers.py
+-rw-r--r--   0        0        0     6616 2024-02-16 04:29:15.687297 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/video_helpers.py
+-rw-r--r--   0        0        0      899 2024-02-16 04:29:15.687414 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/__init__.py
+-rw-r--r--   0        0        0     1069 2024-02-16 04:29:15.687528 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/LICENSE
+-rw-r--r--   0        0        0      297 2024-02-16 04:29:15.687593 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/README.md
+-rw-r--r--   0        0        0      135 2024-02-16 04:29:15.687649 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/__init__.py
+-rw-r--r--   0        0        0      502 2024-02-16 04:29:15.687708 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/config.py
+-rw-r--r--   0        0        0     7388 2024-02-16 04:29:15.687792 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/core.py
+-rw-r--r--   0        0        0       90 2024-02-16 04:29:15.687864 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/data.py
+-rw-r--r--   0        0        0     1121 2024-02-16 04:29:15.687939 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py
+-rw-r--r--   0        0        0     2949 2024-02-16 04:29:15.688017 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py
+-rw-r--r--   0        0        0     8189 2024-02-16 04:29:15.688115 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/types.py
+-rw-r--r--   0        0        0     2802 2024-02-16 04:29:15.688197 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/error.py
+-rw-r--r--   0        0        0      955 2024-02-16 04:29:15.688274 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/helpers.py
+-rw-r--r--   0        0        0       19 2024-02-16 04:29:15.688368 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/parser/__init__.py
+-rw-r--r--   0        0        0     7525 2024-02-16 04:29:15.688453 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/parser/sfs.py
+-rw-r--r--   0        0        0    19071 2024-02-16 04:29:15.688536 scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/validate.py
+-rw-r--r--   0        0        0     4104 1970-01-01 00:00:00.000000 scale_sensor_fusion_io-0.4.8/PKG-INFO
```

### Comparing `scale_sensor_fusion_io-0.4.7/docs/README.md` & `scale_sensor_fusion_io-0.4.8/docs/README.md`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/pyproject.toml` & `scale_sensor_fusion_io-0.4.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale_sensor_fusion_io"
-version = "0.4.7"
+version = "0.4.8"
 description = "Library for working with timestamp-based sensor fusion scenes"
 authors = [
     "Michael Choi <michael.choi@scale.com>",
     "Rodrigo Belfiore <rodrigo.belfiore@scale.com>"
 ]
 readme = ["docs/README.md"]
```

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/loaders/bs5_loader.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/loaders/bs5_loader.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/loaders/sfs_loader.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/loaders/sfs_loader.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/model_converters/sfs.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/model_converters/sfs.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/Pose.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/Pose.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/box_2d.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/box_2d.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/cuboid.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/cuboid.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/event.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/event.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/labeled_points.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/labeled_points.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/localization_adjustment.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/localization_adjustment.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/annotations/polygon.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/annotations/polygon.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/common.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/common.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/paths/cuboid_path.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/paths/cuboid_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/paths/pose_path.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/paths/pose_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/paths/spacial_path.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/paths/spacial_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/paths/transformable_path.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/paths/transformable_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/scene.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/scene.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     id: SensorID
     poses: PosePath
     intrinsics: CameraIntrinsics
     video: Optional[CameraSensorVideo] = None
     images: Optional[List[CameraSensorImage]] = None
     type: Literal[SensorKind.Camera] = SensorKind.Camera
     parent_id: Optional[SensorID] = None
+    coordinates: Literal["ego", "world"] = "world"
 
     video_loader: Optional[VideoReader] = None
 
     def __init__(
         self,
         id: SensorID,
         poses: PosePath,
```

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/points/points_sensor.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/points/points_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/spec/sfs/types.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/spec/sfs/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/spec/v5/types.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/spec/v5/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/camera_helpers.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/camera_helpers.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/downsample.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/downsample.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/models_common_helpers.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/models_common_helpers.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/photocolors.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/photocolors.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/pose_helpers.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/pose_helpers.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/pose_path_helpers.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/pose_path_helpers.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/utils/video_helpers.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/utils/video_helpers.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/__init__.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/LICENSE` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/LICENSE`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/core.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/core.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/dacite_internal/types.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/dacite_internal/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/error.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/error.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/helpers.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/helpers.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/parser/sfs.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/parser/sfs.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/scale_sensor_fusion_io/validation/validate.py` & `scale_sensor_fusion_io-0.4.8/scale_sensor_fusion_io/validation/validate.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.4.7/PKG-INFO` & `scale_sensor_fusion_io-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scale-sensor-fusion-io
-Version: 0.4.7
+Name: scale_sensor_fusion_io
+Version: 0.4.8
 Summary: Library for working with timestamp-based sensor fusion scenes
 Author: Michael Choi
 Author-email: michael.choi@scale.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

