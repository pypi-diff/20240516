# Comparing `tmp/solidipes-0.1.7.tar.gz` & `tmp/solidipes-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidipes-0.1.7.tar", max compression
+gzip compressed data, was "solidipes-0.1.8.tar", max compression
```

## Comparing `solidipes-0.1.7.tar` & `solidipes-0.1.8.tar`

### file list

```diff
@@ -1,76 +1,89 @@
--rw-r--r--   0        0        0    35129 2023-11-16 16:27:48.372772 solidipes-0.1.7/LICENSE
--rw-r--r--   0        0        0     1272 2023-08-31 08:58:28.521412 solidipes-0.1.7/README.md
--rw-r--r--   0        0        0     2467 2023-12-20 15:24:22.388500 solidipes-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      156 2023-12-20 15:24:22.388500 solidipes-0.1.7/solidipes/__init__.py
--rw-r--r--   0        0        0      568 2023-12-18 21:57:02.311931 solidipes-0.1.7/solidipes/loaders/__init__.py
--rw-r--r--   0        0        0      738 2023-09-29 11:10:03.262944 solidipes-0.1.7/solidipes/loaders/binary.py
--rw-r--r--   0        0        0     3198 2023-11-13 14:52:18.660850 solidipes-0.1.7/solidipes/loaders/cached_metadata.py
--rw-r--r--   0        0        0      483 2023-12-18 21:57:02.311931 solidipes-0.1.7/solidipes/loaders/code_snippet.py
--rw-r--r--   0        0        0     5371 2023-09-29 11:10:03.266944 solidipes-0.1.7/solidipes/loaders/data_container.py
--rw-r--r--   0        0        0     3982 2023-10-13 08:41:37.123747 solidipes-0.1.7/solidipes/loaders/file.py
--rw-r--r--   0        0        0     1258 2023-09-29 11:10:03.266944 solidipes-0.1.7/solidipes/loaders/file_sequence.py
--rw-r--r--   0        0        0      545 2023-09-14 07:55:00.579056 solidipes-0.1.7/solidipes/loaders/geof_mesh.py
--rw-r--r--   0        0        0      586 2023-12-18 21:57:02.311931 solidipes-0.1.7/solidipes/loaders/hdf5.py
--rw-r--r--   0        0        0     2033 2023-09-29 11:10:03.266944 solidipes-0.1.7/solidipes/loaders/image.py
--rw-r--r--   0        0        0     1598 2023-09-29 11:10:03.266944 solidipes-0.1.7/solidipes/loaders/image_sequence.py
--rw-r--r--   0        0        0      701 2023-11-13 10:57:28.615984 solidipes-0.1.7/solidipes/loaders/matlab.py
--rw-r--r--   0        0        0      486 2023-09-29 11:10:03.266944 solidipes-0.1.7/solidipes/loaders/meshio.py
--rw-r--r--   0        0        0    75245 2023-11-13 10:57:28.615984 solidipes-0.1.7/solidipes/loaders/mime_types.py
--rw-r--r--   0        0        0     6704 2023-11-10 06:39:48.213075 solidipes-0.1.7/solidipes/loaders/parse_inp.py
--rw-r--r--   0        0        0      726 2023-09-29 11:10:03.270944 solidipes-0.1.7/solidipes/loaders/pdf.py
--rw-r--r--   0        0        0     5329 2023-09-29 11:10:03.270944 solidipes-0.1.7/solidipes/loaders/pyvista_mesh.py
--rw-r--r--   0        0        0     1336 2023-09-14 07:55:00.583056 solidipes-0.1.7/solidipes/loaders/sequence.py
--rw-r--r--   0        0        0     1512 2023-09-29 11:10:03.270944 solidipes-0.1.7/solidipes/loaders/symlink.py
--rw-r--r--   0        0        0     1738 2023-09-29 11:10:03.270944 solidipes-0.1.7/solidipes/loaders/table.py
--rw-r--r--   0        0        0      915 2023-09-29 11:10:03.274944 solidipes-0.1.7/solidipes/loaders/text.py
--rw-r--r--   0        0        0      526 2023-09-29 11:10:03.274944 solidipes-0.1.7/solidipes/loaders/video.py
--rw-r--r--   0        0        0        0 2023-12-20 15:24:09.976685 solidipes-0.1.7/solidipes/reports/__init__.py
--rw-r--r--   0        0        0     2504 2023-09-29 11:10:03.274944 solidipes-0.1.7/solidipes/reports/curation.py
--rw-r--r--   0        0        0     6598 2023-09-29 11:10:03.274944 solidipes-0.1.7/solidipes/reports/jtcam.py
--rw-r--r--   0        0        0     8405 2023-04-26 08:20:51.882613 solidipes-0.1.7/solidipes/reports/jtcam_small_logo.png
--rw-r--r--   0        0        0    28449 2023-04-26 08:20:51.882613 solidipes-0.1.7/solidipes/reports/jupyter_logo.png
--rw-r--r--   0        0        0    26483 2023-12-18 21:57:02.315931 solidipes-0.1.7/solidipes/reports/web_report.py
--rw-r--r--   0        0        0     7827 2023-12-19 13:39:16.988423 solidipes-0.1.7/solidipes/reports/widgets/custom_widgets.py
--rw-r--r--   0        0        0     1099 2023-06-20 13:42:58.863308 solidipes-0.1.7/solidipes/reports/widgets/git_infos.py
--rw-r--r--   0        0        0     2498 2023-06-20 13:42:58.863308 solidipes-0.1.7/solidipes/reports/widgets/gitlab_issues.py
--rw-r--r--   0        0        0      631 2023-09-14 07:55:00.591056 solidipes-0.1.7/solidipes/reports/widgets/speech_bubble.css
--rw-r--r--   0        0        0      109 2023-09-14 07:55:00.591056 solidipes-0.1.7/solidipes/reports/widgets/speech_bubble.html
--rw-r--r--   0        0        0    18471 2023-12-20 14:06:56.760923 solidipes-0.1.7/solidipes/reports/widgets/zenodo.py
--rw-r--r--   0        0        0     6230 2023-09-29 11:10:03.278945 solidipes-0.1.7/solidipes/scanners/scanner.py
--rw-r--r--   0        0        0        0 2023-12-20 15:24:09.976685 solidipes-0.1.7/solidipes/scripts/__init__.py
--rw-r--r--   0        0        0     3276 2023-09-29 11:10:03.278945 solidipes-0.1.7/solidipes/scripts/download.py
--rw-r--r--   0        0        0     1492 2023-09-29 11:10:03.278945 solidipes-0.1.7/solidipes/scripts/generate_report.py
--rw-r--r--   0        0        0     4213 2023-10-13 10:22:44.982905 solidipes-0.1.7/solidipes/scripts/init.py
--rw-r--r--   0        0        0     1022 2023-09-14 07:55:00.595056 solidipes-0.1.7/solidipes/scripts/main.py
--rw-r--r--   0        0        0     9892 2023-12-18 21:57:02.315931 solidipes-0.1.7/solidipes/scripts/mount.py
--rw-r--r--   0        0        0     1082 2023-11-13 10:57:28.615984 solidipes-0.1.7/solidipes/scripts/quick_view.py
--rw-r--r--   0        0        0     2534 2023-09-29 11:10:03.282945 solidipes-0.1.7/solidipes/scripts/unmount.py
--rw-r--r--   0        0        0     1670 2023-12-18 21:57:02.315931 solidipes-0.1.7/solidipes/scripts/upload.py
--rw-r--r--   0        0        0        0 2023-12-20 15:24:09.976685 solidipes-0.1.7/solidipes/uploaders/__init__.py
--rw-r--r--   0        0        0     3209 2023-12-18 21:57:02.315931 solidipes-0.1.7/solidipes/uploaders/renku.py
--rw-r--r--   0        0        0      241 2023-12-18 21:57:02.315931 solidipes-0.1.7/solidipes/uploaders/uploader.py
--rw-r--r--   0        0        0    11170 2023-12-18 21:57:02.319931 solidipes-0.1.7/solidipes/uploaders/zenodo.py
--rw-r--r--   0        0        0     1962 2023-11-13 14:52:18.664850 solidipes-0.1.7/solidipes/utils/__init__.py
--rw-r--r--   0        0        0    17161 2023-12-19 09:01:40.370213 solidipes-0.1.7/solidipes/utils/cloud.py
--rw-r--r--   0        0        0     1395 2023-09-29 11:10:03.286945 solidipes-0.1.7/solidipes/utils/config.py
--rw-r--r--   0        0        0    24251 2023-09-29 11:10:03.286945 solidipes-0.1.7/solidipes/utils/languages-iso-639-2.csv
--rw-r--r--   0        0        0    16110 2023-09-29 11:10:03.286945 solidipes-0.1.7/solidipes/utils/licenses.csv
--rw-r--r--   0        0        0     1133 2023-09-29 11:10:03.290945 solidipes-0.1.7/solidipes/utils/metadata.py
--rw-r--r--   0        0        0     1442 2023-09-29 11:10:03.290945 solidipes-0.1.7/solidipes/utils/solidipes_logging.py
--rw-r--r--   0        0        0    13816 2023-12-18 21:57:02.319931 solidipes-0.1.7/solidipes/utils/utils.py
--rw-r--r--   0        0        0     1535 2023-09-29 11:10:03.290945 solidipes-0.1.7/solidipes/utils/viewer_backends.py
--rw-r--r--   0        0        0     8609 2023-12-19 12:17:13.645596 solidipes-0.1.7/solidipes/utils/zenodo_utils.py
--rw-r--r--   0        0        0      553 2023-12-18 21:57:02.319931 solidipes-0.1.7/solidipes/viewers/__init__.py
--rw-r--r--   0        0        0     1387 2023-11-10 23:35:49.904012 solidipes-0.1.7/solidipes/viewers/binary.py
--rw-r--r--   0        0        0     1014 2023-09-29 11:10:03.290945 solidipes-0.1.7/solidipes/viewers/code_snippet.py
--rw-r--r--   0        0        0     2564 2023-12-18 21:57:02.319931 solidipes-0.1.7/solidipes/viewers/hdf5.py
--rw-r--r--   0        0        0     1588 2023-09-29 11:10:03.294945 solidipes-0.1.7/solidipes/viewers/image.py
--rw-r--r--   0        0        0     1197 2023-11-13 10:57:28.619984 solidipes-0.1.7/solidipes/viewers/matlab.py
--rw-r--r--   0        0        0     1553 2023-09-29 11:10:03.294945 solidipes-0.1.7/solidipes/viewers/pdf.py
--rw-r--r--   0        0        0     5092 2023-09-29 11:10:03.294945 solidipes-0.1.7/solidipes/viewers/pyvista_plotter.py
--rw-r--r--   0        0        0      853 2023-09-29 11:10:03.294945 solidipes-0.1.7/solidipes/viewers/symlink.py
--rw-r--r--   0        0        0     3527 2023-12-18 21:57:02.323931 solidipes-0.1.7/solidipes/viewers/table.py
--rw-r--r--   0        0        0     2031 2023-09-29 11:10:03.294945 solidipes-0.1.7/solidipes/viewers/text.py
--rw-r--r--   0        0        0      849 2023-09-29 11:10:03.294945 solidipes-0.1.7/solidipes/viewers/video.py
--rw-r--r--   0        0        0     2228 2023-09-29 11:10:03.294945 solidipes-0.1.7/solidipes/viewers/viewer.py
--rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 solidipes-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      774 2023-11-16 16:27:01.101462 solidipes-0.1.8/AUTHORS
+-rw-r--r--   0        0        0    35129 2023-11-16 16:27:01.105461 solidipes-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1272 2023-08-31 08:57:41.644682 solidipes-0.1.8/README.md
+-rw-r--r--   0        0        0     2605 2024-05-16 10:52:39.708777 solidipes-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      379 2024-05-16 10:52:39.712777 solidipes-0.1.8/solidipes/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-26 09:02:52.939581 solidipes-0.1.8/solidipes/loaders/__init__.py
+-rw-r--r--   0        0        0     5707 2024-04-15 07:08:11.288179 solidipes-0.1.8/solidipes/loaders/abaqus.py
+-rw-r--r--   0        0        0      532 2024-05-15 12:13:53.770557 solidipes-0.1.8/solidipes/loaders/binary.py
+-rw-r--r--   0        0        0     9147 2024-05-02 15:05:35.925093 solidipes-0.1.8/solidipes/loaders/cached_metadata.py
+-rw-r--r--   0        0        0     1975 2024-05-02 15:47:42.837257 solidipes-0.1.8/solidipes/loaders/code_snippet.py
+-rw-r--r--   0        0        0     6049 2024-04-19 17:51:44.056123 solidipes-0.1.8/solidipes/loaders/data_container.py
+-rw-r--r--   0        0        0     6131 2024-05-02 15:05:35.925093 solidipes-0.1.8/solidipes/loaders/file.py
+-rw-r--r--   0        0        0     2320 2024-04-26 09:02:52.939581 solidipes-0.1.8/solidipes/loaders/file_sequence.py
+-rw-r--r--   0        0        0      335 2024-04-15 11:23:15.272215 solidipes-0.1.8/solidipes/loaders/geof_mesh.py
+-rw-r--r--   0        0        0     1657 2024-04-26 09:36:07.215633 solidipes-0.1.8/solidipes/loaders/group.py
+-rw-r--r--   0        0        0      355 2024-04-15 07:08:11.292179 solidipes-0.1.8/solidipes/loaders/hdf5.py
+-rw-r--r--   0        0        0     1589 2024-04-15 07:08:11.292179 solidipes-0.1.8/solidipes/loaders/image.py
+-rw-r--r--   0        0        0     1386 2024-04-15 07:08:11.292179 solidipes-0.1.8/solidipes/loaders/image_sequence.py
+-rw-r--r--   0        0        0      449 2024-04-15 07:08:11.292179 solidipes-0.1.8/solidipes/loaders/matlab.py
+-rw-r--r--   0        0        0      336 2024-04-24 16:29:05.346347 solidipes-0.1.8/solidipes/loaders/meshio.py
+-rw-r--r--   0        0        0    75469 2024-04-15 11:23:15.276215 solidipes-0.1.8/solidipes/loaders/mime_types.py
+-rw-r--r--   0        0        0      392 2024-04-15 07:08:11.296179 solidipes-0.1.8/solidipes/loaders/notebook.py
+-rw-r--r--   0        0        0     6704 2023-11-10 06:38:59.297788 solidipes-0.1.8/solidipes/loaders/parse_inp.py
+-rw-r--r--   0        0        0      598 2024-04-15 07:08:11.296179 solidipes-0.1.8/solidipes/loaders/pdf.py
+-rw-r--r--   0        0        0     4970 2024-04-15 11:23:15.276215 solidipes-0.1.8/solidipes/loaders/pyvista_mesh.py
+-rw-r--r--   0        0        0     1471 2024-04-15 07:08:11.296179 solidipes-0.1.8/solidipes/loaders/sequence.py
+-rw-r--r--   0        0        0      596 2024-04-22 10:44:07.489071 solidipes-0.1.8/solidipes/loaders/symlink.py
+-rw-r--r--   0        0        0     1702 2024-04-15 07:08:11.296179 solidipes-0.1.8/solidipes/loaders/table.py
+-rw-r--r--   0        0        0      721 2024-04-15 07:08:11.300179 solidipes-0.1.8/solidipes/loaders/text.py
+-rw-r--r--   0        0        0      329 2024-04-15 07:08:11.300179 solidipes-0.1.8/solidipes/loaders/video.py
+-rw-r--r--   0        0        0     5001 2024-04-15 07:08:11.300179 solidipes-0.1.8/solidipes/loaders/xdmf.py
+-rw-r--r--   0        0        0      452 2024-04-15 07:08:11.300179 solidipes-0.1.8/solidipes/loaders/xml.py
+-rw-r--r--   0        0        0        0 2024-05-16 10:52:32.348613 solidipes-0.1.8/solidipes/reports/__init__.py
+-rw-r--r--   0        0        0     3537 2024-04-26 17:57:48.050239 solidipes-0.1.8/solidipes/reports/curation.py
+-rw-r--r--   0        0        0     6480 2024-04-22 10:44:07.489071 solidipes-0.1.8/solidipes/reports/jtcam.py
+-rw-r--r--   0        0        0     8405 2023-04-26 08:20:35.886224 solidipes-0.1.8/solidipes/reports/jtcam_small_logo.png
+-rw-r--r--   0        0        0    28449 2023-04-26 08:20:35.890224 solidipes-0.1.8/solidipes/reports/jupyter_logo.png
+-rw-r--r--   0        0        0      310 2024-04-22 10:44:07.489071 solidipes-0.1.8/solidipes/reports/report.py
+-rw-r--r--   0        0        0    28738 2024-05-16 10:52:17.832288 solidipes-0.1.8/solidipes/reports/web_report.py
+-rw-r--r--   0        0        0        0 2024-05-16 10:52:32.348613 solidipes-0.1.8/solidipes/reports/widgets/__init__.py
+-rw-r--r--   0        0        0     7827 2023-12-19 14:01:29.288781 solidipes-0.1.8/solidipes/reports/widgets/custom_widgets.py
+-rw-r--r--   0        0        0     2530 2024-04-22 10:44:07.489071 solidipes-0.1.8/solidipes/reports/widgets/gitlab_issues.py
+-rw-r--r--   0        0        0      631 2023-09-14 07:54:57.371005 solidipes-0.1.8/solidipes/reports/widgets/speech_bubble.css
+-rw-r--r--   0        0        0      109 2023-09-14 07:54:57.371005 solidipes-0.1.8/solidipes/reports/widgets/speech_bubble.html
+-rw-r--r--   0        0        0    18299 2024-04-24 16:29:05.346347 solidipes-0.1.8/solidipes/reports/widgets/zenodo.py
+-rw-r--r--   0        0        0      132 2024-04-22 10:44:07.489071 solidipes-0.1.8/solidipes/scanners/__init__.py
+-rw-r--r--   0        0        0    13080 2024-05-02 14:10:42.580154 solidipes-0.1.8/solidipes/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2024-05-16 10:52:32.348613 solidipes-0.1.8/solidipes/scripts/__init__.py
+-rw-r--r--   0        0        0     3276 2023-09-29 11:08:26.065427 solidipes-0.1.8/solidipes/scripts/download.py
+-rw-r--r--   0        0        0     1255 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/scripts/generate_report.py
+-rw-r--r--   0        0        0     4213 2023-10-13 10:23:46.696651 solidipes-0.1.8/solidipes/scripts/init.py
+-rw-r--r--   0        0        0     1022 2023-09-14 07:54:57.371005 solidipes-0.1.8/solidipes/scripts/main.py
+-rw-r--r--   0        0        0    10148 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/scripts/mount.py
+-rw-r--r--   0        0        0     1133 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/scripts/quick_view.py
+-rw-r--r--   0        0        0     2570 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/scripts/unmount.py
+-rw-r--r--   0        0        0     1189 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/scripts/upload.py
+-rw-r--r--   0        0        0        0 2024-05-16 10:52:32.348613 solidipes-0.1.8/solidipes/uploaders/__init__.py
+-rw-r--r--   0        0        0     3167 2024-04-15 07:08:11.312179 solidipes-0.1.8/solidipes/uploaders/renku.py
+-rw-r--r--   0        0        0      314 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/uploaders/uploader.py
+-rw-r--r--   0        0        0    10769 2024-04-26 17:57:48.050239 solidipes-0.1.8/solidipes/uploaders/zenodo.py
+-rw-r--r--   0        0        0     1457 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/utils/__init__.py
+-rw-r--r--   0        0        0    18232 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/utils/cloud.py
+-rw-r--r--   0        0        0     1863 2024-04-26 08:08:46.255817 solidipes-0.1.8/solidipes/utils/config.py
+-rw-r--r--   0        0        0     1151 2024-04-22 10:44:07.497071 solidipes-0.1.8/solidipes/utils/git_infos.py
+-rw-r--r--   0        0        0    24251 2023-09-29 11:08:26.069427 solidipes-0.1.8/solidipes/utils/languages-iso-639-2.csv
+-rw-r--r--   0        0        0    16110 2023-09-29 11:08:26.073427 solidipes-0.1.8/solidipes/utils/licenses.csv
+-rw-r--r--   0        0        0     1177 2024-04-22 10:44:07.497071 solidipes-0.1.8/solidipes/utils/list_subclasses.py
+-rw-r--r--   0        0        0     1133 2023-09-29 11:08:26.073427 solidipes-0.1.8/solidipes/utils/metadata.py
+-rw-r--r--   0        0        0     2500 2024-04-22 10:44:07.497071 solidipes-0.1.8/solidipes/utils/solidipes_logging.py
+-rw-r--r--   0        0        0    12754 2024-05-01 15:10:16.133710 solidipes-0.1.8/solidipes/utils/utils.py
+-rw-r--r--   0        0        0     1535 2024-04-19 17:51:44.064123 solidipes-0.1.8/solidipes/utils/viewer_backends.py
+-rw-r--r--   0        0        0     8610 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/utils/zenodo_utils.py
+-rw-r--r--   0        0        0      584 2024-04-22 10:44:07.497071 solidipes-0.1.8/solidipes/viewers/__init__.py
+-rw-r--r--   0        0        0     1382 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/viewers/binary.py
+-rw-r--r--   0        0        0     1857 2024-04-24 16:29:05.346347 solidipes-0.1.8/solidipes/viewers/code_snippet.py
+-rw-r--r--   0        0        0     2963 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/viewers/hdf5.py
+-rw-r--r--   0        0        0     1588 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/viewers/image.py
+-rw-r--r--   0        0        0     1197 2023-11-13 10:56:42.404659 solidipes-0.1.8/solidipes/viewers/matlab.py
+-rw-r--r--   0        0        0     1765 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/viewers/notebook.py
+-rw-r--r--   0        0        0     1553 2023-09-29 11:08:26.077427 solidipes-0.1.8/solidipes/viewers/pdf.py
+-rw-r--r--   0        0        0     5256 2024-04-19 17:51:44.068123 solidipes-0.1.8/solidipes/viewers/pyvista_plotter.py
+-rw-r--r--   0        0        0      853 2023-09-29 11:08:26.077427 solidipes-0.1.8/solidipes/viewers/symlink.py
+-rw-r--r--   0        0        0     3806 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/viewers/table.py
+-rw-r--r--   0        0        0     2031 2023-09-29 11:08:26.077427 solidipes-0.1.8/solidipes/viewers/text.py
+-rw-r--r--   0        0        0      849 2023-09-29 11:08:26.077427 solidipes-0.1.8/solidipes/viewers/video.py
+-rw-r--r--   0        0        0     2228 2023-09-29 11:08:26.077427 solidipes-0.1.8/solidipes/viewers/viewer.py
+-rw-r--r--   0        0        0      799 2024-04-15 11:23:15.284216 solidipes-0.1.8/solidipes/viewers/xdmf.py
+-rw-r--r--   0        0        0     1024 2024-04-15 11:23:15.284216 solidipes-0.1.8/solidipes/viewers/xml.py
+-rw-r--r--   0        0        0     3518 1970-01-01 00:00:00.000000 solidipes-0.1.8/PKG-INFO
```

### Comparing `solidipes-0.1.7/LICENSE` & `solidipes-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/README.md` & `solidipes-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/pyproject.toml` & `solidipes-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,92 @@
 [tool.poetry]
 name = "solidipes"
