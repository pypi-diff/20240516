# Comparing `tmp/comet_llm-2.2.3.tar.gz` & `tmp/comet_llm-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_llm-2.2.3.tar", last modified: Tue May 14 16:09:14 2024, max compression
+gzip compressed data, was "comet_llm-2.2.4.tar", last modified: Thu May 16 10:50:37 2024, max compression
```

## Comparing `comet_llm-2.2.3.tar` & `comet_llm-2.2.4.tar`

### file list

```diff
@@ -1,108 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.337236 comet_llm-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-14 16:09:09.000000 comet_llm-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-14 16:09:14.337236 comet_llm-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-14 16:09:09.000000 comet_llm-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:09:14.337236 comet_llm-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-14 16:09:09.000000 comet_llm-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.317236 comet_llm-2.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.325236 comet_llm-2.2.3/src/comet_llm/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.325236 comet_llm-2.2.3/src/comet_llm/api_key/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/api_key/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/api_key/base64_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/api_key/comet_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.325236 comet_llm-2.2.3/src/comet_llm/api_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/api_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/api_objects/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/api_objects/llm_trace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.329236 comet_llm-2.2.3/src/comet_llm/autologgers/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/autologgers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/autologgers/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.329236 comet_llm-2.2.3/src/comet_llm/autologgers/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/autologgers/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/autologgers/openai/chat_completion_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/autologgers/openai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/autologgers/openai/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/autologgers/openai/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/autologgers/openai/patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/backend_error_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.329236 comet_llm-2.2.3/src/comet_llm/chains/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/chains/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/chains/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/chains/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/chains/deepmerge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/chains/span.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/chains/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/chains/thread_context_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/chains/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/datetimes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.329236 comet_llm-2.2.3/src/comet_llm/dummy_api/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/dummy_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/dummy_api/dummy_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.329236 comet_llm-2.2.3/src/comet_llm/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/exceptions/filter_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.333236 comet_llm-2.2.3/src/comet_llm/experiment_api/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/experiment_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/experiment_api/comet_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/experiment_api/experiment_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/experiment_api/failed_response_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/experiment_api/request_exception_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/experiment_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.333236 comet_llm-2.2.3/src/comet_llm/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.333236 comet_llm-2.2.3/src/comet_llm/import_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/import_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/import_hooks/callable_extenders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/import_hooks/callback_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/import_hooks/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/import_hooks/module_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/import_hooks/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/import_hooks/patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/import_hooks/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/import_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/import_hooks/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/import_hooks/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/llm_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/logging_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.333236 comet_llm-2.2.3/src/comet_llm/message_processing/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/message_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/message_processing/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/message_processing/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/message_processing/offline_message_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.333236 comet_llm-2.2.3/src/comet_llm/message_processing/offline_senders/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/message_processing/offline_senders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/message_processing/offline_senders/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/message_processing/offline_senders/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/message_processing/online_message_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.337236 comet_llm-2.2.3/src/comet_llm/message_processing/online_senders/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/message_processing/online_senders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/message_processing/online_senders/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/message_processing/online_senders/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.337236 comet_llm-2.2.3/src/comet_llm/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/prompts/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/prompts/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/prompts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/query_dsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-14 16:09:09.000000 comet_llm-2.2.3/src/comet_llm/url_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.337236 comet_llm-2.2.3/src/comet_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-14 16:09:14.000000 comet_llm-2.2.3/src/comet_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-14 16:09:14.000000 comet_llm-2.2.3/src/comet_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:09:14.000000 comet_llm-2.2.3/src/comet_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:09:14.000000 comet_llm-2.2.3/src/comet_llm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 16:09:14.000000 comet_llm-2.2.3/src/comet_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 16:09:14.000000 comet_llm-2.2.3/src/comet_llm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:09:14.337236 comet_llm-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-14 16:09:09.000000 comet_llm-2.2.3/tests/testlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.410051 comet_llm-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-16 10:50:33.000000 comet_llm-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-16 10:50:37.410051 comet_llm-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-16 10:50:33.000000 comet_llm-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:50:37.410051 comet_llm-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-16 10:50:33.000000 comet_llm-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.394051 comet_llm-2.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.398051 comet_llm-2.2.4/src/comet_llm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.402052 comet_llm-2.2.4/src/comet_llm/api_key/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/api_key/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/api_key/base64_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/api_key/comet_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.402052 comet_llm-2.2.4/src/comet_llm/api_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/api_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/api_objects/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/api_objects/llm_trace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.402052 comet_llm-2.2.4/src/comet_llm/autologgers/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/autologgers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/autologgers/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.402052 comet_llm-2.2.4/src/comet_llm/autologgers/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/autologgers/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/autologgers/openai/chat_completion_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/autologgers/openai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/autologgers/openai/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/autologgers/openai/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/autologgers/openai/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/backend_error_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.406051 comet_llm-2.2.4/src/comet_llm/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/chains/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/chains/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/chains/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/chains/deepmerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/chains/span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/chains/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/chains/thread_context_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/chains/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/datetimes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.406051 comet_llm-2.2.4/src/comet_llm/dummy_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/dummy_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/dummy_api/dummy_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.406051 comet_llm-2.2.4/src/comet_llm/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/exceptions/filter_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.406051 comet_llm-2.2.4/src/comet_llm/experiment_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/experiment_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/experiment_api/comet_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/experiment_api/error_codes_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/experiment_api/experiment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/experiment_api/payload_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/experiment_api/request_exception_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/experiment_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.406051 comet_llm-2.2.4/src/comet_llm/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.410051 comet_llm-2.2.4/src/comet_llm/import_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/import_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/import_hooks/callable_extenders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/import_hooks/callback_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/import_hooks/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/import_hooks/module_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/import_hooks/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/import_hooks/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/import_hooks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/import_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/import_hooks/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/import_hooks/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/llm_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/logging_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.410051 comet_llm-2.2.4/src/comet_llm/message_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/offline_message_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.410051 comet_llm-2.2.4/src/comet_llm/message_processing/offline_senders/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/offline_senders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/offline_senders/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/offline_senders/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/online_message_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.410051 comet_llm-2.2.4/src/comet_llm/message_processing/online_senders/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/online_senders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/online_senders/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/online_senders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/message_processing/online_senders/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.410051 comet_llm-2.2.4/src/comet_llm/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/prompts/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/prompts/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/prompts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/query_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/semantic_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-16 10:50:33.000000 comet_llm-2.2.4/src/comet_llm/url_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.410051 comet_llm-2.2.4/src/comet_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-16 10:50:37.000000 comet_llm-2.2.4/src/comet_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-16 10:50:37.000000 comet_llm-2.2.4/src/comet_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:50:37.000000 comet_llm-2.2.4/src/comet_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:50:37.000000 comet_llm-2.2.4/src/comet_llm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 10:50:37.000000 comet_llm-2.2.4/src/comet_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 10:50:37.000000 comet_llm-2.2.4/src/comet_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:50:37.410051 comet_llm-2.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-16 10:50:33.000000 comet_llm-2.2.4/tests/testlib.py
```

### Comparing `comet_llm-2.2.3/LICENSE` & `comet_llm-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/PKG-INFO` & `comet_llm-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_llm
-Version: 2.2.3
+Version: 2.2.4
 Summary: Comet logger for LLM
 Home-page: https://www.comet.com
 Author: Comet ML Inc.
 Author-email: mail@comet.com
 License: MIT
 Project-URL: Source code, https://github.com/comet-ml/comet-llm
 Keywords: comet_llm
