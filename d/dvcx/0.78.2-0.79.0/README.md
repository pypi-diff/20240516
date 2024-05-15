# Comparing `tmp/dvcx-0.78.2.tar.gz` & `tmp/dvcx-0.79.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.78.2.tar", last modified: Mon May 13 22:08:28 2024, max compression
+gzip compressed data, was "dvcx-0.79.0.tar", last modified: Wed May 15 22:48:56 2024, max compression
```

## Comparing `dvcx-0.78.2.tar` & `dvcx-0.79.0.tar`

### file list

```diff
@@ -1,251 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.270123 dvcx-0.78.2/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-13 22:08:22.000000 dvcx-0.78.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 22:08:22.000000 dvcx-0.78.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-13 22:08:22.000000 dvcx-0.78.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-13 22:08:22.000000 dvcx-0.78.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-13 22:08:22.000000 dvcx-0.78.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-13 22:08:22.000000 dvcx-0.78.2/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 22:08:22.000000 dvcx-0.78.2/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-13 22:08:22.000000 dvcx-0.78.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-13 22:08:22.000000 dvcx-0.78.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-13 22:08:22.000000 dvcx-0.78.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-13 22:08:22.000000 dvcx-0.78.2/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-13 22:08:22.000000 dvcx-0.78.2/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-13 22:08:22.000000 dvcx-0.78.2/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-13 22:08:28.270123 dvcx-0.78.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-13 22:08:22.000000 dvcx-0.78.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.226122 dvcx-0.78.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-13 22:08:22.000000 dvcx-0.78.2/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.230123 dvcx-0.78.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.230123 dvcx-0.78.2/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.234123 dvcx-0.78.2/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.234123 dvcx-0.78.2/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 22:08:22.000000 dvcx-0.78.2/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-13 22:08:22.000000 dvcx-0.78.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-13 22:08:22.000000 dvcx-0.78.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 22:08:28.270123 dvcx-0.78.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.222123 dvcx-0.78.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.238123 dvcx-0.78.2/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.238123 dvcx-0.78.2/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72305 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/catalog/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    31034 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.242123 dvcx-0.78.2/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11679 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.242123 dvcx-0.78.2/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45621 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30778 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    34860 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.246123 dvcx-0.78.2/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16870 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/tar_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    60449 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.250123 dvcx-0.78.2/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-13 22:08:22.000000 dvcx-0.78.2/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.266123 dvcx-0.78.2/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 22:08:28.000000 dvcx-0.78.2/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.254123 dvcx-0.78.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.254123 dvcx-0.78.2/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.254123 dvcx-0.78.2/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35673 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   113286 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26674 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.258123 dvcx-0.78.2/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.262123 dvcx-0.78.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.262123 dvcx-0.78.2/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-13 22:08:22.000000 dvcx-0.78.2/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.262123 dvcx-0.78.2/tests/unit/sql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:28.266123 dvcx-0.78.2/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_catalog_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_dataset_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-13 22:08:23.000000 dvcx-0.78.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.405135 dvcx-0.79.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-15 22:48:47.000000 dvcx-0.79.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 22:48:47.000000 dvcx-0.79.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-15 22:48:47.000000 dvcx-0.79.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-15 22:48:47.000000 dvcx-0.79.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-15 22:48:47.000000 dvcx-0.79.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 22:48:47.000000 dvcx-0.79.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-15 22:48:47.000000 dvcx-0.79.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-15 22:48:47.000000 dvcx-0.79.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-15 22:48:47.000000 dvcx-0.79.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-15 22:48:47.000000 dvcx-0.79.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-15 22:48:47.000000 dvcx-0.79.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-15 22:48:47.000000 dvcx-0.79.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-15 22:48:56.405135 dvcx-0.79.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-15 22:48:47.000000 dvcx-0.79.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-15 22:48:47.000000 dvcx-0.79.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.353135 dvcx-0.79.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.353135 dvcx-0.79.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.357135 dvcx-0.79.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.357135 dvcx-0.79.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-15 22:48:47.000000 dvcx-0.79.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-15 22:48:47.000000 dvcx-0.79.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 22:48:56.405135 dvcx-0.79.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.345135 dvcx-0.79.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.361135 dvcx-0.79.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.361135 dvcx-0.79.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72958 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/catalog/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31032 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.365135 dvcx-0.79.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.365135 dvcx-0.79.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45892 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30749 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34870 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17671 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.373135 dvcx-0.79.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16852 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/tar_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.377135 dvcx-0.79.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60126 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.377135 dvcx-0.79.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.377135 dvcx-0.79.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.381135 dvcx-0.79.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.381135 dvcx-0.79.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.381135 dvcx-0.79.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.397135 dvcx-0.79.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.385135 dvcx-0.79.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.385135 dvcx-0.79.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16205 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.389135 dvcx-0.79.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35731 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113348 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28867 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.389135 dvcx-0.79.0/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.393135 dvcx-0.79.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.397135 dvcx-0.79.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.397135 dvcx-0.79.0/tests/unit/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.397135 dvcx-0.79.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_catalog_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/utils.py
```

### Comparing `dvcx-0.78.2/.cruft.json` & `dvcx-0.79.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.79.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.79.0/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/.github/workflows/benchmarks.yml` & `dvcx-0.79.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/.github/workflows/release.yml` & `dvcx-0.79.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/.github/workflows/tests.yml` & `dvcx-0.79.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/.gitignore` & `dvcx-0.79.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/.pre-commit-config.yaml` & `dvcx-0.79.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/CODE_OF_CONDUCT.rst` & `dvcx-0.79.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/CONTRIBUTING.rst` & `dvcx-0.79.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/LICENSE` & `dvcx-0.79.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/LICENSES/Apache-2.0.txt` & `dvcx-0.79.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/LICENSES/BSD-3-Clause.txt` & `dvcx-0.79.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/LICENSES/Python-2.0.txt` & `dvcx-0.79.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/PKG-INFO` & `dvcx-0.79.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.78.2
+Version: 0.79.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.78.2/README.rst` & `dvcx-0.79.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/docs/udfs.md` & `dvcx-0.79.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/blip2_image_desc_lib.py` & `dvcx-0.79.0/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/clip.py` & `dvcx-0.79.0/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/common_sql_functions.py` & `dvcx-0.79.0/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/dir_expansion.py` & `dvcx-0.79.0/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/hf_pipeline.py` & `dvcx-0.79.0/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/llava2_image_desc_lib.py` & `dvcx-0.79.0/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/llm-claude-aggregate-query.py` & `dvcx-0.79.0/examples/llm-claude-aggregate-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/llm-claude-simple-query.py` & `dvcx-0.79.0/examples/llm-claude-simple-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/llm-claude.py` & `dvcx-0.79.0/examples/llm-claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/loader.py` & `dvcx-0.79.0/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/neurips/README` & `dvcx-0.79.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/neurips/distance_to_query.py` & `dvcx-0.79.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/neurips/llm_chat.py` & `dvcx-0.79.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/neurips/single_query.py` & `dvcx-0.79.0/examples/neurips/single_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 PDF_SUBSET_MOD = 512
 
 BASE_URL = "https://proceedings.neurips.cc/paper_files/paper/"
 
 
 def chomp(ss, prefix):
     assert ss.startswith(prefix)
