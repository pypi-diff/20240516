# Comparing `tmp/opperai-0.6.0.tar.gz` & `tmp/opperai-0.6.1.tar.gz`

## Comparing `opperai-0.6.0.tar` & `opperai-0.6.1.tar`

### file list

```diff
@@ -1,92 +1,95 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.6.0/pytest.ini
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.6.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/__init__.py
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/_client.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/_http_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/functions/__init__.py
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/functions/_async_functions.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/functions/_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/indexes/__init__.py
--rw-r--r--   0        0        0    12400 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/indexes/_async_indexes.py
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/indexes/_indexes.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/spans/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/spans/_async_spans.py
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/spans/_decorator.py
--rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/spans/_spans.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/utils/__init__.py
--rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/functions/async_functions.py
--rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/functions/functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/functions/decorator/__init__.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/functions/decorator/_decorator.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/functions/decorator/_schemas.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/indexes/async_indexes.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/indexes/indexes.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/spans/async_spans.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/spans/spans.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/types/exceptions.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/types/indexes.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/types/spans.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/types/validators.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_async_functions.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_async_indexes.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_async_spans.py
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_fn_decorator.py
--rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_functions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_indexes.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_trace_decorator.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_types.py
--rw-r--r--   0        0        0   173874 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/images/fossil.jpg
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0   236306 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_image_file.yaml
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_image_url.yaml
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0   237017 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_image_file.yaml
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_image_url.yaml
--rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.6.0/.gitignore
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.6.0/LICENSE
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 opperai-0.6.0/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 opperai-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.6.1/pytest.ini
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.6.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/__init__.py
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/_client.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/_http_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/functions/__init__.py
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/functions/_async_functions.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/functions/_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/indexes/__init__.py
+-rw-r--r--   0        0        0    12400 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/indexes/_async_indexes.py
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/indexes/_indexes.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/spans/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/spans/_async_spans.py
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/spans/_decorator.py
+-rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/spans/_spans.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/core/utils/__init__.py
+-rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/functions/async_functions.py
+-rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/functions/functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/functions/decorator/__init__.py
+-rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/functions/decorator/_decorator.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/functions/decorator/_schemas.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/indexes/async_indexes.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/indexes/indexes.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/spans/async_spans.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/spans/spans.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/types/exceptions.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/types/indexes.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/types/spans.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.6.1/src/opperai/types/validators.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/conftest.py
+-rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/test_async_functions.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/test_async_indexes.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/test_async_spans.py
+-rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/test_fn_decorator.py
+-rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/test_functions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/test_indexes.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/test_trace_decorator.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/test_types.py
+-rw-r--r--   0        0        0   173874 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/images/fossil.jpg
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/images/letters.png
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0   236306 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_image_file.yaml
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_image_url.yaml
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml
+-rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_image.yaml
+-rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_image_async.yaml
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0   237017 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_image_file.yaml
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_image_url.yaml
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.6.1/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.6.1/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 opperai-0.6.1/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 opperai-0.6.1/PKG-INFO
```

### Comparing `opperai-0.6.0/.github/workflows/publish.yml` & `opperai-0.6.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/__init__.py` & `opperai-0.6.1/src/opperai/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/_client.py` & `opperai-0.6.1/src/opperai/_client.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/core/_http_clients.py` & `opperai-0.6.1/src/opperai/core/_http_clients.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/core/functions/_async_functions.py` & `opperai-0.6.1/src/opperai/core/functions/_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/core/functions/_functions.py` & `opperai-0.6.1/src/opperai/core/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/core/indexes/_async_indexes.py` & `opperai-0.6.1/src/opperai/core/indexes/_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/core/indexes/_indexes.py` & `opperai-0.6.1/src/opperai/core/indexes/_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/core/spans/_async_spans.py` & `opperai-0.6.1/src/opperai/core/spans/_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/core/spans/_decorator.py` & `opperai-0.6.1/src/opperai/core/spans/_decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 class SpanContext:
     def __init__(self, client: Client, span_uuid: str):
         self.client = client
         self.span_uuid = span_uuid
         self.output = None
 
 
