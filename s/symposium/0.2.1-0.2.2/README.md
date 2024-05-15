# Comparing `tmp/symposium-0.2.1.tar.gz` & `tmp/symposium-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symposium-0.2.1.tar", last modified: Sat Apr 27 16:20:26 2024, max compression
+gzip compressed data, was "symposium-0.2.2.tar", last modified: Wed May 15 22:30:14 2024, max compression
```

## Comparing `symposium-0.2.1.tar` & `symposium-0.2.2.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.939495 symposium-0.2.1/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2023-09-13 23:21:39.000000 symposium-0.2.1/LICENSE
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)     9081 2024-04-27 16:20:26.939495 symposium-0.2.1/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     7903 2024-04-14 20:40:51.000000 symposium-0.2.1/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1025 2024-04-01 00:21:09.000000 symposium-0.2.1/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-04-27 16:20:26.939495 symposium-0.2.1/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.927495 symposium-0.2.1/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.931495 symposium-0.2.1/src/manual_testing/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1119 2024-03-21 15:06:52.000000 symposium-0.2.1/src/manual_testing/anthropic_native_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      984 2024-03-31 22:54:55.000000 symposium-0.2.1/src/manual_testing/anthropic_rest_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1997 2024-03-20 12:18:54.000000 symposium-0.2.1/src/manual_testing/gemini_rest_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2723 2024-04-27 16:17:06.000000 symposium-0.2.1/src/manual_testing/groq_rest_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      771 2024-03-16 13:50:13.000000 symposium-0.2.1/src/manual_testing/openai_native_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2695 2024-03-20 00:25:32.000000 symposium-0.2.1/src/manual_testing/openai_rest_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2387 2024-03-20 14:26:20.000000 symposium-0.2.1/src/manual_testing/palm_rest_test.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      385 2024-04-09 18:06:23.000000 symposium-0.2.1/src/manual_testing/yaml_config.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.931495 symposium-0.2.1/src/symposium/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-13 23:21:39.000000 symposium-0.2.1/src/symposium/__init__.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.931495 symposium-0.2.1/src/symposium/adapters/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-08 23:53:58.000000 symposium-0.2.1/src/symposium/adapters/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3226 2024-03-31 22:54:55.000000 symposium-0.2.1/src/symposium/adapters/anth.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2012 2024-03-20 00:25:32.000000 symposium-0.2.1/src/symposium/adapters/gem_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2796 2024-04-27 16:07:01.000000 symposium-0.2.1/src/symposium/adapters/grq_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      245 2024-03-19 23:38:45.000000 symposium-0.2.1/src/symposium/adapters/oai_native.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2799 2024-03-20 00:01:26.000000 symposium-0.2.1/src/symposium/adapters/oai_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1552 2024-03-20 13:30:26.000000 symposium-0.2.1/src/symposium/adapters/plm_rest.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.935495 symposium-0.2.1/src/symposium/connectors/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      753 2024-03-15 20:42:25.000000 symposium-0.2.1/src/symposium/connectors/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4825 2024-03-21 14:50:52.000000 symposium-0.2.1/src/symposium/connectors/anthropic_native.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4634 2024-03-31 22:50:13.000000 symposium-0.2.1/src/symposium/connectors/anthropic_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-02 14:53:27.000000 symposium-0.2.1/src/symposium/connectors/bedrock.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3406 2024-01-03 15:06:20.000000 symposium-0.2.1/src/symposium/connectors/brcloud.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      766 2024-03-06 19:20:16.000000 symposium-0.2.1/src/symposium/connectors/gemini_google.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6347 2024-03-20 00:25:32.000000 symposium-0.2.1/src/symposium/connectors/gemini_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6715 2023-10-24 22:57:19.000000 symposium-0.2.1/src/symposium/connectors/govert.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4139 2024-04-27 16:17:06.000000 symposium-0.2.1/src/symposium/connectors/groq_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      896 2023-10-29 23:20:06.000000 symposium-0.2.1/src/symposium/connectors/hugface.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6529 2024-03-16 13:50:13.000000 symposium-0.2.1/src/symposium/connectors/openai_native.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)    11100 2024-03-20 00:08:34.000000 symposium-0.2.1/src/symposium/connectors/openai_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1311 2024-03-03 14:20:15.000000 symposium-0.2.1/src/symposium/connectors/palm_google.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6420 2024-03-20 13:47:08.000000 symposium-0.2.1/src/symposium/connectors/palm_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-11-16 19:25:23.000000 symposium-0.2.1/src/symposium/connectors/together.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-02 14:53:27.000000 symposium-0.2.1/src/symposium/connectors/vertex.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6420 2023-12-08 20:56:28.000000 symposium-0.2.1/src/symposium/connectors/vertrest.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.935495 symposium-0.2.1/src/symposium/recorders/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      428 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/recorders/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4591 2024-04-12 12:32:29.000000 symposium-0.2.1/src/symposium/recorders/githublog.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.939495 symposium-0.2.1/src/symposium/templates/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/templates/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      311 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/templates/four_hypotheses.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      285 2023-09-26 18:39:22.000000 symposium-0.2.1/src/symposium/templates/one_thread.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3783 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/templates/sentence.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2834 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/templates/three_branch.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-21 19:23:09.000000 symposium-0.2.1/src/symposium/templates/two_branch.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.939495 symposium-0.2.1/src/symposium/util/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-19 23:31:57.000000 symposium-0.2.1/src/symposium/util/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2407 2024-03-19 23:38:45.000000 symposium-0.2.1/src/symposium/util/xml_tags.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.939495 symposium-0.2.1/src/symposium.egg-info/
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)     9081 2024-04-27 16:20:26.000000 symposium-0.2.1/src/symposium.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2017 2024-04-27 16:20:26.000000 symposium-0.2.1/src/symposium.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-04-27 16:20:26.000000 symposium-0.2.1/src/symposium.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      262 2024-04-27 16:20:26.000000 symposium-0.2.1/src/symposium.egg-info/requires.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       31 2024-04-27 16:20:26.000000 symposium-0.2.1/src/symposium.egg-info/top_level.txt
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-04-27 16:20:26.939495 symposium-0.2.1/src/tests/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        0 2024-03-05 19:48:52.000000 symposium-0.2.1/src/tests/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      847 2024-03-15 20:42:25.000000 symposium-0.2.1/src/tests/test_anthropic.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1273 2024-03-06 18:23:43.000000 symposium-0.2.1/src/tests/test_anthropic_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      404 2024-03-05 20:37:21.000000 symposium-0.2.1/src/tests/test_gemini_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      470 2024-03-15 20:42:25.000000 symposium-0.2.1/src/tests/test_openai.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      305 2024-03-05 20:00:36.000000 symposium-0.2.1/src/tests/test_openai_rest.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1884 2024-03-06 18:49:23.000000 symposium-0.2.1/src/tests/test_palm_rest.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-15 22:30:14.719122 symposium-0.2.2/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2023-09-13 23:21:39.000000 symposium-0.2.2/LICENSE
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)     9081 2024-05-15 22:30:14.719122 symposium-0.2.2/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     7903 2024-04-14 20:40:51.000000 symposium-0.2.2/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1025 2024-05-15 22:05:44.000000 symposium-0.2.2/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-15 22:30:14.719122 symposium-0.2.2/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-15 22:30:14.707122 symposium-0.2.2/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-15 22:30:14.707122 symposium-0.2.2/src/manual_testing/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1119 2024-03-21 15:06:52.000000 symposium-0.2.2/src/manual_testing/anthropic_native_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      984 2024-03-31 22:54:55.000000 symposium-0.2.2/src/manual_testing/anthropic_rest_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2018 2024-05-15 15:47:13.000000 symposium-0.2.2/src/manual_testing/gemini_google_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2038 2024-05-15 22:25:42.000000 symposium-0.2.2/src/manual_testing/gemini_rest_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2723 2024-04-27 16:17:06.000000 symposium-0.2.2/src/manual_testing/groq_rest_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      771 2024-03-16 13:50:13.000000 symposium-0.2.2/src/manual_testing/openai_native_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2695 2024-03-20 00:25:32.000000 symposium-0.2.2/src/manual_testing/openai_rest_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2387 2024-03-20 14:26:20.000000 symposium-0.2.2/src/manual_testing/palm_rest_test.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      385 2024-04-09 18:06:23.000000 symposium-0.2.2/src/manual_testing/yaml_config.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-15 22:30:14.707122 symposium-0.2.2/src/symposium/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-13 23:21:39.000000 symposium-0.2.2/src/symposium/__init__.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-15 22:30:14.711122 symposium-0.2.2/src/symposium/adapters/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-08 23:53:58.000000 symposium-0.2.2/src/symposium/adapters/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3226 2024-03-31 22:54:55.000000 symposium-0.2.2/src/symposium/adapters/anth.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2012 2024-03-20 00:25:32.000000 symposium-0.2.2/src/symposium/adapters/gem_native.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2012 2024-03-20 00:25:32.000000 symposium-0.2.2/src/symposium/adapters/gem_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2796 2024-04-27 16:07:01.000000 symposium-0.2.2/src/symposium/adapters/grq_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      245 2024-03-19 23:38:45.000000 symposium-0.2.2/src/symposium/adapters/oai_native.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2799 2024-03-20 00:01:26.000000 symposium-0.2.2/src/symposium/adapters/oai_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1552 2024-03-20 13:30:26.000000 symposium-0.2.2/src/symposium/adapters/plm_rest.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-15 22:30:14.715122 symposium-0.2.2/src/symposium/connectors/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      753 2024-03-15 20:42:25.000000 symposium-0.2.2/src/symposium/connectors/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4825 2024-03-21 14:50:52.000000 symposium-0.2.2/src/symposium/connectors/anthropic_native.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4634 2024-03-31 22:50:13.000000 symposium-0.2.2/src/symposium/connectors/anthropic_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-02 14:53:27.000000 symposium-0.2.2/src/symposium/connectors/bedrock.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3406 2024-01-03 15:06:20.000000 symposium-0.2.2/src/symposium/connectors/brcloud.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1048 2024-05-15 22:11:15.000000 symposium-0.2.2/src/symposium/connectors/gemini_google.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6347 2024-03-20 00:25:32.000000 symposium-0.2.2/src/symposium/connectors/gemini_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6715 2023-10-24 22:57:19.000000 symposium-0.2.2/src/symposium/connectors/govert.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4139 2024-04-27 16:17:06.000000 symposium-0.2.2/src/symposium/connectors/groq_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      896 2023-10-29 23:20:06.000000 symposium-0.2.2/src/symposium/connectors/hugface.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6529 2024-03-16 13:50:13.000000 symposium-0.2.2/src/symposium/connectors/openai_native.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)    11100 2024-03-20 00:08:34.000000 symposium-0.2.2/src/symposium/connectors/openai_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1311 2024-03-03 14:20:15.000000 symposium-0.2.2/src/symposium/connectors/palm_google.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6420 2024-03-20 13:47:08.000000 symposium-0.2.2/src/symposium/connectors/palm_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-11-16 19:25:23.000000 symposium-0.2.2/src/symposium/connectors/together.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-02 14:53:27.000000 symposium-0.2.2/src/symposium/connectors/vertex.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     6420 2023-12-08 20:56:28.000000 symposium-0.2.2/src/symposium/connectors/vertrest.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-15 22:30:14.715122 symposium-0.2.2/src/symposium/recorders/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      428 2023-09-21 19:23:09.000000 symposium-0.2.2/src/symposium/recorders/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4591 2024-04-12 12:32:29.000000 symposium-0.2.2/src/symposium/recorders/githublog.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-15 22:30:14.715122 symposium-0.2.2/src/symposium/templates/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-21 19:23:09.000000 symposium-0.2.2/src/symposium/templates/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      311 2023-09-21 19:23:09.000000 symposium-0.2.2/src/symposium/templates/four_hypotheses.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      285 2023-09-26 18:39:22.000000 symposium-0.2.2/src/symposium/templates/one_thread.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     3783 2023-09-21 19:23:09.000000 symposium-0.2.2/src/symposium/templates/sentence.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2834 2023-09-21 19:23:09.000000 symposium-0.2.2/src/symposium/templates/three_branch.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-09-21 19:23:09.000000 symposium-0.2.2/src/symposium/templates/two_branch.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-15 22:30:14.715122 symposium-0.2.2/src/symposium/util/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2024-03-19 23:31:57.000000 symposium-0.2.2/src/symposium/util/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2407 2024-03-19 23:38:45.000000 symposium-0.2.2/src/symposium/util/xml_tags.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-15 22:30:14.719122 symposium-0.2.2/src/symposium.egg-info/
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)     9081 2024-05-15 22:30:14.000000 symposium-0.2.2/src/symposium.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2095 2024-05-15 22:30:14.000000 symposium-0.2.2/src/symposium.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-15 22:30:14.000000 symposium-0.2.2/src/symposium.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      262 2024-05-15 22:30:14.000000 symposium-0.2.2/src/symposium.egg-info/requires.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       31 2024-05-15 22:30:14.000000 symposium-0.2.2/src/symposium.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-15 22:30:14.719122 symposium-0.2.2/src/tests/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        0 2024-03-05 19:48:52.000000 symposium-0.2.2/src/tests/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      847 2024-03-15 20:42:25.000000 symposium-0.2.2/src/tests/test_anthropic.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1273 2024-03-06 18:23:43.000000 symposium-0.2.2/src/tests/test_anthropic_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      404 2024-03-05 20:37:21.000000 symposium-0.2.2/src/tests/test_gemini_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      470 2024-03-15 20:42:25.000000 symposium-0.2.2/src/tests/test_openai.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      305 2024-03-05 20:00:36.000000 symposium-0.2.2/src/tests/test_openai_rest.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1884 2024-03-06 18:49:23.000000 symposium-0.2.2/src/tests/test_palm_rest.py
```

### Comparing `symposium-0.2.1/LICENSE` & `symposium-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/PKG-INFO` & `symposium-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symposium
-Version: 0.2.1
+Version: 0.2.2
 Summary: Interaction of multiple language models
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/symposium
 Project-URL: Bug Tracker, https://github.com/multilogue/sumposium/issues
 Keywords: symposium,conversations,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Requires-Dist: urllib3>=1.26.16
 Requires-Dist: grammateus>=0.0.10
 Provides-Extra: openai-native
 Requires-Dist: openai>=1.14.0; extra == "openai-native"
 Provides-Extra: anthropic-native
 Requires-Dist: anthropic>=0.21.1; extra == "anthropic-native"
 Provides-Extra: gemini-google