-    ss = ss[len(prefix) :]
-    return ss
+    return ss[len(prefix) :]
 
 
 @udf(
     params=(Object(load_bibtex),),
     output={
         "bib_parent": String,
         "bib_name": String,
@@ -87,16 +86,15 @@
 def embed_page(pages):
     openai_api_key = os.environ["OPENAI_API_KEY"]
     assert openai_api_key.startswith("sk-")
     openai = OpenAIEmbeddings(openai_api_key=openai_api_key)
     del openai_api_key
 
     embed = openai.embed_documents([page[0] for page in pages])
-    embed = [(ee,) for ee in embed]
-    return embed
+    return [(ee,) for ee in embed]
 
 
 # Remove last line to include post-2000 papers
 subset_ds = (
     DatasetQuery("s3://neurips-papers/")
     .filter(~C.name.glob("*.zip"))
     .filter(~(C.parent.glob("20*/file") | C.parent.glob("20*/hash")))
```

### Comparing `dvcx-0.78.2/examples/neurips/text_loaders.py` & `dvcx-0.79.0/examples/neurips/text_loaders.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 from dvcx.sql.types import Int, String
 
 logger = logging.getLogger("dvcx")
 
 
 def sanitize_utf8(original):
     """Clean up invalid UTF characters that may cause failures when writing to a DB."""
-    sanitized = (
+    return (
         original.encode("utf-8", "ignore").decode("utf-8", "ignore").replace("\x00", "")
     )
-    return sanitized
 
 
 def sanitize_ascii(original):
     """More restrictive than sanitize_utf8 when we want just basic keyboard chars.
     This also puts all the text on a single line by eliminating all line breaks.
     If we expect a large amount of non-English text, then it makes sense to first use
     the Unidecode package.
@@ -34,47 +33,48 @@
     assert sanitized.isascii()
     assert sanitized.isprintable()
     return sanitized
 
 
 def compress_whitespace(original):
     """PDF parsers often result in some weird whitespace."""
-    sanitized = " ".join(original.split())
-    return sanitized
+    return " ".join(original.split())
 
 
 def load_pdf_pages(raw):
     raw_name = raw.info()["name"]
 
     pages = []
     try:
         pdf_reader = PyPDF2.PdfReader(raw)
         pages = [sanitize_utf8(page.extract_text()) for page in pdf_reader.pages]
-    except Exception as error:
+    except Exception as error:  # noqa: BLE001
         error_type = type(error).__name__
         logger.warning(
-            f"A pdf reader error occurred in {raw_name}: {error_type} - {error}"
+            "A pdf reader error occurred in %s: %s - %s",
+            raw_name,
+            error_type,
+            error,
         )
     return pages
 
 
 @udf(
-    params=(Object(load_pdf_pages),) + tuple(DatasetRow.schema.keys()),
+    params=(Object(load_pdf_pages), *tuple(DatasetRow.schema.keys())),
     output={**DatasetRow.schema, "n_page": Int, "total_pages": Int, "page": String},
 )
 def pdf_pages(pages, *args):
     record = dict(zip(DatasetRow.schema.keys(), args))
     del record["random"]  # random will be populated automatically
     record["is_latest"] = record["is_latest"] > 0  # needs to be a bool
 
     total_pages = len(pages)
     for n_page, page in enumerate(pages):
         page = sanitize_ascii(page)
         page = compress_whitespace(page)
-        yield DatasetRow.create(**record) + (n_page, total_pages, page)
+        yield (*DatasetRow.create(**record), n_page, total_pages, page)
 
 
 def load_bibtex(raw):
     bibtex_str = raw.read().decode("utf-8")
     parser = bibtex.Parser()
-    bib_data = parser.parse_string(bibtex_str)
-    return bib_data
+    return parser.parse_string(bibtex_str)
```

### Comparing `dvcx-0.78.2/examples/openai_image_desc_lib.py` & `dvcx-0.79.0/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/openimage-detect.py` & `dvcx-0.79.0/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/pose_detection.py` & `dvcx-0.79.0/examples/pose_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,20 +59,19 @@
 
 
 def mask_image(detection_result):
     # This only takes the most confident detection.
     # We could union all the detections or do a generator over each.
     segmentation_mask = detection_result.segmentation_masks[0].numpy_view()
     visualized_mask = np.repeat(segmentation_mask[:, :, np.newaxis], 3, axis=2) * 255
-    visualized_mask = visualized_mask.astype(np.uint8)
-    return visualized_mask
+    return visualized_mask.astype(np.uint8)
 
 
 @udf(
-    params=(Stream(),) + tuple(DatasetRow.schema.keys()),
+    params=(Stream(), *tuple(DatasetRow.schema.keys())),
     output={**DatasetRow.schema, "pose": JSON},
 )
 class PoseDetector:
     annotated_folder = "annotated_images"
     mask_folder = "mask_images"
 
     def __init__(
@@ -98,15 +97,15 @@
         cloud_file = fsspec.open(urlpath=urlpath, mode="wb")
         with cloud_file as fp:
             image.save(fp, format=format)
 
         # Get the blob info
         info_ = self.client.fs.info(urlpath)
         entry = self.client.convert_info(info_, folder)
-        row = DatasetRow.create(
+        return DatasetRow.create(
             name=name,
             source=source,
             parent=folder,
             size=entry.size,
             location=None,
             vtype="",
             dir_type=0,
@@ -114,15 +113,14 @@
             owner_id=entry.owner_id,
             is_latest=entry.is_latest,
             last_modified=entry.last_modified,
             version=entry.version,
             etag=entry.etag,
             anno=entry.anno,
         )
-        return row
 
     def __call__(
         self,
         stream,
         *args,
     ):
         # Build a dict from row contents
@@ -146,15 +144,15 @@
         # Move into protobuf list for next step
         pose = [landmarks_list_to_pb2(lm) for lm in detection_result.pose_landmarks]
 
         # Turn into json
         pose_json = [pb2_to_dict(lmp) for lmp in pose]
 
         # Yield same row back (with json pose info)
-        yield row + (json.dumps(pose_json),)
+        yield (*row, json.dumps(pose_json))
 
         # No detections ==> we can stop here
         if len(pose) == 0:
             return
 
         # Annotate image
         annotated_image = annotate_image(image.numpy_view(), pose)
@@ -164,29 +162,29 @@
         row = self.save(
             image=annotated_image,
             source=record["source"],
             folder=self.annotated_folder,
             name=record["name"],
             format=image_format,
         )
-        yield row + (json.dumps(pose_json),)
+        yield (*row, json.dumps(pose_json))
 
         # Now do mask
         visualized_mask = mask_image(detection_result)
         visualized_mask = Image.fromarray(visualized_mask)  # make PIL object
 
         # Save the image and get the cloud object info
         row = self.save(
             image=visualized_mask,
             source=record["source"],
             folder=self.mask_folder,
             name=record["name"],
             format=image_format,
         )
-        yield row + (json.dumps(pose_json),)
+        yield (*row, json.dumps(pose_json))
 
 
 cloud_prefix = "s3://"  # for GCP just switch to "gcs://"
 bucket = "dvcx-50k-laion-files-writable"  # which bucket to use for both read and write
 bucket_region = "us-east-2"  # no need to specify for GCP
 
 # Use: !wget -O pose_landmarker.task -q https://storage.googleapis.com/mediapipe-models/pose_landmarker/pose_landmarker_heavy/float16/1/pose_landmarker_heavy.task
```

### Comparing `dvcx-0.78.2/examples/torch-loader.py` & `dvcx-0.79.0/examples/torch-loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 
     def forward(self, x):
         x = torch.relu(self.conv1(x))
         x = torch.relu(self.conv2(x))
         x = torch.relu(self.conv3(x))
         x = x.view(-1, 64 * 8 * 8)
         x = torch.relu(self.fc1(x))
-        x = self.fc2(x)
-        return x
+        return self.fc2(x)
 
 
 if __name__ == "__main__":
     ds = (
         Dataset(STORAGE)
         .filter(C.name.glob("*.jpg"))
         .map(lambda name: (name[:3],), output={"label": str})
```

### Comparing `dvcx-0.78.2/examples/udfs/batching.py` & `dvcx-0.79.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/udfs/image_transformation.py` & `dvcx-0.79.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/udfs/parallel.py` & `dvcx-0.79.0/examples/udfs/parallel.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,16 +36,15 @@
     },  # Signals being returned by the UDF, with the signal name and type.
 )
 def name_len_benchmark(name):
     # Run the fibonacci benchmark as an example of a single-threaded CPU-bound UDF
     fibonacci(35)
     if name.endswith(".json"):
         return (-1,)
-    else:
-        return (len(name),)
+    return (len(name),)
 
 
 # Save as a new dataset
 DatasetQuery(
     path="gcs://dvcx-datalakes/dogs-and-cats/",
     anon=True,
 ).filter(C.name.glob("*cat*")).add_signals(name_len_benchmark, parallel=-1).save(
```

### Comparing `dvcx-0.78.2/examples/udfs/simple.py` & `dvcx-0.79.0/examples/udfs/simple.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     {
         "name_len": Int
     },  # Signals being returned by the UDF, with the signal name and type.
 )
 def name_len(name):
     if name.endswith(".json"):
         return (-1,)
-    else:
-        return (len(name),)
+    return (len(name),)
 
 
 if __name__ == "__main__":
     ds_name = uuid.uuid4().hex
     print(f"Saving to dataset: {ds_name}")
     # Save as a new dataset
     DatasetQuery(
```

### Comparing `dvcx-0.78.2/examples/udfs/stateful.py` & `dvcx-0.79.0/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/udfs/stateful_similarity.py` & `dvcx-0.79.0/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/unstructured-text.py` & `dvcx-0.79.0/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/wds.py` & `dvcx-0.79.0/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/wds_filtered.py` & `dvcx-0.79.0/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/wds_meta.py` & `dvcx-0.79.0/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/examples/zalando/zalando_clip.py` & `dvcx-0.79.0/examples/zalando/zalando_clip.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,15 @@
     def __init__(self):
         self.fclip = FashionCLIP("fashion-clip")
 
     def fashion_clip(self, inputs):
         embeddings = self.fclip.encode_images(
             [input[0] for input in inputs], batch_size=1
         )
-        emb_json = [(json.dumps(emb),) for emb in embeddings.tolist()]
-        return emb_json
+        return [(json.dumps(emb),) for emb in embeddings.tolist()]
 
 
 if __name__ == "__main__":
     # This example processes 5 objects in the new dataset and generates the
     # embeddings for them.
     DatasetQuery(path="gcs://dvcx-zalando-hd-resized/zalando-hd-resized/").filter(
         C.name.glob("*.jpg")
```

### Comparing `dvcx-0.78.2/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.79.0/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/noxfile.py` & `dvcx-0.79.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/pyproject.toml` & `dvcx-0.79.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -156,15 +156,21 @@
 show-fixes = true
 
 [tool.ruff.lint]
 ignore = [
   "S101",  # assert
   "PLR2004",  # magic-value-comparison
   "PLW2901",  # redefined-loop-name
-  "PLC0105"  # type-name-incorrect-variance
+  "PLC0105",  # type-name-incorrect-variance
+  "ISC001",  # single-line-implicit-string-concatenation, incompatible with ruff format
+  "RET502",  # implicit-return-value
+  "RET503",  # implicit-return
+  "SIM105",  # suppressible-exception
+  "SIM108",  # if-else-block-instead-of-if-exp
+  "SIM117"  # multiple-with-statements
 ]
 select = [
   "B",  # flake8-bugbear
   "C4",  # flake8-comprehensions
   "C90",  # mccabe
   "W",  # pycodestyle - Warning
   "E",  # pycodestyle - Error
@@ -172,15 +178,41 @@
   "I",  # isort
   "T10",  # flake8-debugger
   "S",  # flake8-bandit
   "PL",  # pylint
   "TCH",  # flake8-type-checking
   "UP",  # pyupgrade
   "N",  # pep8-naming
-  "PIE"  # flake8-pie
+  "YTT",  # flake8-2020
+  "ASYNC",  # flake8-async
+  "EXE",  # flake8-executable
+  "ISC",  # flake8-implicit-str-concat
+  "ICN",  # flake8-import-conventions
+  "PIE",  # flake8-pie
+  "LOG",  # flake8-logging
+  "G",  # flake8-logging-format
+  "PYI",  # flake8-pyi
+  "Q",  # flake8-quotes
+  "SLOT",  # flake8-slots
+  "PGH",  # pygrep-hooks
+  "FLY",  # flynt
+  "PERF101",  # perflint - unnecessary-list-cast
+  "TID",  # flake8-tidy-imports
+  "RSE",  # flake8-raise
+  "INP",  # flake8-no-pep420
+  "RUF",  # ruff rules
+  "BLE",  # flake8-blind-except
+  "SIM",  # flake8-simplify
+  "RSE",  # flake8-raise
+  "RET",  # flake8-return
+  "DTZ",  # flake8-datetimez
+  "TRY004",  # type-check-without-type-error
+  "TRY201",  # verbose-raise
+  "TRY302",  # useless-try-except
+  "TRY401"  # verbose-log-message
 ]
 
 [tool.ruff.lint.flake8-bugbear]
 # Allow default arguments like, e.g., `data: List[str] = fastapi.Query(None)`.
 extend-immutable-calls = ["dvcx.storage.StorageURI"]
 
 [tool.ruff.lint.flake8-type-checking]
@@ -193,7 +225,12 @@
 max-args = 16
 max-branches = 16
 max-public-methods = 32
 max-statements = 64
 
 [tool.ruff.lint.mccabe]
 max-complexity = 15
+
+[tool.ruff.lint.per-file-ignores]
+"examples/**" = ["INP001"]
+"tests/scripts/**" = ["INP001"]
+"tests/**" = ["DTZ"]
```

### Comparing `dvcx-0.78.2/src/dvcx/asyn.py` & `dvcx-0.79.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/cache.py` & `dvcx-0.79.0/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/catalog/catalog.py` & `dvcx-0.79.0/src/dvcx/catalog/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,17 +177,17 @@
     def done_task(self, done):
         for task in done:
             task.result()
 
     def _check_dependencies(self) -> None:
         try:
             import lz4.frame  # noqa: F401
-            import numpy  # noqa: F401
-            import pandas  # noqa: F401
-            import pyarrow  # noqa: F401
+            import numpy as np  # noqa: F401
+            import pandas as pd  # noqa: F401
+            import pyarrow as pa  # noqa: F401
         except ImportError as exc:
             raise Exception(
                 f"Missing dependency: {exc.name}\n"
                 "To install run:\n"
                 "\tpip install 'dvcx[remote]'"
             ) from None
 
@@ -314,35 +314,32 @@
 ) -> str:
     """
     Checks the dataset filename for existence or if it should be force-overwritten.
     """
     dataset_file = (
         dataset_filename if dataset_filename else output + DATASET_FILE_SUFFIX
     )
-    if not skip_check_edvcx:
-        if os.path.exists(dataset_file):
-            if force:
-                os.remove(dataset_file)
-            else:
-                raise RuntimeError(
-                    f"Output dataset file already exists: {dataset_file}"
-                )
+    if not skip_check_edvcx and os.path.exists(dataset_file):
+        if force:
+            os.remove(dataset_file)
+        else:
+            raise RuntimeError(f"Output dataset file already exists: {dataset_file}")
     return dataset_file
 
 
 def parse_edvcx_file(filename: str) -> list[dict[str, Any]]:
     with open(filename, encoding="utf-8") as f:
         contents = yaml.safe_load(f)
 
     if not isinstance(contents, list):
         contents = [contents]
 
     for entry in contents:
         if not isinstance(entry, dict):
-            raise ValueError(
+            raise TypeError(
                 "Failed parsing EDVCX file, "
                 "each data source entry must be a dictionary"
             )
         if "data-source" not in entry or "files" not in entry:
             raise ValueError(
                 "Failed parsing EDVCX file, "
                 "each data source entry must contain the "
@@ -556,17 +553,17 @@
         return src.get_node_full_path_from_path(full_path)
     if column == "size":
         return str(row[field_lookup["size"]])
     if column == "type":
         dt = row[field_lookup["dir_type"]]
         if dt == DirType.DIR:
             return "d"
-        elif dt == DirType.FILE:
+        if dt == DirType.FILE:
             return "f"
-        elif dt == DirType.TAR_ARCHIVE:
+        if dt == DirType.TAR_ARCHIVE:
             return "t"
         # Unknown - this only happens if a type was added elsewhere but not here
         return "u"
     return ""
 
 
 class Catalog:
@@ -721,17 +718,18 @@
             source_metastore = self.metastore.clone(
                 uri=client.uri, partial_id=partial_id
             )
             source_warehouse = self.warehouse.clone(
                 uri=client.uri, partial_id=partial_id
             )
             lst = Listing(storage, source_metastore, source_warehouse, client)
-            logger.debug(  # type: ignore[unreachable]
-                f"Using cached listing {storage.uri}."
-                + f" Valid till: {storage.expires_to_local}"
+            logger.debug(
+                "Using cached listing %s. Valid till: %s",
+                storage.uri,
+                storage.expires_to_local,
             )
             # Listing has to have correct version of data storage
             # initialized with correct Storage
             return lst, path
 
         source_metastore.init_partial_id(client.uri)
         partial_id = source_metastore.get_next_partial_id(client.uri)
@@ -1025,24 +1023,22 @@
             )
 
         if validate_version and not dataset.is_valid_next_version(version):
             raise DatasetInvalidVersionError(
                 f"Version {version} must be higher than the current latest one"
             )
 
-        dataset = self.create_new_dataset_version(
+        return self.create_new_dataset_version(
             dataset,
             version,
             query_script=query_script,
             create_rows_table=create_rows,
             custom_columns=custom_columns,
         )
 
-        return dataset
-
     def create_new_dataset_version(
         self,
         dataset: DatasetRecord,
         version: int,
         sources="",
         query_script="",
         error_message="",
@@ -1077,34 +1073,51 @@
 
         if create_rows_table:
             table_name = self.warehouse.dataset_table_name(dataset.name, version)
             self.warehouse.create_dataset_rows_table(
                 table_name, custom_columns=custom_columns
             )
 
-            self.update_dataset_version_with_stats(dataset, version)
+            self.update_dataset_version_with_warehouse_info(dataset, version)
 
         return dataset
 
-    def update_dataset_version_with_stats(
+    def update_dataset_version_with_warehouse_info(
         self, dataset: DatasetRecord, version: int, **kwargs
     ) -> None:
         dataset_version = dataset.get_version(version)
 
-        num_objects = dataset_version.num_objects
-        size = dataset_version.size
-        if not num_objects:
+        values = {**kwargs}
+
+        if not dataset_version.num_objects:
             num_objects, size = self.warehouse.dataset_stats(dataset, version)
+            if num_objects != dataset_version.num_objects:
+                values["num_objects"] = num_objects
+            if size != dataset_version.size:
+                values["size"] = size
+
+        if not dataset_version.preview and (
+            dataset_rows := list(
+                self.ls_dataset_rows(
+                    dataset.name,
+                    version,
+                    limit=20,
+                    custom_columns=True,
+                )
+            )
+        ):
+            values["preview"] = [row.to_preview_dict() for row in dataset_rows]
+
+        if not values:
+            return
 
         self.metastore.update_dataset_version(
             dataset,
             version,
-            num_objects=num_objects,
-            size=size,
-            **kwargs,
+            **values,
         )
 
     def update_dataset(
         self, dataset: DatasetRecord, conn=None, **kwargs
     ) -> DatasetRecord:
         """Updates dataset fields."""
         old_name = None
@@ -1195,24 +1208,24 @@
                 ds,
                 DatasetStatus.FAILED,
                 version=ds.latest_version,
                 error_message=DATASET_INTERNAL_ERROR_MESSAGE,
                 error_stack=traceback.format_exc(),
             )
             self.warehouse.drop_dataset_rows_table(ds, ds.latest_version)
-            self.update_dataset_version_with_stats(
+            self.update_dataset_version_with_warehouse_info(
                 ds,
                 ds.latest_version,
                 sources="\n".join(sources),
             )
             raise
 
         ds = self.get_dataset(name)
 
-        self.update_dataset_version_with_stats(
+        self.update_dataset_version_with_warehouse_info(
             ds,
             ds.latest_version,
             sources="\n".join(sources),
         )
 
         return self.get_dataset(name)
 
@@ -1253,14 +1266,19 @@
             error_stack=dataset_version.error_stack,
             script_output=dataset_version.script_output,
             created_at=dataset_version.created_at,
             finished_at=dataset_version.finished_at,
             custom_column_types=dataset_version.custom_column_types_serialized,
             num_objects=dataset_version.num_objects,
             size=dataset_version.size,
+            preview=(
+                [row.to_preview_dict() for row in dataset_version.preview]
+                if dataset_version.preview
+                else None
+            ),
         )
         # to avoid re-creating rows table, we are just renaming it for a new version
         # of target dataset
         self.warehouse.rename_dataset_table(
             dataset.name,
             target_dataset.name,
             old_version=version,
@@ -1454,15 +1472,15 @@
                 dst_version=dst_version,  # type: ignore[arg-type]
             )
             merged_custom_column_types = {
                 **src.custom_column_types_serialized,
                 **dst.custom_column_types_serialized,
             }
             self.update_dataset(dst, custom_column_types=merged_custom_column_types)
-            self.update_dataset_version_with_stats(
+            self.update_dataset_version_with_warehouse_info(
                 dst,
                 dst_version,  # type: ignore[arg-type]
                 custom_column_types=merged_custom_column_types,
             )
             for dep in src_dep:
                 if dep and dep not in dst_dep:
                     self.metastore.add_dependency(
@@ -1492,15 +1510,15 @@
             )
             self.warehouse.merge_dataset_rows(
                 src,
                 dst,
                 src_version,
                 dst_version,
             )
-            self.update_dataset_version_with_stats(dst, dst_version)
+            self.update_dataset_version_with_warehouse_info(dst, dst_version)
             for dep in set(src_dep + dst_dep):
                 if dep:
                     self.metastore.add_dependency(dep, dst.name, dst_version)
 
         return dst
 
     def open_object(self, row: DatasetRow, use_cache: bool = True, **config: Any):
@@ -1534,15 +1552,15 @@
 
     def get_storage(self, uri: StorageURI) -> Storage:
         return self.metastore.get_storage(uri)
 
     def ls_storages(self) -> list[Storage]:
         return self.metastore.list_storages()
 
-    def pull_dataset(  # noqa: C901, PLR0911
+    def pull_dataset(
         self,
         dataset_uri: str,
         output: Optional[str] = None,
         no_cp: bool = False,
         force: bool = False,
         edvcx: bool = False,
         edvcx_file: Optional[str] = None,
@@ -1684,15 +1702,15 @@
             dataset,
             DatasetStatus.COMPLETE,
             version=version,
             error_message=remote_dataset.error_message,
             error_stack=remote_dataset.error_stack,
             script_output=remote_dataset.error_stack,
         )
-        self.update_dataset_version_with_stats(dataset, version)
+        self.update_dataset_version_with_warehouse_info(dataset, version)
 
         dataset_save_progress_bar.close()
         print(f"Dataset {dataset_uri} saved locally")
 
         _instantiate_dataset()
 
     def clone(
@@ -2112,15 +2130,15 @@
                 client = self.get_client(bucket.uri, **client_config)
                 print(f"Registering storage {client.uri}")
                 self.metastore.create_storage_if_not_registered(client.uri)
 
         if index_processors and not isinstance(index_processors, list):
             processors = [index_processors]
         else:
-            processors = index_processors  # type: ignore
+            processors = index_processors  # type: ignore[assignment]
         self.enlist_sources(
             non_root_sources,
             ttl,
             update,
             client_config=client_config,
             index_processors=processors,
             only_index=True,
```

### Comparing `dvcx-0.78.2/src/dvcx/catalog/datasource.py` & `dvcx-0.79.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/catalog/formats.py` & `dvcx-0.79.0/src/dvcx/catalog/formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import tarfile
 import uuid
 from abc import ABC, abstractmethod
 from collections.abc import Iterable, Iterator
 from contextlib import AbstractContextManager
 from datetime import datetime, timezone
 from itertools import groupby, islice
+from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
+    ClassVar,
     Generic,
     Optional,
     TypeVar,
     Union,
 )
 
 import attrs
@@ -23,16 +25,14 @@
 from sqlalchemy.types import TypeEngine
 from tqdm import tqdm
 
 from dvcx.cache import UniqueId
 from dvcx.node import DirType, Entry, get_path
 
 if TYPE_CHECKING:
-    from types import TracebackType
-
     from dvcx.data_storage.schema import SignalsTable
     from dvcx.listing import Listing
     from dvcx.storage import StorageURI
 
 logger = logging.getLogger("dvcx")
 
 PROCESSING_BATCH_SIZE = 1000  # Batch size for inserting entries.
@@ -50,21 +50,21 @@
     for key, value in d.items():
         new_key = parent_key + delimiter + key if parent_key else key
         if value is None:
             continue
         if (isinstance(value, (dict, list))) and not value:
             # skipping empty lists and dicts
             continue
-        elif isinstance(value, list) and isinstance(value[0], list):
+        if isinstance(value, list) and isinstance(value[0], list):
             # skipping list of lists
             continue
-        elif isinstance(value, list) and isinstance(value[0], dict):
+        if isinstance(value, list) and isinstance(value[0], dict):
             # skipping list of dicts
             continue
-        elif isinstance(value, dict):
+        if isinstance(value, dict):
             items.extend(flatten_signals(value, new_key, delimiter=delimiter).items())
         else:
             items.append((new_key, value))
 
     return dict(items)
 
 
@@ -136,15 +136,15 @@
     def __call__(self, items):
         self.listing.warehouse.insert_nodes(items)
 
     def __exit__(
         self,
         exc_type: Optional[type[BaseException]],
         exc_val: Optional[BaseException],
-        exc_tb: Optional["TracebackType"],
+        exc_tb: Optional[TracebackType],
     ):
         self.listing.warehouse.insert_nodes_done()
 
 
 class InsertSignals(Operation):
     """Insert rows into a signals table."""
 
@@ -181,15 +181,15 @@
         self.table = self.listing.warehouse.create_signals_table()
         return self
 
     def __exit__(
         self,
         exc_type: Optional[type[BaseException]],
         exc_val: Optional[BaseException],
-        exc_tb: Optional["TracebackType"],
+        exc_tb: Optional[TracebackType],
     ):
         wh = self.listing.warehouse
         try:
             if exc_val is None:
                 wh.extend_index_with_signals(wh.nodes, self.table)
         finally:
             wh.db.execute(DropTable(self.table.table))
@@ -395,15 +395,18 @@
 class JSONPair(IndexingFormat[ObjectInfo]):
     """
     Load signals from .json files and attach them to objects with the same base name.
     """
 
     processing_message = "Loading json annotations"
 
-    IGNORED_EXTS = [".json", ".txt"]  # File extensions not to attach loaded signals to.
+    IGNORED_EXTS: ClassVar[list[str]] = [
+        ".json",
+        ".txt",
+    ]  # File extensions not to attach loaded signals to.
 
     def begin(self, listing: "Listing") -> Operation:
         return InsertJSONSignals(listing)
 
     def filter(self, listing: "Listing", paths: list[str]) -> Iterator[ObjectInfo]:
         for path in paths:
             for node in listing.expand_path(path):
@@ -449,15 +452,15 @@
         return os.path.splitext(entry.path)[0]
 
 
 def apply_processors(
     listing: "Listing", path: str, processors: list[IndexingFormat]
 ) -> None:
     for processor in processors:
-        msg = getattr(processor, "processing_message", None or "Processing")
+        msg = getattr(processor, "processing_message", "Processing")
         with processor.begin(listing) as op:
             with tqdm(desc=msg, unit=" objects") as pbar:
                 entries = processor.filter(listing.clone(), [path])
                 results = processor.process(listing.clone(), entries)
                 for batch in _batch(results, PROCESSING_BATCH_SIZE):
                     pbar.update(len(batch))
                     op(batch)
```

### Comparing `dvcx-0.78.2/src/dvcx/catalog/loader.py` & `dvcx-0.79.0/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/cli.py` & `dvcx-0.79.0/src/dvcx/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,15 +556,15 @@
         choices=shtab.SUPPORTED_SHELLS,
     )
 
 
 def get_logging_level(args: Namespace) -> int:
     if args.quiet:
         return logging.CRITICAL
-    elif args.verbose:
+    if args.verbose:
         return logging.DEBUG
     return logging.INFO
 
 
 def ls_urls(
     sources,
     catalog: "Catalog",
```

### Comparing `dvcx-0.78.2/src/dvcx/cli_utils.py` & `dvcx-0.79.0/src/dvcx/cli_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,22 +50,22 @@
             setattr(namespace, self.dest, not option_string.startswith("--no-"))
 
     def format_usage(self):
         return " | ".join(self.option_strings)
 
 
 class CommaSeparatedArgs(_AppendAction):  # pylint: disable=protected-access
-    def __call__(self, parser, namespace, values, option_string=None):  # noqa: ARG002
+    def __call__(self, parser, namespace, values, option_string=None):
         items = getattr(namespace, self.dest) or []
         items.extend(v for value in values.split(",") if (v := value.strip()))
         setattr(namespace, self.dest, list(dict.fromkeys(items)))
 
 
 class KeyValueArgs(_AppendAction):  # pylint: disable=protected-access
-    def __call__(self, parser, namespace, values, option_string=None):  # noqa: ARG002
+    def __call__(self, parser, namespace, values, option_string=None):
         items = getattr(namespace, self.dest) or {}
         for raw_value in filter(bool, values):
             key, sep, value = raw_value.partition("=")
             if not key or not sep or value == "":
                 raise ArgumentError(self, f"expected 'key=value', got {raw_value!r}")
             items[key.strip()] = value
```

### Comparing `dvcx-0.78.2/src/dvcx/client/azure.py` & `dvcx-0.79.0/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/client/fileslice.py` & `dvcx-0.79.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/client/fsspec.py` & `dvcx-0.79.0/src/dvcx/client/fsspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,19 @@
         from .azure import AzureClient
         from .gcs import GCSClient
         from .local import FileClient
         from .s3 import ClientS3
 
         if url.lower().startswith(ClientS3.PREFIX):
             return ClientS3
-        elif url.lower().startswith(GCSClient.PREFIX):
+        if url.lower().startswith(GCSClient.PREFIX):
             return GCSClient
-        elif url.lower().startswith(AzureClient.PREFIX):
+        if url.lower().startswith(AzureClient.PREFIX):
             return AzureClient
-        elif url.lower().startswith(FileClient.PREFIX) or url == "":
+        if url.lower().startswith(FileClient.PREFIX) or url == "":
             return FileClient
         raise RuntimeError(f"Unsupported data source format '{url}'")
 
     @staticmethod
     def parse_url(
         source: str,
         metastore: "AbstractMetastore",
@@ -173,19 +173,19 @@
         async def worker(queue) -> None:
             while True:
                 prefix = await queue.get()
                 try:
                     subdirs = await self._fetch_dir(prefix, progress_bar, result_queue)
                     for subdir in subdirs:
                         queue.put_nowait(subdir)
-                except Exception as exc:
+                except Exception:
                     while not queue.empty():
                         queue.get_nowait()
                         queue.task_done()
-                    raise exc
+                    raise
 
                 finally:
                     queue.task_done()
 
         try:
             workers = []
             for _ in range(FETCH_WORKERS):
@@ -283,15 +283,15 @@
             copy2(src, dst)
 
     def open_object(self, uid: UniqueId, use_cache: bool = True) -> BinaryIO:
         """Open a file, including files in tar archives."""
         if uid.vtype == "tar":
             return self._open_tar(uid, use_cache=True)
         if use_cache and (cache_path := self.cache.get_path(uid)):
-            return open(cache_path, mode="rb")
+            return open(cache_path, mode="rb")  # noqa: SIM115
         return self.fs.open(self.get_full_path(uid.path))
 
     def _open_tar(self, uid: UniqueId, use_cache: bool = True):
         assert uid.location is not None
         loc_stack = (
             json.loads(uid.location) if isinstance(uid.location, str) else uid.location
         )
```

### Comparing `dvcx-0.78.2/src/dvcx/client/gcs.py` & `dvcx-0.79.0/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/client/local.py` & `dvcx-0.79.0/src/dvcx/client/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 from fsspec.implementations.local import LocalFileSystem
 
 from dvcx.error import StorageNotFoundError
 from dvcx.node import Entry
+from dvcx.storage import StorageURI
 
-from ..storage import StorageURI
 from .fsspec import Client
 
 if TYPE_CHECKING:
     from dvcx.data_storage import AbstractMetastore
 
 
 class FileClient(Client):
```

### Comparing `dvcx-0.78.2/src/dvcx/client/s3.py` & `dvcx-0.79.0/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/config.py` & `dvcx-0.79.0/src/dvcx/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         raise Exception(
             f"missing config section for default remote: remote.{remote}"
         ) from None
     except Exception as exc:
         raise Exception("invalid config") from exc
 
     if not isinstance(remote_conf, Mapping):
-        raise Exception(f"config section remote.{remote} must be a mapping")
+        raise TypeError(f"config section remote.{remote} must be a mapping")
 
     remote_type = remote_conf.get("type")
     if remote_type not in ("local", "http"):
         raise Exception(
             f'config section remote.{remote} must have "type" with one of: '
             '"local", "http"'
         )
```

### Comparing `dvcx-0.78.2/src/dvcx/data_storage/db_engine.py` & `dvcx-0.79.0/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/data_storage/id_generator.py` & `dvcx-0.79.0/src/dvcx/data_storage/id_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,37 +23,37 @@
     unique IDs for each prefix (e.g. S3 bucket or dataset).
     """
 
     @abstractmethod
     def clone(self) -> "AbstractIDGenerator":
         """Clones AbstractIDGenerator implementation."""
 
-    def init(self) -> None:  # noqa: B027
+    def init(self) -> None:
         """Initialize ID generator."""
 
-    def cleanup_for_tests(self):  # noqa: B027
+    def cleanup_for_tests(self):
         """Cleanup for tests."""
 
     @abstractmethod
     def init_id(self, uri: str) -> None:
         """Initializes the ID generator for the given URI with zero last_id."""
 
     @abstractmethod
     def get_next_ids(self, uri: str, count: int) -> range:
         """Returns a range of IDs for the given URI."""
 
     def get_next_id(self, uri: str) -> int:
         """Returns the next ID for the given URI."""
         return self.get_next_ids(uri, 1)[0]
 
-    def delete_uri(self, uri: str):  # noqa: B027
+    def delete_uri(self, uri: str):
         """Deletes the given URI."""
         self.delete_uris([uri])
 
-    def delete_uris(self, uris: Iterable[str]):  # noqa: B027
+    def delete_uris(self, uris: Iterable[str]):
         """Deletes the given URIs."""
 
 
 class AbstractDBIDGenerator(AbstractIDGenerator):
     """
     Abstract ID Generator class, to be implemented by any Database Adapters
     for a specific database system. This class is responsible for generating
```

### Comparing `dvcx-0.78.2/src/dvcx/data_storage/metastore.py` & `dvcx-0.79.0/src/dvcx/data_storage/metastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,24 +74,24 @@
         use_new_connection: bool = False,
     ) -> "AbstractMetastore":
         """Clones AbstractMetastore implementation for some Storage input.
         Setting use_new_connection will always use a new database connection.
         New connections should only be used if needed due to errors with
         closed connections."""
 
-    def init(self, uri: StorageURI, partial_id: int) -> None:  # noqa: B027
+    def init(self, uri: StorageURI, partial_id: int) -> None:
         """Initialize metastore."""
 
-    def close(self) -> None:  # noqa: B027
+    def close(self) -> None:
         """Closes any active database or HTTP connections."""
 
-    def cleanup_temp_tables(self, temp_table_names: list[str]):  # noqa: B027
+    def cleanup_temp_tables(self, temp_table_names: list[str]):
         """Cleanup temp tables."""
 
-    def cleanup_for_tests(self):  # noqa: B027
+    def cleanup_for_tests(self):
         """Cleanup for tests."""
 
     #
     # Storages
     #
 
     @abstractmethod
@@ -115,15 +115,15 @@
             - boolean saying if this storage is newly created
         """
 
     @abstractmethod
     def find_stale_storages(self) -> None:
         """
         Finds all pending storages for which the last inserted node has happened
-        before STALE_HOURS_LIMIT hours, and marks it as STALE.
+        before STALE_MINUTES_LIMIT minutes, and marks it as STALE.
         """
 
     @abstractmethod
     def mark_storage_indexed(
         self,
         uri: StorageURI,
         status: int,
@@ -220,14 +220,15 @@
         script_output: str = "",
         created_at: Optional[datetime] = None,
         finished_at: Optional[datetime] = None,
         custom_column_types: Optional[dict[str, Any]] = None,
         ignore_if_exists: bool = False,
         num_objects: Optional[int] = None,
         size: Optional[int] = None,
+        preview: Optional[list[dict]] = None,
     ) -> DatasetRecord:
         """Creates new dataset version."""
 
     @abstractmethod
     def remove_dataset(self, dataset: DatasetRecord) -> None:
         """Removes dataset."""
 
@@ -449,14 +450,15 @@
             Column("created_at", DateTime(timezone=True)),
             Column("finished_at", DateTime(timezone=True)),
             Column("error_message", Text, nullable=False, default=""),
             Column("error_stack", Text, nullable=False, default=""),
             Column("script_output", Text, nullable=False, default=""),
             Column("num_objects", BigInteger, nullable=True),
             Column("size", BigInteger, nullable=True),
+            Column("preview", JSON, nullable=True),
             Column("job_id", Text, nullable=True),
             Column("sources", Text, nullable=False, default=""),
             Column("query_script", Text, nullable=False, default=""),
             Column("custom_column_types", JSON, nullable=True),
             UniqueConstraint("dataset_id", "version"),
         ]
 
@@ -714,15 +716,15 @@
 
             storage = self.mark_storage_pending(storage, conn=conn)
             return storage, True, False, None
 
     def find_stale_storages(self) -> None:
         """
         Finds all pending storages for which the last inserted node has happened
-        before STALE_HOURS_LIMIT hours, and marks it as STALE.
+        before STALE_MINUTES_LIMIT minutes, and marks it as STALE.
         """
         s = self._storages
         with self.db.transaction() as conn:
             pending_storages = map(
                 self.storage_class._make,
                 self.db.execute(
                     self._storages_select().where(s.c.status == StorageStatus.PENDING),
@@ -941,19 +943,17 @@
             query_script=query_script,
             custom_column_types=json.dumps(column_types),
         )
         if ignore_if_exists:
             query = query.on_conflict_do_nothing(index_elements=["name"])
         self.db.execute(query)
 
-        dataset = self.get_dataset(name)
+        return self.get_dataset(name)
 
-        return dataset
-
-    def create_dataset_version(
+    def create_dataset_version(  # noqa: PLR0913
         self,
         dataset: DatasetRecord,
         version: int,
         status: int = DatasetStatus.CREATED,
         sources: str = "",
         query_script: str = "",
         error_message: str = "",
@@ -961,14 +961,15 @@
         script_output: str = "",
         created_at: Optional[datetime] = None,
         finished_at: Optional[datetime] = None,
         custom_column_types: Optional[dict[str, Any]] = None,
         ignore_if_exists: bool = False,
         num_objects: Optional[int] = None,
         size: Optional[int] = None,
+        preview: Optional[list[dict]] = None,
         conn=None,
     ) -> DatasetRecord:
         """Creates new dataset version."""
         if status in [DatasetStatus.COMPLETE, DatasetStatus.FAILED]:
             finished_at = finished_at or datetime.now(timezone.utc)
         else:
             finished_at = None
@@ -983,14 +984,15 @@
             error_stack=error_stack,
             script_output=script_output,
             sources=sources,
             query_script=query_script,
             custom_column_types=json.dumps(custom_column_types or {}),
             num_objects=num_objects,
             size=size,
+            preview=json.dumps(preview) if preview else None,
         )
         if ignore_if_exists:
             query = query.on_conflict_do_nothing(
                 index_elements=["dataset_id", "version"]
             )
         self.db.execute(query, conn=conn)
 
@@ -1047,14 +1049,16 @@
         for field, value in kwargs.items():
             if field in self._dataset_version_fields[1:]:
                 if field == "custom_column_types":
                     dataset_version.update(
                         **{field: DatasetRecord.parse_custom_column_types(value)}
                     )
                     values[field] = json.dumps(value) if value else None
+                elif field == "preview" and isinstance(value, list):
+                    values[field] = json.dumps(value)
                 else:
                     values[field] = value
                     dataset_version.update(**{field: value})
 
         if not values:
             # Nothing to update
             return dataset_version
```

### Comparing `dvcx-0.78.2/src/dvcx/data_storage/schema.py` & `dvcx-0.79.0/src/dvcx/data_storage/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
     c_set: dict[str, sa.Column] = {}
     for c in columns:
         if ec := c_set.get(c.name, None):
             if str(ec.type) != str(c.type):
                 raise ValueError(
                     f"conflicting types for column {c.name}:"
-                    f"{str(c.type)} and {str(ec.type)}"
+                    f"{c.type!s} and {ec.type!s}"
                 )
             continue
         c_set[c.name] = c
 
     return list(c_set.values())
```

### Comparing `dvcx-0.78.2/src/dvcx/data_storage/serializer.py` & `dvcx-0.79.0/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/data_storage/sqlite.py` & `dvcx-0.79.0/src/dvcx/data_storage/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from contextlib import contextmanager
 from functools import wraps
 from time import sleep
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    ClassVar,
     Optional,
     Union,
 )
 
 import sqlalchemy
 from attrs import frozen
 from sqlalchemy import MetaData, Table, UniqueConstraint, exists, select
@@ -438,24 +439,20 @@
             raise ValueError("uri for init() cannot be empty")
         partials_table = self._partials_table(uri)
         self.db.create_table(partials_table, if_not_exists=True)
 
     @classmethod
     def _buckets_columns(cls) -> list["SchemaItem"]:
         """Buckets (storages) table columns."""
-        return super()._buckets_columns() + [
-            UniqueConstraint("uri"),
-        ]
+        return [*super()._buckets_columns(), UniqueConstraint("uri")]
 
     @classmethod
     def _datasets_columns(cls) -> list["SchemaItem"]:
         """Datasets table columns."""
-        return super()._datasets_columns() + [
-            UniqueConstraint("name"),
-        ]
+        return [*super()._datasets_columns(), UniqueConstraint("name")]
 
     def _storages_insert(self):
         return sqlite.insert(self._storages)
 
     def _partials_insert(self):
         return sqlite.insert(self._partials)
 
@@ -504,15 +501,15 @@
     This is currently used for the local cli.
     """
 
     id_generator: "SQLiteIDGenerator"
     db: "SQLiteDatabaseEngine"
 
     # Cache for our defined column types to dialect specific TypeEngine relations
-    _col_python_type: dict[type, "TypeEngine"] = {}
+    _col_python_type: ClassVar[dict[type, "TypeEngine"]] = {}
 
     def __init__(
         self,
         id_generator: "SQLiteIDGenerator",
         uri: StorageURI = StorageURI(""),
         partial_id: Optional[int] = None,
         db: Optional["SQLiteDatabaseEngine"] = None,
@@ -705,15 +702,15 @@
         )
 
     def insert_rows(self, table: Table, rows: Iterable[dict[str, Any]]) -> None:
         rows = list(rows)
         if not rows:
             return
         self.db.executemany(
-            table.insert().values({f: bindparam(f) for f in rows[0].keys()}),
+            table.insert().values({f: bindparam(f) for f in rows[0]}),
             rows,
         )
 
     def insert_dataset_rows(self, df, dataset: DatasetRecord, version: int) -> int:
         dr = self.dataset_rows(dataset, version)
         return self.db.insert_dataframe(dr.table.name, df)
```

### Comparing `dvcx-0.78.2/src/dvcx/data_storage/warehouse.py` & `dvcx-0.79.0/src/dvcx/data_storage/warehouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     ):
         self.id_generator = id_generator
         self.uri = uri
         self.partial_id: Optional[int] = partial_id
         self._nodes: Optional["schema.Node"] = None
         self.node_fields = [c.name for c in self.schema.node_cls.default_columns()]
 
-    def cleanup_for_tests(self):  # noqa: B027
+    def cleanup_for_tests(self):
         """Cleanup for tests."""
 
     def convert_type(self, val: Any, col_type: SQLType) -> Any:  # noqa: PLR0911
         """
         Tries to convert value to specific type if needed and if compatible,
         otherwise throws an ValueError.
         If value is a list or some other iterable, it tries to convert sub elements
@@ -111,27 +111,25 @@
                     if item_pyton_type == float and isinstance(val[0], int):
                         return [float(i) for i in val]
                 return [self.convert_type(i, col_type.item_type) for i in val]
             # special use case with JSON type as we save it as string
             if col_python_type == dict:
                 if value_type == str:
                     return val
-                elif value_type in (dict, list):
+                if value_type in (dict, list):
                     return json.dumps(val)
-                else:
-                    raise ValueError(
-                        f"Cannot convert value {val!r} with type"
-                        f"{value_type} to JSON"
-                    )
+                raise ValueError(
+                    f"Cannot convert value {val!r} with type" f"{value_type} to JSON"
+                )
 
             if isinstance(val, col_python_type):
                 return val
             if col_python_type == float and isinstance(val, int):
                 return float(val)
-        except Exception as e:
+        except Exception as e:  # noqa: BLE001
             exc = e
         raise ValueError(
             f"Value {val!r} with type {value_type} incompatible for "
             f"column type {type(col_type).__name__}"
         ) from exc
 
     @abstractmethod
@@ -215,15 +213,15 @@
                 cols.source,
                 cols.parent,
                 cols.name,
                 cols.version,
                 cols.etag,
             ]
         else:
-            ordering = order_by  # type: ignore
+            ordering = order_by  # type: ignore[assignment]
 
         # reset query order by and apply new order by id
         paginated_query = query.order_by(None).order_by(*ordering).limit(page_size)
 
         results = None
         offset = 0
         num_yielded = 0
@@ -348,14 +346,17 @@
         version: int,
         offset: Optional[int] = 0,
         limit: Optional[int] = 20,
         custom_columns=False,
         source: Optional[str] = None,
     ) -> Iterator[DatasetRow]:
         """Gets dataset rows."""
+        if not self.db.has_table(self.dataset_table_name(dataset.name, version)):
+            return
+
         # if custom_columns are to be returned, we are setting columns to None to
         # retrieve all columns from a table (default ones and custom)
         columns = list(DATASET_CORE_COLUMN_NAMES) if not custom_columns else None
         dr = self.dataset_rows(dataset, version)
 
         if not columns:
             # fetching all columns if specific columns are not defined
@@ -470,25 +471,25 @@
         Inserts file or directory node into the database
         """
 
     @abstractmethod
     def insert_nodes(self, entries: Iterable[Entry]) -> None:
         """Inserts file or directory nodes into the database"""
 
-    def insert_nodes_done(self):  # noqa: B027
+    def insert_nodes_done(self):
         """
         Only needed for certain implementations
         to signal when node inserts are complete.
         """
 
     @abstractmethod
     def insert_rows(self, table: Table, rows: Iterable[dict[str, Any]]) -> None:
         """Does batch inserts of any kind of rows into table"""
 
-    def insert_rows_done(self, table: Table) -> None:  # noqa: B027
+    def insert_rows_done(self, table: Table) -> None:
         """
         Only needed for certain implementations
         to signal when rows inserts are complete.
         """
 
     @abstractmethod
     def insert_dataset_rows(self, df, dataset: DatasetRecord, version: int) -> int:
@@ -599,15 +600,15 @@
         return self.get_nodes(query)
 
     def _get_nodes_by_glob_path_pattern(
         self, path_list: list[str], glob_name: str
     ) -> Iterator[Node]:
         """Finds all Nodes that correspond to GLOB like path pattern."""
         n = self.nodes
-        path_glob = "/".join(path_list + [glob_name])
+        path_glob = "/".join([*path_list, glob_name])
         dirpath = path_glob[: -len(glob_name)]
         relpath = func.substr(self.path_expr(n), len(dirpath) + 1)
 
         return self.get_nodes(
             n.select(*n.default_columns())
             .where(
                 (self.path_expr(n).op("GLOB")(path_glob))
@@ -655,15 +656,15 @@
         for curr_name in path_list[:-1]:
             if set(curr_name).intersection(GLOB_CHARS):
                 new_paths = []
                 for path in matched_paths:
                     nodes = self._get_nodes_by_glob_path_pattern(path, curr_name)
                     for node in nodes:
                         if node.is_container:
-                            new_paths.append(path + [node.name or ""])
+                            new_paths.append([*path, node.name or ""])
                 matched_paths = new_paths
             else:
                 for path in matched_paths:
                     path.append(curr_name)
         curr_name = path_list[-1]
         if set(curr_name).intersection(GLOB_CHARS):
             result: list[Node] = []
@@ -779,16 +780,15 @@
                     (self.path_expr(n).op("GLOB")(sub_glob)) & (n.c.is_latest == true())
                 )
             ),
             (0, 0),
         )
         if count_files:
             return results[0] or 0, results[1] or 0
-        else:
-            return results[0] or 0, 0
+        return results[0] or 0, 0
 
     def path_expr(self, t):
         return case((t.c.parent == "", t.c.name), else_=t.c.parent + "/" + t.c.name)
 
     def _find_query(
         self,
         node: Node,
```

### Comparing `dvcx-0.78.2/src/dvcx/dataset.py` & `dvcx-0.79.0/src/dvcx/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 )
 from urllib.parse import urlparse
 
 import attrs
 from dateutil.parser import isoparse
 
 from dvcx.sql.types import NAME_TYPES_MAPPING, SQLType
+from dvcx.utils import JSONSerialize
 
 from .cache import UniqueId
 
 if TYPE_CHECKING:
     from dvcx.storage import StorageURI
 
 T = TypeVar("T", bound="DatasetRecord")
@@ -77,15 +78,15 @@
     type: str
     name: str  # when the type is STORAGE, this is actually StorageURI
     version: str  # string until we'll have proper bucket listing versions
     created_at: datetime
     dependencies: list[Optional["DatasetDependency"]]
 
     @classmethod
-    def parse(  # noqa: PLR0913
+    def parse(
         cls: builtins.type[DD],
         id: int,
         dataset_id: Optional[int],
         dataset_version_id: Optional[int],
         bucket_id: Optional[int],
         bucket_version: Optional[str],
         dataset_name: Optional[str],
@@ -104,28 +105,27 @@
                     str(dataset_version)  # type: ignore[arg-type]
                     if dataset_version
                     else None
                 ),
                 dataset_version_created_at or dataset_created_at,  # type: ignore[arg-type]
                 [],
             )
-        elif bucket_uri:
+        if bucket_uri:
             return cls(
                 id,
                 DatasetDependencyType.STORAGE,
                 bucket_uri,
                 bucket_version,  # type: ignore[arg-type]
                 isoparse(bucket_version),  # type: ignore[arg-type]
                 [],
             )
-        else:
-            # dependency has been removed
-            # TODO we should introduce flags for removed datasets, instead of
-            # removing them from tables so that we can still have references
-            return None
+        # dependency has been removed
+        # TODO we should introduce flags for removed datasets, instead of
+        # removing them from tables so that we can still have references
+        return None
 
     @property
     def is_dataset(self) -> bool:
         return self.type == DatasetDependencyType.DATASET
 
     def __eq__(self, other):
         if not isinstance(other, DatasetDependency):
@@ -165,32 +165,34 @@
     finished_at: Optional[datetime]
     error_message: str
     error_stack: str
     script_output: str
     custom_column_types: dict[str, Union[SQLType, type[SQLType]]]
     num_objects: Optional[int]
     size: Optional[int]
+    preview: Optional[list["DatasetRow"]]
     job_id: Optional[str] = None
     sources: str = ""
     query_script: str = ""
 
     @classmethod
-    def parse(
+    def parse(  # noqa: PLR0913
         cls: type[V],
         id: int,
         dataset_id: int,
         version: int,
         status: int,
         created_at: datetime,
         finished_at: Optional[datetime],
         error_message: str,
         error_stack: str,
         script_output: str,
         num_objects: Optional[int],
         size: Optional[int],
+        preview: Optional[str],
         job_id: Optional[str],
         custom_column_types: dict[str, Union[SQLType, type[SQLType]]],
         sources: str = "",
         query_script: str = "",
     ):
         return cls(
             id,
@@ -201,14 +203,19 @@
             finished_at,
             error_message,
             error_stack,
             script_output,
             custom_column_types,
             num_objects,
             size,
+            (
+                [DatasetRow.from_preview_dict(row) for row in json.loads(preview)]
+                if preview
+                else None
+            ),
             job_id,
             sources,
             query_script,
         )
 
     def __eq__(self, other):
         if not isinstance(other, DatasetVersion):
@@ -302,14 +309,15 @@
         version_created_at: datetime,
         version_finished_at: Optional[datetime],
         version_error_message: str,
         version_error_stack: str,
         version_script_output: str,
         version_num_objects: Optional[int],
         version_size: Optional[int],
+        version_preview: Optional[str],
         version_job_id: Optional[str],
         version_sources: Optional[str],
         version_query_script: Optional[str],
         version_custom_column_types: str,
     ) -> "DatasetRecord":
         labels_lst: list[str] = json.loads(labels) if labels else []
         custom_column_types_dct: dict[str, Any] = (
@@ -329,14 +337,15 @@
             version_created_at,
             version_finished_at,
             version_error_message,
             version_error_stack,
             version_script_output,
             version_num_objects,
             version_size,
+            version_preview,
             version_job_id,
             cls.parse_custom_column_types(version_custom_column_types_dct),  # type: ignore[arg-type]
             version_sources,  # type: ignore[arg-type]
             version_query_script,  # type: ignore[arg-type]
         )
 
         return cls(
@@ -529,21 +538,56 @@
         del d["parent_id"]  # parent_id is deprecated
         d.update(d.pop("custom", {}))
         return d
 
     def __getitem__(self, col):
         if hasattr(self, col):
             return getattr(self, col)
-        elif self.custom and col in self.custom:
+        if self.custom and col in self.custom:
             return self.custom[col]
         raise KeyError
 
     def as_uid(self) -> UniqueId:
         return UniqueId(
             self.source,
             self.parent,
             self.name,
             self.etag,
             self.size,
             self.vtype,
             self.location,
         )
+
+    def to_preview_dict(self):
+        return {
+            "id": self.id,
+            "vtype": self.vtype,
+            "dir_type": self.dir_type,
+            "parent_id": self.parent_id,
+            "parent": self.parent,
+            "name": self.name,
+            "checksum": self.checksum,
+            "etag": self.etag,
+            "version": self.version,
+            "is_latest": self.is_latest,
+            "last_modified": (
+                self.last_modified.isoformat() if self.last_modified else None
+            ),
+            "size": self.size,
+            "owner_name": self.owner_name,
+            "owner_id": self.owner_id,
+            "anno": self.anno,
+            "random": self.random,
+            "location": self.location,
+            "source": self.source,
+            "custom": (
+                json.dumps(self.custom, cls=JSONSerialize) if self.custom else None
+            ),
+        }
+
+    @classmethod
+    def from_preview_dict(cls, row: dict[str, Any]) -> "DatasetRow":
+        if custom := row.pop("custom"):
+            row = {**row, **json.loads(custom)}
+        if last_modified := row.get("last_modified"):
+            row["last_modified"] = isoparse(last_modified)
+        return cls.from_dict(row)
```

### Comparing `dvcx-0.78.2/src/dvcx/error.py` & `dvcx-0.79.0/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/lib/cached_stream.py` & `dvcx-0.79.0/src/dvcx/lib/cached_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.cached_file = None
 
         self.temp_file = None
         self.temp_file_pos = 0
 
     def __enter__(self):
         if os.path.exists(self.target_path):
-            self.cached_file = open(self.target_path, mode=self.mode)
+            self.cached_file = open(self.target_path, mode=self.mode)  # noqa: SIM115
             return self.cached_file
 
         tmp_dir = self.catalog.cache.tmp_dir
         if not os.path.exists(tmp_dir):
             os.makedirs(tmp_dir)
         self.temp_file = tempfile.NamedTemporaryFile(
             prefix=str(self.uid.get_hash()), dir=tmp_dir, delete=False
@@ -103,15 +103,15 @@
         self.cached_file = None
 
     def get_path_in_cache(self):
         return self.catalog.cache.path_from_checksum(self.uid.get_hash())
 
     def __enter__(self):
         self.client.download(self.uid)
-        self.cached_file = open(self.get_path_in_cache(), self.mode)
+        self.cached_file = open(self.get_path_in_cache(), self.mode)  # noqa: SIM115
         return self.cached_file
 
     def __exit__(self, *args):
         self.cached_file.close()
 
 
 class PreDownloadStream(PreCachedStream):
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/claude.py` & `dvcx-0.79.0/src/dvcx/lib/claude.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from json import JSONDecodeError
 from typing import Literal
 
 import anthropic
 from anthropic.types import Usage
 from anthropic.types.message import Message
+from pydantic import Field
 
 from dvcx.lib.feature import Feature
 from dvcx.lib.feature_types import FeatureLike, pydantic_to_feature
 from dvcx.lib.feature_udf import FeatureAggregator, FeatureMapper
 from dvcx.lib.file import FileInfo, TextFile
 
 default_model_name = "claude-3-haiku-20240307"
@@ -26,15 +27,15 @@
     status: Literal["Success", "Failure"] = "Failure"
     explanation: str = ""
     usage: UsageFeature = UsageFeature(input_tokens=0, output_tokens=0)  # type: ignore[valid-type,call-arg]
     error: str = ""
 
 
 class Summary(Feature):
-    reasons: list[str] = []
+    reasons: list[str] = Field(default_factory=list)
     usage: UsageFeature = UsageFeature(input_tokens=0, output_tokens=0)  # type: ignore[valid-type,call-arg]
     error: str = ""
 
 
 class ClaudeClient:
     def __init__(
         self,
@@ -68,20 +69,20 @@
         self.model = None
 
     def llm_call(self, text):
         try:
             response = self.model.messages.create(  # type: ignore[attr-defined]
                 model=self.model_name,
                 system=self.prompt,
-                messages=[{"role": "user", "content": text}] + self.messages,
+                messages=[{"role": "user", "content": text}, *self.messages],
                 **self.kwargs,
             )
 
             return Claude(**response.model_dump())
-        except Exception as exc:
+        except Exception as exc:  # noqa: BLE001
             return Claude(
                 id="",
                 content=[],
                 model="",
                 role="assistant",
                 type="message",
                 usage={"input_tokens": 0, "output_tokens": 0},
@@ -96,15 +97,15 @@
             text = claude.content[0].text
             try:
                 j = json.loads(text)
                 response = Rating(**j)
                 response.usage = claude.usage
             except JSONDecodeError as exc:
                 response = Rating(
-                    error=f"json parsing error '{text}': {str(exc)}", usage=claude.usage
+                    error=f"json parsing error '{text}': {exc!s}", usage=claude.usage
                 )
         else:
             response = Rating(
                 status="Failure", error="no responses", usage=claude.usage
             )
         return response
 
@@ -153,13 +154,13 @@
                     result = Summary(reasons=j, usage=claude.usage)
                 else:
                     result = Summary(
                         error=f"result is not list but '{j}'", usage=claude.usage
                     )
             except JSONDecodeError as exc:
                 result = Summary(
-                    error=f"json parsing error '{text}': {str(exc)}", usage=claude.usage
+                    error=f"json parsing error '{text}': {exc!s}", usage=claude.usage
                 )
         else:
             result = Summary(error=claude.error, usage=claude.usage)
 
         yield FileInfo(name="", vtype="claude-agg"), result
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/dataset.py` & `dvcx-0.79.0/src/dvcx/lib/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,16 +371,15 @@
 
         return fr._to_udf_spec()
 
     def _extend_features(self, method_name, *args):
         super_func = getattr(super(), method_name)
 
         columns = self._args_to_columns(*args)
-        res = super_func(*columns)
-        return res
+        return super_func(*columns)
 
     @detach
     def select(self, *args, **kwargs) -> "Self":
         return self._extend_features("select", *args)
 
     @detach
     def select_except(self, *args) -> "Self":
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/feature.py` & `dvcx-0.79.0/src/dvcx/lib/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", name)
         return re.sub("([a-z0-9])([A-Z])", r"\1_\2", s1).lower()
 
     @staticmethod
     def _convert_type(typ):  # noqa: PLR0911
         if inspect.isclass(typ) and issubclass(typ, SQLType):
             return typ
-        res = TYPE_TO_DVCX.get(typ, None)
+        res = TYPE_TO_DVCX.get(typ)
         if res:
             return res
 
         orig = get_origin(typ)
 
         if orig in (Literal, LiteralEx):
             return String
@@ -133,19 +133,18 @@
             return Feature._convert_type(args[0])
 
         # Special case for list in JSON: Union[dict, list[dict]]
         if orig == Union and len(args) >= 2:
             args_no_nones = [arg for arg in args if arg != type(None)]
             if len(args_no_nones) == 2:
                 args_no_dicts = [arg for arg in args_no_nones if arg != dict]
-                if len(args_no_dicts) == 1:
-                    if get_origin(args_no_dicts[0]) == list:
-                        arg = get_args(args_no_dicts[0])
-                        if len(arg) == 1 and arg[0] == dict:
-                            return JSON
+                if len(args_no_dicts) == 1 and get_origin(args_no_dicts[0]) == list:
+                    arg = get_args(args_no_dicts[0])
+                    if len(arg) == 1 and arg[0] == dict:
+                        return JSON
 
         raise RuntimeError(f"Cannot recognize type {typ}")
 
     @staticmethod
     def _iter_fields(fields):
         for name, f_info in fields.items():
             yield name, f_info.annotation, f_info.is_required()
@@ -162,23 +161,23 @@
                     anno = anno[0]
                 is_list = True
             else:
                 is_list = False
 
             expanded_name = name
             if cls._expand_name:
-                lst = [cls._prefix()] + name_path + [name]
+                lst = [cls._prefix(), *name_path, name]
                 expanded_name = cls._delimiter.join(lst)
 
             if Feature._is_feature_class(anno):
                 if is_list:
                     yield expanded_name, Array(JSON), is_required
                 else:
                     yield from cls._flatten_full_schema(
-                        anno.model_fields, name_path + [name]
+                        anno.model_fields, [*name_path, name]
                     )
             else:
                 typ = Feature._convert_type(anno)
                 if is_list:
                     typ = Array(typ)
                 yield expanded_name, typ, is_required
 
@@ -204,15 +203,15 @@
         )
 
     def _flatten_fields_values(self, fields, dump):
         for name, anno, _ in self._iter_fields(fields):
             value = dump[name]
             if (
                 inspect.isclass(anno)
-                and not anno.__module__ == "builtins"
+                and anno.__module__ != "builtins"
                 and issubclass(anno, Feature)
             ):
                 yield from self._flatten_fields_values(anno.model_fields, value)
             else:
                 yield value
 
     def _flatten(self):
@@ -233,16 +232,15 @@
                 curr_path = name_norm
 
             if inspect.isclass(anno) and issubclass(anno, Feature):
                 val = anno._unflatten_with_path(dump, curr_path)
                 res[name] = val
             else:
                 res[name] = dump[curr_path]
-        r = cls(**res)
-        return r
+        return cls(**res)
 
     @classmethod
     def _unflatten(cls, dump):
         return cls._unflatten_with_path(dump, cls._prefix())
 
 
 class RestrictedAttribute:
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/feature_types.py` & `dvcx-0.79.0/src/dvcx/lib/feature_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
             if is_list:
                 anno = list[anno]  # type: ignore[valid-type]
         fields[name] = (anno, field_info.default)
 
     cls = create_model(
         data_cls.__name__,
-        __base__=(data_cls, Feature),  # type: ignore
+        __base__=(data_cls, Feature),  # type: ignore[call-overload]
         **fields,
     )
     feature_registry[data_cls] = cls
     return cls
 
 
 class FeatureTypes:
@@ -80,15 +80,15 @@
             name = name.name
 
         fields = {name: (typ, default)}
         new_class_name = f"{new_class.__name__}_{name}"
 
         obj = create_model(
             new_class_name,
-            __base__=new_class,  # type: ignore
+            __base__=new_class,  # type: ignore[call-overload]
             **fields,
         )
 
         obj._get_column_value = lambda self: getattr(self, name)
 
         if value_func:
             obj.get_value = lambda self: value_func(obj._get_column_value(self))
@@ -113,15 +113,15 @@
         }
 
         cls_suffix = "_".join(fields_text_keys.keys())
         new_class = ShallowFeature
 
         obj = create_model(
             f"{new_class.__name__}_{cls_suffix}",
-            __base__=new_class,  # type: ignore
+            __base__=new_class,  # type: ignore[call-overload]
             **fields_text_keys,
         )
 
         obj._get_column_value = lambda self: tuple(
             [getattr(self, name) for name in fields_text_keys]
         )
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/feature_udf.py` & `dvcx-0.79.0/src/dvcx/lib/feature_udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 
 class ValidationError(DvcxError):
     pass
 
 
 class SchemaError(ValidationError):
     def __init__(self, udf_name: str, context: str, message: str):
-        super().__init__(
-            f"'{udf_name}' {context} " f"schema validation error: {message}"
-        )
+        super().__init__(f"'{udf_name}' {context} schema validation error: {message}")
 
 
 class OutputError(ValidationError):
     def __init__(self, udf_name: str, message: str, num: Optional[int] = None):
         num_str = "" if num is None else f"#{num + 1} "
         super().__init__(f"Output {num_str}of '{udf_name}' error: {message}")
 
@@ -81,25 +79,23 @@
 
     @staticmethod
     def get_flattened_params(fr_classes: Sequence[type[Feature]]):
         udf_params_spec = Feature._features_to_udf_spec(fr_classes)
         stream_prm = (
             [Stream()] if FeatureConverter.has_feature_stream(fr_classes) else []
         )
-        param_list = stream_prm + list(udf_params_spec.keys())
-        return param_list
+        return stream_prm + list(udf_params_spec.keys())
 
     @staticmethod
     def _convert_to_sequence(
         arg: Union[FeatureLike, Sequence[FeatureLike]],
     ) -> tuple[Sequence[type[Feature]], bool]:
         if not isinstance(arg, Sequence):
             return FeatureTypes._to_features(*[arg]), True
-        else:
-            return FeatureTypes._to_features(*arg), False
+        return FeatureTypes._to_features(*arg), False
 
     @staticmethod
     def deserialize(
         rows: Sequence[Sequence],
         params: Sequence[str],
         fr_classes: Sequence[type[Feature]],
         catalog: Catalog,
@@ -233,15 +229,15 @@
         return res
 
     def run_user_code(self, obj_rows):
         try:
             result_objs = self._udf.process(obj_rows)
             if inspect.isgeneratorfunction(self._udf.process):
                 result_objs = list(result_objs)
-        except Exception as e:
+        except Exception as e:  # noqa: BLE001
             msg = (
                 f"============== Error in user code: '{self._udf.name}' =============="
             )
             print(msg)
             exc_type, exc_value, exc_traceback = sys.exc_info()
             traceback.print_exception(exc_type, exc_value, exc_traceback.tb_next)
             print("=" * len(msg))
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/file.py` & `dvcx-0.79.0/src/dvcx/lib/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import json
 from abc import ABC, abstractmethod
 from datetime import datetime
 from pathlib import Path
 from random import getrandbits
-from typing import Optional, Union
+from typing import ClassVar, Optional, Union
 
 from pydantic import Field, field_validator
 
 from dvcx.cache import UniqueId
 from dvcx.lib.cached_stream import PreCachedStream, PreDownloadStream
 from dvcx.lib.feature import ShallowFeature
 from dvcx.lib.utils import DvcxError
 from dvcx.utils import TIME_ZERO
 
 
 class FileFeature(ShallowFeature):
     _is_file = True
 
     def set_file(self, stream, caching_enabled: bool) -> None:
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def open(self):
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def read(self):
         with self.open() as stream:
             return stream.read()
 
     def get_value(self):
         return self.read()
@@ -46,15 +46,15 @@
     @classmethod
     @abstractmethod
     def open(cls, file: "File", location: list[dict]):
         pass
 
 
 class VFileRegistry:
-    _vtype_readers: dict[str, type["VFile"]] = {}
+    _vtype_readers: ClassVar[dict[str, type["VFile"]]] = {}
 
     @classmethod
     def register(cls, reader: type["VFile"]):
         cls._vtype_readers[reader.get_vtype()] = reader
 
     @classmethod
     def resolve(cls, file: "File", location: list[dict]):
@@ -77,26 +77,34 @@
     name: str
     version: str = Field(default="")
     etag: str = Field(default="")
     size: int = Field(default=0)
     vtype: str = Field(default="")
     location: Optional[Union[dict, list[dict]]] = Field(default=None)
 
-    _unique_id_keys = ["source", "parent", "name", "etag", "size", "vtype", "location"]
+    _unique_id_keys: ClassVar[list[str]] = [
+        "source",
+        "parent",
+        "name",
+        "etag",
+        "size",
+        "vtype",
+        "location",
+    ]
 
     @staticmethod
     def to_dict(
         v: Optional[Union[str, dict, list[dict]]],
     ) -> Optional[Union[str, dict, list[dict]]]:
         if v is None or v == "":
             return None
         if isinstance(v, str):
             try:
                 return json.loads(v)
-            except Exception as e:
+            except Exception as e:  # noqa: BLE001
                 raise ValueError(
                     f"Unable to convert string '{v}' to dict for File feature: {e}"
                 ) from None
         return v
 
     # Workaround for empty JSONs converted to empty strings in some DBs.
     @field_validator("location", mode="before")
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.79.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.79.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 try:
-    import numpy
+    import numpy as np
     import torch
     from PIL import Image, ImageOps, UnidentifiedImageError
     from transformers import (
         AutoProcessor,
         Blip2ForConditionalGeneration,
         Blip2Processor,
         LlavaForConditionalGeneration,
@@ -25,23 +25,21 @@
 def encode_image(raw):
     try:
         img = Image.open(raw)
     except UnidentifiedImageError:
         return None
     img.load()
     img = img.convert("RGB")
-    img = ImageOps.fit(img, DEFAULT_FIT_BOX)
-    return img
+    return ImageOps.fit(img, DEFAULT_FIT_BOX)
 
 
 def infer_dtype(device):
     if device == "cpu":
         return torch.float32
-    else:
-        return torch.float16
+    return torch.float16
 
 
 @udf(
     params=(Object(encode_image),),  # Columns consumed by the UDF.
     output={
         "description": String,
         "error": String,
@@ -57,15 +55,15 @@
             model, torch_dtype=self.torch_dtype
         )
         self.device = device
         self.model.to(device)
         self.max_tokens = max_tokens
 
     def describe(self, imgs):
-        images = numpy.squeeze(numpy.asarray(imgs))
+        images = np.squeeze(np.asarray(imgs))
         inputs = self.processor(images=images, return_tensors="pt").to(
             self.device, self.torch_dtype
         )
 
         generated_ids = self.model.generate(**inputs, max_new_tokens=self.max_tokens)
         generated_text = self.processor.batch_decode(
             generated_ids, skip_special_tokens=True
@@ -91,15 +89,15 @@
             model, torch_dtype=self.torch_dtype, low_cpu_mem_usage=True
         )
         self.model.to(device)
         self.max_tokens = max_tokens
         self.prompt = "USER: <image>\nDescribe this picture\nASSISTANT:"
 
     def describe(self, imgs):
-        images = numpy.squeeze(numpy.asarray(imgs))
+        images = np.squeeze(np.asarray(imgs))
         inputs = self.processor(
             text=[self.prompt] * len(imgs), images=images, return_tensors="pt"
         ).to(self.device, self.torch_dtype)
 
         generated_ids = self.model.generate(**inputs, max_new_tokens=self.max_tokens)
         generated_text = self.processor.batch_decode(
             generated_ids, skip_special_tokens=True
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.79.0/src/dvcx/lib/hf_pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,26 +20,23 @@
 
 def read_image(raw):
     try:
         img = Image.open(raw)
     except UnidentifiedImageError:
         return None
     img.load()
-    img = img.convert("RGB")
-    return img
+    return img.convert("RGB")
 
 
 def read_object(raw):
-    buffer = raw.read()
-    return buffer
+    return raw.read()
 
 
 def read_text(raw):
-    buffer = read_object(raw).decode("utf-8")
-    return buffer
+    return read_object(raw).decode("utf-8")
 
 
 @udf(
     params=(Object(read_image),),  # Columns consumed by the UDF.
     output={
         "model_output": JSON,
         "error": String,
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/image.py` & `dvcx-0.79.0/src/dvcx/lib/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     if mode:
         img = img.convert(mode)
     if size:
         img = img.resize(size)
     if transform:
         img = transform(img)
         if open_clip_model:
-            img = img.unsqueeze(0)  # type: ignore
+            img = img.unsqueeze(0)  # type: ignore[attr-defined]
     if open_clip_model:
         method_name = "encode_image"
         if not (
             hasattr(open_clip_model, method_name)
             and inspect.ismethod(getattr(open_clip_model, method_name))
         ):
             raise ValueError(
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/image_transform.py` & `dvcx-0.79.0/src/dvcx/lib/image_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     img = Image.open(raw)
     img.load()
     return img
 
 
 @udf(
     output=DatasetRow.schema,
-    params=(Object(load_image),) + tuple(DatasetRow.schema.keys()),
+    params=(Object(load_image), *tuple(DatasetRow.schema.keys())),
 )
 class ImageTransform:
     def __init__(
         self,
         *,
         image_filter,
         bucket_name,
@@ -36,16 +36,15 @@
         self.prefix = prefix
         self.vtype = vtype
 
         catalog = get_catalog()
         self.client, _ = catalog.parse_url(os.path.join(self.prefix, bucket_name))
 
     def apply_filter(self, image):
-        image_b = image.filter(self.image_filter)
-        return image_b
+        return image.filter(self.image_filter)
 
     def save(self, image, source, name, format):
         # Make name for new image
         new_name = f"{self.file_prefix}{name}"
 
         # Do writeback
         blob_name = os.path.join(self.folder_name, new_name)
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.79.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,25 @@
     },  # Signals being returned by the UDF.
     method="image_description",
 )
 class GetMetadata:
     def cast(self, v):  # to JSON serializable types
         if isinstance(v, TiffImagePlugin.IFDRational):
             return float(v)
-        elif isinstance(v, tuple):
+        if isinstance(v, tuple):
             return tuple(self.cast(t) for t in v)
-        elif isinstance(v, bytes):
+        if isinstance(v, bytes):
             return v.decode(encoding="utf-8", errors="ignore")
-        elif isinstance(v, dict):
+        if isinstance(v, dict):
             for kk, vv in v.items():
                 v[kk] = self.cast(vv)
             return v
-        elif isinstance(v, list):
-            vv = [self.cast(kk) for kk in v]
-            return vv
-        else:
-            return v
+        if isinstance(v, list):
+            return [self.cast(kk) for kk in v]
+        return v
 
     def image_description(self, img):
         (xmp, exif, iptc) = ({}, {}, {})
         if img is None:
             error = "Image format not understood"
             return ({}, {}, {}, error)
         error = ""
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/pytorch.py` & `dvcx-0.79.0/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/lib/reader.py` & `dvcx-0.79.0/src/dvcx/lib/reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/lib/tar_file.py` & `dvcx-0.79.0/src/dvcx/lib/tar_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/lib/text.py` & `dvcx-0.79.0/src/dvcx/lib/text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/lib/udf.py` & `dvcx-0.79.0/src/dvcx/lib/udf.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         raise ValueError(
             f"UDF '{func_name}' output type must be str or int"
             f" while {return_annotation} was provided"
         )
 
     def _validate_result_type(self, results, *args):
         if not isinstance(results, tuple):
-            raise ValueError(
+            raise TypeError(
                 f"{self.name} returned {type(results)} values"
                 f" while tuple was expected. Inputs: {args} Result: {results}"
             )
 
     def _validate_result_length(self, results, *args):
         out_len = len(self.output)
         res_len = len(results)
@@ -123,15 +123,15 @@
             )
 
     def _validate_result_batch_length(self, results, *args):
         out_len = len(self.output)
 
         for res in results:
             if not isinstance(res, tuple):
-                raise ValueError(
+                raise TypeError(
                     f"{self.name} must return a sequence of tuples."
                     f" This may occur if using 'return' instead of 'yield'."
                     f" Inputs: {args} Result: {res}"
                 )
 
             res_len = len(res)
             if out_len != res_len:
@@ -165,16 +165,15 @@
         self._validate_result_length(results, *args)
         return results
 
     @classmethod
     def from_func(cls, func, params=None, output=None, batch=1) -> "Mapper":
         if batch == 1:
             return super()._from_func(func, params, output)
-        else:
-            return super(Mapper, BatchMapper)._from_func(func, params, output, batch)
+        return super(Mapper, BatchMapper)._from_func(func, params, output, batch)
 
 
 class BatchMapper(Mapper):
     def __init__(self, params=None, output=None, batch=1000):
         if batch == 1:
             raise ValueError(f"{self.name} must be batch UDF")
         UDFBase.__init__(self, params, output, batch)
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/unstructured.py` & `dvcx-0.79.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/lib/utils.py` & `dvcx-0.79.0/src/dvcx/lib/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,39 +7,37 @@
 class DvcxError(Exception):
     def __init__(self, message):
         super().__init__(message)
 
 
 def row_to_pandas(args, params):
     data = dict(zip([i.name for i in params], args))
-    return pd.Series(data, name=data.get("name", None))
+    return pd.Series(data, name=data.get("name"))
 
 
 def row_list_to_pandas(args, params):
-    df = pd.DataFrame(args, columns=[i.name for i in params])
-    return df
+    return pd.DataFrame(args, columns=[i.name for i in params])
 
 
 def bin_to_array(data):
-    integers = [
+    return [
         int.from_bytes(data[i : i + 4], byteorder="big") for i in range(0, len(data), 4)
     ]
-    return integers
 
 
 def array_to_bin(integers):
     return b"".join(int.to_bytes(i, length=4, byteorder="big") for i in integers)
 
 
 def union_dicts(*dicts):
     """Union dictionaries.
     Equivalent to `d1 | d2 | d3` in Python3.9+ but works in older versions.
     """
     result = None
     for d in dicts:
         if not isinstance(d, dict):
-            raise ValueError("All arguments must be dictionaries.")
+            raise TypeError("All arguments must be dictionaries.")
         if not result:
             result = d.copy()
         else:
             result.update(d)
     return result
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/webdataset.py` & `dvcx-0.79.0/src/dvcx/lib/webdataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import hashlib
 import json
 import tarfile
 from collections.abc import Sequence
-from typing import Optional, Union, get_args, get_origin
+from typing import Any, ClassVar, Optional, Union, get_args, get_origin
 
 from pydantic import Field
 
 from dvcx.lib.feature import Feature
 from dvcx.lib.feature_udf import FeatureGenerator
 from dvcx.lib.file import File, FileInfo
 from dvcx.lib.tar_file import TarVFile
@@ -49,15 +49,15 @@
     cap: Optional[str] = Field(default=None)
     transcript: Optional[str] = Field(default=None)
     cls: Optional[int] = Field(default=None)
     cls2: Optional[int] = Field(default=None)
     index: Optional[int] = Field(default=None)
     inx: Optional[int] = Field(default=None)
     id: Optional[int] = Field(default=None)
-    json: Optional[dict] = Field(default=None)  # type: ignore
+    json: Optional[dict] = Field(default=None)  # type: ignore[assignment]
     jsn: Optional[dict] = Field(default=None)
 
     pyd: Optional[bytes] = Field(default=None)
     pickle: Optional[bytes] = Field(default=None)
     pth: Optional[bytes] = Field(default=None)
     ten: Optional[bytes] = Field(default=None)
     tb: Optional[bytes] = Field(default=None)
@@ -67,26 +67,26 @@
     npz: Optional[bytes] = Field(default=None)
     cbor: Optional[bytes] = Field(default=None)
 
 
 class WDSReadableSubclass(Feature):
     @staticmethod
     def _reader(builder, item: tarfile.TarInfo) -> "WDSReadableSubclass":
-        raise NotImplementedError()
+        raise NotImplementedError
 
 
 class BuilderState:
     def __init__(self):
         self.stem = None
         self.core_file = None
         self.data = {}
 
 
 class Builder:
-    DEFAULT_TYPES_READERS = {
+    DEFAULT_TYPES_READERS: ClassVar[dict[type, Any]] = {
         str: lambda bld, item: bld.read_text(item),
         int: lambda bld, item: int(bld.read_text(item)),
         float: lambda bld, item: float(bld.read_text(item)),
         bytes: lambda bld, item: bld.read(item),
         dict: lambda bld, item: json.loads(bld.read_text(item)),
     }
 
@@ -113,15 +113,15 @@
 
     def add(self, file: tarfile.TarInfo):
         fstream = File(name=file.name)
         ext = fstream.get_file_ext()
         stem = fstream.get_file_stem()
 
         if self.state.stem is not None and self.state.stem != stem:
-            raise StopIteration()
+            raise StopIteration
 
         if self.state.stem is None:
             self.state.stem = stem
 
         if ext in self._core_extensions:
             if self.state.core_file is not None:
                 raise CoreFileDuplicationError(
@@ -200,15 +200,15 @@
 
 
 class TarStream(File):
     @staticmethod
     def to_text(data):
         return data.decode("utf-8")
 
-    _DATA_CONVERTERS = {
+    _DATA_CONVERTERS: ClassVar[dict[type, Any]] = {
         str: lambda data: TarStream.to_text(data),
         int: lambda data: int(TarStream.to_text(data)),
         float: lambda data: float(TarStream.to_text(data)),
         bytes: lambda data: data,
         dict: lambda data: json.loads(TarStream.to_text(data)),
     }
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.79.0/src/dvcx/lib/webdataset_laion.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
     @staticmethod
     def _reader(builder, item):
         return Laion.model_validate_json(builder.read_text(item))
 
 
 class WDSLaion(WDSBasic):
     txt: Optional[str] = Field(default=None)
-    json: Laion  # type: ignore
+    json: Laion  # type: ignore[assignment]
```

### Comparing `dvcx-0.78.2/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.79.0/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/listing.py` & `dvcx-0.79.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/node.py` & `dvcx-0.79.0/src/dvcx/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 def get_path(parent: str, name: str):
     return f"{parent}/{name}" if parent else name
 
 
 @attrs.define
 class NodeWithPath:
     n: Node
-    path: list[str] = []
+    path: list[str] = attrs.field(factory=list)
 
     def append_to_file(self, fd):
         return self.n.append_to_file(fd, "/".join(self.path))
 
     def get_metafile_data(self):
         return self.n.get_metafile_data("/".join(self.path))
```

### Comparing `dvcx-0.78.2/src/dvcx/nodes_fetcher.py` & `dvcx-0.79.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/nodes_thread_pool.py` & `dvcx-0.79.0/src/dvcx/nodes_thread_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,15 @@
         if node:
             bucket.append(node)
             total_size += node.size
             total_files += 1
 
         if bucket:
             return bucket
-        else:
-            raise StopIteration
+        raise StopIteration
 
 
 class NodesThreadPool(ABC):
     def __init__(self, max_threads):
         self._max_threads = max_threads
         self._thread_counter = 0
         self._thread_lock = threading.Lock()
```

### Comparing `dvcx-0.78.2/src/dvcx/progress.py` & `dvcx-0.79.0/src/dvcx/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,23 @@
     BYTES_DEFAULTS: ClassVar[dict[str, Any]] = {
         "unit": "B",
         "unit_scale": True,
         "unit_divisor": 1024,
         "miniters": 1,
     }
 
-    def __init__(  # noqa: PLR0913
+    def __init__(
         self,
         iterable=None,
         disable=None,
         level=logging.ERROR,
         desc=None,
         leave=False,
         bar_format=None,
-        bytes=False,  # noqa: A002
+        bytes=False,
         file=None,
         total=None,
         postfix=None,
         **kwargs,
     ):
         """
         bytes   : shortcut for
```

### Comparing `dvcx-0.78.2/src/dvcx/query/batch.py` & `dvcx-0.79.0/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/query/builtins.py` & `dvcx-0.79.0/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/query/dataset.py` & `dvcx-0.79.0/src/dvcx/query/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import contextlib
-import datetime
 import inspect
 import json
 import logging
 import os
 import random
 import re
 import string
@@ -48,15 +47,15 @@
 )
 from dvcx.dataset import DatasetRow
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DatasetNotFoundError, QueryScriptCancelError
 from dvcx.sql.functions import rand
 from dvcx.sql.types import SQLType
 from dvcx.storage import StorageURI