+def utcnow():
+    return datetime.datetime.now(datetime.timezone.utc)
+
+
 @contextmanager
 def start_span(
     name: str,
     input: Optional[str] = None,
     metadata: Optional[dict] = None,
     client: Optional[Client] = None,
 ):
@@ -51,24 +55,24 @@
     span = Span(
         uuid=span_id,
         meta=metadata,
         input=input,
         parent_uuid=parent_span_id if parent_span_id is not None else None,
         project=project,
         name=name,
-        start_time=datetime.datetime.utcnow(),
+        start_time=utcnow(),
     )
     span_uuid = c.spans.create(span)
 
     span_token = _current_span_id.set(span_id)
     span_context = SpanContext(c, span_uuid)
     try:
         yield span_context  # This allows the block inside the 'with' statement to execute and interact with the span_context
     finally:
-        end_time = datetime.datetime.utcnow()
+        end_time = utcnow()
         update_kwargs = {
             "end_time": end_time,
         }
         if span_context.output is not None:
             update_kwargs["output"] = span_context.output
 
         c.spans.update(span_uuid, **update_kwargs)
@@ -98,27 +102,27 @@
                 )
             span = Span(
                 uuid=span_id,
                 parent_uuid=parent_span_id if parent_span_id is not None else None,
                 project=project,
                 name=span_name,
                 input=inputs,
-                start_time=datetime.datetime.utcnow(),
+                start_time=utcnow(),
             )
             span_uuid = c.spans.create(span)
 
             span_token = _current_span_id.set(span_id)
             try:
                 if asyncio.iscoroutinefunction(func):
                     result = await func(*args, **kwargs)
                 else:
                     result = func(*args, **kwargs)
                 c.spans.update(
                     span_uuid,
-                    end_time=datetime.datetime.utcnow(),
+                    end_time=utcnow(),
                     output=json.dumps(result) if trace_io else None,
                 )
             finally:
                 _current_span_id.reset(span_token)
 
             return result
 
@@ -136,24 +140,24 @@
                 )
             span = Span(
                 uuid=span_id,
                 parent_uuid=parent_span_id if parent_span_id is not None else None,
                 project=project,
                 name=span_name,
                 input=inputs,
-                start_time=datetime.datetime.utcnow(),
+                start_time=utcnow(),
             )
             span_uuid = c.spans.create(span)
 
             span_token = _current_span_id.set(span_id)
             try:
                 result = func(*args, **kwargs)
                 c.spans.update(
                     span_uuid,
-                    end_time=datetime.datetime.utcnow(),
+                    end_time=utcnow(),
                     output=json.dumps(result) if trace_io else None,
                 )
             finally:
                 _current_span_id.reset(span_token)
 
             return result
```

### Comparing `opperai-0.6.0/src/opperai/core/spans/_spans.py` & `opperai-0.6.1/src/opperai/core/spans/_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/core/utils/__init__.py` & `opperai-0.6.1/src/opperai/core/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import json
 from datetime import datetime
+from inspect import signature
 from uuid import UUID
-from pydantic import BaseModel
 
-
-from inspect import signature
+from opperai.types import ImageMessageContent
+from pydantic import BaseModel
 
 
 def convert_function_call_to_json(func, *args, **kwargs):
+    media = []
     input_data = dict(zip(signature(func).parameters, args))
     input_data.update(kwargs)
+
+    input = {}
     for key, value in input_data.items():
-        if isinstance(value, BaseModel):
-            input_data[key] = value.model_dump()
+        if isinstance(value, ImageMessageContent):
+            media.append(value)
+        elif isinstance(value, BaseModel):
+            input[key] = value.model_dump()
         elif isinstance(value, list) and all(isinstance(v, BaseModel) for v in value):
-            input_data[key] = [v.model_dump() for v in value]
-    return input_data
+            input[key] = [v.model_dump() for v in value]
+        else:
+            input[key] = value
+
+    return input, media
 
 
 class DateTimeEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, datetime):
             return obj.isoformat()
         if isinstance(obj, UUID):