-Requires-Dist: google-generativeai>=0.4.1; extra == "gemini-google"
+Requires-Dist: google-generativeai>=0.5.3; extra == "gemini-google"
 Provides-Extra: bedrock
 Requires-Dist: boto3>=1.28.57; extra == "bedrock"
 Provides-Extra: vertex
 Requires-Dist: google-cloud-aiplatform>=1.43.0; extra == "vertex"
 Provides-Extra: github
 Requires-Dist: PyGithub>=1.59.0; extra == "github"
```

### Comparing `symposium-0.2.1/README.md` & `symposium-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/pyproject.toml` & `symposium-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "symposium"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Interaction of multiple language models"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
@@ -20,14 +20,14 @@
     "requests >= 2.31.0",
     "urllib3 >= 1.26.16",
     "grammateus >= 0.0.10",
 ]
 [project.optional-dependencies]
 openai_native = ["openai >= 1.14.0"]
 anthropic_native = ["anthropic >= 0.21.1"]
-gemini_google = ["google-generativeai >= 0.4.1"]
+gemini_google = ["google-generativeai >= 0.5.3"]
 bedrock = ["boto3 >= 1.28.57"]
 vertex = ["google-cloud-aiplatform >= 1.43.0"]
 github = ["PyGithub >= 1.59.0"]
 [project.urls]
 "Homepage" = "https://github.com/multilogue/symposium"
 "Bug Tracker" = "https://github.com/multilogue/sumposium/issues"