-from dvcx.utils import chunk, determine_processes
+from dvcx.utils import JSONSerialize, chunk, determine_processes
 
 from .batch import DatasetRowsBatch
 from .schema import C, UDFParamSpec, normalize_param
 from .session import Session
 from .udf import UDFBase, UDFClassWrapper, UDFFactory, UDFType
 
 if TYPE_CHECKING:
@@ -350,16 +349,19 @@
         # validate and convert type if needed and possible
         try:
             # check if type is already instantiated or not
             col_type = col_type() if inspect.isclass(col_type) else col_type
             row[col_name] = warehouse.convert_type(row_val, col_type)
         except ValueError as e:
             logger.exception(
-                f"Error while validating/converting type for column "
-                f"{col_name} with value {row_val}, original error {e}"
+                "Error while validating/converting type for column "
+                "%s with value %s, original error %s",
+                col_name,
+                row_val,
+                e,  # noqa: TRY401
             )
             raise
     return row
 
 
 def process_udf_outputs(
     warehouse: "AbstractWarehouse",
@@ -684,15 +686,15 @@
         def q(*columns):
             cols1 = []
             cols2 = []
             for c in columns:
                 if c.name in partition_col_names:
                     continue
                 cols.append(signal_name_cols.get(c.name, c))
-                if c.name in signal_name_cols.keys():
+                if c.name in signal_name_cols:
                     cols2.append(c)
                 else:
                     cols1.append(c)
 
             if cols2:
                 res = (
                     sqlalchemy.select(*cols1)
@@ -909,27 +911,25 @@
                 q2_c = q2.c.get(c.name)
 
                 if c.table.name == q1.name and q1_c is None:
                     raise ValueError(
                         f"Column {c.name} was not found in left part of the join"
                     )
 
-                elif c.table.name == q2.name and q2_c is None:
+                if c.table.name == q2.name and q2_c is None:
                     raise ValueError(
                         f"Column {c.name} was not found in right part of the join"
                     )
-                elif c.table.name not in [q1.name, q2.name]:
+                if c.table.name not in [q1.name, q2.name]:
                     raise ValueError(
                         f"Column {c.name} was not found in left or right"
                         " part of the join"
                     )
-                else:
-                    continue
-            else:
-                self.validate_expression(c, q1, q2)
+                continue
+            self.validate_expression(c, q1, q2)
 
     def apply(
         self, query_generator: QueryGenerator, temp_tables: list[str]
     ) -> StepResult:
         q1 = self.query1.apply_steps().select().subquery(self.query1.table.name)
         temp_tables.extend(self.query1.temp_table_names)
         q2 = self.query2.apply_steps().select().subquery(self.query2.table.name)
@@ -956,15 +956,15 @@
             if isinstance(p, ColumnClause):
                 expressions.append(self.query1.c(p.name) == self.query2.c(p.name))
             elif isinstance(p, str):
                 expressions.append(self.query1.c(p) == self.query2.c(p))
             elif isinstance(p, ColumnElement):
                 expressions.append(p)
             else:
-                raise ValueError(f"Unsupported predicate {p} for join expression")
+                raise TypeError(f"Unsupported predicate {p} for join expression")
 
         if not expressions:
             raise ValueError("Missing predicates")
 
         join_expression = sqlalchemy.and_(*expressions)
         self.validate_expression(join_expression, q1, q2)
 
@@ -1178,15 +1178,15 @@
                 no_limit_steps.append(step)
         # Chunk the limit
         if limit:
             limit_modulo = limit % total
             limit = limit // total
             if index < limit_modulo:
                 limit += 1
-            return no_limit_steps + [SQLLimit(limit)]
+            return [*no_limit_steps, SQLLimit(limit)]
         return steps
 
     def cleanup(self) -> None:
         """Cleanup any temporary tables."""
         if not self.temp_table_names:
             # Nothing to clean up.
             return
@@ -1202,16 +1202,15 @@
         self.temp_table_names = []
 
     def results(self, row_factory=None, **kwargs):
         with self.as_iterable(**kwargs) as result:
             if row_factory:
                 cols = result.columns
                 return [row_factory(cols, r) for r in result]
-            else:
-                return list(result)
+            return list(result)
 
     @contextlib.contextmanager
     def as_iterable(self, **kwargs) -> Iterator[ResultIter]:
         try:
             query = self.apply_steps().select()
             selected_columns = [c.name for c in query.columns]
             yield ResultIter(
@@ -1677,15 +1676,15 @@
                 sqlalchemy.insert(dr.get_table()).from_select(cols, q),
                 **kwargs,
             )
 
             self.catalog.metastore.update_dataset_status(
                 dataset, DatasetStatus.COMPLETE, version=version
             )
-            self.catalog.update_dataset_version_with_stats(dataset, version)
+            self.catalog.update_dataset_version_with_warehouse_info(dataset, version)
 
             self._add_dependencies(dataset, version)  # type: ignore [arg-type]
         finally:
             self.cleanup()
 
         return DatasetQuery(name=name, version=version, catalog=self.catalog)
 
@@ -1708,22 +1707,14 @@
     preview: list[dict] = attrs.field(factory=list)
     dataset: Optional[tuple[str, int]] = None
 
 
 def _send_result(
     dataset_query: DatasetQuery, dataset: Optional[tuple[str, int]] = None
 ):
-    class JSONSerialize(json.JSONEncoder):
-        def default(self, obj):
-            if isinstance(obj, (datetime.datetime, datetime.date)):
-                return obj.isoformat()
-            if isinstance(obj, bytes):
-                return [f"{b:02x}" for b in obj[:1024]]
-            return super().default(obj)
-
     try:
         preview_args: dict[str, Any] = json.loads(
             os.getenv("DVCX_QUERY_PREVIEW_ARGS", "")
         )
     except ValueError:
         preview_args = {}
```

### Comparing `dvcx-0.78.2/src/dvcx/query/dispatch.py` & `dvcx-0.79.0/src/dvcx/query/dispatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
 
             if hasattr(self.udf.func, "teardown") and callable(self.udf.func.teardown):
                 self.udf.func.teardown()
 
             put_into_queue(self.done_queue, {"status": FINISHED_STATUS})
         except (Exception, KeyboardInterrupt) as e:
             put_into_queue(self.done_queue, {"status": FAILED_STATUS, "exception": e})
-            raise e
+            raise
 
     def _call_udf(self, row):
         if not self.initialized:
             raise RuntimeError("Internal Error: Attempted to call uninitialized UDF!")
         return self.udf(
             self.catalog, row, is_generator=self.is_generator, cache=self.cache
         )
```

### Comparing `dvcx-0.78.2/src/dvcx/query/params.py` & `dvcx-0.79.0/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/query/schema.py` & `dvcx-0.79.0/src/dvcx/query/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import functools
 import json
 from abc import ABC, abstractmethod
 from datetime import datetime, timezone
 from fnmatch import fnmatch
 from random import getrandbits
-from typing import TYPE_CHECKING, Any, Callable, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Optional, Union
 
 import attrs
 import sqlalchemy as sa
 
 from dvcx.data_storage.warehouse import RANDOM_BITS
-from dvcx.sql.types import JSON, Boolean, DateTime, Int, String
+from dvcx.sql.types import JSON, Boolean, DateTime, Int, SQLType, String
 
 if TYPE_CHECKING:
     from dvcx.catalog import Catalog
     from dvcx.dataset import DatasetRow as Row
 
 
 class ColumnMeta(type):
-    def __getattr__(cls, name: str):  # noqa: N805
+    def __getattr__(cls, name: str):
         return cls(name)
 
 
 class Column(sa.ColumnClause, metaclass=ColumnMeta):
     inherit_cache: Optional[bool] = True
 
     def __init__(self, text, type_=None, is_literal=False, _selectable=None):
@@ -120,54 +120,51 @@
     then only files matching the glob will be returned,
     otherwise None will be returned.
     """
 
     glob: Optional[str] = None
 
     def get_value(self, catalog: "Catalog", row: "Row", **kwargs) -> Optional[str]:
-        if self.glob:
-            if not fnmatch(row.name, self.glob):  # type: ignore[type-var]
-                # If the glob pattern is specified and the row filename
-                # does not match it, then return None
-                return None
+        if self.glob and not fnmatch(row.name, self.glob):  # type: ignore[type-var]
+            # If the glob pattern is specified and the row filename
+            # does not match it, then return None
+            return None
         client = catalog.get_client(row.source)
         uid = row.as_uid()
         client.download(uid)
         return client.cache.get_path(uid)
 
     async def get_value_async(
         self, catalog: "Catalog", row: "Row", mapper, **kwargs
     ) -> Optional[str]:
-        if self.glob:
-            if not fnmatch(row.name, self.glob):  # type: ignore[type-var]
-                # If the glob pattern is specified and the row filename
-                # does not match it, then return None
-                return None
+        if self.glob and not fnmatch(row.name, self.glob):  # type: ignore[type-var]
+            # If the glob pattern is specified and the row filename
+            # does not match it, then return None
+            return None
         client = catalog.get_client(row.source)
         uid = row.as_uid()
         await client._download(uid)
         return client.cache.get_path(uid)
 
 
 UDFParamSpec = Union[str, Column, UDFParameter]
 
 
 def normalize_param(param: UDFParamSpec) -> UDFParameter:
     if isinstance(param, str):
         return ColumnParameter(param)
-    elif isinstance(param, Column):
+    if isinstance(param, Column):
         return ColumnParameter(param.name)
-    elif isinstance(param, UDFParameter):
+    if isinstance(param, UDFParameter):
         return param
-    else:
-        raise TypeError(f"Invalid UDF parameter: {param}")
+    raise TypeError(f"Invalid UDF parameter: {param}")
 
 
 class DatasetRow:
-    schema = {
+    schema: ClassVar[dict[str, type[SQLType]]] = {
         "source": String,
         "parent": String,
         "name": String,
         "size": Int,
         "location": JSON,
         "vtype": String,
         "dir_type": Int,
```

### Comparing `dvcx-0.78.2/src/dvcx/query/session.py` & `dvcx-0.79.0/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/query/udf.py` & `dvcx-0.79.0/src/dvcx/query/udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         raise TypeError(f"'output' must be a mapping, got {type(output).__name__}")
 
     properties = UDFProperties([normalize_param(p) for p in params], output, batch)
 
     def decorator(udf_base: Union[Callable, type]):
         if isclass(udf_base):
             return UDFClassWrapper(udf_base, properties, method=method)
-        elif callable(udf_base):
+        if callable(udf_base):
             return UDFWrapper(udf_base, properties)
 
     return decorator
 
 
 class UDFBase:
     """A base class for implementing stateful UDFs."""
@@ -123,23 +123,22 @@
     ) -> Iterable[UDFResult]:
         if isinstance(param, DatasetRowsBatch):
             udf_inputs = [
                 self.parameter_parser(catalog, row, cache=cache) for row in param.rows
             ]
             udf_outputs = self.func(udf_inputs)
             return self._process_results(param.rows, udf_outputs, is_generator)
-        elif isinstance(param, DatasetRow):
+        if isinstance(param, DatasetRow):
             udf_inputs = self.parameter_parser(catalog, param, cache=cache)
             udf_outputs = self.func(*udf_inputs)
             if not is_generator:
                 # udf_outputs is generator already if is_generator=True
                 udf_outputs = [udf_outputs]
             return self._process_results([param], udf_outputs, is_generator)
-        else:
-            raise ValueError(f"unexpected UDF parameter {param}")
+        raise ValueError(f"unexpected UDF parameter {param}")
 
     def _process_results(
         self,
         rows: Sequence["DatasetRow"],
         results: Sequence[Sequence[Any]],
         is_generator=False,
     ) -> Iterable[UDFResult]:
```

### Comparing `dvcx-0.78.2/src/dvcx/remote/studio.py` & `dvcx-0.79.0/src/dvcx/remote/studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,16 +126,16 @@
         try:
             data = json.loads(response.content.decode("utf-8"))
         except json.decoder.JSONDecodeError:
             data = {}
 
         if not ok:
             logger.error(
-                f'Got bad response from Studio'
-                f', content is {response.content.decode("utf-8")}'
+                "Got bad response from Studio, content is %s",
+                response.content.decode("utf-8"),
             )
             if response.status_code == 403:
                 message = "Not authorized"
             else:
                 message = data.get("message", "")
         else:
             message = ""
@@ -158,16 +158,15 @@
 
             timestamp = values[0]
             if has_timezone:
                 timezone_offset = values[1]
                 return datetime.fromtimestamp(
                     timestamp, timezone(timedelta(seconds=timezone_offset))
                 )
-            else:
-                return datetime.fromtimestamp(timestamp)
+            return datetime.fromtimestamp(timestamp)  # noqa: DTZ006
 
         return msgpack.ExtType(code, data)
 
     def ls(self, paths: Iterable[str]) -> Iterator[tuple[str, Response[LsData]]]:
         # TODO: change LsData (response.data value) to be list of lists
         # to handle cases where a path will be expanded (i.e. globs)
         response: Response[LsData]
```

### Comparing `dvcx-0.78.2/src/dvcx/sql/default/base.py` & `dvcx-0.79.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/sql/functions/array.py` & `dvcx-0.79.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/sql/functions/path.py` & `dvcx-0.79.0/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/sql/selectable.py` & `dvcx-0.79.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/sql/sqlite/base.py` & `dvcx-0.79.0/src/dvcx/sql/sqlite/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     if setup_is_complete:
         return
 
     # sqlite 3.31.1 is the earliest version tested in CI
     if sqlite3.sqlite_version_info < (3, 31, 1):
         logger.warning(
             "Possible sqlite incompatibility. The earliest tested version of "
-            f"sqlite is 3.31.1 but you have {sqlite3.sqlite_version}"
+            "sqlite is 3.31.1 but you have %s",
+            sqlite3.sqlite_version,
         )
 
     # We want to show tracebacks for user-defined functions
     sqlite3.enable_callback_tracebacks(True)
     sqlite3.register_adapter(datetime, adapt_datetime)
     sqlite3.register_converter("datetime", convert_datetime)
 
@@ -98,15 +99,15 @@
     """
     Returns True if all function names are defined for the given connection.
     """
 
     names = list(names)
     for n in names:
         if not isinstance(n, str):
-            raise ValueError(
+            raise TypeError(
                 "functions_exist(): names argument must contain str values. "
                 f"Found value of type {type(n).__name__}: {n!r}"
             )
 
     if connection is None:
         connection = sqlite3.connect(":memory:")
```

### Comparing `dvcx-0.78.2/src/dvcx/sql/sqlite/types.py` & `dvcx-0.79.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/sql/types.py` & `dvcx-0.79.0/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/sql/utils.py` & `dvcx-0.79.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/src/dvcx/storage.py` & `dvcx-0.79.0/src/dvcx/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime, timedelta, timezone
 from functools import cached_property
 from typing import NamedTuple, NewType, Optional, Union
 from urllib.parse import urlparse
 
 from dvcx.utils import is_expired, time_to_local_str, time_to_str
 
-STALE_HOURS_LIMIT = 4
+STALE_MINUTES_LIMIT = 15
 
 # StorageURI represents a normalised URI to a valid storage location (full bucket or
 # absolute local path).
 # Valid examples: s3://foo, file:///var/data
 # Invalid examples: s3://foo/, s3://foo/bar, file://~
 StorageURI = NewType("StorageURI", str)
 
@@ -85,15 +85,15 @@
 
     @property
     def is_pending(self) -> bool:
         return self.status == Status.PENDING
 
     @property
     def is_stale(self) -> bool:
-        limit = datetime.now(timezone.utc) - timedelta(hours=STALE_HOURS_LIMIT)
+        limit = datetime.now(timezone.utc) - timedelta(minutes=STALE_MINUTES_LIMIT)
         date_to_check = self.last_inserted_at or self.started_inserting_at
 
         return self.is_pending and date_to_check < limit  # type: ignore [operator]
 
     @property
     def need_indexing(self) -> bool:
         return self.is_expired or not self.is_indexed
```

### Comparing `dvcx-0.78.2/src/dvcx/utils.py` & `dvcx-0.79.0/src/dvcx/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import importlib.util
+import json
 import os
 import os.path as osp
 import random
 import stat
 import sys
 import time
 from collections.abc import Iterable, Sequence
-from datetime import datetime, timezone
+from datetime import date, datetime, timezone
 from itertools import islice
 from typing import TYPE_CHECKING, Any, Optional, TypeVar, Union
+from uuid import UUID
 
 from dateutil import tz
 from dateutil.parser import isoparse
 
 if TYPE_CHECKING:
     import pandas as pd
 
@@ -113,15 +115,15 @@
 
 def time_to_local_str(dt: Union[datetime, str]) -> str:
     return time_to_str(time_to_local(dt))
 
 
 def is_expired(expires: Optional[Union[datetime, str]]):
     if expires:
-        return time_to_local(expires) < time_to_local(datetime.now())
+        return time_to_local(expires) < time_to_local(datetime.now())  # noqa: DTZ005
 
     return False
 
 
 SIZE_SUFFIXES = ["", "K", "M", "G", "T", "P", "E", "Z", "Y", "R", "Q"]
 
 
@@ -349,7 +351,19 @@
 
     if not records:
         return
 
     index = [row.pop("id") for row in records]
     df = pd.DataFrame.from_records(records, index=index)
     return show_df(df, collapse_columns=collapse_columns, system_columns=system_columns)
+
+
+class JSONSerialize(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, bytes):
+            return [f"{b:02x}" for b in obj[:1024]]
+        if isinstance(obj, (datetime, date)):
+            return obj.isoformat()
+        if isinstance(obj, UUID):
+            return str(obj)
+
+        return super().default(obj)
```

### Comparing `dvcx-0.78.2/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.79.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.78.2
+Version: 0.79.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.78.2/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.79.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -195,23 +195,26 @@
 tests/unit/test_query_params.py
 tests/unit/test_serializer.py
 tests/unit/test_session.py
 tests/unit/test_storage.py
 tests/unit/test_udf.py
 tests/unit/test_utils.py
 tests/unit/test_warehouse.py
+tests/unit/lib/__init__.py
 tests/unit/lib/test_cached_stream.py
 tests/unit/lib/test_feature.py
 tests/unit/lib/test_feature_udf.py
 tests/unit/lib/test_file.py
 tests/unit/lib/test_image.py
 tests/unit/lib/test_reader.py
 tests/unit/lib/test_text.py
 tests/unit/lib/test_webdataset.py
 tests/unit/lib/test_webdataset_meta.py
+tests/unit/sql/__init__.py
 tests/unit/sql/test_array.py
 tests/unit/sql/test_conditional.py
 tests/unit/sql/test_path.py
 tests/unit/sql/test_random.py
 tests/unit/sql/test_selectable.py
 tests/unit/sql/test_string.py
+tests/unit/sql/sqlite/__init__.py
 tests/unit/sql/sqlite/test_utils.py
```

### Comparing `dvcx-0.78.2/src/dvcx.egg-info/requires.txt` & `dvcx-0.79.0/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/benchmarks/conftest.py` & `dvcx-0.79.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/conftest.py` & `dvcx-0.79.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from dvcx.catalog.loader import get_id_generator, get_metastore, get_warehouse
 from dvcx.data_storage.sqlite import (
     SQLiteDatabaseEngine,
     SQLiteIDGenerator,
     SQLiteMetastore,
     SQLiteWarehouse,
 )
-from dvcx.dataset import DatasetRecord
+from dvcx.dataset import DatasetRecord, DatasetRow
 from dvcx.query.session import Session
 from dvcx.utils import DVCXDir, get_env_list
 
 from .utils import DEFAULT_TREE, get_simple_ds_query, instantiate_tree
 
 DEFAULT_DVCX_BIN = "dvcx"
 DEFAULT_DVCX_GIT_REPO = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
@@ -489,7 +489,53 @@
         description="",
         labels=[],
         versions=[],
         shadow=False,
         status=1,
         custom_column_types={},
     )
+
+
+@pytest.fixture
+def dataset_rows():
+    int_example = 25
+    return [
+        DatasetRow.from_dict(
+            {
+                "id": i,
+                "location": "",
+                "source": "s3://my-bucket",
+                "dir_type": 0,
+                "vtype": "",
+                "parent_id": None,
+                "parent": "input/text_emd_1m",
+                "version": "7e589b7d-382c-49a5-931f-2b999c930c5e",
+                "is_latest": True,
+                "name": f"dql_1m_meta_text_emd.parquet_3_{i}_0.snappy.parquet",
+                "etag": f"72b35c8e9b8eed1636c91eb94241c2f8-{i}",
+                "owner_id": "owner",
+                "owner_name": "aws-iterative-sandbox",
+                "last_modified": "2024-02-23T10:42:31.842944+00:00",
+                "size": 49807360,
+                "checksum": "",
+                "anno": None,
+                "random": 12123123123,
+                "custom": {
+                    "int_col": 5,
+                    "int_col_32": 5,
+                    "int_col_64": 5,
+                    "float_col": 0.5,
+                    "float_col_32": 0.5,
+                    "float_col_64": 0.5,
+                    "array_col": [0.5],
+                    "array_col_nested": [[0.5]],
+                    "array_col_32": [0.5],
+                    "array_col_64": [0.5],
+                    "string_col": "a string",
+                    "bool_col": True,
+                    "json_col": '{"a": 1}',
+                    "binary_col": int_example.to_bytes(2, "big"),
+                },
+            }
+        )
+        for i in range(19)
+    ]
```

### Comparing `dvcx-0.78.2/tests/data.py` & `dvcx-0.79.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/func/test_catalog.py` & `dvcx-0.79.0/tests/func/test_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 from dvcx.cli import garbage_collect
 from dvcx.error import (
     QueryScriptCompileError,
     QueryScriptDatasetNotFound,
     QueryScriptRunError,
     StorageNotFoundError,
 )
-
-from ..data import ENTRIES
-from ..utils import (
+from tests.data import ENTRIES
+from tests.utils import (
     DEFAULT_TREE,
     TARRED_TREE,
     WEBFORMAT_TREE,
+    assert_row_names,
     make_index,
     skip_if_not_sqlite,
     tree_from_path,
 )
 
 
 @pytest.fixture
@@ -939,20 +939,25 @@
     from dvcx.query import C, DatasetQuery
     DatasetQuery({src_uri!r})
     """
     query_script = dedent(query_script)
 
     dataset, version, query_output, _ = catalog.query(query_script, save=True)
     assert dataset
-    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
+    assert_row_names(
+        catalog,
+        dataset,
+        version,
+        {
+            "dog1",
+            "dog2",
+            "dog3",
+            "dog4",
+        },
+    )
     assert dataset.query_script == query_script
     assert dataset.sources == ""
 
 
 def test_query_save_size(cloud_test_catalog, mock_popen_dataset_created):
     catalog = cloud_test_catalog.catalog
     src_uri = cloud_test_catalog.src_uri
```

### Comparing `dvcx-0.78.2/tests/func/test_client.py` & `dvcx-0.79.0/tests/func/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 import pytest
 from fsspec.asyn import sync
 from tqdm import tqdm
 
 from dvcx.asyn import get_loop
 from dvcx.client import Client
-
-from ..data import ENTRIES
+from tests.data import ENTRIES
 
 
 @pytest.fixture
 def client(cloud_server, cloud_server_credentials):
     uri = cloud_server.src_uri
     return Client.get_implementation(uri).from_source(
         uri, cache=None, **cloud_server.client_config
@@ -29,15 +28,15 @@
 
 async def find(client, prefix):
     results = []
     try:
         async for entries in client.scandir(prefix):
             results.extend(entries)
     except BaseException as exc:
-        print(f"find: {repr(exc)}")
+        print(f"find: {exc!r}")
         raise
     return results
 
 
 def scandir(client, prefix):
     return sync(get_loop(), find, client, prefix)
```

### Comparing `dvcx-0.78.2/tests/func/test_dataset_query.py` & `dvcx-0.79.0/tests/func/test_dataset_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,23 +47,23 @@
     Float64,
     Int,
     Int32,
     Int64,
     SQLType,
     String,
 )
-
-from ..data import ENTRIES
-from ..utils import (
+from tests.data import ENTRIES
+from tests.utils import (
     DEFAULT_TREE,
     NUM_TREE,
     SIMPLE_DS_QUERY_RECORDS,
     TARRED_TREE,
     WEBFORMAT_TREE,
     adjusted_float_diff,
+    assert_row_names,
     dataset_dependency_asdict,
     insert_nodes,
     text_embedding,
 )
 
 
 @pytest.fixture
@@ -231,19 +231,17 @@
 )
 def test_instance_returned_after_save(cloud_test_catalog, dogs_cats_dataset):
     catalog = cloud_test_catalog.catalog
     ds = DatasetQuery(name=dogs_cats_dataset.name, version=1, catalog=catalog)
 
     ds2 = ds.save("dogs_cats_2")
     assert isinstance(ds2, DatasetQuery)
-    assert (
-        {row.name for row in catalog.ls_dataset_rows(dogs_cats_dataset.name, 1)}
-        == {row.name for row in catalog.ls_dataset_rows("dogs_cats_2", 1)}
-        == {"cat1", "cat2", "dog1", "dog2", "dog3", "dog4"}
-    )
+    expected_names = {"cat1", "cat2", "dog1", "dog2", "dog3", "dog4"}
+    assert_row_names(catalog, dogs_cats_dataset, 1, expected_names)
+    assert_row_names(catalog, catalog.get_dataset("dogs_cats_2"), 1, expected_names)
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
@@ -331,21 +329,18 @@
     indirect=True,
 )
 def test_chain_after_save(cloud_test_catalog, dogs_cats_dataset):
     catalog = cloud_test_catalog.catalog
     ds = DatasetQuery(name=dogs_cats_dataset.name, version=1, catalog=catalog)
     ds.filter(C.name.glob("dog*")).save("ds1").filter(C.size < 4).save("ds2")
 
-    assert {row.name for row in catalog.ls_dataset_rows("ds1", 1)} == {
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
-    assert {row.name for row in catalog.ls_dataset_rows("ds2", 1)} == {"dog2"}
+    assert_row_names(
+        catalog, catalog.get_dataset("ds1"), 1, {"dog1", "dog2", "dog3", "dog4"}
+    )
+    assert_row_names(catalog, catalog.get_dataset("ds2"), 1, {"dog2"})
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
@@ -1447,15 +1442,15 @@
         r["sig1"] == 1 and r["sig2"] == int_default
         for r in joined_records
         if r["name"] in cat_records_names
     )
     # check core duplicated columns
     for r in joined_records:
         dog_r = next(dr for dr in dogs_cats_records if dr["name"] == r["name"])
-        assert all([r[f"{k}_right"] == dog_r[k]] for k in dog_r.keys())
+        assert all([r[f"{k}_right"] == dog_r[k]] for k in dog_r)
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
@@ -1506,15 +1501,15 @@
         r["sig1"] == 1 and r["sig2"] == int_default
         for r in joined_records
         if r["name"] in cat_records_names
     )
     # check core duplicated columns
     for r in joined_records:
         dog_r = next(dr for dr in dogs_cats_records if dr["name"] == r["name"])