-version = "0.1.7"
+version = "0.1.8"
 description = "Python package for the DCSM project"
 authors = [
 	"Guillaume Anciaux <guillaume.anciaux@epfl.ch>",
 	"Son Pham-Ba <son.phamba@epfl.ch>"
 ]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "solidipes"}]
 homepage = "https://gitlab.com/groups/dcsm"
 repository = "https://gitlab.com/dcsm/solidipes"
 documentation = "https://solidipes.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
 python = ">=3.9.12,<3.13"
+panel = "1.3.0"
 filetype = "^1.2.0"
 pandas = ">=1.5.3"
 openpyxl = "^3.1.1"
 meshio = {extras = ["all"], version = "^5.3.4"}
 pyvista = "^0.38.1"
 trame = "^2.2.6"
 streamlit = "^1.17.0"
 stpyvista = "^0.0.8"
 datasize = "^1.0.0"
 ipydatawidgets = "4.3.2"
 streamlit-tree-select = "^0.0.5"
 streamlit-js-eval = "^0.1.5"
 scipy = ">=1.10.1"
 sympy = ">=1.11.1"
-requests = "2.29.0"
+requests = "^2.31.0"
 pyyaml = "^6.0"
 tqdm = "^4.65.0"
 streamlit-option-menu = "^0.3.2"
-requests-toolbelt = "^0.10.1"
 argcomplete = "^3.0.5"
 streamlit-ace = "^0.1.1"
 markdown = "^3.4.3"
 python-gitlab = "^3.14.0"
 matplotlib = ">=3.7.1"
 cairosvg = "^2.7.0"
 markdownify = "^0.11.6"
 streamlit-quill = "^0.0.3"
 streamlit-editable-list = "0.0.5"
 psycopg2 = "^2.9.9"
+xmltodict = "^0.13.0"
+mergedeep = "^1.3.4"
+zodb = "^6.0"
+btrees = "^5.2"
+lazy-loader = "^0.4"
+nbformat = "^5.10.4"
+pylint = "^3.1.0"
+traitlets = "5.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.4"
 build = "^0.10.0"
-pytest = "^7.2.1"
+pytest = "^8.1.1"
 jupyter = "^1.0.0"
 jupyterlab = "^3.6.1"
 jupyterlab-widgets = "^3.0.5"
 itkwidgets = "^0.32.5"
-sphinx = "^5.3.0"
-sphinx-rtd-theme = "^1.2.0"
-myst-parser = "^0.18.1"
+sphinx = "^7.2.6"
+sphinx-rtd-theme = "^2.0.0"
+myst-parser = "^2.0.0"
 coverage = "^7.2.1"
 pillow = "^9.4.0"
 pixelmatch = "^0.3.0"
-seleniumbase = "^4.14.2"
+seleniumbase = "^4.25.1"
 requests-mock = "^1.10.0"
 git-changelog = "^1.0.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3.1"
+pytest = "^8.1.1"
 pillow = "^9.5.0"
 pixelmatch = "^0.3.0"
-seleniumbase = "^4.14.2"
+seleniumbase = "^4.25.1"
 requests-mock = "^1.10.0"
 
 [tool.poetry.group.doc.dependencies]
 urllib3 = "<2"
-sphinx = "^5.3.0"
-sphinx-rtd-theme = "^1.2.0"
-myst-parser = "^0.18.1"
+sphinx = "^7.2.6"
+sphinx-rtd-theme = "^2.0.0"
+myst-parser = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `solidipes-0.1.7/solidipes/loaders/binary.py` & `solidipes-0.1.8/solidipes/loaders/binary.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,28 +3,20 @@
 from .. import viewers
 from .file import File
 
 
 class Binary(File):
     """File of unsupported type"""
 
-    initial_data_collection_keys = File.initial_data_collection_keys + ["metadata"]
-
-    def __init__(self, path):
-        super().__init__(path)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
         self.add("metadata")
         self.default_viewer = viewers.Binary
 
-    def _load_data(self, key):
-        """Put metadata in a Text data object"""
-
-        data = super()._load_data(key)
-        if data is not None:
-            return data
-
+    @File.cached_property
+    def text(self):
         text = ""
-
         if self.file_info.type is not None:
             text += f"File type: {self.file_info.type}\n"
 
         text += f"File size: {DataSize(self.file_info.size):.2a}"
         return text
```