```

### Comparing `comet_llm-2.2.3/README.md` & `comet_llm-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/setup.py` & `comet_llm-2.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,11 +55,11 @@
     include_package_data=True,
     keywords="comet_llm",
     name="comet_llm",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://www.comet.com",
     project_urls=project_urls,
-    version="2.2.3",
+    version="2.2.4",
     zip_safe=False,
     license="MIT",
 )
```

### Comparing `comet_llm-2.2.3/src/comet_llm/__init__.py` & `comet_llm-2.2.4/src/comet_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/api.py` & `comet_llm-2.2.4/src/comet_llm/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/api_key/__init__.py` & `comet_llm-2.2.4/src/comet_llm/api_key/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/api_key/base64_helper.py` & `comet_llm-2.2.4/src/comet_llm/api_key/base64_helper.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/api_key/comet_api_key.py` & `comet_llm-2.2.4/src/comet_llm/api_key/comet_api_key.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/api_objects/__init__.py` & `comet_llm-2.2.4/src/comet_llm/api_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/api_objects/api.py` & `comet_llm-2.2.4/src/comet_llm/api_objects/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/api_objects/llm_trace_api.py` & `comet_llm-2.2.4/src/comet_llm/api_objects/llm_trace_api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/app.py` & `comet_llm-2.2.4/src/comet_llm/app.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/autologgers/__init__.py` & `comet_llm-2.2.4/src/comet_llm/autologgers/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/autologgers/api.py` & `comet_llm-2.2.4/src/comet_llm/autologgers/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/autologgers/openai/__init__.py` & `comet_llm-2.2.4/src/comet_llm/autologgers/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/autologgers/openai/chat_completion_parsers.py` & `comet_llm-2.2.4/src/comet_llm/autologgers/openai/chat_completion_parsers.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/autologgers/openai/context.py` & `comet_llm-2.2.4/src/comet_llm/autologgers/openai/context.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/autologgers/openai/hooks.py` & `comet_llm-2.2.4/src/comet_llm/autologgers/openai/hooks.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/autologgers/openai/metadata.py` & `comet_llm-2.2.4/src/comet_llm/autologgers/openai/metadata.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/autologgers/openai/patcher.py` & `comet_llm-2.2.4/src/comet_llm/autologgers/openai/patcher.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/backend_error_codes.py` & `comet_llm-2.2.4/src/comet_llm/backend_error_codes.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/chains/__init__.py` & `comet_llm-2.2.4/src/comet_llm/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/chains/api.py` & `comet_llm-2.2.4/src/comet_llm/chains/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     return log_chain(global_chain)
 
 
 def log_chain(chain: chain.Chain) -> Optional[llm_result.LLMResult]:
     chain_data = chain.as_dict()
 
     message = messages.ChainMessage(
+        id=messages.generate_id(),
         experiment_info_=chain.experiment_info,
         tags=chain.tags,
         chain_data=chain_data,
         duration=chain_data["chain_duration"],
         metadata=chain_data["metadata"],
         others=chain.others,
     )