-        assert all([r[f"{k}_right"] == dog_r[k]] for k in dog_r.keys())
+        assert all([r[f"{k}_right"] == dog_r[k]] for k in dog_r)
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
@@ -1751,26 +1746,26 @@
         name=dogs_dataset.name, version=1, catalog=catalog
     ).to_records()
 
     # check custom columns
     assert all(r["sig1"] == 1 and r["sig2"] == 2 for r in joined_records)
     for r in joined_records:
         dog_r = next(dr for dr in dogs_records if dr["name"] == r["name"])
-        assert all([r[f"{k}_right"] == dog_r[k]] for k in dog_r.keys())
+        assert all([r[f"{k}_right"] == dog_r[k]] for k in dog_r)
 
     # joining on multiple fields
     joined_records = dogs_cats.join(dogs, ["parent", "name"], inner=True).to_records()
     assert len(joined_records) == 4
 
     # check custom columns
     assert all(r["sig1"] == 1 and r["sig2"] == 2 for r in joined_records)
     # check core duplicated columns
     for r in joined_records:
         dog_r = next(dr for dr in dogs_records if dr["name"] == r["name"])
-        assert all([r[f"{k}_right"] == dog_r[k]] for k in dog_r.keys())
+        assert all([r[f"{k}_right"] == dog_r[k]] for k in dog_r)
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
@@ -1793,15 +1788,15 @@
     assert len(joined_records) == 4
 
     # check custom columns
     assert all(r["sig1"] == 1 and r["sig1_right"] == 1 for r in joined_records)
     # check core duplicated columns
     for r in joined_records:
         dog_r = next(dr for dr in dogs_records if dr["name"] == r["name"])
