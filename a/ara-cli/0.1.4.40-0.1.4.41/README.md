# Comparing `tmp/ara_cli-0.1.4.40.tar.gz` & `tmp/ara_cli-0.1.4.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ara_cli-0.1.4.40.tar", last modified: Wed May 15 09:05:53 2024, max compression
+gzip compressed data, was "ara_cli-0.1.4.41.tar", last modified: Wed May 15 12:23:13 2024, max compression
```

## Comparing `ara_cli-0.1.4.40.tar` & `ara_cli-0.1.4.41.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.759873 ara_cli-0.1.4.40/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       37 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/MANIFEST.in
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-15 09:05:53.759873 ara_cli-0.1.4.40/PKG-INFO
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4668 2024-05-15 07:58:45.000000 ara_cli-0.1.4.40/README.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.747873 ara_cli-0.1.4.40/ara_cli/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       33 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/__init__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)    10783 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/__main__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2182 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/ara_config.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1916 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/artefact.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4786 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/artefact_creator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1583 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/artefact_deleter.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3710 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/artefact_link_updater.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      652 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/artefact_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3913 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/artefact_renamer.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3569 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/chat.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1446 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/classifier.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      108 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/classifier_validator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2690 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/directory_navigator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1369 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/file_classifier.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1695 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/file_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      118 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/filename_validator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5242 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/prompt_extractor.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)    15580 2024-05-15 06:23:20.000000 ara_cli-0.1.4.40/ara_cli/prompt_handler.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5674 2024-05-15 07:13:02.000000 ara_cli-0.1.4.40/ara_cli/prompt_rag.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2428 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/run_file_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6919 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/template_manager.py
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.751873 ara_cli-0.1.4.40/ara_cli/templates/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     8185 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/agile.artefacts
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.743873 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.751873 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.751873 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/prompts/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/prompts/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/prompts/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/prompts/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/prompts/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/prompts/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/prompts/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/prompts/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/prompts/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.755873 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.743873 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.755873 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      829 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_artefact_classification_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1061 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_artefact_extension_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      798 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_artefact_formulation_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1414 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_code_generation_complex_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      837 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_code_generation_simple_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      808 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_empty_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1426 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_error_fixing_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      833 2024-05-15 08:53:30.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_js_code_generation_simple_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1028 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_refactoring_analysis_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      933 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_refactoring_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      685 2024-05-15 08:07:38.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_reverse_engineer_feature_file_commands.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.755873 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      140 2024-05-15 08:43:22.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/extend_scenario_outline_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      126 2024-05-15 08:43:22.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/fix_steps_for_scenario_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      155 2024-05-15 08:43:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/formulate_new_feature_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      254 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_classify_task_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_empty_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      206 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_error_fixing_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      448 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_extend_feature_and_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       92 2024-05-15 08:09:32.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_feature_reverse_formulation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      391 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_feature_scenario_adaption_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      288 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_feature_scenario_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      207 2024-05-15 08:53:30.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_js_implementation_from_task_description_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      247 2024-05-15 08:53:30.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_js_steps_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      215 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_python_cli_implementation_with_test_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      450 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_python_code_understanding_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      288 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/prompts/template_python_implementation_from_task_description_intention_and_context.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.755873 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/rules/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       71 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/rules/template_empty_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1024 2024-05-15 09:05:07.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/rules/template_error_analysis_expert_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      471 2024-05-15 08:09:07.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/rules/template_gherkin_expert_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      814 2024-05-15 09:04:46.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/rules/template_js_expert_developer_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/rules/template_product_owner_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      600 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/rules/template_python_expert_developer_rules.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.759873 ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      893 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.concept.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2117 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1460 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.customer.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2273 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2329 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.persona.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4183 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1052 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.step.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.step_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      952 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.technology.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2274 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      559 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.businessgoal
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      217 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.businessgoal_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      523 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.capability
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.capability_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      680 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.epic
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.epic_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      416 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.example
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.example_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1053 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.feature
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.feature_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      745 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.issue
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      803 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.keyfeature
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      211 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.keyfeature_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.steps_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      533 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.task
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.task_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      727 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.userstory
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.userstory_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      640 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.vision
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      226 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/templates/template.vision_exploration.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.759873 ara_cli-0.1.4.40/ara_cli/tests/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/tests/__init__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2457 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/tests/test_artefact_link_updater.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5275 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/tests/test_artefact_renamer.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      236 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/tests/test_directory_navigator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3727 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/tests/test_file_creator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4036 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/tests/test_template_manager.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5402 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/ara_cli/vectorDB.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      146 2024-05-15 09:04:42.000000 ara_cli-0.1.4.40/ara_cli/version.py
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 09:05:53.747873 ara_cli-0.1.4.40/ara_cli.egg-info/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-15 09:05:53.000000 ara_cli-0.1.4.40/ara_cli.egg-info/PKG-INFO
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6997 2024-05-15 09:05:53.000000 ara_cli-0.1.4.40/ara_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        1 2024-05-15 09:05:53.000000 ara_cli-0.1.4.40/ara_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       78 2024-05-15 09:05:53.000000 ara_cli-0.1.4.40/ara_cli.egg-info/entry_points.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      145 2024-05-15 09:05:53.000000 ara_cli-0.1.4.40/ara_cli.egg-info/requires.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        8 2024-05-15 09:05:53.000000 ara_cli-0.1.4.40/ara_cli.egg-info/top_level.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       38 2024-05-15 09:05:53.759873 ara_cli-0.1.4.40/setup.cfg
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      782 2024-05-14 09:39:23.000000 ara_cli-0.1.4.40/setup.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.549416 ara_cli-0.1.4.41/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       37 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/MANIFEST.in
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-15 12:23:13.549416 ara_cli-0.1.4.41/PKG-INFO
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3774 2024-05-15 09:50:35.000000 ara_cli-0.1.4.41/README.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.533416 ara_cli-0.1.4.41/ara_cli/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       33 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/__init__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)    10783 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/__main__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2182 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/ara_config.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1916 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/artefact.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4786 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/artefact_creator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1583 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/artefact_deleter.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3710 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/artefact_link_updater.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      652 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/artefact_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3913 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/artefact_renamer.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3569 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/chat.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1446 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/classifier.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      108 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/classifier_validator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2690 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/directory_navigator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1369 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/file_classifier.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1695 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/file_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      118 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/filename_validator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5548 2024-05-15 11:55:09.000000 ara_cli-0.1.4.41/ara_cli/prompt_extractor.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)    15580 2024-05-15 06:23:20.000000 ara_cli-0.1.4.41/ara_cli/prompt_handler.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5674 2024-05-15 07:13:02.000000 ara_cli-0.1.4.41/ara_cli/prompt_rag.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2428 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/run_file_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6919 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/template_manager.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.537416 ara_cli-0.1.4.41/ara_cli/templates/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     8185 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/agile.artefacts
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.529416 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.537416 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.541416 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/prompts/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/prompts/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/prompts/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/prompts/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/prompts/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/prompts/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/prompts/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/prompts/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/prompts/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.541416 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.529416 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.541416 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      829 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_artefact_classification_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1061 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_artefact_extension_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      798 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_artefact_formulation_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1414 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_code_generation_complex_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      837 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_code_generation_simple_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      808 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_empty_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1426 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_error_fixing_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      833 2024-05-15 08:53:30.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_js_code_generation_simple_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1028 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_refactoring_analysis_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      933 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_refactoring_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      685 2024-05-15 08:07:38.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_reverse_engineer_feature_file_commands.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.545416 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      140 2024-05-15 08:43:22.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/extend_scenario_outline_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      126 2024-05-15 08:43:22.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/fix_steps_for_scenario_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      155 2024-05-15 08:43:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/formulate_new_feature_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      254 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_classify_task_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_empty_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      206 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_error_fixing_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      448 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_extend_feature_and_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       92 2024-05-15 08:09:32.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_feature_reverse_formulation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      391 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_feature_scenario_adaption_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      288 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_feature_scenario_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      207 2024-05-15 08:53:30.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_js_implementation_from_task_description_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      247 2024-05-15 08:53:30.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_js_steps_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      215 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_python_cli_implementation_with_test_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      450 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_python_code_understanding_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      288 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/prompts/template_python_implementation_from_task_description_intention_and_context.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.545416 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/rules/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       71 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/rules/template_empty_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1024 2024-05-15 09:05:07.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/rules/template_error_analysis_expert_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      471 2024-05-15 08:09:07.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/rules/template_gherkin_expert_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      814 2024-05-15 09:04:46.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/rules/template_js_expert_developer_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/rules/template_product_owner_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      600 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/rules/template_python_expert_developer_rules.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.545416 ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      893 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.concept.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2117 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1460 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.customer.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2273 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2329 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.persona.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4183 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1052 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.step.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.step_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      952 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.technology.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2274 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      559 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.businessgoal
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      217 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.businessgoal_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      523 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.capability
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.capability_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      680 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.epic
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.epic_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      416 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.example
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.example_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1053 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.feature
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.feature_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      745 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.issue
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      803 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.keyfeature
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      211 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.keyfeature_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.steps_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      533 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.task
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.task_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      727 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.userstory
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.userstory_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      640 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.vision
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      226 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/templates/template.vision_exploration.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.545416 ara_cli-0.1.4.41/ara_cli/tests/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/tests/__init__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2457 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/tests/test_artefact_link_updater.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5275 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/tests/test_artefact_renamer.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      236 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/tests/test_directory_navigator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3727 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/tests/test_file_creator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4036 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/tests/test_template_manager.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5402 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/ara_cli/vectorDB.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      146 2024-05-15 12:00:29.000000 ara_cli-0.1.4.41/ara_cli/version.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 12:23:13.533416 ara_cli-0.1.4.41/ara_cli.egg-info/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-15 12:23:13.000000 ara_cli-0.1.4.41/ara_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6997 2024-05-15 12:23:13.000000 ara_cli-0.1.4.41/ara_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        1 2024-05-15 12:23:13.000000 ara_cli-0.1.4.41/ara_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       78 2024-05-15 12:23:13.000000 ara_cli-0.1.4.41/ara_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      145 2024-05-15 12:23:13.000000 ara_cli-0.1.4.41/ara_cli.egg-info/requires.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        8 2024-05-15 12:23:13.000000 ara_cli-0.1.4.41/ara_cli.egg-info/top_level.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       38 2024-05-15 12:23:13.549416 ara_cli-0.1.4.41/setup.cfg
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      782 2024-05-14 09:39:23.000000 ara_cli-0.1.4.41/setup.py
```

### Comparing `ara_cli-0.1.4.40/README.md` & `ara_cli-0.1.4.41/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,17 @@
-- [ara-cli usage](#ara-cli-usage)
-  - [ara create](#ara-create)
-  - [ara prompt](#ara-prompt)
-    - [init / init-rag](#init--init-rag)
-  - [load](#load)
-  - [send](#send)
-  - [extract](#extract)
+- [ara usage](#ara-usage)
 - [ara-cli publish](#ara-cli-publish)
   - [best practices commit and merge and recreate workspace](#best-practices-commit-and-merge-and-recreate-workspace)
   - [test and run during development](#test-and-run-during-development)
   - [set version and build and install locally for testing outside of container](#set-version-and-build-and-install-locally-for-testing-outside-of-container)
   - [upload to test pypi with test pypi API key](#upload-to-test-pypi-with-test-pypi-api-key)
   - [upload to live pypi with talsen team production API key (from main branch)](#upload-to-live-pypi-with-talsen-team-production-api-key-from-main-branch)
 
-# ara-cli usage
-## ara create
-create an artefact with .data folder:
-
-    ara create <name> <classifier>
-
-## ara prompt
-### init / init-rag
-Initialize a prompt from an artefact (mostly a task)
-
-    ara prompt <name> <classifier> init
-
-or for interactive init:
-
-    ara prompt <name> <classifier> init-rag
-
-afterwards:
-
-* Write detailed artefact description
-* select files for "givens" section
-* select prompt templates (rules, intention&context, commands)
-
-## load
-
-    ara prompt <name> <classifier> load
-
-* refine promt templates
-
-## send
-
-    ara prompt <name> <classifier> send
-
-* select valuable parts of response 
-  
-## extract
-  copy to files. Make sure that only what you want to extract is marked with `# [x] extract`
-
-    ara prompt <name> <classifier> extract
-
-
+# ara usage 
+See [user readme](docs/README.md)
 
 # ara-cli publish
 ## best practices commit and merge and recreate workspace
 1. commit and publish everything in the branch
 2. go to git and merge
 3. destroy old workspace from merged branch from within the working directory
    > workspace destroy
```

### Comparing `ara_cli-0.1.4.40/ara_cli/__main__.py` & `ara_cli-0.1.4.41/ara_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/ara_config.py` & `ara_cli-0.1.4.41/ara_cli/ara_config.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/artefact.py` & `ara_cli-0.1.4.41/ara_cli/artefact.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/artefact_creator.py` & `ara_cli-0.1.4.41/ara_cli/artefact_creator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/artefact_deleter.py` & `ara_cli-0.1.4.41/ara_cli/artefact_deleter.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/artefact_link_updater.py` & `ara_cli-0.1.4.41/ara_cli/artefact_link_updater.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/artefact_lister.py` & `ara_cli-0.1.4.41/ara_cli/artefact_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/artefact_renamer.py` & `ara_cli-0.1.4.41/ara_cli/artefact_renamer.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/chat.py` & `ara_cli-0.1.4.41/ara_cli/chat.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/classifier.py` & `ara_cli-0.1.4.41/ara_cli/classifier.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/directory_navigator.py` & `ara_cli-0.1.4.41/ara_cli/directory_navigator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/file_classifier.py` & `ara_cli-0.1.4.41/ara_cli/file_classifier.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/file_lister.py` & `ara_cli-0.1.4.41/ara_cli/file_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/prompt_extractor.py` & `ara_cli-0.1.4.41/ara_cli/prompt_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,29 +47,34 @@
 
         if filename_from_response != file_path:
             user_decision = prompt_user_decision("Filename does not match, overwrite? (y/n): ")
             if user_decision.lower() not in ['y', 'yes']:
                 print("Debug: User chose not to overwrite")
                 print("Skipping block.")
                 return
-        content = response_data['content']
+        # Strip the first 2 lines from the content
+        content_lines = response_data['content'].split('\n')[2:]
+        stripped_content = '\n'.join(content_lines)
         with open(file_path, 'w', encoding='utf-8') as file:
-            file.write(content)
+            file.write(stripped_content)
             print(f"Debug: File {file_path} updated successfully.")
     except json.JSONDecodeError as ex:
         print(f"ERROR: Failed to decode JSON response: {ex}")
 
 def create_file_if_not_exist(filename, content):
     print(f"Debug: Checking if file exists: {filename}")
     if not os.path.exists(filename):
         print("Debug: File does not exist, prompting user")
         user_decision = prompt_user_decision("File does not exist. Create? (y/n): ")
         if user_decision.lower() in ['y', 'yes']:
+            # Strip the first 2 lines from the content
+            content_lines = content.split('\n')[2:]
+            stripped_content = '\n'.join(content_lines)
             with open(filename, 'w', encoding='utf-8') as file:
-                file.write(content)
+                file.write(stripped_content)
                 print(f"Debug: File {filename} created successfully.")
         else:
             print("Debug: User skipped file creation")
             print("File creation skipped by user.")
 
 def create_prompt_for_file_modification(content_str, filename):
     print(f"Debug: Creating modification prompt for {filename}")
```

### Comparing `ara_cli-0.1.4.40/ara_cli/prompt_handler.py` & `ara_cli-0.1.4.41/ara_cli/prompt_handler.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/prompt_rag.py` & `ara_cli-0.1.4.41/ara_cli/prompt_rag.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/run_file_lister.py` & `ara_cli-0.1.4.41/ara_cli/run_file_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/template_manager.py` & `ara_cli-0.1.4.41/ara_cli/template_manager.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/agile.artefacts` & `ara_cli-0.1.4.41/ara_cli/templates/agile.artefacts`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_businessgoal.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_businessgoal.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_capability.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_capability.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_epic.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_epic.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_feature.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_feature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_keyfeature.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_keyfeature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_task.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_task.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_userstory.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_userstory.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/commands/template_vision.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/commands/template_vision.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_businessgoal.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_businessgoal.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_capability.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_capability.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_epic.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_epic.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_feature.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_feature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_keyfeature.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_keyfeature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_task.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_task.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_userstory.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_userstory.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-creation/rules/template_vision.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-creation/rules/template_vision.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_artefact_classification_commands.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_artefact_classification_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_artefact_extension_commands.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_artefact_extension_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_artefact_formulation_commands.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_artefact_formulation_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_code_generation_complex_commands.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_code_generation_complex_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_code_generation_simple_commands.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_code_generation_simple_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_empty_commands.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_empty_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_error_fixing_commands.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_error_fixing_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_js_code_generation_simple_commands.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_js_code_generation_simple_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_refactoring_analysis_commands.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_refactoring_analysis_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_refactoring_commands.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_refactoring_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/commands/template_reverse_engineer_feature_file_commands.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/commands/template_reverse_engineer_feature_file_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/rules/template_error_analysis_expert_rules.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/rules/template_error_analysis_expert_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/rules/template_js_expert_developer_rules.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/rules/template_js_expert_developer_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/rules/template_product_owner_rules.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/rules/template_product_owner_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/prompt-modules/rules/template_python_expert_developer_rules.md` & `ara_cli-0.1.4.41/ara_cli/templates/prompt-modules/rules/template_python_expert_developer_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.concept.md` & `ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.concept.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md` & `ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.customer.md` & `ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.customer.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md` & `ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.persona.md` & `ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.persona.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md` & `ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.step.md` & `ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.step.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.technology.md` & `ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.technology.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md` & `ara_cli-0.1.4.41/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/template.businessgoal` & `ara_cli-0.1.4.41/ara_cli/templates/template.businessgoal`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/template.capability` & `ara_cli-0.1.4.41/ara_cli/templates/template.capability`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/template.epic` & `ara_cli-0.1.4.41/ara_cli/templates/template.epic`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/template.feature` & `ara_cli-0.1.4.41/ara_cli/templates/template.feature`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/template.issue` & `ara_cli-0.1.4.41/ara_cli/templates/template.issue`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/template.keyfeature` & `ara_cli-0.1.4.41/ara_cli/templates/template.keyfeature`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/template.task` & `ara_cli-0.1.4.41/ara_cli/templates/template.task`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/template.userstory` & `ara_cli-0.1.4.41/ara_cli/templates/template.userstory`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/templates/template.vision` & `ara_cli-0.1.4.41/ara_cli/templates/template.vision`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/tests/test_artefact_link_updater.py` & `ara_cli-0.1.4.41/ara_cli/tests/test_artefact_link_updater.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/tests/test_artefact_renamer.py` & `ara_cli-0.1.4.41/ara_cli/tests/test_artefact_renamer.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/tests/test_file_creator.py` & `ara_cli-0.1.4.41/ara_cli/tests/test_file_creator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/tests/test_template_manager.py` & `ara_cli-0.1.4.41/ara_cli/tests/test_template_manager.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli/vectorDB.py` & `ara_cli-0.1.4.41/ara_cli/vectorDB.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/ara_cli.egg-info/SOURCES.txt` & `ara_cli-0.1.4.41/ara_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.40/setup.py` & `ara_cli-0.1.4.41/setup.py`

 * *Files identical despite different names*