```

### Comparing `comet_llm-2.2.3/src/comet_llm/chains/chain.py` & `comet_llm-2.2.4/src/comet_llm/chains/chain.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/chains/context.py` & `comet_llm-2.2.4/src/comet_llm/chains/context.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/chains/deepmerge.py` & `comet_llm-2.2.4/src/comet_llm/chains/deepmerge.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/chains/span.py` & `comet_llm-2.2.4/src/comet_llm/chains/span.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/chains/state.py` & `comet_llm-2.2.4/src/comet_llm/chains/state.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/chains/thread_context_registry.py` & `comet_llm-2.2.4/src/comet_llm/chains/thread_context_registry.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/chains/version.py` & `comet_llm-2.2.4/src/comet_llm/chains/version.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/config.py` & `comet_llm-2.2.4/src/comet_llm/config.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/config_helper.py` & `comet_llm-2.2.4/src/comet_llm/config_helper.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/constants.py` & `comet_llm-2.2.4/src/comet_llm/constants.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/convert.py` & `comet_llm-2.2.4/src/comet_llm/convert.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/datetimes.py` & `comet_llm-2.2.4/src/comet_llm/datetimes.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/dummy_api/__init__.py` & `comet_llm-2.2.4/src/comet_llm/dummy_api/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/dummy_api/dummy_class.py` & `comet_llm-2.2.4/src/comet_llm/dummy_api/dummy_class.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/exceptions/__init__.py` & `comet_llm-2.2.4/src/comet_llm/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/exceptions/exceptions.py` & `comet_llm-2.2.4/src/comet_llm/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/exceptions/filter_decorator.py` & `comet_llm-2.2.4/src/comet_llm/exceptions/filter_decorator.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/experiment_api/__init__.py` & `comet_llm-2.2.4/src/comet_llm/experiment_api/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/experiment_api/comet_api_client.py` & `comet_llm-2.2.4/src/comet_llm/experiment_api/comet_api_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,34 +9,47 @@
 #  Sign up for free at https://www.comet.com
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this package.
 # *******************************************************
 
 import functools