```

### Comparing `symposium-0.2.1/src/manual_testing/anthropic_native_test.py` & `symposium-0.2.2/src/manual_testing/anthropic_native_test.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/manual_testing/anthropic_rest_test.py` & `symposium-0.2.2/src/manual_testing/anthropic_rest_test.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/manual_testing/gemini_rest_test.py` & `symposium-0.2.2/src/manual_testing/gemini_rest_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 
 grammateus = Grammateus(origin='gemini', location='convers.log')
 
 messages = [
         {"role":"human", "name":"alex", "content":"Put your name between the <name></name> tags."},
 ]
 kwargs = {
+    "model": "gemini-1.5-flash-latest",
     "max_tokens": 256
 }
+
 message = gemini_message(
     messages=messages,
     recorder=grammateus,
     **kwargs
 )
 response=message
 print('ok')
```

### Comparing `symposium-0.2.1/src/manual_testing/groq_rest_test.py` & `symposium-0.2.2/src/manual_testing/groq_rest_test.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/manual_testing/openai_native_test.py` & `symposium-0.2.2/src/manual_testing/openai_native_test.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/manual_testing/openai_rest_test.py` & `symposium-0.2.2/src/manual_testing/openai_rest_test.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/manual_testing/palm_rest_test.py` & `symposium-0.2.2/src/manual_testing/palm_rest_test.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/adapters/anth.py` & `symposium-0.2.2/src/symposium/adapters/anth.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/adapters/gem_rest.py` & `symposium-0.2.2/src/symposium/adapters/gem_native.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/adapters/grq_rest.py` & `symposium-0.2.2/src/symposium/adapters/grq_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/adapters/oai_rest.py` & `symposium-0.2.2/src/symposium/adapters/oai_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/adapters/plm_rest.py` & `symposium-0.2.2/src/symposium/adapters/plm_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/__init__.py` & `symposium-0.2.2/src/symposium/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/anthropic_native.py` & `symposium-0.2.2/src/symposium/connectors/anthropic_native.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/anthropic_rest.py` & `symposium-0.2.2/src/symposium/connectors/anthropic_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/brcloud.py` & `symposium-0.2.2/src/symposium/connectors/brcloud.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/gemini_rest.py` & `symposium-0.2.2/src/symposium/connectors/gemini_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/govert.py` & `symposium-0.2.2/src/symposium/connectors/govert.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/groq_rest.py` & `symposium-0.2.2/src/symposium/connectors/groq_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/hugface.py` & `symposium-0.2.2/src/symposium/connectors/hugface.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/openai_native.py` & `symposium-0.2.2/src/symposium/connectors/openai_native.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/openai_rest.py` & `symposium-0.2.2/src/symposium/connectors/openai_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/palm_google.py` & `symposium-0.2.2/src/symposium/connectors/palm_google.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/palm_rest.py` & `symposium-0.2.2/src/symposium/connectors/palm_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/connectors/vertrest.py` & `symposium-0.2.2/src/symposium/connectors/vertrest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/recorders/githublog.py` & `symposium-0.2.2/src/symposium/recorders/githublog.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/templates/sentence.py` & `symposium-0.2.2/src/symposium/templates/sentence.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/templates/three_branch.py` & `symposium-0.2.2/src/symposium/templates/three_branch.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium/util/xml_tags.py` & `symposium-0.2.2/src/symposium/util/xml_tags.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/symposium.egg-info/PKG-INFO` & `symposium-0.2.2/src/symposium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symposium
-Version: 0.2.1
+Version: 0.2.2
 Summary: Interaction of multiple language models
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/symposium
 Project-URL: Bug Tracker, https://github.com/multilogue/sumposium/issues
 Keywords: symposium,conversations,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Requires-Dist: urllib3>=1.26.16
 Requires-Dist: grammateus>=0.0.10
 Provides-Extra: openai-native
 Requires-Dist: openai>=1.14.0; extra == "openai-native"
 Provides-Extra: anthropic-native
 Requires-Dist: anthropic>=0.21.1; extra == "anthropic-native"
 Provides-Extra: gemini-google
