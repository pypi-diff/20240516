# Comparing `tmp/langfun-0.0.2.dev20240514.tar.gz` & `tmp/langfun-0.0.2.dev20240515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240514.tar", last modified: Tue May 14 08:03:52 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240515.tar", last modified: Wed May 15 08:04:19 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240514.tar` & `langfun-0.0.2.dev20240515.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.483254 langfun-0.0.2.dev20240514/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-14 08:03:52.483254 langfun-0.0.2.dev20240514/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.463254 langfun-0.0.2.dev20240514/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.467254 langfun-0.0.2.dev20240514/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.467254 langfun-0.0.2.dev20240514/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.471254 langfun-0.0.2.dev20240514/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.471254 langfun-0.0.2.dev20240514/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/eval/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/eval/patching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20202 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.475254 langfun-0.0.2.dev20240514/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.475254 langfun-0.0.2.dev20240514/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/openai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/llms/vertexai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.475254 langfun-0.0.2.dev20240514/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.475254 langfun-0.0.2.dev20240514/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.479254 langfun-0.0.2.dev20240514/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.483254 langfun-0.0.2.dev20240514/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:52.483254 langfun-0.0.2.dev20240514/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-14 08:03:52.000000 langfun-0.0.2.dev20240514/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-14 08:03:52.000000 langfun-0.0.2.dev20240514/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:03:52.000000 langfun-0.0.2.dev20240514/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 08:03:52.000000 langfun-0.0.2.dev20240514/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 08:03:52.000000 langfun-0.0.2.dev20240514/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:03:52.483254 langfun-0.0.2.dev20240514/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-14 08:03:23.000000 langfun-0.0.2.dev20240514/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.987388 langfun-0.0.2.dev20240515/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.995388 langfun-0.0.2.dev20240515/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.995388 langfun-0.0.2.dev20240515/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.995388 langfun-0.0.2.dev20240515/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.999389 langfun-0.0.2.dev20240515/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/patching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20202 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.999389 langfun-0.0.2.dev20240515/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.003389 langfun-0.0.2.dev20240515/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/openai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/vertexai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/vertexai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.003389 langfun-0.0.2.dev20240515/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.003389 langfun-0.0.2.dev20240515/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-15 08:04:18.000000 langfun-0.0.2.dev20240515/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-15 08:04:18.000000 langfun-0.0.2.dev20240515/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:04:18.000000 langfun-0.0.2.dev20240515/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 08:04:18.000000 langfun-0.0.2.dev20240515/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 08:04:18.000000 langfun-0.0.2.dev20240515/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/setup.py
```

### Comparing `langfun-0.0.2.dev20240514/LICENSE` & `langfun-0.0.2.dev20240515/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/PKG-INFO` & `langfun-0.0.2.dev20240515/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240514
+Version: 0.0.2.dev20240515
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240514/README.md` & `langfun-0.0.2.dev20240515/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/__init__.py` & `langfun-0.0.2.dev20240515/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/__init__.py` & `langfun-0.0.2.dev20240515/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240515/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/component.py` & `langfun-0.0.2.dev20240515/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/component_test.py` & `langfun-0.0.2.dev20240515/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240515/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240515/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/console.py` & `langfun-0.0.2.dev20240515/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/console_test.py` & `langfun-0.0.2.dev20240515/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240515/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240515/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240515/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240515/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240515/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/eval/patching.py` & `langfun-0.0.2.dev20240515/langfun/core/eval/patching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/eval/patching_test.py` & `langfun-0.0.2.dev20240515/langfun/core/eval/patching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240515/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240515/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240515/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240515/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/language_model.py` & `langfun-0.0.2.dev20240515/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240515/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,33 +31,47 @@
 from langfun.core.llms.google_genai import GeminiProVision
 from langfun.core.llms.google_genai import Palm2
 from langfun.core.llms.google_genai import Palm2_IT
 
 # OpenAI models.
 from langfun.core.llms.openai import OpenAI
 
+from langfun.core.llms.openai import Gpt4o
+from langfun.core.llms.openai import Gpt4o_20240513
+
 from langfun.core.llms.openai import Gpt4Turbo
 from langfun.core.llms.openai import Gpt4Turbo_20240409
 from langfun.core.llms.openai import Gpt4TurboPreview
-from langfun.core.llms.openai import Gpt4TurboPreview_0125
-from langfun.core.llms.openai import Gpt4TurboPreview_1106
+from langfun.core.llms.openai import Gpt4TurboPreview_20240125
+from langfun.core.llms.openai import Gpt4TurboPreview_20231106
 from langfun.core.llms.openai import Gpt4VisionPreview