+import logging
 import urllib.parse
 import warnings
-from typing import IO, List, Optional
+from typing import IO, Any, Dict, List, Optional
 
 import requests  # type: ignore
 import urllib3.exceptions
 
-from .. import config
+from .. import config, exceptions, semantic_version
 from ..types import JSONEncodable
-from . import request_exception_wrapper
+from . import error_codes_mapping, payload_constructor
 
 ResponseContent = JSONEncodable
 
+LOGGER = logging.getLogger(__name__)
+
 
 class CometAPIClient:
     def __init__(self, api_key: str, comet_url: str, session: requests.Session):
         self._headers = {"Authorization": api_key}
         self._comet_url = comet_url
         self._session = session
 
+        self.backend_version = semantic_version.SemanticVersion.parse(
+            self.is_alive_ver()["version"]
+        )
+
+    def is_alive_ver(self) -> ResponseContent:
+        return self._request(
+            "GET",
+            "api/isAlive/ver",
+        )
+
     def create_experiment(
         self,
         type_: str,
         workspace: Optional[str],
         project: Optional[str],
     ) -> ResponseContent:
         return self._request(
@@ -118,14 +131,64 @@
             json={
                 "experimentKey": experiment_key,
                 "key": name,
                 "value": value,
             },
         )
 
+    def log_chain(
+        self,
+        experiment_key: str,
+        chain_asset: Dict[str, JSONEncodable],
+        workspace: Optional[str] = None,
+        project: Optional[str] = None,
+        parameters: Optional[Dict[str, JSONEncodable]] = None,
+        metrics: Optional[Dict[str, JSONEncodable]] = None,
+        tags: Optional[List[str]] = None,
+        others: Optional[Dict[str, JSONEncodable]] = None,
+    ) -> ResponseContent:
+        json = [
+            {
+                "experimentKey": experiment_key,
+                "createExperimentRequest": {
+                    "workspaceName": workspace,
+                    "projectName": project,
+                    "type": "LLM",
+                },
+                "parameters": payload_constructor.chain_parameters_payload(parameters),
+                "metrics": payload_constructor.chain_metrics_payload(metrics),
+                "others": payload_constructor.chain_others_payload(others),
+                "tags": tags,
+                "jsonAsset": {
+                    "extension": "json",
+                    "type": "llm_data",
+                    "fileName": "comet_llm_data.json",
+                    "file": chain_asset,
+                },
+            }
+        ]  # we make a list because endpoint is designed for batches
+
+        batched_response: Dict[str, Dict[str, Any]] = self._request(
+            "POST",
+            "api/rest/v2/write/experiment/llm",
+            json=json,
+        )
+        sub_response = list(batched_response.values())[0]
+        status = sub_response["status"]
+        if status != 200:
+            LOGGER.debug(
+                "Failed to send trace: \nPayload %s, Response %s",
+                str(json),
+                str(batched_response),
+            )
+            error_code = sub_response["content"]["sdk_error_code"]
+            raise exceptions.CometLLMException(error_codes_mapping.MESSAGES[error_code])
+
+        return sub_response["content"]
+
     def _request(self, method: str, path: str, *args, **kwargs) -> ResponseContent:  # type: ignore
         url = urllib.parse.urljoin(self._comet_url, path)
         response = self._session.request(
             method=method,
             url=url,
             headers=self._headers,
             *args,
```

### Comparing `comet_llm-2.2.3/src/comet_llm/experiment_api/experiment_api.py` & `comet_llm-2.2.4/src/comet_llm/experiment_api/experiment_api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/experiment_api/request_exception_wrapper.py` & `comet_llm-2.2.4/src/comet_llm/experiment_api/request_exception_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 #  Sign up for free at https://www.comet.com
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this package.
 # *******************************************************
 
 import functools
+import json
 import logging
 import urllib.parse
 from pprint import pformat
-from typing import Any, Callable, List
+from typing import Any, Callable, List, NoReturn
 
 import requests  # type: ignore
 
 from .. import config, exceptions, logging_messages
-from . import failed_response_handler
+from . import error_codes_mapping
 
 LOGGER = logging.getLogger(__name__)
 
 
 def wrap(check_on_prem: bool = False) -> Callable:
     def inner_wrap(func: Callable) -> Callable:
         @functools.wraps(func)
@@ -45,15 +46,15 @@
                         ) from exception
 
                 if exception.response is None:
                     raise exceptions.CometLLMException(
                         logging_messages.FAILED_TO_SEND_DATA_TO_SERVER
                     ) from exception
 