```

### Comparing `opperai-0.6.0/src/opperai/functions/async_functions.py` & `opperai-0.6.1/src/opperai/functions/async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/functions/functions.py` & `opperai-0.6.1/src/opperai/functions/functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/functions/decorator/_decorator.py` & `opperai-0.6.1/src/opperai/functions/decorator/_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 from typing import Any, List, Tuple, get_args, get_origin, get_type_hints
 
 from opperai._client import AsyncClient, Client
 from opperai.core.spans import get_current_span_id
 from opperai.core.utils import convert_function_call_to_json
 from opperai.functions.async_functions import AsyncFunctionResponse
 from opperai.functions.functions import FunctionResponse
-from opperai.types import CacheConfiguration, ChatPayload, Function, Message
+from opperai.types import (
+    CacheConfiguration,
+    ChatPayload,
+    Function,
+    Message,
+)
 from pydantic import BaseModel
 
 from ._schemas import get_output_schema
 
 _thread_local = threading.local()
 
 
@@ -180,44 +185,50 @@
                     (get_origin(return_type) == list or get_origin(return_type) == List)
                     and inspect.isclass(get_args(return_type)[0])
                     and issubclass(get_args(return_type)[0], BaseModel)
                 ):
                     response = [get_args(return_type)[0](**item) for item in response]
             return response
 
-        def _prepare_payload(input):
+        def _prepare_payload(input, images):
+            messages = [
+                Message(role="user", content=json.dumps(input, cls=json_encoder))
+            ]
+            if images:
+                messages.append(Message(role="user", content=images))
+
             return ChatPayload(
                 parent_span_uuid=get_current_span_id(),
-                messages=[
-                    Message(role="user", content=json.dumps(input, cls=json_encoder))
-                ],
+                messages=messages,
             )
 
         @wraps(func)
         async def async_wrapper(*args, **kwargs):
             await async_setup()
 
-            input = convert_function_call_to_json(func, *args, **kwargs)
-            _response = await c.functions.chat(func_path, _prepare_payload(input))
+            input, media = convert_function_call_to_json(func, *args, **kwargs)
+            _response = await c.functions.chat(
+                func_path, _prepare_payload(input, media)
+            )
 
             _thread_local.span_id = _response.span_id
 
             return_type = get_type_hints(func).get("return")
             answer = _unmarshal_response(_response.json_payload, return_type)
 
             response = AsyncFunctionResponse(client=c, **_response.model_dump())
 
             return answer, response
 
         @wraps(func)
         def sync_wrapper(*args, **kwargs):
             setup()
 
-            input = convert_function_call_to_json(func, *args, **kwargs)
-            _response = c.functions.chat(func_path, _prepare_payload(input))
+            input, media = convert_function_call_to_json(func, *args, **kwargs)
+            _response = c.functions.chat(func_path, _prepare_payload(input, media))
 
             _thread_local.span_id = _response.span_id
 
             return_type = get_type_hints(func).get("return")
             answer = _unmarshal_response(_response.json_payload, return_type)
 
             response = FunctionResponse(client=c, **_response.model_dump())
```

### Comparing `opperai-0.6.0/src/opperai/functions/decorator/_schemas.py` & `opperai-0.6.1/src/opperai/functions/decorator/_schemas.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/indexes/async_indexes.py` & `opperai-0.6.1/src/opperai/indexes/async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/indexes/indexes.py` & `opperai-0.6.1/src/opperai/indexes/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/spans/async_spans.py` & `opperai-0.6.1/src/opperai/spans/async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/spans/spans.py` & `opperai-0.6.1/src/opperai/spans/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/types/__init__.py` & `opperai-0.6.1/src/opperai/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,24 @@
         return ImageMessageContent(image_url=ImageMessageFile(path=path))
 
     @classmethod
     def image_url(cls, url: str) -> ImageMessageContent:
         return ImageMessageContent(image_url=ImageMessageUrl(url=url))
 
 
