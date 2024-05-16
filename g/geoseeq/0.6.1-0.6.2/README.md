# Comparing `tmp/geoseeq-0.6.1.tar.gz` & `tmp/geoseeq-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoseeq-0.6.1.tar", last modified: Sat May  4 21:12:30 2024, max compression
+gzip compressed data, was "geoseeq-0.6.2.tar", last modified: Thu May 16 15:40:35 2024, max compression
```

## Comparing `geoseeq-0.6.1.tar` & `geoseeq-0.6.2.tar`

### file list

```diff
@@ -1,112 +1,116 @@
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1067 2023-03-22 01:07:34.000000 geoseeq-0.6.1/LICENSE
--rw-r--r--   0 dcdanko   (1000) dcdanko   (1000)     4803 2024-05-04 21:12:30.685011 geoseeq-0.6.1/PKG-INFO
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4254 2024-04-15 16:42:26.000000 geoseeq-0.6.1/README.md
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      946 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/__init__.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2387 2023-08-13 06:22:51.000000 geoseeq-0.6.1/geoseeq/app.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      188 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/blob_constructors.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2115 2023-06-14 19:17:52.000000 geoseeq-0.6.1/geoseeq/bulk_creators.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq/cli/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       24 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/cli/__init__.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      176 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/cli/constants.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2275 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/copy.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4132 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/detail.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    17766 2024-04-24 00:22:47.000000 geoseeq-0.6.1/geoseeq/cli/download.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3083 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/cli/fastq_utils.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      997 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/get_eula.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3791 2024-05-04 21:12:08.000000 geoseeq-0.6.1/geoseeq/cli/main.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     5929 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/manage.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      738 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/progress_bar.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3030 2024-04-24 14:28:45.000000 geoseeq-0.6.1/geoseeq/cli/project.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1884 2023-08-15 00:17:43.000000 geoseeq-0.6.1/geoseeq/cli/raw.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3838 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/run.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1015 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/search.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq/cli/shared_params/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      325 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/shared_params/__init__.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4095 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/shared_params/common_state.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1072 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/shared_params/config.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     9299 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/shared_params/id_handlers.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2741 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/shared_params/obj_getters.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2083 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/shared_params/opts_and_args.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq/cli/upload/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      627 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/upload/__init__.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    10081 2024-05-04 19:25:40.000000 geoseeq-0.6.1/geoseeq/cli/upload/upload.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3434 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/upload/upload_advanced.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    10706 2024-05-04 18:41:04.000000 geoseeq-0.6.1/geoseeq/cli/upload/upload_reads.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      925 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/cli/user.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2873 2023-08-12 19:50:20.000000 geoseeq-0.6.1/geoseeq/cli/utils.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     6783 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/cli/view.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      431 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/constants.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq/contrib/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/contrib/__init__.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq/contrib/ncbi/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/contrib/ncbi/__init__.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1056 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/contrib/ncbi/api.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4341 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/contrib/ncbi/bioproject.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2400 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/contrib/ncbi/cli.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      175 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/contrib/ncbi/setup_logging.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4138 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/file_system_cache.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq/id_constructors/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      126 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/id_constructors/__init__.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     5702 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/id_constructors/from_blobs.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3151 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/id_constructors/from_ids.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4174 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/id_constructors/from_names.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3305 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/id_constructors/from_uuids.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2676 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/id_constructors/resolvers.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      723 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/id_constructors/utils.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     7965 2024-04-15 16:42:46.000000 geoseeq-0.6.1/geoseeq/knex.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2462 2023-06-14 19:17:52.000000 geoseeq-0.6.1/geoseeq/organization.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     9873 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/pipeline.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq/plotting/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      154 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/plotting/__init__.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      285 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/plotting/constants.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4096 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/plotting/highcharts.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq/plotting/map/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      295 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/plotting/map/__init__.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4329 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/plotting/map/base_layer.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3907 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/plotting/map/map.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1795 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/plotting/map/overlay.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2554 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/plotting/selectable.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    13741 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/project.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     7131 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/remote_object.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq/result/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      356 2023-08-12 19:50:20.000000 geoseeq-0.6.1/geoseeq/result/__init__.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1782 2023-08-12 19:50:20.000000 geoseeq-0.6.1/geoseeq/result/bioinfo.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1758 2024-05-03 02:52:42.000000 geoseeq-0.6.1/geoseeq/result/file_chunker.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     7805 2024-05-04 21:09:29.000000 geoseeq-0.6.1/geoseeq/result/file_download.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    10648 2024-05-04 19:34:06.000000 geoseeq-0.6.1/geoseeq/result/file_upload.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     8677 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/result/result_file.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    11122 2024-05-04 19:22:58.000000 geoseeq-0.6.1/geoseeq/result/result_folder.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3667 2024-05-04 21:10:12.000000 geoseeq-0.6.1/geoseeq/result/resumable_download_tracker.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3811 2024-05-04 19:09:33.000000 geoseeq-0.6.1/geoseeq/result/resumable_upload_tracker.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2772 2023-08-13 00:32:52.000000 geoseeq-0.6.1/geoseeq/result/utils.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     7981 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/sample.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3388 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/search.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     8757 2024-05-04 20:42:40.000000 geoseeq-0.6.1/geoseeq/upload_download_manager.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      690 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/user.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3577 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/utils.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq/vc/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/vc/__init__.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      710 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/vc/checksum.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2803 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/vc/cli.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2486 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/vc/clone.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       19 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/vc/constants.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      730 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/vc/vc_cache.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      457 2023-03-22 01:07:34.000000 geoseeq-0.6.1/geoseeq/vc/vc_dir.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3850 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/vc/vc_sample.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3110 2024-04-15 16:42:26.000000 geoseeq-0.6.1/geoseeq/vc/vc_stub.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     8071 2023-06-14 19:17:52.000000 geoseeq-0.6.1/geoseeq/work_orders.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/geoseeq.egg-info/
--rw-r--r--   0 dcdanko   (1000) dcdanko   (1000)     4803 2024-05-04 21:12:30.000000 geoseeq-0.6.1/geoseeq.egg-info/PKG-INFO
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2602 2024-05-04 21:12:30.000000 geoseeq-0.6.1/geoseeq.egg-info/SOURCES.txt
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        1 2024-05-04 21:12:30.000000 geoseeq-0.6.1/geoseeq.egg-info/dependency_links.txt
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       45 2024-05-04 21:12:30.000000 geoseeq-0.6.1/geoseeq.egg-info/entry_points.txt
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       14 2024-05-04 21:12:30.000000 geoseeq-0.6.1/geoseeq.egg-info/top_level.txt
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      641 2024-05-04 21:12:15.000000 geoseeq-0.6.1/pyproject.toml
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       38 2024-05-04 21:12:30.685011 geoseeq-0.6.1/setup.cfg
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      831 2024-04-15 16:42:26.000000 geoseeq-0.6.1/setup.py
-drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 21:12:30.685011 geoseeq-0.6.1/tests/
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2022-11-29 19:57:49.000000 geoseeq-0.6.1/tests/__init__.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    12810 2024-04-15 16:42:26.000000 geoseeq-0.6.1/tests/test_api_client.py
--rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      784 2024-04-15 16:42:26.000000 geoseeq-0.6.1/tests/test_plotting.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1067 2023-03-22 01:07:34.000000 geoseeq-0.6.2/LICENSE
+-rw-r--r--   0 dcdanko   (1000) dcdanko   (1000)     4803 2024-05-16 15:40:35.768579 geoseeq-0.6.2/PKG-INFO
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4254 2024-04-15 16:42:26.000000 geoseeq-0.6.2/README.md
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      946 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2387 2023-08-13 06:22:51.000000 geoseeq-0.6.2/geoseeq/app.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      188 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/blob_constructors.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2115 2023-06-14 19:17:52.000000 geoseeq-0.6.2/geoseeq/bulk_creators.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/cli/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       24 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/cli/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      176 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/cli/constants.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2275 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/copy.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4132 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/detail.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    17766 2024-04-24 00:22:47.000000 geoseeq-0.6.2/geoseeq/cli/download.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3083 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/cli/fastq_utils.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      997 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/get_eula.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3791 2024-05-16 15:40:14.000000 geoseeq-0.6.2/geoseeq/cli/main.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     5929 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/manage.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      738 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/progress_bar.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3030 2024-04-24 14:28:45.000000 geoseeq-0.6.2/geoseeq/cli/project.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1884 2023-08-15 00:17:43.000000 geoseeq-0.6.2/geoseeq/cli/raw.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3838 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/run.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1015 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/search.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/cli/shared_params/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      325 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/shared_params/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4095 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/shared_params/common_state.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1072 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/shared_params/config.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     9299 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/shared_params/id_handlers.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2741 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/shared_params/obj_getters.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2083 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/shared_params/opts_and_args.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/cli/upload/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      627 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/upload/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    10081 2024-05-04 19:25:40.000000 geoseeq-0.6.2/geoseeq/cli/upload/upload.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3434 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/upload/upload_advanced.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    10706 2024-05-04 18:41:04.000000 geoseeq-0.6.2/geoseeq/cli/upload/upload_reads.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      925 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/cli/user.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2873 2023-08-12 19:50:20.000000 geoseeq-0.6.2/geoseeq/cli/utils.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     6783 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/cli/view.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      431 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/constants.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/contrib/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/contrib/__init__.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/contrib/ncbi/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/contrib/ncbi/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1056 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/contrib/ncbi/api.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4341 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/contrib/ncbi/bioproject.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2400 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/contrib/ncbi/cli.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      175 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/contrib/ncbi/setup_logging.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/file_system/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:39:43.000000 geoseeq-0.6.2/geoseeq/file_system/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    16963 2024-04-24 14:27:13.000000 geoseeq-0.6.2/geoseeq/file_system/filesystem_download.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3627 2024-04-23 14:40:08.000000 geoseeq-0.6.2/geoseeq/file_system/main.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4138 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/file_system_cache.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/id_constructors/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      126 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/id_constructors/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     5702 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/id_constructors/from_blobs.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3151 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/id_constructors/from_ids.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4174 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/id_constructors/from_names.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3305 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/id_constructors/from_uuids.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2676 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/id_constructors/resolvers.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      723 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/id_constructors/utils.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     7965 2024-04-15 16:42:46.000000 geoseeq-0.6.2/geoseeq/knex.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2462 2023-06-14 19:17:52.000000 geoseeq-0.6.2/geoseeq/organization.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     9873 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/pipeline.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/plotting/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      154 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/plotting/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      285 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/plotting/constants.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4096 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/plotting/highcharts.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/plotting/map/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      295 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/plotting/map/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4329 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/plotting/map/base_layer.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3907 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/plotting/map/map.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1795 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/plotting/map/overlay.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2554 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/plotting/selectable.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    13741 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/project.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     7131 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/remote_object.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/result/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      356 2023-08-12 19:50:20.000000 geoseeq-0.6.2/geoseeq/result/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1782 2023-08-12 19:50:20.000000 geoseeq-0.6.2/geoseeq/result/bioinfo.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1758 2024-05-03 02:52:42.000000 geoseeq-0.6.2/geoseeq/result/file_chunker.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     7805 2024-05-04 21:09:29.000000 geoseeq-0.6.2/geoseeq/result/file_download.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    10648 2024-05-04 19:34:06.000000 geoseeq-0.6.2/geoseeq/result/file_upload.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     8677 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/result/result_file.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    11122 2024-05-04 19:22:58.000000 geoseeq-0.6.2/geoseeq/result/result_folder.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3667 2024-05-04 21:10:12.000000 geoseeq-0.6.2/geoseeq/result/resumable_download_tracker.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3811 2024-05-04 19:09:33.000000 geoseeq-0.6.2/geoseeq/result/resumable_upload_tracker.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2772 2023-08-13 00:32:52.000000 geoseeq-0.6.2/geoseeq/result/utils.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     7981 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/sample.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3388 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/search.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     8757 2024-05-04 20:42:40.000000 geoseeq-0.6.2/geoseeq/upload_download_manager.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      690 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/user.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3577 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/utils.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq/vc/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/vc/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      710 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/vc/checksum.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2803 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/vc/cli.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2486 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/vc/clone.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       19 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/vc/constants.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      730 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/vc/vc_cache.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      457 2023-03-22 01:07:34.000000 geoseeq-0.6.2/geoseeq/vc/vc_dir.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3850 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/vc/vc_sample.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3110 2024-04-15 16:42:26.000000 geoseeq-0.6.2/geoseeq/vc/vc_stub.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     8071 2023-06-14 19:17:52.000000 geoseeq-0.6.2/geoseeq/work_orders.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/geoseeq.egg-info/
+-rw-r--r--   0 dcdanko   (1000) dcdanko   (1000)     4803 2024-05-16 15:40:35.000000 geoseeq-0.6.2/geoseeq.egg-info/PKG-INFO
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2705 2024-05-16 15:40:35.000000 geoseeq-0.6.2/geoseeq.egg-info/SOURCES.txt
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        1 2024-05-16 15:40:35.000000 geoseeq-0.6.2/geoseeq.egg-info/dependency_links.txt
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       45 2024-05-16 15:40:35.000000 geoseeq-0.6.2/geoseeq.egg-info/entry_points.txt
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       14 2024-05-16 15:40:35.000000 geoseeq-0.6.2/geoseeq.egg-info/top_level.txt
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      641 2024-05-16 15:40:06.000000 geoseeq-0.6.2/pyproject.toml
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       38 2024-05-16 15:40:35.768579 geoseeq-0.6.2/setup.cfg
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      831 2024-04-15 16:42:26.000000 geoseeq-0.6.2/setup.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-16 15:40:35.768579 geoseeq-0.6.2/tests/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2022-11-29 19:57:49.000000 geoseeq-0.6.2/tests/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    12810 2024-04-15 16:42:26.000000 geoseeq-0.6.2/tests/test_api_client.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      784 2024-04-15 16:42:26.000000 geoseeq-0.6.2/tests/test_plotting.py
```

### Comparing `geoseeq-0.6.1/LICENSE` & `geoseeq-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/PKG-INFO` & `geoseeq-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.6.1
+Version: 0.6.2
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.6.1/README.md` & `geoseeq-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/__init__.py` & `geoseeq-0.6.2/geoseeq/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/app.py` & `geoseeq-0.6.2/geoseeq/app.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/bulk_creators.py` & `geoseeq-0.6.2/geoseeq/bulk_creators.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/copy.py` & `geoseeq-0.6.2/geoseeq/cli/copy.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/detail.py` & `geoseeq-0.6.2/geoseeq/cli/detail.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/download.py` & `geoseeq-0.6.2/geoseeq/cli/download.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/fastq_utils.py` & `geoseeq-0.6.2/geoseeq/cli/fastq_utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/get_eula.py` & `geoseeq-0.6.2/geoseeq/cli/get_eula.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/main.py` & `geoseeq-0.6.2/geoseeq/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     """Print the version of the Geoseeq API being used.
 
     ---
     
     Use of this tool implies acceptance of the GeoSeeq End User License Agreement.
     Run `geoseeq eula show` to view the EULA.
     """