### Comparing `solidipes-0.1.7/solidipes/loaders/data_container.py` & `solidipes-0.1.8/solidipes/loaders/data_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+from ..utils import solidipes_logging as logging
+
+logger = logging.getLogger()
+
+################################################################
+
+
 def wrap_errors(func):
     def foo(self, *args, **kwargs):
         try:
             return func(self, *args, **kwargs)
         except Exception as e:
             self.errors.append(str(e))
 
@@ -10,43 +17,40 @@
 
 ################################################################
 
 
 class DataContainer:
     """Container class for other structured data containers"""
 
-    #: List of keys that should be present in the data collection. Augment this list in subclasses if needed.
-    initial_data_collection_keys = []
+    def __init__(self, initial_data={}, name=None, unique_identifier=None, **kwargs):
+        logger.debug(f"Creating data container {type(self)}")
+        self.name = None
+        self.unique_identifier = unique_identifier
+
+        #: Dictionary of other DataContainer or arbitrary objects.
+        #: Set entry to "None" to mark as loadable.
+        self._data_collection = initial_data.copy()
+        clss = set([self.__class__])
+        while clss:
+            new_clss = set()
+            for cls in clss:
+                for key, v in cls.__dict__.items():
+                    if isinstance(v, DataContainer.loadable):
+                        if key not in self._data_collection:
+                            self.add(key)
+                for c in cls.__bases__:
+                    new_clss.add(c)
+            clss = new_clss
+
+        #: Default viewer for this file. Optionally override this in
+        #: subclasses.
+        self.default_viewer = None
 
-    def __init__(self, initial_data={}):
-        if not self._has_native_attr("name"):
-            self.name = ""
-
-        if not self._has_native_attr("unique_identifier"):
-            self.unique_identifier = ""
-
-        if self._has_native_attr("_data_collection"):
-            self._data_collection.update(initial_data)
-        else:
-            #: Dictionary of other DataContainer or arbitrary objects.
-            #: Set entry to "None" to mark as loadable.
-            self._data_collection = initial_data.copy()
-
-        for key in self.initial_data_collection_keys:
-            if key not in self._data_collection:
-                self.add(key)
-
-        if not self._has_native_attr("default_viewer"):
-            #: Default viewer for this file. Optionally override this in
-            #: subclasses.
-            self.default_viewer = None
-
-        if not self._has_native_attr("errors"):
-            #: stores the error messages during loading
-            self.errors = []
+        #: stores the error messages during loading
+        self.errors = []
 
     def _valid_loading(self):
         if self.errors:
             return False
         return True
 
     def copy(self):
@@ -84,49 +88,45 @@
 
         # Return data
         if len(self._data_collection) == 1:
             return list(self._data_collection.values())[0]
         else:
             return self._data_collection
 
-    def _load_data(self, key):
-        """Load data or build sub-data dictionary and return it
-
-        Override this method in subclasses to define how data is loaded or
-        built.
-        """
-        return None
-
     @wrap_errors
     def load_all(self):
         """Load all data"""
         # Find keys that have a None value and load them
-        for key in self._data_collection:
+        keys = [e for e in self._data_collection.keys()]
+        for key in keys:
             if self._data_collection[key] is None:
                 # Trigger loading of data
                 self.get(key)
 
     def add(self, key, data=None):
         """Add an arbitrary object to the data collection"""
         self._data_collection[key] = data
 
     def get(self, key):
         """Get a data object by key, loading it if necessary"""
+
+        logger.debug(f"get({key})")
         try:
             data = self._data_collection[key]
         except KeyError as e:
-            raise KeyError(str(e) + "\n" + f"for {type(self)}, " + f"possible keys are {self._data_collection.keys()}")
+            raise KeyError(f"{e}\nDid you register this key somehow ?")
 
         # Load data
         if data is None:
-            data = self._load_data(key)
+            data = getattr(self, key)
             if data is None:
                 raise Exception(f'Data "{key}" could not be loaded')
             self._data_collection[key] = data
 
+        logger.debug(f"got({key}) = {data}")
         return data
 
     def remove(self, key):
         """Remove a data object from the data collection"""
         del self._data_collection[key]
 
     def has(self, key):
@@ -143,14 +143,15 @@
             return False
 
     def __getattr__(self, name):
         """Get a data object by key, loading it if necessary
 
         Only works if the name is not already an attribute of this class.
         """
+
         try:
             return self.get(name)
         except KeyError:
             raise AttributeError(f"'{self.__class__.__name__}' has no attribute '{name}'")
 
     def view(self, **kwargs):
         """View the file using the default viewer"""
@@ -161,7 +162,29 @@
         return viewer
 
     def __str__(self):
         return self.__class__.__name__
 
     def __repr__(self):
         return self._data_collection.__repr__()
+
+    class loadable(property):
+        def __init__(self, func):
+            key = func.__name__
+
+            def foo(obj, *args, **kwargs):
+                logger.debug(obj)
+                if key in obj._data_collection and obj._data_collection[key] is not None:
+                    return obj._data_collection[key]
+                data = func(obj, *args, **kwargs)
+                if data is None:
+                    raise Exception(f'Data "{key}" could not be loaded')
+                obj._data_collection[key] = data
+                return data
+
+            def foo_setter(obj, value, *args, **kwargs):
+                obj._data_collection[key] = value
+
+            super().__init__(foo, foo_setter)
+
+
+################################################################
```

### Comparing `solidipes-0.1.7/solidipes/loaders/image.py` & `solidipes-0.1.8/solidipes/loaders/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,55 +15,42 @@
         return self.src
 
     def show(self):
         from io import BytesIO
 
         import cairosvg
         import matplotlib.pyplot as plt
-        from PIL import Image
 
         img_png = cairosvg.svg2png(self.src)
         img = Image.open(BytesIO(img_png))
         plt.imshow(img)
 
 
 class Image(File):
     """Image loaded with PIL"""
 
-    cached_metadata_fields = File.cached_metadata_fields.copy()
-    cached_metadata_fields.update(
-        {
-            "exif_data": "exif_data",
-        }
-    )
-    initial_data_collection_keys = File.initial_data_collection_keys + ["image", "exif_data"]
     supported_mime_types = ["image/"]
 
-    def __init__(self, path):
-        super().__init__(path)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
         self.default_viewer = viewers.Image
 
-    def _load_data(self, key):
-        """Load image data with PIL"""
-
-        data = super()._load_data(key)
-        if data is not None:
-            return data
-
-        if key == "image":
-            if self.file_info.type == "image/svg+xml":
-                return SVGWrapper(self.file_info.path)
-            else:
-                return PILImage.open(self.file_info.path)
-
-        elif key == "exif_data":
-            try:
-                return self.get_exif_data()
-            except Exception as err:
-                return str(err)
+    @File.loadable
+    def image(self):
+        if self.file_info.type == "image/svg+xml":
+            return SVGWrapper(self.file_info.path)
+        else:
+            return PILImage.open(self.file_info.path)
+
+    @File.cached_loadable
+    def exif_data(self):
+        try:
+            return self.get_exif_data()
+        except Exception as err:
+            return str(err)
 
     def get_exif_data(self):
         pil_exif = self.image._getexif()
         if pil_exif is None:
             return DataContainer()
 
         exif = {ExifTags.TAGS[k]: v for k, v in pil_exif.items() if k in ExifTags.TAGS}
```

### Comparing `solidipes-0.1.7/solidipes/loaders/image_sequence.py` & `solidipes-0.1.8/solidipes/loaders/image_sequence.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,46 +4,44 @@
 from .file import File
 from .sequence import Sequence
 
 
 class ImageSequence(Sequence, File):
     """Sequence of images loaded with PIL"""
 
-    initial_data_collection_keys = File.initial_data_collection_keys + ["image_sequence", "n_frames"]
     supported_mime_types = ["image/"]
 
-    def __init__(self, path):
-        File.__init__(self, path)
-        Sequence.__init__(self)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
         self.default_viewer = viewers.Image
 
-    def _load_data(self, key):
-        """Load image data with PIL"""
+    @File.loadable
+    def image_sequence(self):
+        return PILImage.open(self.file_info.path)
+
+    @File.loadable
+    def n_frames(self):
+        return self.image_sequence.n_frames
 
-        if key == "image_sequence":
-            return PILImage.open(self.file_info.path)
-
-        elif key == "n_frames" or key == "_element_count":
-            return self.image_sequence.n_frames
-
-        else:
-            return super()._load_data(key)
+    @property
+    def _element_count(self):
+        return self.n_frames
 
     def _load_element(self, n):
         """Load a single frame"""
 
         self.image_sequence.seek(n)
         return self.image_sequence.copy()
 
     def select_frame(self, frame):
         self.select_element(frame)
 
     @property
     def image(self):
-        # cannot be defined with self.add and _load_data because it changes
+        # cannot be defined as loadable because it changes
         return self._current_element
 
     @classmethod
     def check_file_support(cls, path):
         """In addition to File class checks, also check if the file is a sequence of images"""
 
         if not super().check_file_support(path):
```

### Comparing `solidipes-0.1.7/solidipes/loaders/mime_types.py` & `solidipes-0.1.8/solidipes/loaders/mime_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import os
 
 import filetype
 
 from ..utils import get_mimes
+from ..utils import solidipes_logging as logging
+
+logger = logging.getLogger()
 
 _mime_types = """
+application/notebook                            ipynb
 application/x-matlab-data                       mat
 application/paraview                                pvd
 application/vtk                                     vtk vtp vts vtu
 application/1d-interleaved-parityfec
 application/3gpdash-qoe-report+xml
 application/3gpp-ims+xml
 application/3gppHal+json
@@ -1528,15 +1532,16 @@
 application/x-freemind				mm
 application/x-ganttproject			gan
 application/x-gnumeric				gnumeric
 application/x-go-sgf				sgf
 application/x-graphing-calculator		gcf
 application/x-gtar				gtar
 application/x-gtar-compressed			tgz taz
-application/x-hdf				hdf
+application/x-hdf				hdf h5 hdf5
+application/x-hdf5				h5 hdf5
 application/x-hwp				hwp
 application/x-ica				ica
 application/x-info				info
 application/x-internet-signup			ins isp
 application/x-iphone				iii
 application/x-iso9660-image			iso
 application/x-java-jnlp-file			jnlp
@@ -1604,14 +1609,15 @@
 application/xcon-conference-info+xml
 application/xcon-conference-info-diff+xml
 application/xenc+xml
 application/xfdf				xfdf
 application/xhtml+xml				xhtml xhtm xht
 application/xliff+xml				xlf
 application/xml					xml
+application/xdmf                                xdmf
 application/xml-dtd				dtd mod
 application/xml-external-parsed-entity		ent
 application/xml-patch+xml
 application/xmpp+xml
 application/xop+xml				xop
 application/xslt+xml				xsl xslt
 application/xspf+xml				xspf
```

### Comparing `solidipes-0.1.7/solidipes/loaders/parse_inp.py` & `solidipes-0.1.8/solidipes/loaders/parse_inp.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/loaders/pyvista_mesh.py` & `solidipes-0.1.8/solidipes/loaders/pyvista_mesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,53 +47,44 @@
 
     return wrapper
 
 
 class PyvistaMesh(File):
     """Mesh file loaded with pyvista"""
 
-    initial_data_collection_keys = File.initial_data_collection_keys + ["mesh"]
     supported_extensions = ["msh", "stl", "vtu", "pvtu", "vtk"]
 
-    def __init__(self, path):
-        super().__init__(path)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
         #: Fully loaded pyvista mesh
-        self.pyvista_mesh = None
         self.default_viewer = viewers.PyvistaPlotter
 
     def copy_pyvista_data_to_collection(self):
         """Add pyvista data to data collection"""
-        self.add("mesh", self.pyvista_mesh)
-
         for name in self.point_data_names:
             self.add(name + POINT_DATA_SUFFIX, self.get_point_data(name))
 
         for name in self.cell_data_names:
             self.add(name + CELL_DATA_SUFFIX, self.get_cell_data(name))
 
     @property
     def data_info(self):
         """Trigger loading of Pyvista mesh and return info"""
         self.load_all()
         return super().data_info
 
-    def _load_data(self, key):
-        data = super()._load_data(key)
-        if data is not None:
-            return data
+    @File.loadable
+    def pyvista_mesh(self):
+        return pv.read(self.file_info.path)
 
-        self.pyvista_mesh = pv.read(self.file_info.path)
+    @File.loadable
+    def mesh(self):
         self.copy_pyvista_data_to_collection()
         return self.pyvista_mesh
 
-    def load_all(self):
-        """Cannot rely on default implementation of load_all because data
-        dictionary changes size"""
-        self.get("mesh")
-
     @property
     def point_data_names(self):
         return self.pyvista_mesh.point_data.keys()
 
     @property
     def cell_data_names(self):
         return self.pyvista_mesh.cell_data.keys()
```

### Comparing `solidipes-0.1.7/solidipes/loaders/sequence.py` & `solidipes-0.1.8/solidipes/loaders/sequence.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from ..utils import solidipes_logging as logging
 from .data_container import DataContainer
 
+logger = logging.getLogger()
+
 
 class Sequence(DataContainer):
     """Sequence of any subclass of DataContainer"""
 
-    def __init__(self):
-        DataContainer.__init__(self)
-        self.add("_elements", {})
-        self.add("_selected_element", 0)
-        self.add("_element_count")
+    def __init__(self, _selected_element=0, **kwargs):
+        self._elements = {}
+        self._selected_element = _selected_element
+        super().__init__(**kwargs)
 
     @property
     def _current_element(self):
         element = self._elements.get(self._selected_element, None)
 
         # Load element if not already loaded
         if element is None:
@@ -35,13 +37,14 @@
 
         Override this method in subclasses.
         """
 
         raise NotImplementedError
 
     def __getattr__(self, key):