+class ImageContent:
+    @classmethod
+    def from_path(cls, path: str) -> ImageMessageContent:
+        return ImageMessageContent(image_url=ImageMessageFile(path=path))
+
+    @classmethod
+    def from_url(cls, url: str) -> ImageMessageContent:
+        return ImageMessageContent(image_url=ImageMessageUrl(url=url))
+
+
 class Message(BaseModel):
     role: str
     content: Union[str, List[Union[TextMessageContent, ImageMessageContent]]]
 
 
 class ChatPayload(BaseModel):
     model_config: ConfigDict = ConfigDict(extra="allow")
```

### Comparing `opperai-0.6.0/src/opperai/types/indexes.py` & `opperai-0.6.1/src/opperai/types/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/types/spans.py` & `opperai-0.6.1/src/opperai/types/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/src/opperai/types/validators.py` & `opperai-0.6.1/src/opperai/types/validators.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/conftest.py` & `opperai-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/test_async_functions.py` & `opperai-0.6.1/tests/test_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/test_async_indexes.py` & `opperai-0.6.1/tests/test_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/test_async_spans.py` & `opperai-0.6.1/tests/test_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/test_functions.py` & `opperai-0.6.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/test_indexes.py` & `opperai-0.6.1/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/test_trace_decorator.py` & `opperai-0.6.1/tests/test_trace_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/test_types.py` & `opperai-0.6.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/images/fossil.jpg` & `opperai-0.6.1/tests/fixtures/images/fossil.jpg`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_image_file.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_image_file.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_image_url.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_image_url.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,22 @@
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/translate
   response:
     body:
       string: '{"path":"translate","instructions":"Operation: translate\n\nOperation
         description: Translate text to a target language.","id":82,"description":"Translate
-        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"openai/gpt3.5-turbo","language_model_id":2,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '568'
+      - '574'
       content-type:
       - application/json
       date:
-      - Tue, 07 May 2024 20:11:36 GMT
+      - Tue, 14 May 2024 19:47:15 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"id": 82, "path": "translate", "description": "Translate text to a target
@@ -42,22 +42,22 @@
       - application/json
     method: PATCH
     uri: http://localhost:8000/v1/functions/82
   response:
     body:
       string: '{"path":"translate","instructions":"Operation: translate\n\nOperation
         description: Translate text to a target language.","id":82,"description":"Translate
-        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"openai/gpt3.5-turbo","language_model_id":2,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '568'
+      - '574'
       content-type:
       - application/json
       date:
-      - Tue, 07 May 2024 20:11:36 GMT
+      - Tue, 14 May 2024 19:47:15 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"text\":
@@ -71,22 +71,22 @@
       - '123'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/translate
   response:
     body:
-      string: '{"span_id":"0c282ba5-4c82-4b2e-ba84-410535df190f","message":null,"json_payload":"Hola","context":null,"cached":false}'
+      string: '{"span_id":"5702b249-1f6f-40c6-be52-ed97ce1d21f0","message":null,"json_payload":"Hola","context":null,"cached":false}'
     headers:
       content-length:
       - '117'
       content-type:
       - application/json
       date:
-      - Tue, 07 May 2024 20:11:36 GMT
+      - Tue, 14 May 2024 19:47:15 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"text\":
@@ -100,22 +100,22 @@
       - '123'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/translate
   response:
     body:
-      string: '{"span_id":"c48b7221-4efc-4ba7-8f6c-fadfda9e996e","message":null,"json_payload":"Hola","context":null,"cached":false}'
+      string: '{"span_id":"1b820c2e-c858-4420-9676-4c9c8a78fab8","message":null,"json_payload":"Hola","context":null,"cached":false}'
     headers:
       content-length:
       - '117'
       content-type:
       - application/json
       date:
-      - Tue, 07 May 2024 20:11:37 GMT
+      - Tue, 14 May 2024 19:47:15 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"dimension": "metric", "value": 1.0, "comment": null}'
@@ -125,24 +125,24 @@
       connection:
       - keep-alive
       content-length:
       - '54'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/spans/c48b7221-4efc-4ba7-8f6c-fadfda9e996e/metrics
+    uri: http://localhost:8000/v1/spans/1b820c2e-c858-4420-9676-4c9c8a78fab8/metrics
   response:
     body:
-      string: '{"id":"651e4654-0376-4163-8590-ef4d52a2c17e","span_id":"c48b7221-4efc-4ba7-8f6c-fadfda9e996e","dimension":"metric","value":1.0,"comment":null,"updated_at":null,"created_at":"2024-05-07T20:11:38.831035Z"}'
+      string: '{"id":"6ca2cbce-2a0b-4d3e-8169-f7511614ca26","span_id":"1b820c2e-c858-4420-9676-4c9c8a78fab8","dimension":"metric","value":1.0,"comment":null,"updated_at":null,"created_at":"2024-05-14T19:47:17.653381Z"}'
     headers:
       content-length:
       - '203'
       content-type:
       - application/json
       date:
-      - Tue, 07 May 2024 20:11:38 GMT
+      - Tue, 14 May 2024 19:47:16 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,22 @@
       - keep-alive
     method: GET
     uri: http://localhost:8000/v1/functions/by_path/translate
   response:
     body:
       string: '{"path":"translate","instructions":"Operation: translate\n\nOperation
         description: Translate text to a target language.","id":82,"description":"Translate
-        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"openai/gpt3.5-turbo","language_model_id":2,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '568'
+      - '574'
       content-type:
       - application/json
       date:
-      - Tue, 07 May 2024 20:33:23 GMT
+      - Tue, 14 May 2024 19:47:08 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"id": 82, "path": "translate", "description": "Translate text to a target
@@ -42,22 +42,22 @@
       - application/json
     method: PATCH
     uri: http://localhost:8000/v1/functions/82
   response:
     body:
       string: '{"path":"translate","instructions":"Operation: translate\n\nOperation
         description: Translate text to a target language.","id":82,"description":"Translate
-        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"azure/gpt4-eu","language_model_id":8,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
+        text to a target language.","input_schema":null,"out_schema":{"type":"string","$defs":{}},"few_shot":false,"few_shot_count":2,"dataset_uuid":"0331a79c-e4f6-44c3-8176-56d908caaf43","use_semantic_search":false,"model":"openai/gpt3.5-turbo","language_model_id":2,"index_ids":[],"linked_function_ids":null,"revision":1,"cache_configuration":{"exact_match_cache_ttl":0,"semantic_cache_threshold":0.95,"semantic_cache_ttl":0}}'
     headers:
       content-length:
-      - '568'
+      - '574'
       content-type:
       - application/json
       date:
-      - Tue, 07 May 2024 20:33:23 GMT
+      - Tue, 14 May 2024 19:47:08 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"text\":
@@ -71,22 +71,22 @@
       - '123'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/translate
   response:
     body:
-      string: '{"span_id":"2bd94406-84ac-4d87-8b3d-5c81992c63bc","message":null,"json_payload":"Hola","context":null,"cached":false}'
+      string: '{"span_id":"e0ce9a90-60a1-4545-bb3a-cabf0d8cead2","message":null,"json_payload":"Hola","context":null,"cached":false}'
     headers:
       content-length:
       - '117'
       content-type:
       - application/json
       date:
-      - Tue, 07 May 2024 20:33:23 GMT
+      - Tue, 14 May 2024 19:47:08 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"parent_span_uuid": null, "messages": [{"role": "user", "content": "{\"text\":
@@ -100,22 +100,22 @@
       - '123'
       content-type:
       - application/json
     method: POST
     uri: http://localhost:8000/v1/chat/translate
   response:
     body:
-      string: '{"span_id":"f4711620-f3c7-4136-9ad9-eb07a4dcf0cd","message":null,"json_payload":"Hola","context":null,"cached":false}'
+      string: "{\"span_id\":\"60281093-905d-4e50-b0bc-710259ca24c0\",\"message\":null,\"json_payload\":\"\xA1Hola\",\"context\":null,\"cached\":false}"
     headers:
       content-length:
-      - '117'
+      - '119'
       content-type:
       - application/json
       date:
-      - Tue, 07 May 2024 20:33:24 GMT
+      - Tue, 14 May 2024 19:47:09 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 - request:
     body: '{"dimension": "metric", "value": 1.0, "comment": null}'
@@ -125,24 +125,24 @@
       connection:
       - keep-alive
       content-length:
       - '54'
       content-type:
       - application/json
     method: POST
-    uri: http://localhost:8000/v1/spans/f4711620-f3c7-4136-9ad9-eb07a4dcf0cd/metrics
+    uri: http://localhost:8000/v1/spans/60281093-905d-4e50-b0bc-710259ca24c0/metrics
   response:
     body:
-      string: '{"id":"7da4b889-9809-46c6-8fb8-47e59d226d37","span_id":"f4711620-f3c7-4136-9ad9-eb07a4dcf0cd","dimension":"metric","value":1.0,"comment":null,"updated_at":null,"created_at":"2024-05-07T20:33:25.870248Z"}'
+      string: '{"id":"4d172cb9-295e-4456-b560-c8c7e5401b23","span_id":"60281093-905d-4e50-b0bc-710259ca24c0","dimension":"metric","value":1.0,"comment":null,"updated_at":null,"created_at":"2024-05-14T19:47:10.979159Z"}'
     headers:
       content-length:
       - '203'
       content-type:
       - application/json
       date:
-      - Tue, 07 May 2024 20:33:25 GMT
+      - Tue, 14 May 2024 19:47:10 GMT
       server:
       - uvicorn
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_image_file.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_image_file.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_image_url.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_image_url.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml` & `opperai-0.6.1/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/LICENSE` & `opperai-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opperai-0.6.0/README.md` & `opperai-0.6.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -31,14 +31,38 @@
 print(translate("Hello","fr"))
 
 >>> "Bonjour"
 ```
 
 The `fn` decorator automatically creates an Opper function ready to be called like any other function in your code. They're no different than any other function!
 