-from langfun.core.llms.openai import Gpt4VisionPreview_1106
+from langfun.core.llms.openai import Gpt4VisionPreview_20231106
 from langfun.core.llms.openai import Gpt4
-from langfun.core.llms.openai import Gpt4_0613
+from langfun.core.llms.openai import Gpt4_20230613
+
 from langfun.core.llms.openai import Gpt4_32K
-from langfun.core.llms.openai import Gpt4_32K_0613
+from langfun.core.llms.openai import Gpt4_32K_20230613
 
 from langfun.core.llms.openai import Gpt35Turbo
-from langfun.core.llms.openai import Gpt35Turbo_0125
-from langfun.core.llms.openai import Gpt35Turbo_1106
-from langfun.core.llms.openai import Gpt35Turbo_0613
+from langfun.core.llms.openai import Gpt35Turbo_20240125
+from langfun.core.llms.openai import Gpt35Turbo_20231106
+from langfun.core.llms.openai import Gpt35Turbo_20230613
 from langfun.core.llms.openai import Gpt35Turbo16K
-from langfun.core.llms.openai import Gpt35Turbo16K_0613
+from langfun.core.llms.openai import Gpt35Turbo16K_20230613
 
+# For backward compatibility.
+Gpt4TurboPreview_0125 = Gpt4TurboPreview_20240125
+Gpt4TurboPreview_1106 = Gpt4TurboPreview_20231106
+Gpt4VisionPreview_1106 = Gpt4VisionPreview_20231106
+Gpt4_0613 = Gpt4_20230613
+Gpt4_32K_0613 = Gpt4_32K_20230613
+Gpt35Turbo_0125 = Gpt35Turbo_20240125
+Gpt35Turbo_1106 = Gpt35Turbo_20231106
+Gpt35Turbo_0613 = Gpt35Turbo_20230613
+Gpt35Turbo16K_0613 = Gpt35Turbo16K_20230613
 
 from langfun.core.llms.openai import Gpt35
 
 from langfun.core.llms.openai import Gpt3
 from langfun.core.llms.openai import Gpt3Curie
 from langfun.core.llms.openai import Gpt3Babbage
 from langfun.core.llms.openai import Gpt3Ada