-        assert all([r[f"{k}_right"] == dog_r[k]] for k in dog_r.keys())
+        assert all([r[f"{k}_right"] == dog_r[k]] for k in dog_r)
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
@@ -1843,15 +1838,15 @@
     dogs1 = DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
     dogs2 = DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
 
     with pytest.raises(ValueError) as excinfo:
         dogs1.join(dogs2, []).to_records()
     assert str(excinfo.value) == "Missing predicates"
 
-    with pytest.raises(ValueError) as excinfo:
+    with pytest.raises(TypeError) as excinfo:
         dogs1.join(dogs2, [[]]).to_records()
     assert str(excinfo.value) == "Unsupported predicate [] for join expression"
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
@@ -2227,16 +2222,16 @@
     catalog = cloud_test_catalog.catalog
 
     @udf(("name", "parent"), DatasetRow.extend(cnt=Int))
     def gen(inputs):
         cnt = len(inputs)
         for name, parent in inputs:
             parent_path = name if not parent else f"{parent}/{name}"
-            yield DatasetRow.create("subobject", size=50, parent=parent_path) + (cnt,)
-            yield DatasetRow.create("subobject2", size=70, parent=parent_path) + (cnt,)
+            yield (*DatasetRow.create("subobject", size=50, parent=parent_path), cnt)
+            yield (*DatasetRow.create("subobject2", size=70, parent=parent_path), cnt)
 
     result = (
         DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
         .generate(gen, partition_by="parent")
         .to_records()
     )
     parents_names = [(r["parent"], r["name"], r["cnt"]) for r in result]
