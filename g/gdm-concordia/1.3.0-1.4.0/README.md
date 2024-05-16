# Comparing `tmp/gdm-concordia-1.3.0.tar.gz` & `tmp/gdm-concordia-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdm-concordia-1.3.0.tar", last modified: Sat May  4 18:13:24 2024, max compression
+gzip compressed data, was "gdm-concordia-1.4.0.tar", last modified: Thu May 16 11:41:17 2024, max compression
```

## Comparing `gdm-concordia-1.3.0.tar` & `gdm-concordia-1.4.0.tar`

### file list

```diff
@@ -1,112 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.649701 gdm-concordia-1.3.0/concordia/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.649701 gdm-concordia-1.3.0/concordia/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/agents/basic_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.649701 gdm-concordia-1.3.0/concordia/associative_memory/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/associative_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/associative_memory/associative_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/associative_memory/blank_memories.py
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/associative_memory/formative_memories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/associative_memory/importance_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.653701 gdm-concordia-1.3.0/concordia/clocks/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/clocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/clocks/game_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/clocks/game_clock_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.653701 gdm-concordia-1.3.0/concordia/components/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.653701 gdm-concordia-1.3.0/concordia/components/agent/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/all_similar_memories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/creative_reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/dialectical_reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/person_by_situation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/scheduled_hint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/self_perception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/situation_perception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/somatic_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/components/game_master/
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/current_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/current_scene_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/direct_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/player_status_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/relevant_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/time_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/report_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/document/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/document/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/document/document_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/document/interactive_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/document/interactive_document_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/game_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/game_master_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/environment/scenes/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/scenes/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/scenes/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/language_model/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/gcloud_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/gemini_vertex_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/gpt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/ollama_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/retry_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/common_sense_morality.py
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/dass_questionnaire.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/goal_achievement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/opinion_of_others.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/uncertainty_scale_question.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/concordia/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/tests/concordia_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/tests/mock_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/concordia/thought_chains/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/thought_chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/thought_chains/thought_chains.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/concordia/typing/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/game_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/concordia/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/measurements_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/gdm_concordia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-04 18:13:24.000000 gdm-concordia-1.3.0/gdm_concordia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-04 18:13:24.000000 gdm-concordia-1.3.0/gdm_concordia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:13:24.000000 gdm-concordia-1.3.0/gdm_concordia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-04 18:13:24.000000 gdm-concordia-1.3.0/gdm_concordia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-04 18:13:24.000000 gdm-concordia-1.3.0/gdm_concordia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.285225 gdm-concordia-1.4.0/concordia/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.285225 gdm-concordia-1.4.0/concordia/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/agents/basic_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.285225 gdm-concordia-1.4.0/concordia/associative_memory/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/associative_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/associative_memory/associative_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/associative_memory/blank_memories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/associative_memory/formative_memories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/associative_memory/importance_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.285225 gdm-concordia-1.4.0/concordia/clocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/clocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/clocks/game_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/clocks/game_clock_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.289224 gdm-concordia-1.4.0/concordia/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.289224 gdm-concordia-1.4.0/concordia/components/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/all_similar_memories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/creative_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/dialectical_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/justify_recent_voluntary_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/person_by_situation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/scheduled_hint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/self_perception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/situation_perception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/agent/somatic_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/components/game_master/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/current_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/current_scene_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/direct_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/player_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/relevant_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/schelling_diagram_payoffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/game_master/time_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/report_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/components/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/document/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/document/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/document/document_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/document/interactive_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/document/interactive_document_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/game_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/game_master_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/environment/scenes/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/scenes/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/environment/scenes/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/language_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/cloud_vertex_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/google_aistudio_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/gpt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/no_language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/ollama_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/language_model/retry_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.293224 gdm-concordia-1.4.0/concordia/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/common_sense_morality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17111 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/dass_questionnaire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/goal_achievement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/opinion_of_others.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/metrics/uncertainty_scale_question.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/concordia/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/tests/concordia_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/tests/mock_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/concordia/thought_chains/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/thought_chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/thought_chains/thought_chains.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/concordia/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/game_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/typing/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/concordia/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/measurements_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/concordia/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/gdm_concordia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-16 11:41:17.000000 gdm-concordia-1.4.0/gdm_concordia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-16 11:41:17.000000 gdm-concordia-1.4.0/gdm_concordia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 11:41:17.000000 gdm-concordia-1.4.0/gdm_concordia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 11:41:17.000000 gdm-concordia-1.4.0/gdm_concordia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 11:41:17.000000 gdm-concordia-1.4.0/gdm_concordia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 11:41:17.297225 gdm-concordia-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-16 11:41:16.000000 gdm-concordia-1.4.0/setup.py
```

### Comparing `gdm-concordia-1.3.0/LICENSE` & `gdm-concordia-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/PKG-INFO` & `gdm-concordia-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdm-concordia
-Version: 1.3.0
+Version: 1.4.0
 Summary: A library for building a generative model of social interacions.
 Home-page: https://github.com/google-deepmind/concordia
 Author: DeepMind
 Author-email: noreply@google.com
 License: Apache 2.0
 Download-URL: https://github.com/google-deepmind/concordia/releases
 Keywords: multi-agent agent-based-simulation generative-agents python machine-learning