-    click.echo('0.6.1')  # remember to update setup
+    click.echo('0.6.2')  # remember to update setup
 
 
 @main.group('advanced')
 def cli_advanced():
     """Advanced commands."""
     pass
```

### Comparing `geoseeq-0.6.1/geoseeq/cli/manage.py` & `geoseeq-0.6.2/geoseeq/cli/manage.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/progress_bar.py` & `geoseeq-0.6.2/geoseeq/cli/progress_bar.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/project.py` & `geoseeq-0.6.2/geoseeq/cli/project.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/raw.py` & `geoseeq-0.6.2/geoseeq/cli/raw.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/run.py` & `geoseeq-0.6.2/geoseeq/cli/run.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/search.py` & `geoseeq-0.6.2/geoseeq/cli/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/shared_params/common_state.py` & `geoseeq-0.6.2/geoseeq/cli/shared_params/common_state.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/shared_params/config.py` & `geoseeq-0.6.2/geoseeq/cli/shared_params/config.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/shared_params/id_handlers.py` & `geoseeq-0.6.2/geoseeq/cli/shared_params/id_handlers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/shared_params/obj_getters.py` & `geoseeq-0.6.2/geoseeq/cli/shared_params/obj_getters.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/shared_params/opts_and_args.py` & `geoseeq-0.6.2/geoseeq/cli/shared_params/opts_and_args.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/upload/__init__.py` & `geoseeq-0.6.2/geoseeq/cli/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/upload/upload.py` & `geoseeq-0.6.2/geoseeq/cli/upload/upload.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/upload/upload_advanced.py` & `geoseeq-0.6.2/geoseeq/cli/upload/upload_advanced.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/upload/upload_reads.py` & `geoseeq-0.6.2/geoseeq/cli/upload/upload_reads.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/user.py` & `geoseeq-0.6.2/geoseeq/cli/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/utils.py` & `geoseeq-0.6.2/geoseeq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/cli/view.py` & `geoseeq-0.6.2/geoseeq/cli/view.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/contrib/ncbi/api.py` & `geoseeq-0.6.2/geoseeq/contrib/ncbi/api.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/contrib/ncbi/bioproject.py` & `geoseeq-0.6.2/geoseeq/contrib/ncbi/bioproject.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/contrib/ncbi/cli.py` & `geoseeq-0.6.2/geoseeq/contrib/ncbi/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/file_system_cache.py` & `geoseeq-0.6.2/geoseeq/file_system_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/id_constructors/from_blobs.py` & `geoseeq-0.6.2/geoseeq/id_constructors/from_blobs.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/id_constructors/from_ids.py` & `geoseeq-0.6.2/geoseeq/id_constructors/from_ids.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/id_constructors/from_names.py` & `geoseeq-0.6.2/geoseeq/id_constructors/from_names.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/id_constructors/from_uuids.py` & `geoseeq-0.6.2/geoseeq/id_constructors/from_uuids.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/id_constructors/resolvers.py` & `geoseeq-0.6.2/geoseeq/id_constructors/resolvers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/id_constructors/utils.py` & `geoseeq-0.6.2/geoseeq/id_constructors/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/knex.py` & `geoseeq-0.6.2/geoseeq/knex.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/organization.py` & `geoseeq-0.6.2/geoseeq/organization.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/pipeline.py` & `geoseeq-0.6.2/geoseeq/pipeline.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/plotting/highcharts.py` & `geoseeq-0.6.2/geoseeq/plotting/highcharts.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/plotting/map/base_layer.py` & `geoseeq-0.6.2/geoseeq/plotting/map/base_layer.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/plotting/map/map.py` & `geoseeq-0.6.2/geoseeq/plotting/map/map.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/plotting/map/overlay.py` & `geoseeq-0.6.2/geoseeq/plotting/map/overlay.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/plotting/selectable.py` & `geoseeq-0.6.2/geoseeq/plotting/selectable.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/project.py` & `geoseeq-0.6.2/geoseeq/project.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/remote_object.py` & `geoseeq-0.6.2/geoseeq/remote_object.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/result/bioinfo.py` & `geoseeq-0.6.2/geoseeq/result/bioinfo.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/result/file_chunker.py` & `geoseeq-0.6.2/geoseeq/result/file_chunker.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/result/file_download.py` & `geoseeq-0.6.2/geoseeq/result/file_download.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/result/file_upload.py` & `geoseeq-0.6.2/geoseeq/result/file_upload.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/result/result_file.py` & `geoseeq-0.6.2/geoseeq/result/result_file.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/result/result_folder.py` & `geoseeq-0.6.2/geoseeq/result/result_folder.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/result/resumable_download_tracker.py` & `geoseeq-0.6.2/geoseeq/result/resumable_download_tracker.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/result/resumable_upload_tracker.py` & `geoseeq-0.6.2/geoseeq/result/resumable_upload_tracker.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/result/utils.py` & `geoseeq-0.6.2/geoseeq/result/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/sample.py` & `geoseeq-0.6.2/geoseeq/sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/search.py` & `geoseeq-0.6.2/geoseeq/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/upload_download_manager.py` & `geoseeq-0.6.2/geoseeq/upload_download_manager.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/user.py` & `geoseeq-0.6.2/geoseeq/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/utils.py` & `geoseeq-0.6.2/geoseeq/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/vc/checksum.py` & `geoseeq-0.6.2/geoseeq/vc/checksum.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/vc/cli.py` & `geoseeq-0.6.2/geoseeq/vc/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/vc/clone.py` & `geoseeq-0.6.2/geoseeq/vc/clone.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/vc/vc_cache.py` & `geoseeq-0.6.2/geoseeq/vc/vc_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/vc/vc_sample.py` & `geoseeq-0.6.2/geoseeq/vc/vc_sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/vc/vc_stub.py` & `geoseeq-0.6.2/geoseeq/vc/vc_stub.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq/work_orders.py` & `geoseeq-0.6.2/geoseeq/work_orders.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/geoseeq.egg-info/PKG-INFO` & `geoseeq-0.6.2/geoseeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.6.1
+Version: 0.6.2
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.6.1/geoseeq.egg-info/SOURCES.txt` & `geoseeq-0.6.2/geoseeq.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 geoseeq/cli/upload/upload_reads.py
 geoseeq/contrib/__init__.py
 geoseeq/contrib/ncbi/__init__.py
 geoseeq/contrib/ncbi/api.py
 geoseeq/contrib/ncbi/bioproject.py
 geoseeq/contrib/ncbi/cli.py
 geoseeq/contrib/ncbi/setup_logging.py
+geoseeq/file_system/__init__.py
+geoseeq/file_system/filesystem_download.py
+geoseeq/file_system/main.py
 geoseeq/id_constructors/__init__.py
 geoseeq/id_constructors/from_blobs.py
 geoseeq/id_constructors/from_ids.py
 geoseeq/id_constructors/from_names.py
 geoseeq/id_constructors/from_uuids.py
 geoseeq/id_constructors/resolvers.py
 geoseeq/id_constructors/utils.py
```

### Comparing `geoseeq-0.6.1/pyproject.toml` & `geoseeq-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geoseeq"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
   { name="David C. Danko", email="dcdanko@biotia.io" },
 ]
 description = "GeoSeeq command line tools and python API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `geoseeq-0.6.1/setup.py` & `geoseeq-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/tests/test_api_client.py` & `geoseeq-0.6.2/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.6.1/tests/test_plotting.py` & `geoseeq-0.6.2/tests/test_plotting.py`

 * *Files identical despite different names*