@@ -2271,16 +2266,16 @@
     )
 
     @udf(("name", "parent"), DatasetRow.extend(cnt=Int))
     def gen(inputs):
         cnt = len(inputs)
         for name, parent in inputs:
             parent_path = name if not parent else f"{parent}/{name}"
-            yield DatasetRow.create("subobject", size=50, parent=parent_path) + (cnt,)
-            yield DatasetRow.create("subobject2", size=70, parent=parent_path) + (cnt,)
+            yield (*DatasetRow.create("subobject", size=50, parent=parent_path), cnt)
+            yield (*DatasetRow.create("subobject2", size=70, parent=parent_path), cnt)
 
     q = DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog).generate(
         gen, partition_by="parent", parallel=-1
     )
     result = q.to_records()
 
     parents_names = [(r["parent"], r["name"], r["cnt"]) for r in result]
@@ -2307,16 +2302,16 @@
     catalog = cloud_test_catalog.catalog
 
     @udf(("name", "parent"), DatasetRow.extend(cnt=Int), batch=2)
     def gen(inputs):
         cnt = len(inputs)
         for name, parent in inputs:
             parent_path = name if not parent else f"{parent}/{name}"
-            yield DatasetRow.create("subobject", size=50, parent=parent_path) + (cnt,)
-            yield DatasetRow.create("subobject2", size=70, parent=parent_path) + (cnt,)
+            yield (*DatasetRow.create("subobject", size=50, parent=parent_path), cnt)
+            yield (*DatasetRow.create("subobject2", size=70, parent=parent_path), cnt)
 
     result = (
         DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
         .generate(gen, partition_by="parent")
         .to_records()
     )
     parents_names = [(r["parent"], r["name"], r["cnt"]) for r in result]
@@ -2370,15 +2365,16 @@
     )
     class Subobjects:
         def __init__(self):
             pass
 
         def generate_subobjects(self, name, parent):
             parent_path = name if not parent else f"{parent}/{name}"
-            yield DatasetRow.create("subobject", size=50, parent=parent_path) + (
+            yield (
+                *DatasetRow.create("subobject", size=50, parent=parent_path),
                 "some_string",
                 10,
                 11,
                 12,
                 True,
                 0.5,
                 0.5,
@@ -2439,18 +2435,18 @@
         [0.5, 0.5],
         [[0.5], [0.5]],
         [0.5, 0.5],
         [0.5, 0.5],
     )
 
     assert col_values == [
-        ("dogs/dog1", "subobject") + new_col_values,
-        ("dogs/dog2", "subobject") + new_col_values,
-        ("dogs/dog3", "subobject") + new_col_values,
-        ("dogs/others/dog4", "subobject") + new_col_values,
+        ("dogs/dog1", "subobject", *new_col_values),
+        ("dogs/dog2", "subobject", *new_col_values),
+        ("dogs/dog3", "subobject", *new_col_values),
+        ("dogs/others/dog4", "subobject", *new_col_values),
     ]
 
     dataset = catalog.get_dataset("dogs_with_rows_and_signals")
     default_dataset_custom_column_types = {
         c.name: c.type.__class__
         for c in catalog.warehouse.dataset_row_cls.default_columns()
         if isinstance(c.type, SQLType)
@@ -2558,18 +2554,18 @@
         )
         for r in result
     ]
 
     col_values.sort(key=lambda x: (x[1], x[0]))
 
     assert col_values == [
-        ("dogs/dog1", "subobject") + new_col_values_empty,
-        ("dogs/dog2", "subobject") + new_col_values_empty,
-        ("dogs/dog3", "subobject") + new_col_values_empty,
-        ("dogs/others/dog4", "subobject") + new_col_values_empty,
+        ("dogs/dog1", "subobject", *new_col_values_empty),
+        ("dogs/dog2", "subobject", *new_col_values_empty),
+        ("dogs/dog3", "subobject", *new_col_values_empty),
+        ("dogs/others/dog4", "subobject", *new_col_values_empty),
     ]
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
@@ -2597,15 +2593,16 @@
     )
     class Subobjects:
         def __init__(self):
             pass
 
         def generate_subobjects(self, name, parent):
             parent_path = name if not parent else f"{parent}/{name}"