-                failed_response_handler.handle(exception)
+                _handle_request_exception(exception)
 
         return wrapper
 
     return inner_wrap
 
 
 def _is_on_prem(url: str) -> bool:
@@ -69,7 +70,15 @@
 
         if exception.response is not None:
             LOGGER.debug(f"Response:\n{pformat(vars(exception.response))}")
     except Exception:
         # Make sure we won't fail on attempt to debug.
         # It's mainly for tests when response object can be mocked
         pass
+
+
+def _handle_request_exception(exception: requests.RequestException) -> NoReturn:
+    response = exception.response
+    sdk_error_code = json.loads(response.text)["sdk_error_code"]
+    error_message = error_codes_mapping.MESSAGES[sdk_error_code]
+
+    raise exceptions.CometLLMException(error_message) from exception
```

### Comparing `comet_llm-2.2.3/src/comet_llm/experiment_info.py` & `comet_llm-2.2.4/src/comet_llm/experiment_info.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/handlers/__init__.py` & `comet_llm-2.2.4/src/comet_llm/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/import_hooks/__init__.py` & `comet_llm-2.2.4/src/comet_llm/import_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/import_hooks/callable_extenders.py` & `comet_llm-2.2.4/src/comet_llm/import_hooks/callable_extenders.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/import_hooks/callback_runners.py` & `comet_llm-2.2.4/src/comet_llm/import_hooks/callback_runners.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/import_hooks/finder.py` & `comet_llm-2.2.4/src/comet_llm/import_hooks/finder.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/import_hooks/module_extension.py` & `comet_llm-2.2.4/src/comet_llm/import_hooks/module_extension.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/import_hooks/module_loader.py` & `comet_llm-2.2.4/src/comet_llm/import_hooks/module_loader.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/import_hooks/patcher.py` & `comet_llm-2.2.4/src/comet_llm/import_hooks/patcher.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/import_hooks/registry.py` & `comet_llm-2.2.4/src/comet_llm/import_hooks/registry.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/import_hooks/types.py` & `comet_llm-2.2.4/src/comet_llm/import_hooks/types.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/import_hooks/validate.py` & `comet_llm-2.2.4/src/comet_llm/import_hooks/validate.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/import_hooks/wrapper.py` & `comet_llm-2.2.4/src/comet_llm/import_hooks/wrapper.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/llm_result.py` & `comet_llm-2.2.4/src/comet_llm/llm_result.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/logging.py` & `comet_llm-2.2.4/src/comet_llm/logging.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/logging_messages.py` & `comet_llm-2.2.4/src/comet_llm/logging_messages.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/message_processing/__init__.py` & `comet_llm-2.2.4/src/comet_llm/message_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/message_processing/api.py` & `comet_llm-2.2.4/src/comet_llm/message_processing/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/message_processing/messages.py` & `comet_llm-2.2.4/src/comet_llm/message_processing/messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,32 +9,40 @@
 #  Sign up for free at https://www.comet.com
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this package.
 # *******************************************************
 
 import dataclasses
-import inspect
+import uuid
 from typing import Any, ClassVar, Dict, List, Optional, Union
 
 from comet_llm.types import JSONEncodable
 
 from .. import experiment_info, logging_messages
 
 
+def generate_id() -> str:
+    return uuid.uuid4().hex
+
+
 @dataclasses.dataclass
 class BaseMessage:
     experiment_info_: experiment_info.ExperimentInfo