```

### Comparing `gdm-concordia-1.3.0/README.md` & `gdm-concordia-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Concordia 
+# Concordia
 
 *A library for generative social simulation*
 
 [![Python](https://img.shields.io/pypi/pyversions/gdm-concordia.svg)](https://pypi.python.org/pypi/gdm-concordia)
 [![PyPI version](https://img.shields.io/pypi/v/gdm-concordia.svg)](https://pypi.python.org/pypi/gdm-concordia)
 [![PyPI tests](../../actions/workflows/pypi-test.yml/badge.svg)](../../actions/workflows/pypi-test.yml)
 [![Tests](../../actions/workflows/test-concordia.yml/badge.svg)](../../actions/workflows/test-concordia.yml)
@@ -69,19 +69,19 @@
     ```shell
     pytest --pyargs concordia
     ```
 
 
 ## Bring your own LLM
 
-To work, Concordia requires an access to an LLM API. Any LLM API that 
-supports sampling text would work. We tested Concordia with a model with 340B
-parameters. If using a custom LLM API, the user has to provide a text embedder
-to be used by the associative memory. By default we use the Sentence-T5 for
-this, but any fixed-dimensional embedding would work.
+To work, Concordia requires a access to an LLM API. Any LLM API that
+supports sampling text would work. We tested Concordia using a model with 340B
+parameters. The user must also provide a text embedder for the associative
+memory. Any fixed-dimensional embedding would work. Ideally it would be one that
+works well for sentence similarity or semantic search.
 
 ## Example usage
 
 Find below an illustrative social simulation where 4 friends are stuck in a
 snowed in pub. Two of them have a dispute over a crashed car.
 
 The agents are built using a simple reasoning inspired by March and Olsen (2011)
```

### Comparing `gdm-concordia-1.3.0/concordia/__init__.py` & `gdm-concordia-1.4.0/concordia/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/agents/__init__.py` & `gdm-concordia-1.4.0/concordia/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/agents/basic_agent.py` & `gdm-concordia-1.4.0/concordia/agents/basic_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
     self._clock = clock
     self._num_memories_retrieved = num_memories_retrieved
     self._user_controlled = user_controlled
     self._update_interval = update_interval
 
     self._under_interrogation = False
     self._state_lock = threading.Lock()
-    self._state: str | None
 
     self._components = {}
     for comp in components:
       self.add_component(comp)
 
     self._log = []
     self._last_chain_of_thought = None
```

### Comparing `gdm-concordia-1.3.0/concordia/associative_memory/__init__.py` & `gdm-concordia-1.4.0/concordia/associative_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/associative_memory/associative_memory.py` & `gdm-concordia-1.4.0/concordia/associative_memory/associative_memory.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/associative_memory/blank_memories.py` & `gdm-concordia-1.4.0/concordia/associative_memory/blank_memories.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/associative_memory/formative_memories.py` & `gdm-concordia-1.4.0/concordia/associative_memory/formative_memories.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/associative_memory/importance_function.py` & `gdm-concordia-1.4.0/concordia/associative_memory/importance_function.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/clocks/__init__.py` & `gdm-concordia-1.4.0/concordia/clocks/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/clocks/game_clock.py` & `gdm-concordia-1.4.0/concordia/clocks/game_clock.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/clocks/game_clock_test.py` & `gdm-concordia-1.4.0/concordia/clocks/game_clock_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/__init__.py` & `gdm-concordia-1.4.0/concordia/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/__init__.py` & `gdm-concordia-1.4.0/concordia/components/agent/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from concordia.components import report_function
 from concordia.components import sequential
 from concordia.components.agent import all_similar_memories
 from concordia.components.agent import characteristic
 from concordia.components.agent import creative_reflection
 from concordia.components.agent import dialectical_reflection
 from concordia.components.agent import identity
+from concordia.components.agent import justify_recent_voluntary_actions
 from concordia.components.agent import observation
 from concordia.components.agent import person_by_situation
 from concordia.components.agent import plan
 from concordia.components.agent import reflection
 from concordia.components.agent import relationships
 from concordia.components.agent import scheduled_hint
 from concordia.components.agent import self_perception
```

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/all_similar_memories.py` & `gdm-concordia-1.4.0/concordia/components/agent/all_similar_memories.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/characteristic.py` & `gdm-concordia-1.4.0/concordia/components/agent/characteristic.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/creative_reflection.py` & `gdm-concordia-1.4.0/concordia/components/agent/creative_reflection.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/dialectical_reflection.py` & `gdm-concordia-1.4.0/concordia/components/agent/dialectical_reflection.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     self._components = self._intuition_components + self._thinking_components
     if self._topic_component:
       self._components.append(self._topic_component)
 
     self._name = name
     self._history = []
-    self._last_update = self._clock_now() - datetime.timedelta(days=365)
+    self._last_update = datetime.datetime.min
 
   def name(self) -> str:
     return self._name
 
   def state(self) -> str:
     return self._state
```

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/identity.py` & `gdm-concordia-1.4.0/concordia/components/agent/identity.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/observation.py` & `gdm-concordia-1.4.0/concordia/components/agent/observation.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/person_by_situation.py` & `gdm-concordia-1.4.0/concordia/components/agent/person_by_situation.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/plan.py` & `gdm-concordia-1.4.0/concordia/components/agent/plan.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/reflection.py` & `gdm-concordia-1.4.0/concordia/components/agent/reflection.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/relationships.py` & `gdm-concordia-1.4.0/concordia/components/agent/relationships.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/scheduled_hint.py` & `gdm-concordia-1.4.0/concordia/components/agent/scheduled_hint.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/self_perception.py` & `gdm-concordia-1.4.0/concordia/components/agent/self_perception.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/situation_perception.py` & `gdm-concordia-1.4.0/concordia/components/agent/situation_perception.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/agent/somatic_state.py` & `gdm-concordia-1.4.0/concordia/components/agent/somatic_state.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/constant.py` & `gdm-concordia-1.4.0/concordia/components/constant.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/game_master/__init__.py` & `gdm-concordia-1.4.0/concordia/components/game_master/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-"""Library of components specifically for generative game master."""
+"""Library of components specifically for generative game masters."""
 
 from concordia.components.game_master import conversation
 from concordia.components.game_master import current_scene
 from concordia.components.game_master import direct_effect
 from concordia.components.game_master import inventory
 from concordia.components.game_master import player_status
 from concordia.components.game_master import relevant_events
 from concordia.components.game_master import schedule
+from concordia.components.game_master import schelling_diagram_payoffs
 from concordia.components.game_master import time_display
```

### Comparing `gdm-concordia-1.3.0/concordia/components/game_master/conversation.py` & `gdm-concordia-1.4.0/concordia/components/game_master/conversation.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/game_master/current_scene.py` & `gdm-concordia-1.4.0/concordia/components/game_master/current_scene.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,15 @@
   def name(self) -> str:
     return self._name
 
   def state(self) -> str:
     return self._current_scene_type
 
   def update(self) -> None:
+    self._current_scene_type = ''
     retrieved = self._memory.retrieve_by_regex(
         regex=r'\[scene type\].*',
         sort_by_time=True,
     )
     if retrieved:
       result = retrieved[-1]
       self._current_scene_type = result[
```

### Comparing `gdm-concordia-1.3.0/concordia/components/game_master/current_scene_test.py` & `gdm-concordia-1.4.0/concordia/components/game_master/current_scene_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/game_master/direct_effect.py` & `gdm-concordia-1.4.0/concordia/components/game_master/direct_effect.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/game_master/inventory.py` & `gdm-concordia-1.4.0/concordia/components/game_master/inventory.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/game_master/player_status.py` & `gdm-concordia-1.4.0/concordia/components/game_master/player_status.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/game_master/player_status_test.py` & `gdm-concordia-1.4.0/concordia/components/game_master/player_status_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/game_master/relevant_events.py` & `gdm-concordia-1.4.0/concordia/components/game_master/relevant_events.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/game_master/schedule.py` & `gdm-concordia-1.4.0/concordia/components/game_master/schedule.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 # limitations under the License.
 
 
 """This construct implements scheduled events."""
 
 import dataclasses
 import datetime
-from typing import Callable
-from typing import Optional
+from typing import Callable, Optional
 
 from concordia.typing import component
 
 
 @dataclasses.dataclass(frozen=True)
 class EventData:
   """Represents an event scheduled to happen at a specific time in the future.
@@ -42,26 +41,41 @@
 class Schedule(component.Component):
   """A memory construct that represents a schedule of events."""
 
   def __init__(
       self,
       clock_now: Callable[[], datetime.datetime],
       schedule: dict[str, EventData],
+      players_observe: bool = False,
   ):
     self._clock_now = clock_now
     self._schedule = schedule
     self._state = None
+    self._last_update = datetime.datetime.min
+    self._players_observe = players_observe
 
   def name(self) -> str:
     return 'Current events'
 
   def state(self) -> str | None:
     return self._state
 
+  def partial_state(
+      self,
+      player_name: str,
+  ) -> str | None:
+    """Return a player-specific view of the construct's state."""
+    if self._players_observe:
+      if self._state:
+        return self._state
+
   def update(self) -> None:
+    if self._last_update == self._clock_now():
+      return
+    self._last_update = self._clock_now()
     now = self._clock_now()
     events = []
     events_to_pop = []
     for event_name, event_data in self._schedule.items():
       if now == event_data.time:
         events.append(event_data.description)
         if event_data.trigger is not None:
@@ -70,8 +84,8 @@
 
     for event_name in events_to_pop:
       self._schedule.pop(event_name)
 
     if events:
       self._state = '\n'.join(events)
     else:
-      self._state = ''
+      self._state = 'None'
```

### Comparing `gdm-concordia-1.3.0/concordia/components/game_master/time_display.py` & `gdm-concordia-1.4.0/concordia/components/game_master/time_display.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/report_function.py` & `gdm-concordia-1.4.0/concordia/components/report_function.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/components/sequential.py` & `gdm-concordia-1.4.0/concordia/components/sequential.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/document/__init__.py` & `gdm-concordia-1.4.0/concordia/document/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/document/document.py` & `gdm-concordia-1.4.0/concordia/document/document.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/document/document_test.py` & `gdm-concordia-1.4.0/concordia/document/document_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/document/interactive_document.py` & `gdm-concordia-1.4.0/concordia/document/interactive_document.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/document/interactive_document_test.py` & `gdm-concordia-1.4.0/concordia/document/interactive_document_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/environment/__init__.py` & `gdm-concordia-1.4.0/concordia/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/environment/game_master.py` & `gdm-concordia-1.4.0/concordia/environment/game_master.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,20 +147,24 @@
       raise ValueError('Duplicate player names')
 
     self._concurrent_externalities = concurrent_externalities
     self._log = []
 
     self.reset()
 
-  def name(self):
+  @property
+  def name(self) -> str:
     return self._name
 
   def get_history(self):
     return self._log.copy()
 
+  def get_memory(self) -> associative_memory.AssociativeMemory:
+    return self._memory
+
   def get_data_frame(self):
     return self._memory.get_data_frame()
 
   def _print(self, entry, color=None):
     print(termcolor.colored(entry, color or self._log_color))
 
   def reset(self):
```

### Comparing `gdm-concordia-1.3.0/concordia/environment/game_master_test.py` & `gdm-concordia-1.4.0/concordia/environment/game_master_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/environment/scenes/__init__.py` & `gdm-concordia-1.4.0/concordia/environment/scenes/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/environment/scenes/conversation.py` & `gdm-concordia-1.4.0/concordia/environment/scenes/conversation.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/language_model/__init__.py` & `gdm-concordia-1.4.0/concordia/language_model/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/language_model/gcloud_model.py` & `gdm-concordia-1.4.0/concordia/language_model/ollama_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,114 @@
-# Copyright 2023 DeepMind Technologies Limited.
+# Copyright 2024 DeepMind Technologies Limited.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Google Cloud Language Model."""
+
+"""Ollama Language Model."""
 
 from collections.abc import Collection, Sequence
+import re
 
 from concordia.language_model import language_model
 from concordia.utils import measurements as measurements_lib
-from concordia.utils import text
-from google import auth
+from langchain import llms
 from typing_extensions import override
-import vertexai
-from vertexai.preview import language_models as vertex_models
 
-MAX_MULTIPLE_CHOICE_ATTEMPTS = 20
+
+def _extract_choices(text):
+  match = re.search(r"\(?(\w)\)", text)
+  if match:
+    return match.group(1)
+  return None
 
 
-class CloudLanguageModel(language_model.LanguageModel):
-  """Language model via a google cloud API."""
+class OllamaLanguageModel(language_model.LanguageModel):
+  """Language Model that uses Ollama LLM models."""
 
   def __init__(
       self,
-      project_id: str,
-      model_name: str = 'text-bison@001',
-      location: str = 'us-central1',
-      credentials: auth.credentials.Credentials | None = None,
+      model_name: str,
+      *,
+      system_message: str = "",
       measurements: measurements_lib.Measurements | None = None,
       channel: str = language_model.DEFAULT_STATS_CHANNEL,
   ) -> None:
-    """Initializes a model instance using the Google Cloud language model API.
+    """Initializes the instance.
 
     Args:
-      project_id: Google Cloud project id in API calls.
-      model_name: which language model to use
-      location: The location to use when making API calls.
-      credentials: Custom credentials to use when making API calls. If not
-        provided credentials will be ascertained from the environment.
-      measurements: The measurements object to log usage statistics to.
-      channel: The channel to write the statistics to.
+        model_name: The language model to use. For more details, see
+          https://github.com/ollama/ollama.
+        system_message: System message to prefix to requests when prompting the
+          model.
+        measurements: The measurements object to log usage statistics to.
+        channel: The channel to write the statistics to.
     """
-    if credentials is None:
-      credentials, _ = auth.default()
-    vertexai.init(
-        project=project_id, location=location, credentials=credentials
-    )
-    self._model = vertex_models.TextGenerationModel.from_pretrained(model_name)
+    self._model_name = model_name
+    self._system_message = system_message
     self._measurements = measurements
     self._channel = channel
+    self._client = llms.Ollama(model=model_name)
 
   @override
   def sample_text(
       self,
       prompt: str,
       *,
       max_tokens: int = language_model.DEFAULT_MAX_TOKENS,
       max_characters: int = language_model.DEFAULT_MAX_CHARACTERS,
       terminators: Collection[str] = language_model.DEFAULT_TERMINATORS,
       temperature: float = language_model.DEFAULT_TEMPERATURE,
       timeout: float = language_model.DEFAULT_TIMEOUT_SECONDS,
       seed: int | None = None,
   ) -> str:
-    if seed is not None:
-      raise NotImplementedError('Unclear how to set seed for cloud models.')
+    prompt_with_system_message = f"{self._system_message}\n\n{prompt}"
 
-    max_tokens = min(max_tokens, max_characters)
-    sample = self._model.predict(
-        prompt,
+    response = self._client(
+        prompt_with_system_message,
+        stop=terminators,
         temperature=temperature,
-        max_output_tokens=max_tokens,
     )
+
     if self._measurements is not None:
       self._measurements.publish_datum(
-          self._channel,
-          {'raw_text_length': len(sample)})
-    return text.truncate(
-        sample.text, max_length=max_characters, delimiters=terminators
-    )
+          self._channel, {"raw_text_length": len(response)}
+      )
+    return response
 
   @override
   def sample_choice(
       self,
       prompt: str,
       responses: Sequence[str],
       *,
       seed: int | None = None,
   ) -> tuple[int, str, dict[str, float]]:
-    max_characters = max([len(response) for response in responses])
-
-    attempts = 1
-    for _ in range(MAX_MULTIPLE_CHOICE_ATTEMPTS):
-      sample = self.sample_text(
-          prompt,
-          max_tokens=1,
-          max_characters=max_characters,
-          temperature=0.0,
-          seed=seed,
-      )
-      try:
-        idx = responses.index(sample)
-      except ValueError:
-        attempts += 1
-        continue
-      else:
-        if self._measurements is not None:
-          self._measurements.publish_datum(
-              self._channel,
-              {'choices_calls': attempts})
-        debug = {}
-        return idx, responses[idx], debug
-
-    raise language_model.InvalidResponseError(
-        'Too many multiple choice attempts.'
+    max_characters = len(max(responses, key=len))
+    prompt_with_system_message = f"{self._system_message}\n\n{prompt}"
+    sample = self.sample_text(
+        prompt_with_system_message,
+        max_characters=max_characters,
+        temperature=0.0,
+        seed=seed,
     )
+    answer = _extract_choices(sample)
+    try:
+      idx = responses.index(answer)
+    except ValueError:
+      raise language_model.InvalidResponseError(
+          f"Invalid response: {answer}. "
+          f"LLM Input: {prompt}\nLLM Output: {sample}"
+      ) from None
+
+    if self._measurements is not None:
+      self._measurements.publish_datum(self._channel, {"choices_calls": 1})
+    debug = {}
+    return idx, responses[idx], debug
```

### Comparing `gdm-concordia-1.3.0/concordia/language_model/gemini_vertex_model.py` & `gdm-concordia-1.4.0/concordia/language_model/cloud_vertex_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Google Cloud Gemini Vertex Language Model."""
+"""Google Cloud Vertex Language Model."""
 
 from collections.abc import Collection, Sequence
 import copy
 import re
 import time
 
 from concordia.language_model import language_model
@@ -67,16 +67,16 @@
   match = re.search(r'\(?(\w)\)', sample)
   if match:
     return match.group(1)
   else:
     return None
 
 
-class GeminiVertexLanguageModel(language_model.LanguageModel):
-  """Language model via the vertex API for Gemini (google cloud)."""
+class VertexLanguageModel(language_model.LanguageModel):
+  """Language model via the vertex API for Google Cloud."""
 
   def __init__(
       self,
       model_name: str = 'gemini-pro',
       harm_block_threshold: HarmBlockThreshold = HarmBlockThreshold.BLOCK_NONE,
       measurements: measurements_lib.Measurements | None = None,
       channel: str = language_model.DEFAULT_STATS_CHANNEL,
```

### Comparing `gdm-concordia-1.3.0/concordia/language_model/gpt_model.py` & `gdm-concordia-1.4.0/concordia/language_model/gpt_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,20 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Language Model that uses OpenAI's GPT models."""
 
 from collections.abc import Collection, Sequence
+import re
 from concordia.language_model import language_model
 from concordia.utils import measurements as measurements_lib
 import openai
 from typing_extensions import override
 
-_MAX_MULTIPLE_CHOICE_ATTEMPTS = 3
+_MAX_MULTIPLE_CHOICE_ATTEMPTS = 20
+
+
+def extract_response(sample: str):
+  """Given text formatted as 'lorum(a)ipsum', return 'a'."""
+  match = re.search(r'\(?(\w)\)', sample)
+  if match:
+    return match.group(1)
+  else:
+    return None
 
 
 class GptLanguageModel(language_model.LanguageModel):
   """Language Model that uses OpenAI GPT models."""
 
   def __init__(
       self,
@@ -59,15 +69,36 @@
       max_tokens: int = language_model.DEFAULT_MAX_TOKENS,
       max_characters: int = language_model.DEFAULT_MAX_CHARACTERS,
       terminators: Collection[str] = language_model.DEFAULT_TERMINATORS,
       temperature: float = language_model.DEFAULT_TEMPERATURE,
       timeout: float = language_model.DEFAULT_TIMEOUT_SECONDS,
       seed: int | None = None,
   ) -> str:
-    messages = [{'role': 'user', 'content': prompt}]
+    # gpt models do not support `max_characters`.
+    del max_characters
+    # gpt models do not support `max_tokens` > 4096.
+    max_tokens = min(max_tokens, 4000)
+
+    messages = [
+        {'role': 'system',
+         'content': ('You always continue sentences provided ' +
+                     'by the user and you never repeat what ' +
+                     'the user already said.')},
+        {'role': 'user',
+         'content': 'Question: Is Jake a turtle?\nAnswer: Jake is '},
+        {'role': 'assistant',
+         'content': 'not a turtle.'},
+        {'role': 'user',
+         'content': ('Question: What is Priya doing right now?\nAnswer: ' +
+                     'Priya is currently ')},
+        {'role': 'assistant',
+         'content': 'sleeping.'},
+        {'role': 'user',
+         'content': prompt}
+    ]
 
     response = self._client.chat.completions.create(
         model=self._model_name,
         messages=messages,
         temperature=temperature,
         max_tokens=max_tokens,
         timeout=timeout,
@@ -86,44 +117,54 @@
   def sample_choice(
       self,
       prompt: str,
       responses: Sequence[str],
       *,
       seed: int | None = None,
   ) -> tuple[int, str, dict[str, float]]:
-    max_characters = len(max(responses, key=len))
 
     attempts = 1
     prompt = (
         prompt
         + '\nRespond EXACTLY with one of the following strings:\n'
         + '\n'.join(responses) + '.'
     )
 
+    sample = ''
+    answer = ''
     for _ in range(_MAX_MULTIPLE_CHOICE_ATTEMPTS):
       # Increase temperature after the first failed attempt.
       temperature = 0.0
       if attempts > 1:
         temperature = 0.5
 
       sample = self.sample_text(
           prompt,
-          max_characters=max_characters,
           temperature=temperature,
           seed=seed,
       )
+      if len(sample) == 1:
+        # i.e. this would be a sample such as "a"
+        answer = sample
+      elif len(sample) == 2:
+        # i.e. this would be a sample such as "a)"
+        answer = sample[0]
+      else:
+        # extract a substring like "(a)" wherever it may be in a longer string
+        answer = extract_response(sample)
       try:
-        idx = responses.index(sample)
+        idx = responses.index(answer)
       except ValueError:
         attempts += 1
         continue
       else:
         if self._measurements is not None:
           self._measurements.publish_datum(
               self._channel, {'choices_calls': attempts}
           )
         debug = {}
         return idx, responses[idx], debug
 
     raise language_model.InvalidResponseError(
-        'Too many multiple choice attempts.'
+        (f'Too many multiple choice attempts.\nLast attempt: {sample}, ' +
+         f'extracted: {answer}')
     )
```

### Comparing `gdm-concordia-1.3.0/concordia/language_model/language_model.py` & `gdm-concordia-1.4.0/concordia/language_model/language_model.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/language_model/retry_wrapper.py` & `gdm-concordia-1.4.0/concordia/language_model/retry_wrapper.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/metrics/__init__.py` & `gdm-concordia-1.4.0/concordia/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/metrics/common_sense_morality.py` & `gdm-concordia-1.4.0/concordia/metrics/common_sense_morality.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,19 @@
     self._name = name
     self._clock = clock
     self._verbose = verbose
     self._player_name = player_name
     self._scale = scale or DEFAULT_SCALE
     self._measurements = measurements
     self._channel = channel
+    # Get the channel so it is initialized. This is not strictly necessary, but
+    # enables us to know which channels exist after initialization of agents and
+    # GM.
+    if self._measurements:
+      self._measurements.get_channel(self._channel)
 
     self._timestep = 0
 
   def name(
       self,
   ) -> str:
     """See base class."""
```

### Comparing `gdm-concordia-1.3.0/concordia/metrics/dass_questionnaire.py` & `gdm-concordia-1.4.0/concordia/metrics/dass_questionnaire.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,19 @@
     self._name = name
     self._context_fn = context_fn
     self._clock = clock
     self._verbose = verbose
     self._player_name = player_name
     self._measurements = measurements
     self._channel = channel
+    # Get the channel so it is initialized. This is not strictly necessary, but
+    # enables us to know which channels exist after initialization of agents and
+    # GM.
+    if self._measurements:
+      self._measurements.get_channel(self._channel)
     self._log_color = log_color
 
     self._timestep = 0
 
     # Note: the DASS questionnaire normally asks about the previous week.
     self._preprompt = (
         'Please indicate the extent to which the following statement applied ' +
```

### Comparing `gdm-concordia-1.3.0/concordia/metrics/goal_achievement.py` & `gdm-concordia-1.4.0/concordia/metrics/goal_achievement.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,19 @@
     self._player_name = player_name
     self._player_goal = player_goal
     self._clock = clock
     self._name = name
     self._scale = scale
     self._measurements = measurements
     self._channel = channel
+    # Get the channel so it is initialized. This is not strictly necessary, but
+    # enables us to know which channels exist after initialization of agents and
+    # GM.
+    if self._measurements:
+      self._measurements.get_channel(self._channel)
     self._verbose = verbose
 
     self._timestep = 0
 
   def name(
       self,
   ) -> str:
```

### Comparing `gdm-concordia-1.3.0/concordia/metrics/opinion_of_others.py` & `gdm-concordia-1.4.0/concordia/metrics/opinion_of_others.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,19 @@
     self._context_fn = context_fn
     if scale:
       self._scale = list(scale)
     else:
       raise ValueError('scale must be specified.')
     self._measurements = measurements
     self._channel = channel
+    # Get the channel so it is initialized. This is not strictly necessary, but
+    # enables us to know which channels exist after initialization of agents and
+    # GM.
+    if self._measurements:
+      self._measurements.get_channel(self._channel)
     self._question = question
 
     self._timestep = 0
 
   def name(
       self,
   ) -> str:
```

### Comparing `gdm-concordia-1.3.0/concordia/metrics/uncertainty_scale_question.py` & `gdm-concordia-1.4.0/concordia/metrics/uncertainty_scale_question.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,19 @@
     if scale:
       self._scale = list(scale)
     else:
       raise ValueError('scale must be specified.')
     self._verbose = verbose
     self._measurements = measurements
     self._channel = channel
+    # Get the channel so it is initialized. This is not strictly necessary, but
+    # enables us to know which channels exist after initialization of agents and
+    # GM.
+    if self._measurements:
+      self._measurements.get_channel(self._channel)
 
     self._timestep = 0
 
   def name(
       self,
   ) -> str:
     """Returns the name of the measurement."""
```

### Comparing `gdm-concordia-1.3.0/concordia/tests/__init__.py` & `gdm-concordia-1.4.0/concordia/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/tests/concordia_integration_test.py` & `gdm-concordia-1.4.0/concordia/tests/concordia_integration_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/tests/mock_model.py` & `gdm-concordia-1.4.0/concordia/tests/mock_model.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/thought_chains/__init__.py` & `gdm-concordia-1.4.0/concordia/thought_chains/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/thought_chains/thought_chains.py` & `gdm-concordia-1.4.0/concordia/thought_chains/thought_chains.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/typing/__init__.py` & `gdm-concordia-1.4.0/concordia/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/typing/agent.py` & `gdm-concordia-1.4.0/concordia/typing/agent.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/typing/clock.py` & `gdm-concordia-1.4.0/concordia/typing/clock.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/typing/component.py` & `gdm-concordia-1.4.0/concordia/typing/component.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Base class for generative agent (and game master) components."""
 
 import abc
-from typing import Self, Sequence
+from typing import Sequence
 
 
 class Component(metaclass=abc.ABCMeta):
   """A building block of a generative agent / game master.
 
   A concept constructed from memory or observations stream or (game master)
   event statements. Components mediate memory and observations into the
@@ -118,10 +118,10 @@
       self,
   ):
     """Returns a dictionary with latest log of activity."""
     return None
 
   def get_components(
       self,
-  ) -> Sequence[Self]:
+  ) -> Sequence['Component']:
     """Returns a list of components or an empty list."""
     return []
```

### Comparing `gdm-concordia-1.3.0/concordia/typing/game_master.py` & `gdm-concordia-1.4.0/concordia/typing/game_master.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/typing/scene.py` & `gdm-concordia-1.4.0/concordia/typing/scene.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """Dataclasses used to structure simulations using scenes."""
 
 from collections.abc import Callable, Mapping, Sequence
 import dataclasses
 import datetime
 
 from concordia.associative_memory import formative_memories
+from concordia.environment import game_master
 from concordia.typing import agent as agent_lib
 
 
 @dataclasses.dataclass(frozen=True)
 class SceneTypeSpec:
   """A specification for a type of scene.
 
@@ -31,20 +32,23 @@
     premise: map player names to messages they receive before the scene.
       Messages may be either literal strings or functions that return strings.
     conclusion: map player names to messages they receive after the scene.
       Messages may be either literal strings or functions mapping player names
       to strings.
     action_spec: optionally specify an action spec other than the default for
       the game master to ask the agents to produce during steps of this scene.
+    override_game_master: optionally specify a game master to use instead of the
+      default one.
   """
   name: str
   premise: Mapping[str, Sequence[str | Callable[[str], str]]] | None = None
   conclusion: Mapping[str,
                       Sequence[str | Callable[[str], str]]] | None = None
   action_spec: agent_lib.ActionSpec | None = None
+  override_game_master: game_master.GameMaster | None = None
 
 
 @dataclasses.dataclass(frozen=True)
 class SceneSpec:
   """Specify a specific scene.
 
   Attributes:
```

### Comparing `gdm-concordia-1.3.0/concordia/utils/__init__.py` & `gdm-concordia-1.4.0/concordia/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/utils/helper_functions.py` & `gdm-concordia-1.4.0/concordia/utils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/utils/html.py` & `gdm-concordia-1.4.0/concordia/utils/html.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/utils/measurements.py` & `gdm-concordia-1.4.0/concordia/utils/measurements.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/utils/measurements_test.py` & `gdm-concordia-1.4.0/concordia/utils/measurements_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/concordia/utils/plotting.py` & `gdm-concordia-1.4.0/concordia/utils/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
   Args:
     df: The dataframe containing the data to plot.
     scale: The set of possible values to plot.
     title: The title of the plot.
     group_by: Group data by this field, plot each one in its own figure.
     value: The name of the value to aggregate for the pie chart regions.
   """
-  cmap = mpl.colormaps['Paired']
+  cmap = mpl.colormaps['Paired']  # pylint: disable=unsubscriptable-object
   colours = cmap(range(len(scale)))
   scale_to_colour = dict(zip(scale, colours))
 
   for player, group_df in df.groupby(group_by):
     plt.figure()
     counts = group_df[value].value_counts()
     plt.pie(
```

### Comparing `gdm-concordia-1.3.0/concordia/utils/text.py` & `gdm-concordia-1.4.0/concordia/utils/text.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/gdm_concordia.egg-info/PKG-INFO` & `gdm-concordia-1.4.0/gdm_concordia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdm-concordia
-Version: 1.3.0
+Version: 1.4.0
 Summary: A library for building a generative model of social interacions.
 Home-page: https://github.com/google-deepmind/concordia
 Author: DeepMind
 Author-email: noreply@google.com
 License: Apache 2.0
 Download-URL: https://github.com/google-deepmind/concordia/releases
 Keywords: multi-agent agent-based-simulation generative-agents python machine-learning
```

### Comparing `gdm-concordia-1.3.0/gdm_concordia.egg-info/SOURCES.txt` & `gdm-concordia-1.4.0/gdm_concordia.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 concordia/components/sequential.py
 concordia/components/agent/__init__.py
 concordia/components/agent/all_similar_memories.py
 concordia/components/agent/characteristic.py
 concordia/components/agent/creative_reflection.py
 concordia/components/agent/dialectical_reflection.py
 concordia/components/agent/identity.py
+concordia/components/agent/justify_recent_voluntary_actions.py
 concordia/components/agent/observation.py
 concordia/components/agent/person_by_situation.py
 concordia/components/agent/plan.py
 concordia/components/agent/reflection.py
 concordia/components/agent/relationships.py
 concordia/components/agent/scheduled_hint.py
 concordia/components/agent/self_perception.py
@@ -38,31 +39,33 @@
 concordia/components/game_master/current_scene_test.py
 concordia/components/game_master/direct_effect.py
 concordia/components/game_master/inventory.py
 concordia/components/game_master/player_status.py
 concordia/components/game_master/player_status_test.py
 concordia/components/game_master/relevant_events.py
 concordia/components/game_master/schedule.py
+concordia/components/game_master/schelling_diagram_payoffs.py
 concordia/components/game_master/time_display.py
 concordia/document/__init__.py
 concordia/document/document.py
 concordia/document/document_test.py
 concordia/document/interactive_document.py
 concordia/document/interactive_document_test.py
 concordia/environment/__init__.py
 concordia/environment/game_master.py
 concordia/environment/game_master_test.py
 concordia/environment/scenes/__init__.py
 concordia/environment/scenes/conversation.py
 concordia/environment/scenes/runner.py
 concordia/language_model/__init__.py
-concordia/language_model/gcloud_model.py
-concordia/language_model/gemini_vertex_model.py
+concordia/language_model/cloud_vertex_model.py
+concordia/language_model/google_aistudio_model.py
 concordia/language_model/gpt_model.py
 concordia/language_model/language_model.py
+concordia/language_model/no_language_model.py
 concordia/language_model/ollama_model.py
 concordia/language_model/retry_wrapper.py
 concordia/metrics/__init__.py
 concordia/metrics/common_sense_morality.py
 concordia/metrics/dass_questionnaire.py
 concordia/metrics/goal_achievement.py
 concordia/metrics/opinion_of_others.py
```

### Comparing `gdm-concordia-1.3.0/pyproject.toml` & `gdm-concordia-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.3.0/setup.py` & `gdm-concordia-1.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """Install script for setuptools."""
 
 import setuptools
 
 setuptools.setup(
     name='gdm-concordia',
-    version='1.3.0',
+    version='1.4.0',
     license='Apache 2.0',
     license_files=['LICENSE'],
     url='https://github.com/google-deepmind/concordia',
     download_url='https://github.com/google-deepmind/concordia/releases',
     author='DeepMind',
     author_email='noreply@google.com',
     description=(
@@ -49,14 +49,15 @@
     packages=setuptools.find_packages(include=['concordia', 'concordia.*']),
     package_data={},
     python_requires='>=3.11',
     install_requires=(
         # TODO: b/312199199 - remove some requirements.
         'absl-py',
         'google-cloud-aiplatform',
+        'google-generativeai',
         'ipython',
         'langchain',
         'matplotlib',
         'numpy',
         'openai>=1.3.0',
         'pandas<=2.0.3',
         'python-dateutil',
```