-            yield DatasetRow.create("subobject", size=50, parent=parent_path) + (
+            yield (
+                *DatasetRow.create("subobject", size=50, parent=parent_path),
                 np.int32(11),
                 np.int64(12),
                 np.float32(0.5),
                 np.float64(0.5),
                 np.int32(13),
                 np.array([[0.5], [0.5]], dtype=np.float32),
                 np.array([0.5, 0.5], dtype=np.float32),
@@ -2651,18 +2648,18 @@
         [0.5, 0.5],
         [0.5, 0.5],
         [14.0, 15.0],
         [],
     )
 
     assert col_values == [
-        ("dogs/dog1", "subobject") + new_col_values,
-        ("dogs/dog2", "subobject") + new_col_values,
-        ("dogs/dog3", "subobject") + new_col_values,
-        ("dogs/others/dog4", "subobject") + new_col_values,
+        ("dogs/dog1", "subobject", *new_col_values),
+        ("dogs/dog2", "subobject", *new_col_values),
+        ("dogs/dog3", "subobject", *new_col_values),
+        ("dogs/others/dog4", "subobject", *new_col_values),
     ]
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
@@ -2677,15 +2674,15 @@
     )
     class Subobjects:
         def __init__(self):
             pass
 
         def generate_subobjects(self, name, parent):
             parent_path = name if not parent else f"{parent}/{name}"
-            yield DatasetRow.create("subobject", size=50, parent=parent_path) + (0.5,)
+            yield (*DatasetRow.create("subobject", size=50, parent=parent_path), 0.5)
 
     with pytest.raises(ValueError):
         DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog).generate(
             Subobjects
         ).to_records()
 
 
@@ -2695,25 +2692,31 @@
     catalog = ctc.catalog
     catalog.index([ctc.src_uri])
     catalog.create_dataset_from_sources("animals", [ctc.src_uri])
 
     q = DatasetQuery(name="animals", version=1, catalog=catalog).generate(index_tar)
     q.save("extracted")
 
-    rows = list(catalog.ls_dataset_rows("extracted", 1))
-    assert {row.name for row in rows} == {
-        "animals.tar",
-        "cat1",
-        "cat2",
-        "description",
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
+    assert_row_names(
+        catalog,
+        catalog.get_dataset("extracted"),
+        1,
+        {
+            "animals.tar",
+            "cat1",
+            "cat2",
+            "description",
+            "dog1",
+            "dog2",
+            "dog3",
+            "dog4",
+        },
+    )
+
+    rows = catalog.ls_dataset_rows("extracted", 1)
 
     offsets = [
         json.loads(row.location)[0]["offset"]
         for row in rows
         if row.name != "animals.tar"
     ]
     # Check that offsets are unique integers
```

### Comparing `dvcx-0.78.2/tests/func/test_datasets.py` & `dvcx-0.79.0/tests/func/test_datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import uuid
+from datetime import datetime
 from json import dumps
 from unittest.mock import ANY
 
 import pytest
 import sqlalchemy as sa
 from dateutil.parser import isoparse
 
@@ -21,16 +22,15 @@
     Float64,
     Int,
     Int32,
     Int64,
     SQLType,
     String,
 )
-
-from ..utils import dataset_dependency_asdict
+from tests.utils import assert_row_names, dataset_dependency_asdict
 
 
 def add_column(engine, table_name, column, catalog):
     # Simple method that adds new column to a table, with default value if specified
     column_name = column.compile(dialect=engine.dialect)
     column_type = column.type.compile(engine.dialect)
     query_str = f"ALTER TABLE {table_name} ADD COLUMN {column_name} {column_type}"
@@ -205,14 +205,15 @@
 
     assert dataset.custom_column_types == default_dataset_custom_column_types
     assert dataset.query_script == ""
 
     assert dataset_version.custom_column_types == default_dataset_custom_column_types
     assert dataset_version.query_script == ""
     assert dataset_version.num_objects
+    assert dataset_version.preview
 
 
 def test_create_dataset_from_sources_empty_sources(cloud_test_catalog):
     dataset_name = uuid.uuid4().hex
     catalog = cloud_test_catalog.catalog
 
     with pytest.raises(ValueError) as exc_info:
@@ -250,14 +251,15 @@
     assert dataset_version.created_at
     assert dataset_version.finished_at
     assert dataset_version.error_message == DATASET_INTERNAL_ERROR_MESSAGE
     assert dataset_version.error_stack
     assert dataset_version.sources == f"{src_uri}/dogs/*"
     assert dataset_version.num_objects is None
     assert dataset_version.size is None
+    assert dataset_version.preview is None
 
 
 def test_create_dataset_whole_bucket(listed_bucket, cloud_test_catalog):
     dataset_name_1 = uuid.uuid4().hex
     dataset_name_2 = uuid.uuid4().hex
     src_uri = cloud_test_catalog.src_uri
     catalog = cloud_test_catalog.catalog
@@ -275,21 +277,17 @@
         "cat2",
         "dog1",
         "dog2",
         "dog3",
         "dog4",
     }
 
-    assert {
-        r.name for r in catalog.ls_dataset_rows(ds1.name, ds1.latest_version)
-    } == expected_rows
+    assert_row_names(catalog, ds1, ds1.latest_version, expected_rows)
 
-    assert {
-        r.name for r in catalog.ls_dataset_rows(ds2.name, ds2.latest_version)
-    } == expected_rows
+    assert_row_names(catalog, ds2, ds2.latest_version, expected_rows)
 
 
 @pytest.mark.parametrize("target_version", [None, 3])
 def test_registering_dataset(
     cloud_test_catalog, dogs_dataset, cats_dataset, target_version
 ):
     catalog = cloud_test_catalog.catalog
@@ -335,25 +333,35 @@
     assert version2.created_at == dogs_version.created_at
     assert version2.finished_at == dogs_version.finished_at
     assert dogs_version.num_objects
     assert version2.num_objects == dogs_version.num_objects
     assert dogs_version.size
     assert version2.size == dogs_version.size
 
-    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, 1)} == {
-        "cat1",
-        "cat2",
-    }
+    assert_row_names(
+        catalog,
+        dataset,
+        1,
+        {
+            "cat1",
+            "cat2",
+        },
+    )
 
-    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, target_version)} == {
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
+    assert_row_names(
+        catalog,
+        dataset,
+        target_version,
+        {
+            "dog1",
+            "dog2",
+            "dog3",
+            "dog4",
+        },
+    )
 
     with pytest.raises(DatasetNotFoundError):
         # since it had only one version, it should be completely removed
         catalog.get_dataset(dogs_dataset.name)
 
 
 @pytest.mark.parametrize("target_version", [None, 3])
@@ -374,25 +382,35 @@
 
     # if not provided, it will end up being next dataset version
     target_version = target_version or cats_dataset.next_version
 
     assert dataset.name == cats_dataset.name
     assert dataset.versions_values == [1, target_version]
 
-    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, 1)} == {
-        "cat1",
-        "cat2",
-    }
+    assert_row_names(
+        catalog,
+        dataset,
+        1,
+        {
+            "cat1",
+            "cat2",
+        },
+    )
 
-    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, target_version)} == {
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
+    assert_row_names(
+        catalog,
+        dataset,
+        target_version,
+        {
+            "dog1",
+            "dog2",
+            "dog3",
+            "dog4",
+        },
+    )
 
     # check if dogs dataset is still present as it has one more version
     dogs_dataset = catalog.get_dataset(dogs_dataset.name)
     assert dogs_dataset.versions_values == [2]
     dataset_version = dogs_dataset.get_version(2)
     assert dataset_version.num_objects == 0
 
@@ -412,18 +430,15 @@
 
     # if not provided, it will end up being next dataset version
     target_version = target_version or cats_dataset.next_version
 
     assert dataset.name == cats_dataset.name
     assert dataset.versions_values == [target_version]
 
-    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, target_version)} == {
-        "cat1",
-        "cat2",
-    }
+    assert_row_names(catalog, dataset, target_version, {"cat1", "cat2"})
 
 
 def test_registering_dataset_invalid_target_version(
     cloud_test_catalog, cats_dataset, dogs_dataset
 ):
     catalog = cloud_test_catalog.catalog
 
@@ -675,14 +690,89 @@
             "string_col": "s",
             "bool_col": True,
             "json_col": dumps({"a": 1}),
             "binary_col": int_example.to_bytes(2, "big"),
         }
 
 