+### Using the `fn` decorator with images as inputs
+
+```python
+from opperai import fn
+from opperai.types import ImageContent
+from pydantic import BaseModel
+from typing import List
+
+class Word(BaseModel):
+    letters: List[str]
+
+@fn(model="openai/gpt-4o")
+def extract_letters(image: ImageContent) -> Word:
+    """given an image extract the word it represents"""
+
+letters = extract_letters(
+    ImageContent.from_path("tests/fixtures/images/letters.png"),
+)
+
+print(letters)
+```
+
+Note: one need to select the model that can handle images as inputs, see [models](https://docs.opper.ai/functions/models)
+
 ## Calling functions
 
 To call a function you created at [https://platform.opper.ai](https://platform.opper.ai) you can use the following code:
 
 
 ```python
 from opperai import Opper
```

### Comparing `opperai-0.6.0/pyproject.toml` & `opperai-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "opperai"
-version = "0.6.0"
+version = "0.6.1"
 description = "Opper Python client"
 authors = [
   {name = "Opper", email = "opper@opper.ai"},
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `opperai-0.6.0/PKG-INFO` & `opperai-0.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opperai
-Version: 0.6.0
+Version: 0.6.1
 Summary: Opper Python client
 Project-URL: Homepage, https://opper.ai
 Project-URL: Documentation, https://docs.opper.ai
 Project-URL: Platform, https://platform.opper.ai
 Author-email: Opper <opper@opper.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -54,14 +54,38 @@
 print(translate("Hello","fr"))
 
 >>> "Bonjour"
 ```
 
 The `fn` decorator automatically creates an Opper function ready to be called like any other function in your code. They're no different than any other function!
 
+### Using the `fn` decorator with images as inputs
+
+```python
+from opperai import fn
+from opperai.types import ImageContent
+from pydantic import BaseModel
+from typing import List
+
+class Word(BaseModel):
+    letters: List[str]
+
+@fn(model="openai/gpt-4o")
+def extract_letters(image: ImageContent) -> Word:
+    """given an image extract the word it represents"""
+
+letters = extract_letters(
+    ImageContent.from_path("tests/fixtures/images/letters.png"),
+)
+
+print(letters)
+```
+
+Note: one need to select the model that can handle images as inputs, see [models](https://docs.opper.ai/functions/models)
+
 ## Calling functions
 
 To call a function you created at [https://platform.opper.ai](https://platform.opper.ai) you can use the following code:
 
 
 ```python
 from opperai import Opper
```