```

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,17 @@
 # From https://platform.openai.com/settings/organization/limits
 _DEFAULT_TPM = 250000
 _DEFAULT_RPM = 3000
 
 SUPPORTED_MODELS_AND_SETTINGS = {
     # Models from https://platform.openai.com/docs/models
     # RPM is from https://platform.openai.com/docs/guides/rate-limits
-    # GPT-4-Turbo models
+    'gpt-4o': pg.Dict(rpm=10000, tpm=1500000),
+    'gpt-4o-2024-05-13': pg.Dict(rpm=10000, tpm=1500000),
+    # GPT-4-Turbo models.
     'gpt-4-turbo': pg.Dict(rpm=10000, tpm=1500000),
     'gpt-4-turbo-2024-04-09': pg.Dict(rpm=10000, tpm=1500000),
     'gpt-4-turbo-preview': pg.Dict(rpm=10000, tpm=1500000),
     'gpt-4-0125-preview': pg.Dict(rpm=10000, tpm=1500000),
     'gpt-4-1106-preview': pg.Dict(rpm=10000, tpm=1500000),
     'gpt-4-vision-preview': pg.Dict(rpm=10000, tpm=1500000),
     'gpt-4-1106-vision-preview': pg.Dict(
@@ -305,81 +307,93 @@
 
 
 class Gpt4TurboPreview(Gpt4):
   """GPT-4 Turbo Preview with 128k context window. Knowledge up to Dec. 2023."""
   model = 'gpt-4-turbo-preview'
 
 
-class Gpt4TurboPreview_0125(Gpt4TurboPreview):  # pylint: disable=invalid-name
+class Gpt4TurboPreview_20240125(Gpt4TurboPreview):  # pylint: disable=invalid-name
   """GPT-4 Turbo Preview with 128k context window. Knowledge up to Dec. 2023."""
   model = 'gpt-4-0125-preview'
 
 
-class Gpt4TurboPreview_1106(Gpt4TurboPreview):  # pylint: disable=invalid-name
+class Gpt4TurboPreview_20231106(Gpt4TurboPreview):  # pylint: disable=invalid-name
   """GPT-4 Turbo Preview with 128k context window. Knowledge up to Apr. 2023."""
   model = 'gpt-4-1106-preview'
 
 
 class Gpt4VisionPreview(Gpt4):
   """GPT-4 Turbo vision preview. 128k context window. Knowledge to Apr. 2023."""
   model = 'gpt-4-vision-preview'
   multimodal = True
 
 
-class Gpt4VisionPreview_1106(Gpt4):  # pylint: disable=invalid-name
+class Gpt4VisionPreview_20231106(Gpt4):  # pylint: disable=invalid-name
   """GPT-4 Turbo vision preview. 128k context window. Knowledge to Apr. 2023."""
   model = 'gpt-4-1106-vision-preview'
 
 
-class Gpt4_0613(Gpt4):    # pylint:disable=invalid-name
+class Gpt4_20230613(Gpt4):    # pylint:disable=invalid-name
   """GPT-4 @20230613. 8K context window. Knowledge up to 9-2021."""
   model = 'gpt-4-0613'
 
 
 class Gpt4_32K(Gpt4):       # pylint:disable=invalid-name
   """Latest GPT-4 with 32K context window."""
   model = 'gpt-4-32k'
 
 
-class Gpt4_32K_0613(Gpt4_32K):    # pylint:disable=invalid-name
+class Gpt4_32K_20230613(Gpt4_32K):    # pylint:disable=invalid-name
   """GPT-4 @20230613. 32K context window. Knowledge up to 9-2021."""
   model = 'gpt-4-32k-0613'
 
 
+class Gpt4o(OpenAI):
+  """GPT-4o."""
+  model = 'gpt-4o'
+  multimodal = True
+
+
+class Gpt4o_20240513(OpenAI):     # pylint:disable=invalid-name
+  """GPT-4o."""
+  model = 'gpt-4o-2024-05-13'
+  multimodal = True
+
+
 class Gpt35(OpenAI):
   """GPT-3.5. 4K max tokens, trained up on data up to Sep, 2021."""
   model = 'text-davinci-003'
 
 
 class Gpt35Turbo(Gpt35):
   """Most capable GPT-3.5 model, 10x cheaper than GPT35 (text-davinci-003)."""
   model = 'gpt-3.5-turbo'
 
 
-class Gpt35Turbo_0125(Gpt35Turbo):   # pylint:disable=invalid-name
+class Gpt35Turbo_20240125(Gpt35Turbo):   # pylint:disable=invalid-name
   """GPT-3.5 Turbo @20240125. 16K context window. Knowledge up to 09/2021."""
   model = 'gpt-3.5-turbo-0125'
 
 
-class Gpt35Turbo_1106(Gpt35Turbo):   # pylint:disable=invalid-name
+class Gpt35Turbo_20231106(Gpt35Turbo):   # pylint:disable=invalid-name
   """Gpt3.5 Turbo @20231106. 16K context window. Knowledge up to 09/2021."""
   model = 'gpt-3.5-turbo-1106'
 
 
-class Gpt35Turbo_0613(Gpt35Turbo):   # pylint:disable=invalid-name
+class Gpt35Turbo_20230613(Gpt35Turbo):   # pylint:disable=invalid-name
   """Gpt3.5 Turbo snapshot at 2023/06/13, with 4K context window size."""
   model = 'gpt-3.5-turbo-0613'
 
 
 class Gpt35Turbo16K(Gpt35Turbo):
   """Latest GPT-3.5 model with 16K context window size."""
   model = 'gpt-3.5-turbo-16k'
 
 
-class Gpt35Turbo16K_0613(Gpt35Turbo):   # pylint:disable=invalid-name
+class Gpt35Turbo16K_20230613(Gpt35Turbo):   # pylint:disable=invalid-name
   """Gtp 3.5 Turbo 16K 0613."""
   model = 'gpt-3.5-turbo-16k-0613'
 
 
 class Gpt3(OpenAI):
   """Most capable GPT-3 model (Davinci) 2K context window size.
```

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/vertexai.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/llms/vertexai_test.py` & `langfun-0.0.2.dev20240515/langfun/core/llms/vertexai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240515/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240515/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240515/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/memory.py` & `langfun-0.0.2.dev20240515/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/message.py` & `langfun-0.0.2.dev20240515/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/message_test.py` & `langfun-0.0.2.dev20240515/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240515/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240515/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240515/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240515/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240515/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240515/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240515/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/modality.py` & `langfun-0.0.2.dev20240515/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240515/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240515/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240515/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/sampling.py` & `langfun-0.0.2.dev20240515/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240515/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240515/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/subscription.py` & `langfun-0.0.2.dev20240515/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240515/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/template.py` & `langfun-0.0.2.dev20240515/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/template_test.py` & `langfun-0.0.2.dev20240515/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240515/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240515/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240515/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240515/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240515/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240515/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240515/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240515/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240515/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240515/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240515/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240515/langfun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240514
+Version: 0.0.2.dev20240515
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240514/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240515/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240514/setup.py` & `langfun-0.0.2.dev20240515/setup.py`

 * *Files identical despite different names*