+        logger.debug(f"__getattr__({type(self)}, {key})")
         try:
             return self.get(key)
         except KeyError:
             pass
 
         return getattr(self._current_element, key)
```

### Comparing `solidipes-0.1.7/solidipes/loaders/table.py` & `solidipes-0.1.8/solidipes/loaders/table.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 import pandas as pd
 
 from .. import viewers
-from .data_container import wrap_errors
 from .file import File
 
 
 class Table(File):
     """Table file loaded with Pandas"""
 
-    initial_data_collection_keys = File.initial_data_collection_keys + ["header", "table"]
     supported_mime_types = ["text/csv", "application/vnd.ms-excel"]
     supported_extensions = ["csv", "xlsx"]
 
-    def __init__(self, path):
-        super().__init__(path)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+        path = kwargs["path"]
 
         # find loader matching file extension
         if self.file_info.type == "text/csv":
-            self.pandas_loader = pd.read_csv
+            self.pandas_loader = self.read_csv
         elif self.file_info.type == "application/vnd.ms-excel" or self.file_info.extension in ["xlsx"]:
             self.pandas_loader = pd.read_excel
         else:
             raise RuntimeError(f"File type not supported: {path} {self.file_info.type}")
 
         self.default_viewer = viewers.Table
 
+    def read_csv(self, fname, **kwargs):
+        import csv
+
+        with open(fname) as fp:
+            sep = csv.Sniffer().sniff(fp.readline()).delimiter
+            ret = pd.read_csv(fname, sep=sep, **kwargs)
+            return ret
+
     def validate_header(self, header):
         for h in header:
             try:
                 h = float(h)
                 self.errors.append(f"Incorrect header: {header}")
                 break
             except Exception:
                 pass
             if h.startswith("Unnamed"):
                 self.errors.append(f"Incorrect header: {header}")
                 break
 
-    @wrap_errors
-    def _load_data(self, key):
-        """Load header or full table with Pandas"""
-
-        if key == "header":
-            data = self.pandas_loader(self.file_info.path, nrows=0)
-            header = list(data.columns)
-            self.validate_header(header)
-            return ", ".join(header)
-
-        if key == "table":
-            return self.pandas_loader(self.file_info.path)
-            self.validate_header(data.columns)
-
-        return super()._load_data(key)
+    @File.loadable
+    def header(self):
+        data = self.pandas_loader(self.file_info.path, nrows=0)
+        header = list(data.columns)
+        self.validate_header(header)
+        return ", ".join(header)
+
+    @File.loadable
+    def table(self):
+        return self.pandas_loader(self.file_info.path)
```

### Comparing `solidipes-0.1.7/solidipes/loaders/video.py` & `solidipes-0.1.8/solidipes/loaders/text.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 from .. import viewers
 from .file import File
 
 
-class Video(File):
-    """Video file"""
+class Text(File):
+    """Text file, potentially formatted with markdown"""
 
-    initial_data_collection_keys = File.initial_data_collection_keys + ["video"]
-    supported_mime_types = ["video/"]
+    supported_mime_types = ["text/plain"]
+    supported_extensions = ["txt"]
 
-    def __init__(self, path):
-        super().__init__(path)
-        self.default_viewer = viewers.Video
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.default_viewer = viewers.Text
 
-    def _load_data(self, key):
-        """Load image data with PIL"""
+    @File.loadable
+    def text(self):
+        text = ""
+        with open(self.file_info.path, "r") as f:
+            text = f.read()
+        return text
 
-        data = super()._load_data(key)
-        if data is not None:
-            return data
 
-        return open(self.file_info.path, "rb")
+class Markdown(Text):
+    """Markdown file"""
+
+    supported_mime_types = ["text/markdown"]
+    supported_extensions = ["md"]
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.default_viewer = viewers.MarkdownViewer
```

### Comparing `solidipes-0.1.7/solidipes/reports/jtcam.py` & `solidipes-0.1.8/solidipes/reports/jtcam.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import base64
 import os
 
 import pyparsing as pp
 
 ################################################################
 from solidipes.loaders.text import Text
-from solidipes.reports.web_report import Report
+from solidipes.reports.web_report import WebReport, WebReportSpawner
 
 ################################################################
 
 command = "report"
 command_help = "generate report for JTCAM review from a directory"
 ################################################################
 
@@ -23,15 +23,15 @@
     _img = f'<img height="{size}" src="data:image/png;base64,{_jtcam_icon}"><br>'
     return _img
 
 
 ################################################################
 
 