+    id: str
     VERSION: ClassVar[int]
 
     @classmethod
     def from_dict(
         cls, d: Dict[str, Any], api_key: Optional[str] = None
     ) -> "BaseMessage":
-        d.pop("VERSION")  #
+        version = d.pop("VERSION")
+        if version == 1:
+            # Message was dumped before id was introduced. We can generate it now.
+            d["id"] = generate_id()
 
         experiment_info_dict: Dict[str, Optional[str]] = d.pop("experiment_info_")
         experiment_info_ = experiment_info.get(
             **experiment_info_dict,
             api_key=api_key,
             api_key_not_found_message=logging_messages.API_KEY_NOT_CONFIGURED
         )
@@ -53,20 +61,20 @@
 @dataclasses.dataclass
 class PromptMessage(BaseMessage):
     prompt_asset_data: Dict[str, Any]
     duration: Optional[float]
     metadata: Optional[Dict[str, Union[str, bool, float, None]]]
     tags: Optional[List[str]]
 
-    VERSION: ClassVar[int] = 1
+    VERSION: ClassVar[int] = 2
 
 
 @dataclasses.dataclass
 class ChainMessage(BaseMessage):
     chain_data: Dict[str, JSONEncodable]
     duration: float
     tags: Optional[List[str]]
     metadata: Optional[Dict[str, JSONEncodable]]
     others: Dict[str, JSONEncodable]
     # 'other' - is a name of an attribute of experiment, logged via log_other
 
-    VERSION: ClassVar[int] = 1
+    VERSION: ClassVar[int] = 2
```

### Comparing `comet_llm-2.2.3/src/comet_llm/message_processing/offline_message_processor.py` & `comet_llm-2.2.4/src/comet_llm/message_processing/offline_message_processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,23 +40,17 @@
     def process(self, message: messages.BaseMessage) -> None:
         with self._lock:
             self._update_current_file_if_needed()
             assert self._current_file_name is not None
             file_path = pathlib.Path(self._offline_directory, self._current_file_name)
 
             if isinstance(message, messages.PromptMessage):
-                try:
-                    return prompt.send(message, str(file_path))
-                except Exception:
-                    LOGGER.error("Failed to log prompt", exc_info=True)
+                return prompt.send(message, str(file_path))
             elif isinstance(message, messages.ChainMessage):
-                try:
-                    return chain.send(message, str(file_path))
-                except Exception:
-                    LOGGER.error("Failed to log chain", exc_info=True)
+                return chain.send(message, str(file_path))
 
         LOGGER.debug(f"Unsupported message type {message}")
         return None
 
     def _update_current_file_if_needed(self) -> None:
         current_time = time.time()
```

### Comparing `comet_llm-2.2.3/src/comet_llm/message_processing/offline_senders/__init__.py` & `comet_llm-2.2.4/src/comet_llm/message_processing/offline_senders/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/message_processing/offline_senders/chain.py` & `comet_llm-2.2.4/src/comet_llm/message_processing/offline_senders/chain.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/message_processing/offline_senders/prompt.py` & `comet_llm-2.2.4/src/comet_llm/message_processing/offline_senders/prompt.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/message_processing/online_message_processor.py` & `comet_llm-2.2.4/src/comet_llm/message_processing/online_message_processor.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,19 +24,13 @@
 
 class OnlineMessageProcessor:
     def __init__(self) -> None:
         pass
 
     def process(self, message: messages.BaseMessage) -> Optional[llm_result.LLMResult]:
         if isinstance(message, messages.PromptMessage):
-            try:
-                return prompt.send(message)
-            except Exception:
-                LOGGER.error("Failed to log prompt", exc_info=True)
+            return prompt.send(message)
         elif isinstance(message, messages.ChainMessage):
-            try:
-                return chain.send(message)
-            except Exception:
-                LOGGER.error("Failed to log chain", exc_info=True)
+            return chain.send(message)
 
         LOGGER.debug(f"Unsupported message type {message}")
         return None