+def test_dataset_preview_custom_columns(cloud_test_catalog, dogs_dataset):
+    catalog = cloud_test_catalog.catalog
+    int_example = 25
+
+    @udf(
+        (),
+        {
+            "int_col": Int,
+            "int_col_32": Int32,
+            "int_col_64": Int64,
+            "float_col": Float,
+            "float_col_32": Float32,
+            "float_col_64": Float64,
+            "array_col": Array(Float),
+            "array_col_nested": Array(Array(Float)),
+            "array_col_32": Array(Float32),
+            "array_col_64": Array(Float64),
+            "string_col": String,
+            "bool_col": Boolean,
+            "json_col": JSON,
+            "binary_col": Binary,
+        },
+    )
+    def test_types():
+        return (
+            5,
+            5,
+            5,
+            0.5,
+            0.5,
+            0.5,
+            [0.5],
+            [[0.5], [0.5]],
+            [0.5],
+            [0.5],
+            "s",
+            True,
+            dumps({"a": 1}),
+            int_example.to_bytes(2, "big"),
+        )
+
+    (
+        DatasetQuery(name=dogs_dataset.name, catalog=catalog)
+        .add_signals(test_types)
+        .save("dogs_custom_columns")
+    )
+
+    for r in catalog.get_dataset("dogs_custom_columns").get_version(1).preview:
+        assert r.custom == {
+            "int_col": 5,
+            "int_col_32": 5,
+            "int_col_64": 5,
+            "float_col": 0.5,
+            "float_col_32": 0.5,
+            "float_col_64": 0.5,
+            "array_col": [0.5],
+            "array_col_nested": [[0.5], [0.5]],
+            "array_col_32": [0.5],
+            "array_col_64": [0.5],
+            "string_col": "s",
+            "bool_col": 1,
+            "json_col": '{"a": 1}',
+            "binary_col": ["00", "19"],
+        }
+
+
+def test_dataset_preview_last_modified(cloud_test_catalog, dogs_dataset):
+    catalog = cloud_test_catalog.catalog
+
+    DatasetQuery(name=dogs_dataset.name, catalog=catalog).save("dogs_custom_columns")
+
+    for r in catalog.get_dataset("dogs_custom_columns").get_version(1).preview:
+        assert isinstance(r.last_modified, datetime)
+
+
 def test_merge_datasets(cloud_test_catalog, dogs_dataset, cats_dataset):
     catalog = cloud_test_catalog.catalog
     catalog.merge_datasets(
         cats_dataset,
         dogs_dataset,
         1,
         dst_version=2,
```

### Comparing `dvcx-0.78.2/tests/func/test_ls.py` & `dvcx-0.79.0/tests/func/test_ls.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from typing import Any
 
 import msgpack
 import pytest
 from sqlalchemy import select
 
 from dvcx.cli import ls
-
-from ..utils import uppercase_scheme
+from tests.utils import uppercase_scheme
 
 
 def same_lines(lines1, lines2):
     return sorted(lines1.split("\n")) == sorted(lines2.split("\n"))
 
 
 def test_ls_no_args(cloud_test_catalog, capsys):
@@ -113,15 +112,15 @@
     ls([f"{src}/dogs/others/"], catalog=cloud_test_catalog.catalog)
     # These sleep calls are here to ensure that capsys can fully capture the output
     # and to avoid any flaky tests due to multithreading generating output out of order
     sleep(0.05)
     captured = capsys.readouterr()
     assert get_partial_indexed_paths(src_metastore) == ["dogs/others/"]
     assert "Listing" in captured.err
-    assert "dog4\n" == captured.out
+    assert captured.out == "dog4\n"
 
     ls([f"{src}/cats/"], catalog=cloud_test_catalog.catalog)
     sleep(0.05)
     captured = capsys.readouterr()
     assert get_partial_indexed_paths(src_metastore) == ["cats/", "dogs/others/"]
     assert "Listing" in captured.err
     assert same_lines("cat1\ncat2\n", captured.out)
@@ -184,17 +183,16 @@
 
 
 def _pack_extended_types(obj):
     if isinstance(obj, datetime):
         if obj.tzinfo:
             data = (obj.timestamp(), int(obj.utcoffset().total_seconds()))
             return msgpack.ExtType(42, pack("!dl", *data))
-        else:
-            data = (obj.timestamp(),)
-            return msgpack.ExtType(42, pack("!d", *data))
+        data = (obj.timestamp(),)
+        return msgpack.ExtType(42, pack("!d", *data))
     raise TypeError(f"Unknown type: {type(obj)}")
 
 
 ls_remote_sources_output = """\
 {src}:
 cats/
 dogs/
```

### Comparing `dvcx-0.78.2/tests/func/test_pull.py` & `dvcx-0.79.0/tests/func/test_pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import io
 from datetime import datetime
 
 import attrs
-import lz4.frame  # noqa: F401
+import lz4.frame
 import pandas as pd
 import pytest
 
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DVCXError
 from dvcx.node import DirType
-
-from ..data import ENTRIES
-from ..utils import skip_if_not_sqlite
+from tests.data import ENTRIES
+from tests.utils import assert_row_names, skip_if_not_sqlite
 
 
 @pytest.fixture
 def dog_entries():
     return [
         attrs.asdict(e) for e in ENTRIES if e.name.startswith("dog") and not e.is_dir
     ]
@@ -80,31 +79,32 @@
         "random": {"type": "Int64"},
         "location": {"type": "String"},
         "source": {"type": "String"},
     }
 
 
 @pytest.fixture
-def remote_dataset_version(custom_column_types):
+def remote_dataset_version(custom_column_types, dataset_rows):
     return {
         "id": 1,
         "dataset_id": 1,
         "version": 1,
         "status": 4,
         "created_at": "2024-02-23T10:42:31.842944+00:00",
         "finished_at": "2024-02-23T10:43:31.842944+00:00",
         "error_message": "",
         "error_stack": "",
         "num_objects": 5,
         "size": 1073741824,
+        "preview": [dataset_row.to_preview_dict() for dataset_row in dataset_rows],
         "script_output": "",
         "custom_column_types": custom_column_types,
         "sources": "",
         "query_script": (
-            'from dvcx.query import DatasetQuery\nDatasetQuery(path="s3://ldb-public)',
+            'from dvcx.query import DatasetQuery\nDatasetQuery(path="s3://ldb-public")',
         ),
         "created_by_id": 1,
     }
 
 
 @pytest.fixture
 def remote_dataset(remote_dataset_version, custom_column_types):
@@ -181,22 +181,25 @@
     assert dataset_version.status == DatasetStatus.COMPLETE
     assert dataset_version.created_at
     assert dataset_version.finished_at
     assert dataset_version.custom_column_types
     assert dataset_version.num_objects == 4
     assert dataset_version.size == 15
 
-    expected_rows = {
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
-
-    assert {r.name for r in catalog.ls_dataset_rows("dogs", 1)} == expected_rows
+    assert_row_names(
+        catalog,
+        dataset,
+        1,
+        {
+            "dog1",
+            "dog2",
+            "dog3",
+            "dog4",
+        },
+    )
 
 
 @pytest.mark.parametrize("cloud_type, version_aware", [("s3", False)], indirect=True)
 def test_pull_dataset_wrong_dataset_uri_format(
     requests_mock,
     cloud_test_catalog,
     remote_config,
```

### Comparing `dvcx-0.78.2/tests/func/test_pytorch.py` & `dvcx-0.79.0/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/func/test_query.py` & `dvcx-0.79.0/tests/func/test_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from textwrap import dedent
 
 import dill
 import pytest
 
 from dvcx.catalog import QUERY_DATASET_PREFIX
 from dvcx.cli import query
+from tests.utils import assert_row_names
 
 
 @pytest.fixture
 def catalog_info_filepath(cloud_test_catalog_tmpfile, tmp_path):
     catalog = cloud_test_catalog_tmpfile.catalog
 
     catalog_info = {
@@ -97,23 +98,28 @@
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
     dataset, version, output, _ = catalog.query(query_script, save=True)
     assert dataset.name.startswith(QUERY_DATASET_PREFIX)
     assert dataset.query_script == query_script
     assert version == 1
     assert dataset.versions_values == [1]
-    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
-        "cat1",
-        "cat2",
-        "description",
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
+    assert_row_names(
+        catalog,
+        dataset,
+        version,
+        {
+            "cat1",
+            "cat2",
+            "description",
+            "dog1",
+            "dog2",
+            "dog3",
+            "dog4",
+        },
+    )
 
 
 @pytest.mark.parametrize(
     "params,count",
     (
         (None, 7),
         ({"limit": 1}, 1),
@@ -158,20 +164,25 @@
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
     dataset, version, output, _ = catalog.query(query_script, save=True)
     assert not dataset.name.startswith(QUERY_DATASET_PREFIX)
     assert dataset.query_script == query_script
     assert version == 1
     assert dataset.versions_values == [1]
-    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
+    assert_row_names(
+        catalog,
+        dataset,
+        version,
+        {
+            "dog1",
+            "dog2",
+            "dog3",
+            "dog4",
+        },
+    )
 
 
 def test_query_where_last_command_is_attached_dataset_query_created_from_save(
     cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath
 ):
     """
     Testing use case where last command is instance of DatasetQuery which is
@@ -191,20 +202,25 @@
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
     dataset, version, output, _ = catalog.query(query_script, save=True)
     assert dataset.name == "dogs"
     assert dataset.query_script == query_script
     assert version == 1
     assert dataset.versions_values == [1]
-    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
+    assert_row_names(
+        catalog,
+        dataset,
+        version,
+        {
+            "dog1",
+            "dog2",
+            "dog3",
+            "dog4",
+        },
+    )
 
 
 def test_query_where_last_command_is_attached_dataset_query_created_from_query(
     cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath
 ):
     """
     Testing use case where last command is instance of DatasetQuery which is
@@ -224,13 +240,18 @@
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
     dataset, version, output, _ = catalog.query(query_script, save=True)
     assert dataset.name == "dogs"
     assert dataset.query_script == query_script
     assert version == 1
     assert dataset.versions_values == [1]
-    assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
+    assert_row_names(
+        catalog,
+        dataset,
+        version,
+        {
+            "dog1",
+            "dog2",
+            "dog3",
+            "dog4",
+        },
+    )
```

### Comparing `dvcx-0.78.2/tests/scripts/name_len_normal.py` & `dvcx-0.79.0/tests/scripts/name_len_normal.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
     {
         "name_len": Int
     },  # Signals being returned by the UDF, with the signal name and type.
 )
 def name_len(name):
     if name.endswith(".json"):
         return (-1,)
-    else:
-        return (len(name),)
+    return (len(name),)
 
 
 # Save as a new dataset.
 DatasetQuery(
     path="gcs://dvcx-datalakes/dogs-and-cats/",
     anon=True,
 ).filter(C.name.glob("*cat*")).add_signals(name_len, parallel=-1).order_by(  # type: ignore[attr-defined]
```

### Comparing `dvcx-0.78.2/tests/scripts/name_len_slow.py` & `dvcx-0.79.0/tests/scripts/name_len_slow.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,15 @@
     print("UDF Processing Started")
     # Avoid any buffering so that the end-to-end test can react immediately.
     sys.stdout.flush()
     # Process very slowly to emulate a stuck script.
     sleep(1)
     if name.endswith(".json"):
         return (-1,)
-    else:
-        return (len(name),)
+    return (len(name),)
 
 
 # Save as a new dataset.
 DatasetQuery(
     path="gcs://dvcx-datalakes/dogs-and-cats/",
     anon=True,
 ).filter(C.name.glob("*cat*")).add_signals(name_len, parallel=1).save("name_len")  # type: ignore[attr-defined]
```

### Comparing `dvcx-0.78.2/tests/test_cli_e2e.py` & `dvcx-0.79.0/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/test_query_e2e.py` & `dvcx-0.79.0/tests/test_query_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/lib/test_cached_stream.py` & `dvcx-0.79.0/tests/unit/lib/test_cached_stream.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,44 +10,46 @@
 def test_close(catalog):
     input = io.BytesIO()
     input.write(DATA)
     input.seek(0)
 
     with ProgressiveCacheStream(input, len(DATA), catalog, FILE_UID) as stream:
         stream.close()
-        assert open(catalog.cache.get_path(FILE_UID), "rb").read() == DATA
+        with open(catalog.cache.get_path(FILE_UID), "rb") as f:
+            assert f.read() == DATA
 
 
 def test_read_by_parts(catalog):
     input = io.BytesIO()
     input.write(DATA)
     input.seek(0)
 
     with ProgressiveCacheStream(input, len(DATA), catalog, FILE_UID) as stream:
         assert stream.read(1)[0] == DATA[0]
         assert stream.read(5) == DATA[1:6]
         assert stream.read(1)[0] == DATA[6]
         assert stream.read(1024) == DATA[7:]
 
         stream.close()
-        assert open(catalog.cache.get_path(FILE_UID), "rb").read() == DATA
+        with open(catalog.cache.get_path(FILE_UID), "rb") as f:
+            assert f.read() == DATA
 
 
 def test_seek_forward(catalog):
     input = io.BytesIO()
     input.write(DATA)
     input.seek(0)
 
     with ProgressiveCacheStream(input, len(DATA), catalog, FILE_UID) as stream:
         stream.seek(4)
         assert stream.read(1)[0] == DATA[4]
 
         stream.close()
-        in_cache = open(catalog.cache.get_path(FILE_UID), "rb").read()
-        assert in_cache == DATA
+        with open(catalog.cache.get_path(FILE_UID), "rb") as f:
+            assert f.read() == DATA
 
 
 def test_seek_backward(catalog):
     input = io.BytesIO()
     input.write(DATA)
     input.seek(0)
 
@@ -55,16 +57,16 @@
         stream.read(8)
 
         stream.seek(3)
         assert stream.tell() == 3
         assert stream.read(3) == DATA[3:6]
 
         stream.close()
-        in_cache = open(catalog.cache.get_path(FILE_UID), "rb").read()
-        assert in_cache == DATA
+        with open(catalog.cache.get_path(FILE_UID), "rb") as f:
+            assert f.read() == DATA
 
 
 def test_seek_backward_with_intersection(catalog):
     input = io.BytesIO()
     input.write(DATA)
     input.seek(0)
 
@@ -72,9 +74,9 @@
         stream.read(8)
 
         stream.seek(3)
         assert stream.tell() == 3
         assert stream.read(6) == DATA[3:9]
 
         stream.close()
-        in_cache = open(catalog.cache.get_path(FILE_UID), "rb").read()
-        assert in_cache == DATA
+        with open(catalog.cache.get_path(FILE_UID), "rb") as f:
+            assert f.read() == DATA
```

### Comparing `dvcx-0.78.2/tests/unit/lib/test_feature.py` & `dvcx-0.79.0/tests/unit/lib/test_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     ThisIsName: str
     subClass: MyNestedClass  # noqa: N815
 
 
 def test_flatten_schema():
     schema = FileInfo._to_udf_spec()
 
-    assert 4 == len(schema)
+    assert len(schema) == 4
     assert [item[0] for item in schema] == ["parent", "name", "size", "location"]
     assert [item[1] for item in schema] == [String, String, Int, JSON]
 
 
 def test_type_datatype():
     class Test1(Feature):
         d: datetime
@@ -133,15 +133,15 @@
     with pytest.raises(RuntimeError):
         Test1._to_udf_spec()
 
 
 def test_flatten_nested_schema():
     schema = FileInfoEx._to_udf_spec()
 
-    assert 5 == len(schema)
+    assert len(schema) == 5
     assert [item[0] for item in schema] == [
         "parent",
         "name",
         "size",
         "location",
         "type_id",
     ]
@@ -413,15 +413,15 @@
 def test_list_of_dicts_as_dict():
     class MyTest1(Feature):
         val1: Union[dict, list[dict]]
         val2: Optional[Union[list[dict], dict]]
 
     schema = Feature._features_to_udf_spec([MyTest1])
     assert len(schema) == 2
-    assert list(schema.values())[0] == JSON
+    assert next(iter(schema.values())) == JSON
     assert list(schema.values())[1] == JSON
 
 
 def test_create_column():
     name = "my_col"
     default = "NuLL"
 
@@ -542,29 +542,29 @@
 def test_literal():
     class MyTextBlock(Feature):
         id: int
         type: Literal["text"]
 
     schema = Feature._features_to_udf_spec([MyTextBlock])
     assert len(schema) == 2
-    assert list(schema.values())[0] == Int
+    assert next(iter(schema.values())) == Int
     assert list(schema.values())[1] == String
 
 
 def test_pydantic_to_feature():
     class MyTextBlock(BaseModel):
         id: int
         type: Literal["text"]
 
     cls = pydantic_to_feature(MyTextBlock)
     assert Feature._is_feature_class(cls)
 
     schema = Feature._features_to_udf_spec([cls])
     assert len(schema) == 2
-    assert list(schema.values())[0] == Int
+    assert next(iter(schema.values())) == Int
     assert list(schema.values())[1] == String
 
 
 def test_pydantic_to_feature_nested():
     class MyTextBlock(BaseModel):
         id: int
         type: Literal["text"]
@@ -574,38 +574,38 @@
         val2: MyTextBlock
 
     cls = pydantic_to_feature(MyMessage)
     assert Feature._is_feature_class(cls)
 
     schema = Feature._features_to_udf_spec([cls])
     assert len(schema) == 3
-    assert list(schema.values())[0] == String
+    assert next(iter(schema.values())) == String
     assert list(schema.values())[1] == Int
     assert list(schema.values())[2] == String
 
 
 def test_flatten_schema_with_list_of_objects():
     class FileDir(Feature):
         name: str
         files: list[FileBasic]
 
     schema = FileDir._to_udf_spec()
 
-    assert 2 == len(schema)
+    assert len(schema) == 2
     assert [item[0] for item in schema] == ["file_dir__name", "file_dir__files"]
 
     assert schema[0][1] == String
     assert schema[1][1].to_dict() == {"item_type": {"type": "JSON"}, "type": "Array"}
 
 
 def test_flatten_schema_with_list_of_ints():
     class SomeInfo(Feature):
         name: str
         vals: list[int]
 
     schema = SomeInfo._to_udf_spec()
 
-    assert 2 == len(schema)
+    assert len(schema) == 2
     assert [item[0] for item in schema] == ["some_info__name", "some_info__vals"]
 
     assert schema[0][1] == String
     assert schema[1][1].to_dict() == {"item_type": {"type": "Int"}, "type": "Array"}
```

### Comparing `dvcx-0.78.2/tests/unit/lib/test_feature_udf.py` & `dvcx-0.79.0/tests/unit/lib/test_feature_udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     name = "file.txt"
     path = "dir1/dir2"
     size = 16
     params = ((name, path, size),)
 
     agg = MyAgg()
     res = list(agg(params))
-    assert 1 == len(res)
+    assert len(res) == 1
 
     full_path, size_squared = res[0]
     assert full_path == os.path.join(path, name)
     assert size_squared == size**2
 
 
 def test_feature_udf_returns_values():
@@ -75,15 +75,15 @@
     name = "f1.txt"
     path = "d1/d2/d55"
     size = 235
     params = ((name, path, size),)
 
     agg = MyAggReturn()
     res = list(agg(params))
-    assert 1 == len(res)
+    assert len(res) == 1
 
     full_path, size_squared = res[0]
     assert full_path == os.path.join(path, name)
     assert size_squared == size**2
 
 
 class MyAggStream(FeatureAggregator):
@@ -93,19 +93,19 @@
     def process(self, args):
         output = TestOutput(full_path="xx", size_squared=5)
         yield (output,)
 
 
 def test_feature_udf_with_stream():
     stream = File(name="tmp.jpg")
-    args = ([Stream()] + list(stream._flatten()),)
+    args = ([Stream(), *list(stream._flatten())],)
 
     agg = MyAggStream()
     res = list(agg(args))
-    assert 1 == len(res)
+    assert len(res) == 1
 
 
 def test_feature_udf_with_single_input_and_output():
     class MyAgg(FeatureAggregator):
         def __init__(self):
             super().__init__(TestInput, TestOutput)
 
@@ -120,15 +120,15 @@
     name = "f1.txt"
     path = "dd3"
     size = 343
     params = ((name, path, size),)
 
     agg = MyAgg()
     res = list(agg(params))
-    assert 1 == len(res)
+    assert len(res) == 1
 
     full_path, size_squared = res[0]
     assert full_path == os.path.join(path, name)
     assert size_squared == size**2
 
 
 def test_incompatible_params_types():
@@ -198,19 +198,18 @@
 
 def test_mapper():
     class MyMap(FeatureMapper):
         def __init__(self):
             super().__init__(TestInput, TestOutput)
 
         def process(self, test_input):
-            output = TestOutput(
+            return TestOutput(
                 full_path=os.path.join(test_input.parent, test_input.name),
                 size_squared=test_input.size**2,
             )
-            return output
 
     name = "img001.jpg"
     path = "data/dogs"
     size = 56743
     params = (name, path, size)
 
     agg = MyMap()
@@ -224,27 +223,26 @@
 def test_mapper_stream():
     class MyMapStream(FeatureMapper):
         def __init__(self):
             super().__init__([File, TestInput], TestOutput)
 
         def process(self, inputs):
             stream, test_input = inputs
-            output = TestOutput(
+            return TestOutput(
                 full_path=os.path.join(test_input.parent, test_input.name),
                 size_squared=test_input.size**2,
             )
-            return output
 
     stream = File(name="file.jpg")
-    stream_args = tuple([Stream()] + list(stream._flatten()))
+    stream_args = (Stream(), *list(stream._flatten()))
 
     name = "img001.jpg"
     path = "data/dogs"
     size = 56743
-    args = stream_args + (name, path, size)
+    args = (*stream_args, name, path, size)
 
     agg = MyMapStream()
     res = agg(*args)
 
     full_path, size_squared = res
     assert full_path == os.path.join(path, name)
     assert size_squared == size**2
@@ -267,15 +265,15 @@
     path = "data/dogs"
     size = 56743
     params = ((name, path, size), ("1_" + name, "1_" + path, size * 2))
 
     agg = MyBatchMap()
     res = agg(params)
 
-    assert 2 == len(res)
+    assert len(res) == 2
 
     full_path, size_squared = res[0]
     assert full_path == os.path.join(path, name)
     assert size_squared == size**2
 
     full_path, size_squared = res[1]
     assert full_path == os.path.join("1_" + path, "1_" + name)
@@ -302,15 +300,15 @@
     path = "d1/cats"
     size = 384
     params = (name, path, size)
 
     agg = MyGen()
     res = agg(*params)
 
-    assert 2 == len(res)
+    assert len(res) == 2
 
     full_path, size_squared = res[0]
     assert full_path == os.path.join(path, name) + "_1"
     assert size_squared == size**2
 
     full_path, size_squared = res[1]
     assert full_path == os.path.join(path, name) + "_2"
@@ -320,19 +318,18 @@
 def test_feature_udf_output_value_instead_of_list():
     class MyAggOutputValueInsteadOfList(FeatureMapper):
         def __init__(self):
             super().__init__([TestInput], [TestOutput])
 
         def process(self, args):
             input = args[0]
-            output = TestOutput(
+            return TestOutput(
                 full_path=os.path.join(input.parent, input.name),
                 size_squared=input.size**2,
             )
-            return output
 
     name = "file.txt"
     path = "dir1/dir2"
     size = 16
     params = (name, path, size)
 
     agg = MyAggOutputValueInsteadOfList()
@@ -382,15 +379,15 @@
     f2 = File(name="zxc")._flatten()
 
     rows = [f1, f2]
     clean_rows, streams = FeatureConverter._separate_streams_from_rows(rows, features)
     assert clean_rows == rows
     assert streams == [None, None]
 
-    rows_with_streams = [(Stream(),) + f1, (Stream(),) + f2]
+    rows_with_streams = [(Stream(), *f1), (Stream(), *f2)]
     clean_rows, streams = FeatureConverter._separate_streams_from_rows(
         rows_with_streams, features
     )
     assert clean_rows == rows
     assert len(streams) == 2
     assert isinstance(streams[0], Stream)
     assert isinstance(streams[1], Stream)
```

### Comparing `dvcx-0.78.2/tests/unit/lib/test_file.py` & `dvcx-0.79.0/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/lib/test_image.py` & `dvcx-0.79.0/tests/unit/lib/test_image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/lib/test_reader.py` & `dvcx-0.79.0/tests/unit/lib/test_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class PrefixReader(FeatureReader):
     def __call__(self, value):
         return "prefix-" + value
 
 
 class SuffixReader(FeatureReader):
-    def __init__(self, fr_class, suffix):  # noqa: N803
+    def __init__(self, fr_class, suffix):
         self.suffix = suffix
         super().__init__(fr_class)
 
     def __call__(self, value):
         return value + self.suffix
```

### Comparing `dvcx-0.78.2/tests/unit/lib/test_text.py` & `dvcx-0.79.0/tests/unit/lib/test_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/lib/test_webdataset.py` & `dvcx-0.79.0/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.79.0/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/sql/test_array.py` & `dvcx-0.79.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/sql/test_conditional.py` & `dvcx-0.79.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/sql/test_path.py` & `dvcx-0.79.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/sql/test_selectable.py` & `dvcx-0.79.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/sql/test_string.py` & `dvcx-0.79.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_asyn.py` & `dvcx-0.79.0/tests/unit/test_asyn.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,16 +147,15 @@
     assume(any(n[0] for n in inputs))
 
     async def process(input):
         raising, n = input
         await asyncio.sleep(n)
         if raising:
             raise RuntimeError
-        else:
-            return input
+        return input
 
     loop = get_loop()
     mapper = create_mapper(process, inputs, workers=workers, loop=loop)
     with mock_time(loop):
         try:
             with pytest.raises(RuntimeError):
                 list(mapper.iterate(timeout=4))
```

### Comparing `dvcx-0.78.2/tests/unit/test_cache.py` & `dvcx-0.79.0/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_catalog.py` & `dvcx-0.79.0/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_catalog_formats.py` & `dvcx-0.79.0/tests/unit/test_catalog_formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_catalog_loader.py` & `dvcx-0.79.0/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_cli_parsing.py` & `dvcx-0.79.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_client.py` & `dvcx-0.79.0/tests/unit/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pytest
 from hypothesis import HealthCheck, given, settings
 from hypothesis import strategies as st
 
 from dvcx.client import Client
-
-from ..utils import uppercase_scheme
+from tests.utils import uppercase_scheme
 
 
 def test_bad_url():
     bucket = "whatever"
     path = "my/path"
     with pytest.raises(RuntimeError):
         Client.parse_url(bucket + "/" + path + "/", None, None)
```

### Comparing `dvcx-0.78.2/tests/unit/test_client_s3.py` & `dvcx-0.79.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_data_storage.py` & `dvcx-0.79.0/tests/unit/test_data_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
     DateTime,
     Float,
     Float32,
     Float64,
     Int,
     String,
 )
-
-from ..utils import DEFAULT_TREE, TARRED_TREE
+from tests.utils import DEFAULT_TREE, TARRED_TREE
 
 COMPLEX_TREE: dict[str, Any] = {
     **TARRED_TREE,
     **DEFAULT_TREE,
     "nested": {"dir": {"path": {"abc.txt": "abc"}}},
 }
```

### Comparing `dvcx-0.78.2/tests/unit/test_database_engine.py` & `dvcx-0.79.0/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_dataset.py` & `dvcx-0.79.0/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_dispatch.py` & `dvcx-0.79.0/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_fileslice.py` & `dvcx-0.79.0/tests/unit/test_fileslice.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 
 import pytest
 
 from dvcx.client.fileslice import FileSlice
 
 
-def test_positions():  # noqa: N802
+def test_positions():
     data = b"0123456789abcdef"
     base = io.BytesIO(data)
     f = FileSlice(base, 5, 5, "foo")
     assert base.tell() == 0
     assert f.readable()
     assert not f.writable()
     assert f.seekable()
@@ -30,15 +30,15 @@
 
     b = bytearray(5)
     f.seek(0)
     f.readinto(b)
     assert b == data[5:10]
 
 
-def test_invalid_slice():  # noqa: N802
+def test_invalid_slice():
     data = b"0123456789abcdef"
     base = io.BytesIO(data)
     f = FileSlice(base, 10, 10, "foo")
     assert f.read(4) == data[10:14]
     with pytest.raises(RuntimeError):
         f.read()
```

### Comparing `dvcx-0.78.2/tests/unit/test_id_generator.py` & `dvcx-0.79.0/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_listing.py` & `dvcx-0.79.0/tests/unit/test_listing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import posixpath
 
 import pytest
 
 from dvcx.catalog import Catalog
 from dvcx.catalog.catalog import DataSource
 from dvcx.node import DirType, Entry
-
-from ..utils import skip_if_not_sqlite
+from tests.utils import skip_if_not_sqlite
 
 TREE = {
     "dir1": {
         "d2": {None: ["file1.csv", "file2.csv"]},
         None: ["dataset.csv"],
     },
     "dir2": {None: ["diagram.png"]},
```

### Comparing `dvcx-0.78.2/tests/unit/test_metastore.py` & `dvcx-0.79.0/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_query_params.py` & `dvcx-0.79.0/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_serializer.py` & `dvcx-0.79.0/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_session.py` & `dvcx-0.79.0/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_storage.py` & `dvcx-0.79.0/tests/unit/test_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from datetime import datetime, timedelta, timezone
 
 import pytest
 from sqlalchemy import func
 
 from dvcx import utils
 from dvcx.error import StorageNotFoundError
-from dvcx.storage import STALE_HOURS_LIMIT, Status, Storage, StorageURI
-
-from ..utils import skip_if_not_sqlite
+from dvcx.storage import STALE_MINUTES_LIMIT, Status, Storage, StorageURI
+from tests.utils import skip_if_not_sqlite
 
 TS = datetime(2022, 8, 1)
 EXPIRES = datetime(2022, 8, 2)
 
 
 def test_human_time():
     assert utils.human_time_to_int("1236") == 1236
@@ -146,15 +145,15 @@
 
     metastore.mark_storage_pending(metastore.get_storage(uri_stale))
     metastore.mark_storage_pending(metastore.get_storage(uri_not_stale))
 
     # make storage looks stale
     updates = {
         "last_inserted_at": datetime.now(timezone.utc)
-        - timedelta(hours=STALE_HOURS_LIMIT + 1)
+        - timedelta(minutes=STALE_MINUTES_LIMIT + 1)
     }
     s = metastore._storages
     metastore.db.execute(s.update().where(s.c.uri == uri_stale).values(**updates))
 
     metastore.find_stale_storages()
 
     stale_storage = metastore.get_storage(uri_stale)
```

### Comparing `dvcx-0.78.2/tests/unit/test_udf.py` & `dvcx-0.79.0/tests/unit/test_udf.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,15 @@
     result = t(None, row)
     assert result[0] == {"id": 6, "mul": 42, "sum": 13}
 
 
 def test_udf_batching():
     @udf(("id", "size"), {"mul": Integer}, batch=4)
     def t(vals):
-        result = [(a * b,) for (a, b) in vals]
-        return result
+        return [(a * b,) for (a, b) in vals]
 
     inputs = list(zip(range(1, 11), range(21, 31)))
     results = []
     for size, row_id in inputs:
         row = DatasetRow(
             id=row_id,
             vtype="",
```

### Comparing `dvcx-0.78.2/tests/unit/test_utils.py` & `dvcx-0.79.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/unit/test_warehouse.py` & `dvcx-0.79.0/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.78.2/tests/utils.py` & `dvcx-0.79.0/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from string import printable
 from tarfile import DIRTYPE, TarInfo
 from time import sleep, time
 from typing import Any, Callable, Optional
 
 import pytest
 
-from dvcx.dataset import DatasetDependency
+from dvcx.catalog.catalog import Catalog
+from dvcx.dataset import DatasetDependency, DatasetRecord
 from dvcx.node import Entry
 from dvcx.query import C, DatasetQuery
 from dvcx.storage import Status as StorageStatus
 
 
 def insert_nodes(warehouse, entries):
     """
@@ -245,16 +246,15 @@
     """
     Converting to dict with making sure we don't have any additional fields
     that could've been added with subclasses
     """
     if not dep:
         return None
     parsed = {
-        k: dataclasses.asdict(dep)[k]
-        for k in DatasetDependency.__dataclass_fields__.keys()
+        k: dataclasses.asdict(dep)[k] for k in DatasetDependency.__dataclass_fields__
     }
 
     if dep.dependencies:
         parsed["dependencies"] = [
             dataset_dependency_asdict(d) for d in dep.dependencies
         ]
 
@@ -270,7 +270,18 @@
     start_time = time()
     while time() - start_time < timeout:
         result = callback()
         if result:
             return result
         sleep(check_interval)
     raise TimeoutError(f"Timeout expired while waiting for: {message}")
+
+
+def assert_row_names(
+    catalog: Catalog, dataset: DatasetRecord, version: int, expected_names: set
+) -> None:
+    dataset_rows = catalog.ls_dataset_rows(dataset.name, version, limit=20)
+    assert dataset_rows
+    preview = dataset.get_version(version).preview
+    assert preview
+
+    assert {r.name for r in dataset_rows} == {r.name for r in preview} == expected_names
```