-Requires-Dist: google-generativeai>=0.4.1; extra == "gemini-google"
+Requires-Dist: google-generativeai>=0.5.3; extra == "gemini-google"
 Provides-Extra: bedrock
 Requires-Dist: boto3>=1.28.57; extra == "bedrock"
 Provides-Extra: vertex
 Requires-Dist: google-cloud-aiplatform>=1.43.0; extra == "vertex"
 Provides-Extra: github
 Requires-Dist: PyGithub>=1.59.0; extra == "github"
```

### Comparing `symposium-0.2.1/src/symposium.egg-info/SOURCES.txt` & `symposium-0.2.2/src/symposium.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
 src/manual_testing/anthropic_native_test.py
 src/manual_testing/anthropic_rest_test.py
+src/manual_testing/gemini_google_test.py
 src/manual_testing/gemini_rest_test.py
 src/manual_testing/groq_rest_test.py
 src/manual_testing/openai_native_test.py
 src/manual_testing/openai_rest_test.py
 src/manual_testing/palm_rest_test.py
 src/manual_testing/yaml_config.py
 src/symposium/__init__.py
 src/symposium.egg-info/PKG-INFO
 src/symposium.egg-info/SOURCES.txt
 src/symposium.egg-info/dependency_links.txt
 src/symposium.egg-info/requires.txt
 src/symposium.egg-info/top_level.txt
 src/symposium/adapters/__init__.py
 src/symposium/adapters/anth.py
+src/symposium/adapters/gem_native.py
 src/symposium/adapters/gem_rest.py
 src/symposium/adapters/grq_rest.py
 src/symposium/adapters/oai_native.py
 src/symposium/adapters/oai_rest.py
 src/symposium/adapters/plm_rest.py
 src/symposium/connectors/__init__.py
 src/symposium/connectors/anthropic_native.py
```

### Comparing `symposium-0.2.1/src/tests/test_anthropic.py` & `symposium-0.2.2/src/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/tests/test_anthropic_rest.py` & `symposium-0.2.2/src/tests/test_anthropic_rest.py`

 * *Files identical despite different names*

### Comparing `symposium-0.2.1/src/tests/test_palm_rest.py` & `symposium-0.2.2/src/tests/test_palm_rest.py`

 * *Files identical despite different names*