```

### Comparing `comet_llm-2.2.3/src/comet_llm/message_processing/online_senders/__init__.py` & `comet_llm-2.2.4/src/comet_llm/message_processing/online_senders/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/message_processing/online_senders/chain.py` & `comet_llm-2.2.4/src/comet_llm/message_processing/online_senders/chain.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,20 +11,31 @@
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this package.
 # *******************************************************
 
 import io
 import json
 
-from comet_llm import app, convert, experiment_api, llm_result
+from comet_llm import app, convert, experiment_api, llm_result, url_helpers
+from comet_llm.experiment_api import comet_api_client
 
 from .. import messages
+from . import constants
 
 
 def send(message: messages.ChainMessage) -> llm_result.LLMResult:
+    client = comet_api_client.get(message.experiment_info_.api_key)
+
+    if client.backend_version >= constants.V2_BACKEND_VERSION:
+        return _send_v2(message, client)
+
+    return _send_v1(message)
+
+
+def _send_v1(message: messages.ChainMessage) -> llm_result.LLMResult:
     experiment_api_ = experiment_api.ExperimentAPI.create_new(
         api_key=message.experiment_info_.api_key,
         workspace=message.experiment_info_.workspace,
         project_name=message.experiment_info_.project_name,
     )
 
     if message.tags is not None:
@@ -44,7 +55,28 @@
 
     for name, value in message.others.items():
         experiment_api_.log_other(name, value)
 
     return llm_result.LLMResult(
         id=experiment_api_.id, project_url=experiment_api_.project_url
     )
+
+
+def _send_v2(
+    message: messages.ChainMessage, client: comet_api_client.CometAPIClient
+) -> llm_result.LLMResult:
+    metrics = {"chain_duration": message.duration}
+    parameters = convert.chain_metadata_to_flat_parameters(message.metadata)
+
+    response = client.log_chain(
+        experiment_key=message.id,
+        chain_asset=message.chain_data,
+        workspace=message.experiment_info_.workspace,
+        project=message.experiment_info_.project_name,
+        tags=message.tags,
+        metrics=metrics,
+        parameters=parameters,
+        others=message.others,
+    )
+    project_url: str = url_helpers.experiment_to_project_url(response["link"])
+
+    return llm_result.LLMResult(id=message.id, project_url=project_url)
```

### Comparing `comet_llm-2.2.3/src/comet_llm/prompts/__init__.py` & `comet_llm-2.2.4/src/comet_llm/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/prompts/api.py` & `comet_llm-2.2.4/src/comet_llm/prompts/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,17 @@
 #
 #  Sign up for free at https://www.comet.com
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this package.
 # *******************************************************
 
-import io
-import json
 from typing import Dict, List, Optional, Union
 
-import comet_llm.convert
-
-from .. import (
-    app,
-    config,
-    exceptions,
-    experiment_api,
-    experiment_info,
-    llm_result,
-    logging_messages,
-)
+from .. import app, config, exceptions, experiment_info, llm_result, logging_messages
 from ..chains import version
 from ..message_processing import api as message_processing_api, messages
 from . import convert, preprocess
 
 
 @exceptions.filter(allow_raising=config.raising_enabled(), summary=app.SUMMARY)
 def log_prompt(
@@ -128,14 +116,15 @@
         "metadata": metadata,
         "start_timestamp": timestamp,
         "end_timestamp": timestamp,
         "chain_duration": duration,
     }
 
     message = messages.PromptMessage(
+        id=messages.generate_id(),
         experiment_info_=info,
         prompt_asset_data=asset_data,
         duration=duration,
         metadata=metadata,
         tags=tags,
     )
```

### Comparing `comet_llm-2.2.3/src/comet_llm/prompts/convert.py` & `comet_llm-2.2.4/src/comet_llm/prompts/convert.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/prompts/preprocess.py` & `comet_llm-2.2.4/src/comet_llm/prompts/preprocess.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/query_dsl.py` & `comet_llm-2.2.4/src/comet_llm/query_dsl.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/summary.py` & `comet_llm-2.2.4/src/comet_llm/summary.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/types.py` & `comet_llm-2.2.4/src/comet_llm/types.py`

 * *Files identical despite different names*

### Comparing `comet_llm-2.2.3/src/comet_llm/url_helpers.py` & `comet_llm-2.2.4/src/comet_llm/url_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 #  Sign up for free at https://www.comet.com
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this package.
 # *******************************************************
 