-class JTCAMReport(Report):
+class JTCAMReport(WebReport):
     def __init__(self):
         super().__init__()
 
     def main(self, dir_path):
         print(f'Generating JTCAM report for "{dir_path}"')
         self.header_layout.markdown(
             "<center>" + jtcam_icon("60em") + "</center>",
@@ -174,22 +174,16 @@
     #         #         time.sleep(2)
     #         #         st.experimental_rerun()
     #         #     else:
     #         #         open(e.file_info.path, "w").write(previous_version)
     #         #         st.error("Reverted changes")
 
 
-def make(dir_path, additional_arguments="", debug=False):
-    import subprocess
-
-    if debug:
-        os.environ["FULL_SOLIDIPES_LOG"] = "true"
-
-    cmd = f"streamlit run {__file__} {' '.join(additional_arguments)}"
-    print(cmd)
-    subprocess.call(cmd, shell=True, cwd=dir_path)
+class JTCAMReportSpawner(WebReportSpawner):
+    command = "jtcam"
+    command_help = "Launch the web graphical interface for JTCAM curation"
 
 
 ################################################################
 if __name__ == "__main__":
     report = JTCAMReport()
     report.main("./")
```

### Comparing `solidipes-0.1.7/solidipes/reports/jtcam_small_logo.png` & `solidipes-0.1.8/solidipes/reports/jtcam_small_logo.png`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/reports/jupyter_logo.png` & `solidipes-0.1.8/solidipes/reports/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/reports/web_report.py` & `solidipes-0.1.8/solidipes/reports/web_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 #!/bin/env python
 ################################################################
+import argparse
 import base64
 import fnmatch
 import os
+from typing import TYPE_CHECKING
 
-import streamlit as st
-import streamlit.components.v1 as components
 from datasize import DataSize
 
-################################################################
-from streamlit_tree_select import tree_select
-
 from solidipes.loaders.file import File
 from solidipes.loaders.file_sequence import FileSequence
 from solidipes.loaders.mime_types import extension2mime_type, is_valid_extension, mime_types2extensions
 from solidipes.loaders.sequence import Sequence
-from solidipes.reports.widgets.custom_widgets import SpeechBubble
-from solidipes.reports.widgets.gitlab_issues import GitInfos, GitlabIssues
-from solidipes.reports.widgets.zenodo import ZenodoInfos, ZenodoPublish
-from solidipes.scanners.scanner import Scanner, list_files
-
-################################################################
+from solidipes.reports.report import Report
+from solidipes.scanners.scanner import Scanner, StreamlitProgressBar, list_files
 from solidipes.utils import get_git_repository, get_git_root, get_mimes, get_study_metadata, logging, set_mimes
+from solidipes.utils.git_infos import GitInfos
+
+if TYPE_CHECKING:
+    import streamlit as st
+else:
+    import lazy_loader as lazy
+
+    st = lazy.load("streamlit")
 
 print = logging.invalidPrint
 logger = logging.getLogger()
-################################################################
-
-command = "report"
-command_help = "generate report from directory"
-################################################################
 jupyter_icon_filename = os.path.join(os.path.dirname(__file__), "jupyter_logo.png")
 _jupyter_icon = base64.b64encode(open(jupyter_icon_filename, "rb").read()).decode("utf-8")
 
 
 def transform_to_subtree(h, subtree=""):
     tree = []
     for name, f in h.items():
@@ -97,67 +93,67 @@
 
         return getattr(self.f, name)
 
 
 ################################################################
 
 
-class Report(GitInfos):
+class WebReport:
     def __init__(self):
-        super().__init__()
+        self.git_infos = GitInfos()
         self.display_push_button = False
         self.file_wildcard = "*"
         self.file_error_checkbox = None
         self.scanner = Scanner()
-        st.set_page_config(layout="wide")
+        st.set_page_config(layout="wide", page_icon="https://gitlab.com/dcsm/website/-/raw/main/static/favicon.ico")
         if "currently_opened" not in st.session_state:
             st.session_state["currently_opened"] = None
 
         self.createLayouts()
 
     def createLayouts(self):
+        from solidipes.reports.widgets.gitlab_issues import GitlabIssues
+        from solidipes.reports.widgets.zenodo import ZenodoInfos, ZenodoPublish
+
         self.progress_layout = st.sidebar.empty()
 
         st.sidebar.markdown("*Powered by* **Solidipes**")
         st.sidebar.markdown(
-            (
-                '<center><img src="https://gitlab.com/dcsm/solidipes/-/raw/main/logos/solidipes.jpg" width="60%"'
-                ' style="border-radius:50%;" /><br><a style="font-size: 13px;"'
-                ' href="https://gitlab.com/dcsm/solidipes">https://gitlab.com/dcsm/solidipes</a></center>'
-            ),
+            '<center><img src="https://gitlab.com/dcsm/solidipes/-/raw/main/logos/solidipes.jpg" width="60%"'
+            ' style="border-radius:50%;" /><br><a style="font-size: 13px;"'
+            ' href="https://gitlab.com/dcsm/solidipes">https://gitlab.com/dcsm/solidipes</a></center>',
             unsafe_allow_html=True,
         )
         st.sidebar.markdown(
-            (
-                '<p style="font-size: 10px"><center><em>Software funded by</em> <img width="100px"'
-                ' src="https://ethrat.ch/wp-content/uploads/2021/12/ethr_en_rgb_black.svg"/>&nbsp;'
-                '<a style="font-size: 10px" href="https://ethrat.ch/en/">https://ethrat.ch/en/</a></center></p>'
-            ),
+            '<p style="font-size: 10px"><center><em>Software funded by</em> <img width="100px"'
+            ' src="https://ethrat.ch/wp-content/uploads/2021/12/ethr_en_rgb_black.svg"/>&nbsp;'
+            '<a style="font-size: 10px" href="https://ethrat.ch/en/">https://ethrat.ch/en/</a></center></p>',
             unsafe_allow_html=True,
         )
         st.sidebar.markdown("---")
         self.gitlab_control = st.sidebar.container()
         self.jupyter_control = st.sidebar.container()
+        self.filebrowser_control = st.sidebar.container()
         self.update_buttons = st.sidebar.container()
         self.file_selector = st.sidebar.container()
         self.path_selector = st.sidebar.container()
-        if self.git_repository is not None:
+        if self.git_infos.repository is not None:
             self.git_control = st.sidebar.container()
         self.env_layout = st.sidebar.container()
         self.options = st.sidebar.expander("Options")
 
         self.main_layout = st.container()
         self.file_layout = st.container()
         # self.modified_state = self.main_layout.empty()
         self.global_message = self.main_layout.container()
         self.header_layout = self.main_layout.container()
         self.tab_metadata, self.tab_files = self.main_layout.container(), self.main_layout.container()
         self.zenodo_publish = ZenodoPublish(self.tab_metadata, self.global_message, self.progress_layout)
         self.zenodo_infos = ZenodoInfos(self.tab_metadata)
-        if self.git_origin is not None:
+        if self.git_infos.origin is not None:
             self.gitlab_issues = GitlabIssues(self.main_layout)
         self.files_container = self.main_layout.container()
         self.logs = self.main_layout.container()
 
     def alternative_parser(self, e):
         return []
 
@@ -194,15 +190,15 @@
 
     def get_file_edit_link(self, e):
         _path = e.file_info.path
         while os.path.islink(_path):
             dirname = os.path.dirname(_path)
             _path = os.path.join(dirname, os.readlink(_path))
 
-        url = self.git_origin + "/-/edit/master/data/" + _path
+        url = self.git_infos.origin + "/-/edit/master/data/" + _path
         return url
 
     def mime_type_information(self, e, layout, main_layout):
         valid_ext = is_valid_extension(e.file_info.path, e.file_info.type)
         if not e.state.valid and not valid_ext:
             type_choice_box = layout.empty()
             type_choice = type_choice_box.container()
@@ -252,17 +248,17 @@
                     e.clear_cached_metadata(["file_info", "valid_loading"])
                     self.clear_session_state()
                     st.experimental_rerun()
         else:
             layout.info(e.file_info.type)
 
     def show_file(self, e):
-        if not e.state.valid and e.state.errors:
+        if not e.state.valid and e.errors:
             for err in e.errors:
-                st.warning(err)
+                st.error(err)
 
         def close_file():
             st.session_state["currently_opened"] = None
 
         st.sidebar.button(
             "&#8629; Back to file list",
             key=f"close_button_{e.unique_identifier}",
@@ -319,33 +315,40 @@
         try:
             _link = self._get_jupyter_link()
             _link += "/" + os.path.dirname(e.file_info.path)
             col2.markdown(
                 f"[Edit in Jupyterlab]({_link}/)",
                 unsafe_allow_html=True,
             )
+            _link = self._get_filebrowser_link()
+            _link += "/" + os.path.dirname(e.file_info.path)
+            col2.markdown(
+                f"[Edit in Filebrowser]({_link}/)",
+                unsafe_allow_html=True,
+            )
         except RuntimeError:
             pass
 
         col3.button(
             ":speech_balloon: add a comment",
             on_click=lambda: setattr(e.state, "adding_comment", True),
             key=f"add_comment_button_{e.unique_identifier}",
         )
 
         self.mime_type_information(e, col1, st.container())
+        container_error = st.container()
         with st.container():
             try:
                 with st.spinner(f"Loading {e.file_info.path}..."):
                     e.view()
             except Exception as err:
-                st.error("Error trying to display file")
-                st.exception(err)
-                logger.error("Error trying to display file")
-                logger.error(err)
+                with container_error.expander(":warning: Error trying to display file"):
+                    st.exception(err)
+                    logger.error("Error trying to display file")
+                    logger.error(err)
                 # raise err
 
     def display_file(self, e):
         if not fnmatch.fnmatch(e.file_info.path.lower(), self.file_wildcard):
             return
 
         e.state.valid = e.valid_loading
@@ -361,14 +364,16 @@
             e.state.view = True
             st.session_state["currently_opened"] = e.unique_identifier
 
         st.button(f"{title}", use_container_width=True, on_click=open_file_state)
         self.show_discussions(e)
 
     def show_discussions(self, e):
+        from solidipes.reports.widgets.custom_widgets import SpeechBubble
+
         if not e.discussions:
             return
         if not e.archived_discussions:
             st.markdown("### :speech_balloon: Discussions")
             for author, message in e.discussions:
                 SpeechBubble(author, message)
             st.markdown("<br>", unsafe_allow_html=True)
@@ -387,29 +392,32 @@
                     st.button("Archive messages", on_click=e.archive_discussions())
                 else:
                     st.button("Unarchive messages", on_click=e.archive_discussions(False))
 
                 st.markdown("---")
 
     def scan_directories(self, dir_path):
+        from streamlit_tree_select import tree_select
+
         paths_to_explore = []
         all_paths = []
         self._open_in_jupyterlab_button()
+        self._open_in_filebrowser_button()
         self._force_rescan_button()
 
         _st = self.file_selector.expander("File selection tool", expanded=True)
         self.file_wildcard = _st.text_input("File pattern", value=self.file_wildcard)
         self.file_error_checkbox = _st.checkbox("Show only files with errors")
 
         with st.spinner("Loading directories..."):
             if "scanned_files" not in st.session_state:
                 st.session_state["scanned_files"] = {}
-                h = self.scanner.scan(dir_path, scan_files=False)
+                h = self.scanner.get_dirpath_tree()
                 s_files = st.session_state["scanned_files"]
-                s_files["all_paths"] = [d[0] for d in list_files(h)]
+                s_files["all_paths"] = self.scanner.get_path_list()
                 s_files["nodes"] = transform_to_subtree(h)
             else:
                 s_files = st.session_state["scanned_files"]
             nodes = s_files["nodes"]
             all_paths = s_files["all_paths"]
             _st = self.file_selector.expander("Path selection", expanded=True)
             with _st:
@@ -422,14 +430,16 @@
                 paths_to_explore.clear()
                 for c in return_select["checked"]:
                     paths_to_explore.append(c)
 
         return all_paths, paths_to_explore
 
     def main(self, dir_path):
+        self.scanner.root_path = dir_path
+
         if "GUI_files" not in st.session_state:
             st.session_state["GUI_files"] = {}
 
         self.show_advanced = False
 
         if st.session_state["currently_opened"] is not None:
             st.markdown("<br>", unsafe_allow_html=True)
@@ -439,39 +449,39 @@
                 with st.spinner("Loading... please wait"):
                     title = self.get_file_title(f)
                     st.markdown(title)
                     self.show_file(f)
             return
 
         self.gitlab_control.markdown(
-            f"### <center> [View/Edit Gitlab repository]({self.git_origin}) </center>", unsafe_allow_html=True
+            f"### <center> [View/Edit Gitlab repository]({self.git_infos.origin}) </center>", unsafe_allow_html=True
         )
 
         self.show_advanced = self.options.checkbox("Advanced", value=False)
 
         self.zenodo_infos.show()
         if self.show_advanced:
             self.zenodo_publish.show()
         self._environment_info()
-        if self.git_repository is not None:
+        if self.git_infos.repository is not None:
             self._git_info()
 
         if self.display_push_button:
             changed_files = self.git_get_changed_files()
             if changed_files:
                 self.modified_state.button(
                     "Dataset in a modified state: Push Modifications ?",
                     on_click=self.git_push,
                     type="primary",
                     use_container_width=True,
                 )
             else:
                 self.modified_state.empty()
 
-        if self.git_origin is not None:
+        if self.git_infos.origin is not None:
             self.gitlab_issues.show()
 
         st.markdown(
             """
         <style>
         .css-18j515v {
           justify-content: left;
@@ -490,24 +500,21 @@
         all_paths, selected_paths = self.scan_directories(dir_path)
 
         if not selected_paths:
             st.markdown("#### Please select a directory on the left panel")
             return
 
         if "all_found_files" not in st.session_state:
-            with st.spinner("Scanning files..."):
-                found = self.scanner.scan_dirs([p for p in all_paths], recursive=False)
-                files = list_files(found)
-                files_dict = {}
-                for full_path, f in files:
-                    if isinstance(f, dict):
-                        continue
-                    files_dict[f.unique_identifier] = FileWrapper(f)
-                st.session_state["all_found_files"] = files
-                st.session_state["all_found_files_dict"] = files_dict
+            self.scanner.progress_bar = StreamlitProgressBar("Loading files", self.progress_layout)
+            found = self.scanner.get_filtered_loader_tree([p for p in all_paths], recursive=False)
+            files = list_files(found)
+            files_dict = self.scanner.get_filtered_loader_dict([p for p in all_paths], recursive=False)
+            files_dict = {k: FileWrapper(v) for k, v in files_dict.items()}
+            st.session_state["all_found_files"] = files
+            st.session_state["all_found_files_dict"] = files_dict
 
         all_found_files = st.session_state["all_found_files"]
 
         if not all_found_files:
             st.markdown(f"#### Nothing in the paths: {selected_paths}")
             return
 
@@ -534,35 +541,57 @@
                 col2.button("Clear", on_click=clear_log)
                 st.code("\n".join(open(log_filename).read().split("\n")[::-1]))
 
     def _get_jupyter_link(self):
         try:
             session = os.environ["SESSION_URL"]
             dir_path = os.getcwd()
-            rel_path = os.path.relpath(dir_path, self.git_root)
-            _link = f"{session}/lab/tree/{rel_path}"
+            rel_path = os.path.relpath(dir_path, self.git_infos.root)
+            if rel_path == ".":
+                _link = f"{session}/lab/"
+            else:
+                _link = f"{session}/lab/tree/{rel_path}"
+            return _link
+        except Exception:
+            raise RuntimeError("Not in a renku session")
+
+    def _get_filebrowser_link(self):
+        try:
+            session = os.environ["SESSION_URL"]
+            dir_path = os.getcwd()
+            rel_path = os.path.relpath(dir_path, self.git_infos.root)
+            _link = f"{session}/filebrowser/files/{rel_path}"
             return _link
         except Exception:
             raise RuntimeError("Not in a renku session")
 
     def _jupyter_link(self, uri, size):
         _img = f'<a href="{uri}"><img height="{size}" src="data:image/png;base64,{_jupyter_icon}"></a>'
         return _img
 
     def _write_jupyter_link(self):
         try:
             _link = self._get_jupyter_link()
-            # im_link = self._jupyter_link(_link, "50em")
             st.markdown(
                 f"### <center>[View/Edit in Jupyterlab]({_link}) </center>",
                 unsafe_allow_html=True,
             )
         except Exception as err:
             st.error("Jupyter not accessible: " + str(err))
 
+    def _write_filebrowser_link(self):
+        try:
+            _link = self._get_filebrowser_link()
+            st.markdown(
+                f"### <center>[View/Edit with file browser]({_link}) </center>",
+                unsafe_allow_html=True,
+            )
+        except Exception as err:
+            st.error("Filebrowser not accessible: " + str(err))
+
     def display_files(self, files, selected_paths):
         bar = self.progress_layout.progress(0, text="Loading files")
 
         selected_files = []
         for full_path, f in files:
             if os.path.dirname(full_path) not in selected_paths and full_path not in selected_paths:
                 continue
@@ -577,14 +606,16 @@
                 f = FileWrapper(f)
                 self.display_file(f)
             else:
                 self.display_dir(full_path, f)
         self.progress_layout.empty()
 
     def display_dir(self, d, content):
+        import streamlit.components.v1 as components
+
         found_files = False
         for k, v in content.items():
             if isinstance(v, File):
                 if fnmatch.fnmatch(v.file_info.path.lower(), self.file_wildcard):
                     found_files = True
 
         if found_files:
@@ -603,14 +634,18 @@
             if not isinstance(v, File):
                 continue
 
     def _open_in_jupyterlab_button(self):
         with self.jupyter_control:
             self._write_jupyter_link()
 
+    def _open_in_filebrowser_button(self):
+        with self.filebrowser_control:
+            self._write_filebrowser_link()
+
     def _environment_info(self):
         with self.env_layout.expander("Environment"):
             table_env = [k for k in os.environ.items()]
             st.dataframe(table_env)
 
     def _git_info(self):
         with self.git_control.container():
@@ -626,16 +661,16 @@
                         type="primary",
                         use_container_width=True,
                         on_click=self.git_revert,
                     )
 
     def git_get_changed_files(self):
         changed_files = []
-        if self.git_repository:
-            changed_files = [item.a_path for item in self.git_repository.index.diff(None)]
+        if self.git_infos.repository:
+            changed_files = [item.a_path for item in self.git_infos.repository.index.diff(None)]
         return changed_files
 
     def git_revert(self):
         repo = get_git_repository()
         ret = repo.git.reset("--hard")
         logger.info("git revert", ret)
         logger.info("git revert", type(ret))
@@ -662,19 +697,19 @@
 
         save_cwd = os.getcwd()
         try:
             os.chdir(get_git_root())
             changed_files = self.git_get_changed_files()
             # changed_files = [os.path.relpath(e, os.getcwd()) for e in changed_files]
             for e in changed_files:
-                ret = self.git_repository.git.add(e)
+                ret = self.git_infos.repository.git.add(e)
             if ret != "":
                 self.global_message.info(ret)
 
-            ret = self.git_repository.git.commit('-m "Automatic update from solidipes interface"')
+            ret = self.git_infos.repository.git.commit('-m "Automatic update from solidipes interface"')
             if ret != "":
                 self.global_message.info(ret)
 
         except git.GitCommandError as err:
             self.global_message.error(err)
             logger.info(err)
             os.chdir(save_cwd)
@@ -696,15 +731,15 @@
                 self.global_message.error(out.decode())
             if err is not None:
                 self.global_message.error(err.decode())
         else:
             self.global_message.info(out.decode())
 
         try:
-            origin = self.git_repository.remotes.origin
+            origin = self.git_infos.repository.remotes.origin
             origin.push("master")
 
         except git.GitCommandError as err:
             self.global_message.error(err)
             return
 
         self.global_message.success("Update repository complete")
@@ -718,30 +753,57 @@
             self.clear_session_state()
 
     def clear_session_state(self):
         logger.info("Clearing session state")
         keys = [k for k in st.session_state]
         for k in keys:
             del st.session_state[k]
+        from solidipes.loaders.cached_metadata import CachedMetadata
+
+        CachedMetadata.close_cached_metadata()
 
 
 ################################################################
 
 
-def make(dir_path, additional_arguments="", debug=False):
-    import subprocess
+class WebReportSpawner(Report):
+    command = "web_report"
+    command_help = "Launch the web graphical interface"
+
+    def make(self, args: argparse.Namespace):
+        import subprocess
 
-    if debug:
-        os.environ["FULL_SOLIDIPES_LOG"] = "true"
-    logger.debug(additional_arguments)
-    cmd = f"streamlit run {__file__} {' '.join(additional_arguments)}"
-    logger.warning(cmd)
-    subprocess.call(cmd, shell=True, cwd=dir_path)
+        if args.debug:
+            os.environ["FULL_SOLIDIPES_LOG"] = "true"
+        logger.debug(args.additional_arguments)
+
+        cmd = f"streamlit run {__file__} {' '.join(args.additional_arguments)}"
+        logger.warning(cmd)
+        subprocess.call(cmd, shell=True, cwd=args.dir_path)
+
+    def populate_arg_parser(self, parser: argparse.ArgumentParser):
+        parser.add_argument(
+            "dir_path",
+            nargs="?",
+            default=".",
+            help="Path to the directory to generate the report for. Defaults to current directory",
+        )
+        parser.add_argument(
+            "--debug",
+            action="store_true",
+            help="Enable debug mode",
+        )
+
+        parser.add_argument(
+            "additional_arguments",
+            nargs=argparse.REMAINDER,
+            help="Additional arguments to forward to Streamlit",
+        )
 
 
 ################################################################
 if __name__ == "__main__":
     from solidipes.utils import logging
 
     logger.info("starting web_report")
-    report = Report()
-    report.main("./")
+    web_report = WebReport()
+    web_report.main("./")
```

### Comparing `solidipes-0.1.7/solidipes/reports/widgets/custom_widgets.py` & `solidipes-0.1.8/solidipes/reports/widgets/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/reports/widgets/gitlab_issues.py` & `solidipes-0.1.8/solidipes/reports/widgets/gitlab_issues.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/bin/env python
 ################################################################
 import os
 
 import gitlab
 import streamlit as st
 
-from .git_infos import GitInfos
+from solidipes.utils.git_infos import GitInfos
 
 ################################################################
 
 
-class GitlabIssues(GitInfos):
+class GitlabIssues:
     def __init__(self, layout):
-        super().__init__()
+        self.git_infos = GitInfos()
         self.layout = layout
         self.layout_container = layout.container()
 
         if "PROJECT_NAME" not in os.environ:
-            split = self.git_origin.split("/")
+            split = self.git_infos.origin.split("/")
             project_name = split[-1]
             user_name = split[-2]
-            repo_uri = self.git_origin.split(user_name + "/" + project_name)[0]
+            repo_uri = self.git_infos.origin.split(user_name + "/" + project_name)[0]
             os.environ["REPO_URI"] = repo_uri
             os.environ["USER_NAME"] = user_name
             os.environ["PROJECT_NAME"] = project_name
         else:
             project_name = os.environ["PROJECT_NAME"]
-            repo_uri_and_user_name = self.git_origin.split("/" + project_name)[0]
+            repo_uri_and_user_name = self.git_infos.origin.split("/" + project_name)[0]
             user_name = repo_uri_and_user_name.split("/")[-1]
             repo_uri = repo_uri_and_user_name.split("/" + user_name)[0]
             os.environ["USER_NAME"] = user_name
             os.environ["REPO_URI"] = repo_uri
 
         project_name = os.environ["PROJECT_NAME"]
         repo_uri = os.environ["REPO_URI"]
```

### Comparing `solidipes-0.1.7/solidipes/reports/widgets/speech_bubble.css` & `solidipes-0.1.8/solidipes/reports/widgets/speech_bubble.css`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/reports/widgets/zenodo.py` & `solidipes-0.1.8/solidipes/reports/widgets/zenodo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/bin/env python
 ################################################################
 import streamlit as st
 import yaml
 from streamlit_editable_list import editable_list
 
 from solidipes.utils import get_study_metadata, logging, set_study_metadata
+from solidipes.utils.git_infos import GitInfos
 from solidipes.utils.metadata import lang
 from solidipes.utils.metadata import licences_data_or_software as licenses
 from solidipes.utils.zenodo_utils import get_existing_deposition_identifier
 
 from .custom_widgets import EditProgBox, EditTextBox
-from .git_infos import GitInfos
 
 ################################################################
 print = logging.invalidPrint
 logger = logging.getLogger()
 ################################################################
 
 
-class ZenodoInfos(GitInfos):
+class ZenodoInfos:
     def __init__(self, layout):
-        super().__init__()
+        self.git_infos = GitInfos()
         self.layout = layout.container()
         self.zenodo_metadata = get_study_metadata()
 
         self.key = "zenodo_infos"
 
     def _create_stateful_property(self, property_key):
         streamlit_key_template = property_key + "_{self.key}"
@@ -241,15 +241,15 @@
         rels_dicts = self.zenodo_metadata.get("related_identifiers", [])
         if len(rels_dicts) == 0:
             return
 
         formatted = "**Related Identifiers**  \n"
 
         for r in rels_dicts:
-            formatted += f"- {r['relation']} **{r['identifier']}** ({r['resource_type']})\n"
+            formatted += f"- {r['relation']} {r['identifier']} ({r['resource_type']})\n"
 
         st.markdown(formatted)
 
     def edit_related_identifiers(self):
         rels_dicts = self.zenodo_metadata.get("related_identifiers", [])
         rels_lists = [
             [
@@ -350,17 +350,14 @@
 
     def textbox(self, key, **kwargs):
         EditTextBox(self.zenodo_metadata[key], caption=key.capitalize(), key=key, **kwargs)
 
     def description_box(self, **kwargs):
         desc = self.zenodo_metadata["description"]
         with st.expander("**Description (README.md is a generated file: do not edit manually)**", expanded=True):
-            # if self.git_origin:
-            # url = self.git_origin + "/-/edit/master/DESCRIPTION.md"
-            # st.markdown(f"[Edit on Gitlab]({url})", unsafe_allow_html=True)
             EditProgBox(desc, language="markdown", key="description", on_apply=self.save_description, **kwargs)
 
     def show(self):
         with self.layout:
             # Must show editable form temporarily to save new metadata
             erasable = st.empty()
             with erasable:
```

### Comparing `solidipes-0.1.7/solidipes/scripts/download.py` & `solidipes-0.1.8/solidipes/scripts/download.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/scripts/init.py` & `solidipes-0.1.8/solidipes/scripts/init.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/scripts/main.py` & `solidipes-0.1.8/solidipes/scripts/main.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/scripts/mount.py` & `solidipes-0.1.8/solidipes/scripts/mount.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,27 @@
         remove_keys_from_info,
     )
 
     config = get_cloud_info()
 
     # --all: mount all existing mount points
     if args.all:
-        mount_all()
+        mount_all(allow_root=args.allow_root)
         return
 
     # --list-existing: show existing mount points
     if args.list_existing:
         mounts = list_mounts()
         print("Existing mount points:")
 
         for local_path, mount_info in mounts.items():
             mounted_message = " mounted" if mount_info["mounted"] else ""
             print(
-                f"    {local_path} {bcolors.OKGREEN}({mount_info['type']},"
-                f" {mount_info['system']}){mounted_message}{bcolors.ENDC}"
+                f"    {local_path} {bcolors.BRIGHT_GREEN}({mount_info['type']},"
+                f" {mount_info['system']}){mounted_message}{bcolors.RESET}"
             )
 
         return
 
     # Mount or convert, depending on provided and saved configuration
     local_path_relative_to_root = get_path_relative_to_root(args.local_path)
     mount_info_saved = config.get(local_path_relative_to_root, None)
@@ -52,34 +52,34 @@
                 convert_cloud_to_cloud(args.local_path, mount_info_saved, mount_info_provided)
 
             else:
                 if not args.force:
                     print(f'Mount info for "{args.local_path}" already exists. Use --force to replace it. Aborting...')
                     return
                 print("Mounting...")
-                mount(args.local_path, mount_info_provided)
+                mount(args.local_path, mount_info_provided, allow_root=args.allow_root)
 
         else:  # Mount info not provided
             if args.convert:
                 print(f'No mount info provided for converting "{args.local_path}". Aborting...')
                 return
 
             else:
                 add_global_mount_info(mount_info_saved)
                 print("Mounting...")
-                mount(args.local_path, mount_info_saved)
+                mount(args.local_path, mount_info_saved, allow_root=args.allow_root)
 
     else:  # Mount info not saved
         if mount_info_provided is not None:
             if args.convert:
                 convert_local_to_cloud(args.local_path, mount_info_provided)
 
             else:
                 print("Mounting...")
-                mount(args.local_path, mount_info_provided)
+                mount(args.local_path, mount_info_provided, allow_root=args.allow_root)
 
         else:  # Mount info not provided
             print("No mount info provided and no mount info saved for this directory.")
             return
 
     # Save config info if mount is successful
     if local_path_relative_to_root not in config or args.force:
@@ -188,14 +188,20 @@
         "-c",
         "--convert",
         action="store_true",
         help="Send the contents of the local directory to the cloud storage (convert it to cloud storage).",
     )
 
     parser.add_argument(
+        "--allow_root",
+        action="store_true",
+        help="Allow root to access the fuse mounting",
+    )
+
+    parser.add_argument(
         "-k",
         "--public-keys",
         action="store_true",
         help=(
             "Save all access keys publicly in local .solidipes directory. WARNING: when published, everyone will be"
             " able to see your keys and will have full access (possibly write access) to your mounted directory."
         ),
```

### Comparing `solidipes-0.1.7/solidipes/scripts/quick_view.py` & `solidipes-0.1.8/solidipes/scripts/quick_view.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 command_help = "generate a view from a file"
 
 ################################################################
 
 
 def main(args):
     """Generate a .py report for the given directory."""
+    from ..loaders.file import load_file
     from ..loaders.sequence import Sequence
-    from ..utils import load_file, viewer_backends
+    from ..utils import viewer_backends
 
     path = args.path
     _file = load_file(path)
-    print(_file)
+    print(f"Reading {path}: {_file}")
 
     if viewer_backends.current_backend == "streamlit":
         import streamlit as st
 
         st.set_page_config(layout="wide")
 
     if args.item > 0 and isinstance(_file, Sequence):
```

### Comparing `solidipes-0.1.7/solidipes/scripts/unmount.py` & `solidipes-0.1.8/solidipes/scripts/unmount.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     # --list-mounted: show mounted directories
     if args.list_mounted:
         print("Currently mounted directories:")
 
         for local_path, mount_info in mounts.items():
             if not mount_info.get("mounted"):
                 continue
-            print(f"    {local_path} {bcolors.OKGREEN}({mount_info['type']}, {mount_info['system']}){bcolors.ENDC}")
+            print(
+                f"    {local_path} {bcolors.BRIGHT_GREEN}({mount_info['type']}, {mount_info['system']}){bcolors.RESET}"
+            )
 
         return
 
     # --local-path: unmount specified directory, otherwise unmount all
     if args.local_path:
         local_path = args.local_path.rstrip(os.sep)
         if local_path not in mounts:
```

### Comparing `solidipes-0.1.7/solidipes/uploaders/renku.py` & `solidipes-0.1.8/solidipes/uploaders/renku.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,24 +76,22 @@
         repo.git.add(all=True)
         repo.index.commit("initial commit")
 
     return repo
 
 
 def init_renku(template_name):
-    subprocess.run(
-        [
-            "renku",
-            "init",
-            "--template-source",
-            RENKU_TEMPLATES_REPO,
-            "--template-id",
-            template_name,
-        ]
-    )
+    subprocess.run([
+        "renku",
+        "init",
+        "--template-source",
+        RENKU_TEMPLATES_REPO,
+        "--template-id",
+        template_name,
+    ])
 
 
 def add_remote(repo, remote_url):
     if RENKU_REMOTE_NAME in repo.remotes:
         repo.delete_remote(RENKU_REMOTE_NAME)
     repo.create_remote(RENKU_REMOTE_NAME, remote_url)
```

### Comparing `solidipes-0.1.7/solidipes/uploaders/zenodo.py` & `solidipes-0.1.8/solidipes/uploaders/zenodo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 
 from ..utils import include_metadata_description
 from ..utils import study_medatada_mandatory_fields as mandatory_fields
 from ..utils import study_medatada_removed_fields_upload as removed_fields
-from ..utils import study_metadata_filename, zenodo_infos_filename
 from ..utils.zenodo_utils import (
     ZenodoException,
     clean_deposition,
     create_deposition,
     get_access_token,
     get_existing_deposition_identifier,
     get_existing_deposition_infos,
@@ -230,45 +229,41 @@
         _print = config._print
 
     dir_path = config.root_directory
     import tempfile
     import zipfile
 
     from ..scanners.scanner import Scanner
-    from ..utils import bcolors, get_ignore, solidipes_dirname
+    from ..utils import bcolors, solidipes_dirname
 
     temp_dir = tempfile.TemporaryDirectory(dir=config.tmp_dir)
     dir_name = os.path.basename(os.path.normpath(dir_path))
     archive_name = dir_name if dir_name != "." else "archive"
     archive_path = os.path.join(temp_dir.name, f"{archive_name}.zip")
     _print(f"Creating archive {archive_path}...")
 
     scanner = Scanner()
-    scanner.excluded_patterns = get_ignore(initial_path=dir_path)
     # Remove .solidipes from excluded patterns
     if solidipes_dirname in scanner.excluded_patterns:
         scanner.excluded_patterns.remove(solidipes_dirname)
-    # Add Zenodo metadata file and Zenodo infos file to excluded patterns
-    scanner.excluded_patterns.append(os.path.join(solidipes_dirname, study_metadata_filename))
-    scanner.excluded_patterns.append(os.path.join(solidipes_dirname, zenodo_infos_filename))
 
     with zipfile.ZipFile(archive_path, "w", strict_timestamps=False) as zip_file:
         for current_dir, sub_dirs, files in os.walk(dir_path):
             # Remove excluded dirs (except .solidipes, which can be matched to ".*")
             sub_dirs[:] = [
                 d for d in sub_dirs if (not scanner.is_excluded(os.path.join(current_dir, d))) or d == solidipes_dirname
             ]
 
             if current_dir != dir_path:  # prevent addition of "."
                 zip_path = os.path.relpath(current_dir, dir_path)
                 zip_file.write(current_dir, zip_path)
 
                 # Print tree
                 depth = len(zip_path.split(os.sep))
-                _print("│   " * depth + f"{bcolors.OKBLUE}{current_dir.split(os.sep)[-1]}{bcolors.ENDC}")
+                _print("│   " * depth + f"{bcolors.BRIGHT_BLUE}{current_dir.split(os.sep)[-1]}{bcolors.RESET}")
 
             for filename in files:
                 path = os.path.join(current_dir, filename)
 
                 # Exclude files
                 if scanner.is_excluded(path):
                     continue
```

### Comparing `solidipes-0.1.7/solidipes/utils/cloud.py` & `solidipes-0.1.8/solidipes/utils/cloud.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,46 +52,46 @@
         mount_info["mount_id"] = mount_id
     else:
         mount_id = mount_info["mount_id"]
 
     return mount_id
 
 
-def mount(path, mount_info, headless=False):
+def mount(path, mount_info, **kwargs):
     if os.path.ismount(path):
         raise RuntimeError(f'"{path}" is already mounted.')
 
     mount_type = mount_info["type"]
 
     if mount_type == "s3":
         mount_system = mount_info.get("system", "juicefs")
 
         if mount_system == "juicefs":
-            mount_s3_juicefs(path, mount_info)
+            mount_s3_juicefs(path, mount_info, **kwargs)
 
         elif mount_system == "s3fs":
-            mount_s3fs(path, mount_info)
+            mount_s3fs(path, mount_info, **kwargs)
 
     elif mount_type == "ssh":
         mount_system = mount_info.get("system", "sshfs")
 
         if mount_system == "sshfs":
-            mount_sshfs(path, mount_info, headless=headless)
+            mount_sshfs(path, mount_info, **kwargs)
 
     elif mount_type == "nfs":
         mount_system = mount_info.get("system", "mount")
 
         if mount_system == "mount":
-            mount_nfs_with_mount_command(path, mount_info, headless=headless)
+            mount_nfs_with_mount_command(path, mount_info, **kwargs)
 
     elif mount_type == "smb":
         mount_system = mount_info.get("system", "mount")
 
         if mount_system == "mount":
-            mount_smb_with_mount_command(path, mount_info, headless=headless)
+            mount_smb_with_mount_command(path, mount_info, **kwargs)
 
     else:
         raise ValueError(f'Unknown cloud storage type "{mount_type}".')
 
     wait_mount(path)
 
 
@@ -155,30 +155,30 @@
     with tempfile.NamedTemporaryFile(mode="w", suffix=".passwd", delete=False) as f:
         f.write(f"{access_key_id}:{secret_access_key}\n")
         file_path = f.name
 
     return file_path
 
 
-def mount_s3_juicefs(path, mount_info=None):
+def mount_s3_juicefs(path, mount_info=None, **kwargs):
     if mount_info is None:
         mount_info = get_existing_mount_info(path)
 
     logger.debug(mount_info)
     # Create directory if it does not exist
     if not os.path.exists(path):
         os.makedirs(path)
 
     if "database_url" in mount_info:
-        mount_s3_juicefs_psql(path, mount_info)
+        mount_s3_juicefs_psql(path, mount_info, **kwargs)
     else:
-        mount_s3_juicefs_sqlite3(path, mount_info)
+        mount_s3_juicefs_sqlite3(path, mount_info, **kwargs)
 
 
-def mount_s3_juicefs_sqlite3(path, mount_info=None):
+def mount_s3_juicefs_sqlite3(path, mount_info=None, **kwargs):
     mount_id = get_mount_id(mount_info)
     database_filename = f"{mount_id}.db"
     database_path = os.path.join(get_cloud_dir_path(), database_filename)
     database_url = f"sqlite3://{database_path}"
     bucket_url = f"{mount_info['endpoint_url'].rstrip('/')}/{mount_info['bucket_name']}"
 
     os.environ["AWS_ACCESS_KEY"] = mount_info["access_key_id"]
@@ -242,84 +242,112 @@
     except Exception as e:
         message = f"Error connecting to Postgres: {e}"
         raise RuntimeError(message).with_traceback(e.__traceback__)
 
     return connection
 
 
-def mount_s3_juicefs_psql(path, mount_info=None):
+def mount_s3_juicefs_psql(path, mount_info=None, allow_root=False, **kwargs):
     # Create mount_id (if necessary), used to find database file
     mount_id = get_mount_id(mount_info)
 
-    logger.error(mount_info)
+    logger.info(mount_info)
     if mount_info is None:
         mount_info = get_existing_mount_info(path)
-    logger.error(mount_info)
+    logger.info(mount_info)
     # Create directory if it does not exist
     if not os.path.exists(path):
         os.makedirs(path)
 
     # Create mount_id (if necessary), used to find database file
     # mount_id = get_mount_id(mount_info)
     database_url = mount_info["database_url"]
     if not database_url.startswith("postgres://"):
         raise RuntimeError(f"Inconsistent database url: {database_url}")
 
-    logger.error(database_url)
+    logger.debug(database_url)
     protocol, url = database_url.split("://")
     host = url.split("/")[0]
     # database_name = url.split("/")[1].split("?")[0]
     database_name = "dcsm"
     port = 5432
-    username = mount_info["username"]
+
+    if "username" in mount_info:
+        username = mount_info["username"]
+    elif "DCSM_USERNAME" in os.environ:
+        username = os.environ["DCSM_USERNAME"]
+    else:
+        raise RuntimeError("Cannot find DCSM username")
     database_url = (
         protocol
         + "://"
         + username
         + "@"
         + url
         + "/"
         + database_name
         + f"?sslmode=disable&search_path=juicefs-{mount_id}"
     )
     logger.debug(url)
     logger.debug(host)
     logger.debug(database_name)
 
-    psql_password = mount_info["password"]
+    if "password" in mount_info:
+        psql_password = mount_info["password"]
+    elif "DCSM_PASSWORD" in os.environ:
+        psql_password = os.environ["DCSM_PASSWORD"]
+    else:
+        raise RuntimeError("Cannot find DCSM password")
 
     import argparse
 
     psql_config = argparse.Namespace(
         database=database_name, host=host, port=port, username=username, password=psql_password
     )
     conn = connect_to_postgres(psql_config)
     cursor = conn.cursor()
     from psycopg2 import sql
 
-    mount_info_query = sql.SQL("SELECT * from {username}.user_mounts where mount_id = {mount_id}").format(
-        username=sql.Identifier(username), mount_id=sql.Literal(f"juicefs-{mount_id}")
-    )
-    logger.error(mount_info_query)
-    cursor.execute(mount_info_query)
-    db_mount_info = [i for i in cursor][0]
-    logger.debug(db_mount_info)
-    _, _, access_key, secret_key = db_mount_info
-    env = os.environ
-    env.update({"META_PASSWORD": psql_password})
-    env.update({"AWS_ACCESS_KEY": access_key, "AWS_SECRET_ACCESS_KEY": secret_key})
+    if username == "admin":
+        mount_info_query = sql.SQL("SELECT * from storage where mount_id = {mount_id}").format(
+            mount_id=sql.Literal(f"juicefs-{mount_id}")
+        )
+        logger.debug(mount_info_query)
+        cursor.execute(mount_info_query)
+        db_mount_info = [i for i in cursor][0]
+        logger.debug(db_mount_info)
+        _, _, _, _, access_key, secret_key = db_mount_info
+    else:
+        mount_info_query = sql.SQL("SELECT * from {username}.user_mounts where mount_id = {mount_id}").format(
+            username=sql.Identifier(username), mount_id=sql.Literal(f"juicefs-{mount_id}")
+        )
+        logger.debug(mount_info_query)
+        cursor.execute(mount_info_query)
+        db_mount_info = [i for i in cursor][0]
+        logger.debug(db_mount_info)
+        _, _, access_key, secret_key = db_mount_info
+
+    env = {"META_PASSWORD": psql_password, "AWS_ACCESS_KEY": access_key, "AWS_SECRET_ACCESS_KEY": secret_key}
+    logger.error(env)
+    env.update(os.environ)
 
-    cmd = [
-        "juicefs",
-        "mount",
-        "--background",
+    cmd = ["juicefs", "mount", "--background"]
+
+    if allow_root:
+        cmd += [
+            "-o",
+            "allow_root",
+        ]
+
+    cmd += [
         database_url,
         path,
     ]
-    logger.error(cmd)
+
+    logger.debug(cmd)
     # Mount S3 bucket
     mount_process = subprocess.run(
         cmd,
         env=env,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         timeout=cloud_connection_timeout,
@@ -559,28 +587,29 @@
         if only_mounted and not mount_info["mounted"]:
             continue
         mounts[local_path_relative_to_workdir] = mount_info
 
     return mounts
 
 
-def mount_all(headless=False):
+def mount_all(headless=False, allow_root=False):
     """Mount all mounts that are not already mounted"""
 
     mounts = list_mounts()
     for local_path, mount_info in mounts.items():
         if mount_info["mounted"]:
             continue
 
         logger.info(f"Mounting {local_path}...")
         try:
             add_global_mount_info(mount_info)
-            mount(local_path, mount_info, headless=headless)
+            mount(local_path, mount_info, headless=headless, allow_root=allow_root)
         except Exception as e:
-            logger.error(f"{e}")
+            logger.error(f"Abort after raising {type(e)} {e}")
+            raise e
 
     logger.info("Mount All: Done!")
 
 
 def unmount_all(headless=False):
     """Unmount all mounted mounts"""
```

### Comparing `solidipes-0.1.7/solidipes/utils/languages-iso-639-2.csv` & `solidipes-0.1.8/solidipes/utils/languages-iso-639-2.csv`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/utils/licenses.csv` & `solidipes-0.1.8/solidipes/utils/licenses.csv`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/utils/metadata.py` & `solidipes-0.1.8/solidipes/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/utils/utils.py` & `solidipes-0.1.8/solidipes/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,33 @@
-import os
+from functools import cache
 
 from .config import solidipes_dirname
 
 
 class bcolors:
-    HEADER = "\033[95m"
-    OKBLUE = "\033[94m"
-    OKCYAN = "\033[96m"
-    OKGREEN = "\033[92m"
-    WARNING = "\033[93m"
-    FAIL = "\033[91m"
-    ENDC = "\033[0m"
+    RESET = "\033[0m"
     BOLD = "\033[1m"
     UNDERLINE = "\033[4m"
-
-
-def load_file(path):
-    """Load a file from path into the appropriate object type"""
-
-    import os
-
-    from ..loaders.binary import Binary
-    from ..loaders.code_snippet import CodeSnippet
-    from ..loaders.geof_mesh import GeofMesh
-    from ..loaders.hdf5 import HDF5
-    from ..loaders.image import Image
-    from ..loaders.image_sequence import ImageSequence
-    from ..loaders.matlab import MatlabData
-    from ..loaders.pdf import PDF
-    from ..loaders.pyvista_mesh import PyvistaMesh
-    from ..loaders.symlink import SymLink
-    from ..loaders.table import Table
-    from ..loaders.text import Markdown, Text
-    from ..loaders.video import Video
-
-    # Note: the first matching type is used
-    loader_list = [
-        Table,
-        PyvistaMesh,
-        ImageSequence,
-        Image,
-        Markdown,
-        Text,
-        CodeSnippet,
-        GeofMesh,
-        Video,
-        PDF,
-        MatlabData,
-        HDF5,
-    ]
-
-    if os.path.islink(path):
-        return SymLink(path)
-
-    if not os.path.isfile(path):
-        raise FileNotFoundError(f'File "{path}" does not exist')
-
-    for loader in loader_list:
-        if loader.check_file_support(path):
-            return loader(path)
-
-    # if no extension or unknown extension, assume binary
-    file = Binary(path)
-
-    return file
+    BLINK = "\033[5m"
+    BLACK = "\033[30m"
+    RED = "\033[31m"
+    GREEN = "\033[32m"
+    YELLOW = "\033[33m"
+    BLUE = "\033[34m"
+    MAGENTA = "\033[35m"
+    CYAN = "\033[36m"
+    WHITE = "\033[37m"  # light gray
+    BRIGHT_BLACK = "\033[90m"  # dark gray
+    BRIGHT_RED = "\033[91m"
+    BRIGHT_GREEN = "\033[92m"
+    BRIGHT_YELLOW = "\033[93m"
+    BRIGHT_BLUE = "\033[94m"
+    BRIGHT_MAGENTA = "\033[95m"
+    BRIGHT_CYAN = "\033[96m"
+    BRIGHT_WHITE = "\033[97m"
 
 
 def find_config_directory(initial_path="", dir_name=solidipes_dirname):
     """Find a directory in the current path or any of its parents"""
 
     import os
 
@@ -125,23 +85,27 @@
 
     return os.path.dirname(get_solidipes_directory(initial_path))
 
 
 def get_path_relative_to_root(path):
     """Express path relative to study root"""
 
+    import os
+
     path = os.path.abspath(path)  # Also strips trailing slash
     path = os.path.relpath(path, get_study_root_path())
 
     return path
 
 
 def get_path_relative_to_workdir(path):
     """Convert path expressed relative to study root to path expressed relative to current working directory"""
 
+    import os
+
     path = os.path.join(get_study_root_path(), path)
     path = os.path.relpath(path, os.getcwd())
 
     return path
 
 
 def init_git_repository(initial_path=""):
@@ -167,14 +131,22 @@
     git_root = repo.git.rev_parse("--show-toplevel")
     return git_root
 
 
 def get_config_path(filename_var, initial_path="", check_existence=False, user=False):
     import os
 
+    current_working_dir = os.getcwd()
+    return _get_config_path(current_working_dir, filename_var, initial_path, check_existence, user)
+
+
+@cache
+def _get_config_path(current_working_dir, filename_var, initial_path="", check_existence=False, user=False):
+    import os
+
     from . import config
 
     filename = getattr(config, filename_var)
 
     if user:
         config_directory = get_user_solidipes_directory()
     else:
@@ -205,40 +177,48 @@
     with open(filename, "w") as f:
         f.write(yaml.safe_dump(config))
 
     return config
 
 
 def get_study_log_path():
+    import os
+
     config_directory = get_solidipes_directory()
     path = os.path.join(config_directory, "solidipes.logs")
     return path
 
 
 def get_study_metadata_path(*args, **kwargs):
     return get_config_path("study_metadata_filename", *args, **kwargs)
 
 
 def get_readme_path(*args, **kwargs):
+    import os
+
     from .config import readme_filename
 
     return os.path.join(get_study_root_path(*args, **kwargs), readme_filename)
 
 
 def get_study_description_path(*args, **kwargs):
+    import os
+
     from .config import study_description_filename
 
     return os.path.join(get_study_root_path(*args, **kwargs), study_description_filename)
 
 
 def get_mimes_path(*args, **kwargs):
     return get_config_path("mimes_filename", *args, **kwargs)
 
 
 def get_config(filename_var, *args, **kwargs):
+    import os
+
     path = get_config_path(filename_var, *args, **kwargs)
     if not os.path.exists(path):
         return {}
     return load_yaml(path)
 
 
 def set_config(filename_var, config, *args, **kwargs):
@@ -397,86 +377,77 @@
         return {}
 
 
 def set_mimes(config, *args, **kwargs):
     set_config("mimes_filename", config, *args, **kwargs)
 
 
-def get_ignore(*args, **kwargs):
+def get_ignore(*args, **kwargs) -> set[str]:
     from .config import default_ignore_patterns
 
-    ignore = get_config("ignore_filename", *args, **kwargs)
-    if not ignore:
-        ignore = default_ignore_patterns
+    ignore: set[str] = set(get_config("ignore_filename", *args, **kwargs))
+    ignore = ignore.union(default_ignore_patterns)
 
     return ignore
 
 
-def set_ignore(config, *args, **kwargs):
-    set_config("ignore_filename", config, *args, **kwargs)
+def set_ignore(config: set[str], *args, **kwargs):
+    set_config("ignore_filename", list(config), *args, **kwargs)
 
 
 def get_cloud_info(*args, **kwargs):
     return get_config("cloud_info_filename", *args, **kwargs)
 
 
 def set_cloud_info(config, *args, **kwargs):
     set_config("cloud_info_filename", config, *args, **kwargs)
 
 
 def get_cloud_dir_path(*args, **kwargs):
+    import os
+
     cloud_dir_path = get_config_path("cloud_dir_name", *args, **kwargs)
 
     if not os.path.isdir(cloud_dir_path):
         os.makedirs(cloud_dir_path)
 
     return cloud_dir_path
 
 
-def transform_dict_to_data_containers(data):
-    from ..loaders.data_container import DataContainer
-
-    if isinstance(data, dict):
-        data_res = {}
-        for k, v in data.items():
-            data_res[k] = transform_dict_to_data_containers(v)
-        return DataContainer(data_res)
-
-    return data
-
-
-def get_cache_ctime(initial_path="."):
-    try:
-        path = get_config_path("cached_metadata_filename", initial_path=initial_path)
-        stats = os.stat(path)
-        return stats.st_mtime
-    except FileNotFoundError:
-        return 0
-
+def dict_to_pretty_str(d: dict, indent=0, indent_size=4):
+    string = ""
+    indent_string = " " * indent_size
+
+    for key, value in d.items():
+        string += indent_string * indent + str(key) + ": "
+        if isinstance(value, dict):
+            string += "{\n" + dict_to_pretty_str(value, indent + 1) + indent_string * indent + "}\n"
+        else:
+            string += str(value) + "\n"
 
-def get_cached_metadata(initial_path="."):
-    # Find cached metadata from closest .solidipes directory
-    metadata_all_files = get_config("cached_metadata_filename", initial_path=initial_path)
-    for file_path in metadata_all_files:
-        m = metadata_all_files[file_path]
-        for k in m:
-            m[k] = transform_dict_to_data_containers(m[k])
-    return metadata_all_files
+    return string
 
 
 def transform_data_containers_to_dict(data):
     from ..loaders.data_container import DataContainer
 
     if isinstance(data, DataContainer):
         data = data._data_collection
     if isinstance(data, dict):
         data_res = {}
         for k, v in data.items():
             data_res[k] = transform_data_containers_to_dict(v)
         data = data_res
-    # logger.info('transform_data_containers_to_dict:', type(data), data)
+
     return data
 
 
-def set_cached_metadata(config, initial_path="."):
-    # Set cached metadata in closest .solidipes directory
-    set_config("cached_metadata_filename", transform_data_containers_to_dict(config), initial_path=initial_path)
+def transform_dict_to_data_containers(data):
+    from ..loaders.data_container import DataContainer
+
+    if isinstance(data, dict):
+        data_res = {}
+        for k, v in data.items():
+            data_res[k] = transform_dict_to_data_containers(v)
+        return DataContainer(data_res)
+
+    return data
```

### Comparing `solidipes-0.1.7/solidipes/utils/viewer_backends.py` & `solidipes-0.1.8/solidipes/utils/viewer_backends.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/utils/zenodo_utils.py` & `solidipes-0.1.8/solidipes/utils/zenodo_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     data = response.json()
 
     if "message" in data:
         error_message += f" {data['message']}"
 
     if "errors" in data:
         for sub_data in data["errors"]:
-            error_message += f"\n- {sub_data['field']}: {sub_data['message']}"
+            error_message += f"\n- {sub_data['field']}: {sub_data['messages']}"
 
     raise ZenodoException(error_message)
 
 
 # Upload methods ##############################################################
```

### Comparing `solidipes-0.1.7/solidipes/viewers/binary.py` & `solidipes-0.1.8/solidipes/viewers/binary.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 logger = logging.getLogger()
 
 
 class Binary(Viewer):
     """Viewer for (unknown) binary"""
 
     def __init__(self, data=None):
-        self.compatible_data_types = [loaders.Binary, str]
+        self.compatible_data_types = [loaders.Binary]
         self.data = []
         super().__init__(data)
 
     def add(self, data_container):
         """Append text to the viewer"""
         self.check_data_compatibility(data_container)
```

### Comparing `solidipes-0.1.7/solidipes/viewers/code_snippet.py` & `solidipes-0.1.8/solidipes/viewers/code_snippet.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,16 +25,39 @@
 class Code(Text):
     def __init__(self, data=None):
         if data is not None:
             self.path = data.file_info.path
         super().__init__(data)
         self.compatible_data_types = [loaders.CodeSnippet, str]
 
+    def add(self, data_container):
+        """Append code to the viewer"""
+
+        super().add(data_container)
+        self.lint = data_container.lint
+
     def show(self):
         if viewer_backends.current_backend == "jupyter notebook":
             display(self.text)
+            print("pylint")
+            for m in self.lint:
+                print(m)
 
         elif viewer_backends.current_backend == "streamlit":
-            st.code(self.text, language=guess_language(self.path))
+            if len(self.text) > 2000:
+                self.text = self.text[:50000] + "\n... more truncated content ..."
+            st.code(self.text, language=guess_language(self.path), line_numbers=True)
+            with st.expander("Linting feedback"):
+                st.markdown("### Errors")
+                for m in self.lint:
+                    if m[0][0] in ["E", "F"]:
+                        st.text(m[1])
+                st.markdown("### Warnings")
+                for m in self.lint:
+                    if m[0][0] not in ["E", "F"]:
+                        st.text(m[1])
 
         else:  # pure python
             print(self.text)
+            print("pylint")
+            for m in self.lint:
+                print(m)
```

### Comparing `solidipes-0.1.7/solidipes/viewers/hdf5.py` & `solidipes-0.1.8/solidipes/viewers/hdf5.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def add(self, data_container):
         """Replace the viewer's hdf5"""
         self.check_data_compatibility(data_container)
         self.datasets = data_container.datasets
 
     def show(self):
         if viewer_backends.current_backend == "jupyter notebook":
-            display(self.image)
+            display(self.datasets)
 
         elif viewer_backends.current_backend == "streamlit":
             col1, col2 = st.columns(2)
             nodes, labels = scan_hdf5_recursively(self.datasets)
             nodes = [nodes]
             # st.write(nodes)
             with col1:
@@ -67,13 +67,22 @@
                         pass
                     if len(d.shape) == 2 and d.shape[0] > 30 and d.shape[1] > 30:
                         div = [d.shape[i] // 2000 for i in range(len(d.shape))]
                         fig, ax = plt.subplots()
                         filtered = d[:: div[0], :: div[1]]
                         ax.imshow(filtered)
                         st.pyplot(fig)
+                    elif len(d.shape) == 1:
+                        div = d.shape[0] // 2000
+                        if div == 0:
+                            div = 1
+                        fig, ax = plt.subplots()
+                        filtered = d[::div]
+                        ax.plot(filtered, "-o")
+                        ax.set_xlabel("index")
+                        st.pyplot(fig)
                     else:
                         slices = [slice(0, min(20, d.shape[i]), 1) for i in range(len(d.shape))]
                         st.dataframe(d.__getitem__(*slices))
 
         else:  # python
-            self.image.show()
+            print(self.datasets)
```

### Comparing `solidipes-0.1.7/solidipes/viewers/image.py` & `solidipes-0.1.8/solidipes/viewers/image.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from .viewer import Viewer
 
 
 class Image(Viewer):
     """Viewer for images"""
 
     def __init__(self, data=None):
-        self.compatible_data_types = [loaders.Image]
         #: Image to display
         self.image = None
         super().__init__(data)
+        self.compatible_data_types = [loaders.Image]
 
     def add(self, data_container):
         """Replace the viewer's image"""
         self.check_data_compatibility(data_container)
         self.image = data_container.image
 
     def svg_format(self, svg):
```

### Comparing `solidipes-0.1.7/solidipes/viewers/matlab.py` & `solidipes-0.1.8/solidipes/viewers/matlab.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/viewers/pdf.py` & `solidipes-0.1.8/solidipes/viewers/pdf.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/viewers/pyvista_plotter.py` & `solidipes-0.1.8/solidipes/viewers/pyvista_plotter.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,19 @@
 
         Args:
             **kwargs: keyword arguments passed to the pyvista.Plotter.add_mesh
                 method
         """
         self.check_data_compatibility(data_container)
 
-        if isinstance(data_container, loaders.DataContainer):
+        if isinstance(data_container, loaders.Abaqus):
+            for name, m in data_container.meshes.items():
+                self.meshes.append((m, kwargs))
+
+        elif isinstance(data_container, loaders.DataContainer):
             self.add_mesh(data_container, **kwargs)
 
     def add_mesh(self, data_container, **kwargs):
         """Add mesh to the viewer
 
         Args:
             **kwargs: keyword arguments passed to the pyvista.Plotter.add_mesh
```

### Comparing `solidipes-0.1.7/solidipes/viewers/symlink.py` & `solidipes-0.1.8/solidipes/viewers/symlink.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/viewers/table.py` & `solidipes-0.1.8/solidipes/viewers/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,20 @@
         if self.data_container is None:
             raise Exception("No data to show")
 
         if viewer_backends.current_backend == "jupyter notebook":
             display(self.data_container.table)
 
         elif viewer_backends.current_backend == "streamlit":
-            tab_figure, tab_raw = st.tabs(["Figure", "Raw Data"])
-            with tab_figure:
-                self.show_plot()
-            with tab_raw:
-                st.dataframe(self.data_container.table)
+            if self.data_container.table.shape[1] < 20:
+                tab_figure, tab_raw = st.tabs(["Figure", "Raw Data"])
+                with tab_figure:
+                    self.show_plot()
+                with tab_raw:
+                    st.dataframe(self.data_container.table)
+            else:
+                st.dataframe(self.data_container.table.iloc[:20])
+                if self.data_container.table.shape[0] > 20:
+                    st.write("Truncated the long file...")
 
         else:  # python
             print(self.data_container.table)
```

### Comparing `solidipes-0.1.7/solidipes/viewers/text.py` & `solidipes-0.1.8/solidipes/viewers/text.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/viewers/video.py` & `solidipes-0.1.8/solidipes/viewers/video.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/solidipes/viewers/viewer.py` & `solidipes-0.1.8/solidipes/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.7/PKG-INFO` & `solidipes-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 Metadata-Version: 2.1
 Name: solidipes
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package for the DCSM project
 Home-page: https://gitlab.com/groups/dcsm
 License: GPL-3.0-or-later
 Author: Guillaume Anciaux
 Author-email: guillaume.anciaux@epfl.ch
 Requires-Python: >=3.9.12,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argcomplete (>=3.0.5,<4.0.0)
+Requires-Dist: btrees (>=5.2,<6.0)
 Requires-Dist: cairosvg (>=2.7.0,<3.0.0)
 Requires-Dist: datasize (>=1.0.0,<2.0.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: ipydatawidgets (==4.3.2)
+Requires-Dist: lazy-loader (>=0.4,<0.5)
 Requires-Dist: markdown (>=3.4.3,<4.0.0)
 Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Requires-Dist: matplotlib (>=3.7.1)
+Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: meshio[all] (>=5.3.4,<6.0.0)
+Requires-Dist: nbformat (>=5.10.4,<6.0.0)
 Requires-Dist: openpyxl (>=3.1.1,<4.0.0)
 Requires-Dist: pandas (>=1.5.3)
+Requires-Dist: panel (==1.3.0)
 Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
+Requires-Dist: pylint (>=3.1.0,<4.0.0)
 Requires-Dist: python-gitlab (>=3.14.0,<4.0.0)
 Requires-Dist: pyvista (>=0.38.1,<0.39.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (==2.29.0)
-Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scipy (>=1.10.1)
 Requires-Dist: stpyvista (>=0.0.8,<0.0.9)
 Requires-Dist: streamlit (>=1.17.0,<2.0.0)
 Requires-Dist: streamlit-ace (>=0.1.1,<0.2.0)
 Requires-Dist: streamlit-editable-list (==0.0.5)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-option-menu (>=0.3.2,<0.4.0)
 Requires-Dist: streamlit-quill (>=0.0.3,<0.0.4)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Requires-Dist: sympy (>=1.11.1)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: traitlets (==5.2.0)
 Requires-Dist: trame (>=2.2.6,<3.0.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Requires-Dist: zodb (>=6.0,<7.0)
 Project-URL: Documentation, https://solidipes.readthedocs.io/en/latest/
 Project-URL: Repository, https://gitlab.com/dcsm/solidipes
 Description-Content-Type: text/markdown
 
 
 
 # Solidipes
```