+# vendored from and tested in comet-ml
+
 from urllib.parse import urljoin, urlparse, urlunparse
 
 
 def sanitize_url(url: str) -> str:
     """Sanitize an URL, checking that it is a valid URL and ensure it contains an ending slash /"""
     parts = urlparse(url)
     scheme, netloc, path, params, query, fragment = parts
@@ -49,7 +51,11 @@
 
 def get_root_url(url: str) -> str:
     """Remove the path, params, query and fragment from a given URL"""
     parts = urlparse(url)
     scheme, netloc, path, params, query, fragment = parts
 
     return urlunparse((scheme, netloc, "", "", "", ""))
+
+
+def experiment_to_project_url(experiment_url: str) -> str:
+    return "/".join(experiment_url.split("/")[:-1])
```

### Comparing `comet_llm-2.2.3/src/comet_llm.egg-info/PKG-INFO` & `comet_llm-2.2.4/src/comet_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_llm
-Version: 2.2.3
+Version: 2.2.4
 Summary: Comet logger for LLM
 Home-page: https://www.comet.com
 Author: Comet ML Inc.
 Author-email: mail@comet.com
 License: MIT
 Project-URL: Source code, https://github.com/comet-ml/comet-llm
 Keywords: comet_llm
```

### Comparing `comet_llm-2.2.3/src/comet_llm.egg-info/SOURCES.txt` & `comet_llm-2.2.4/src/comet_llm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/comet_llm/convert.py
 src/comet_llm/datetimes.py
 src/comet_llm/experiment_info.py
 src/comet_llm/llm_result.py
 src/comet_llm/logging.py
 src/comet_llm/logging_messages.py
 src/comet_llm/query_dsl.py
+src/comet_llm/semantic_version.py
 src/comet_llm/summary.py
 src/comet_llm/types.py
 src/comet_llm/url_helpers.py
 src/comet_llm.egg-info/PKG-INFO
 src/comet_llm.egg-info/SOURCES.txt
 src/comet_llm.egg-info/dependency_links.txt
 src/comet_llm.egg-info/not-zip-safe
@@ -50,16 +51,17 @@
 src/comet_llm/dummy_api/__init__.py
 src/comet_llm/dummy_api/dummy_class.py
 src/comet_llm/exceptions/__init__.py
 src/comet_llm/exceptions/exceptions.py
 src/comet_llm/exceptions/filter_decorator.py
 src/comet_llm/experiment_api/__init__.py
 src/comet_llm/experiment_api/comet_api_client.py
+src/comet_llm/experiment_api/error_codes_mapping.py
 src/comet_llm/experiment_api/experiment_api.py
-src/comet_llm/experiment_api/failed_response_handler.py
+src/comet_llm/experiment_api/payload_constructor.py
 src/comet_llm/experiment_api/request_exception_wrapper.py
 src/comet_llm/handlers/__init__.py
 src/comet_llm/import_hooks/__init__.py
 src/comet_llm/import_hooks/callable_extenders.py
 src/comet_llm/import_hooks/callback_runners.py
 src/comet_llm/import_hooks/finder.py
 src/comet_llm/import_hooks/module_extension.py
@@ -75,13 +77,14 @@
 src/comet_llm/message_processing/offline_message_processor.py
 src/comet_llm/message_processing/online_message_processor.py
 src/comet_llm/message_processing/offline_senders/__init__.py
 src/comet_llm/message_processing/offline_senders/chain.py
 src/comet_llm/message_processing/offline_senders/prompt.py
 src/comet_llm/message_processing/online_senders/__init__.py
 src/comet_llm/message_processing/online_senders/chain.py
+src/comet_llm/message_processing/online_senders/constants.py
 src/comet_llm/message_processing/online_senders/prompt.py
 src/comet_llm/prompts/__init__.py
 src/comet_llm/prompts/api.py
 src/comet_llm/prompts/convert.py
 src/comet_llm/prompts/preprocess.py
 tests/testlib.py
```

