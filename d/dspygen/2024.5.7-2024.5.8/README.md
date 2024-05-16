# Comparing `tmp/dspygen-2024.5.7.tar.gz` & `tmp/dspygen-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspygen-2024.5.7.tar", max compression
+gzip compressed data, was "dspygen-2024.5.8.tar", max compression
```

## Comparing `dspygen-2024.5.7.tar` & `dspygen-2024.5.8.tar`

### file list

```diff
@@ -1,461 +1,472 @@
--rw-r--r--   0        0        0     1069 2024-05-05 21:39:36.898989 dspygen-2024.5.7/LICENSE
--rw-r--r--   0        0        0    11342 2024-05-05 21:39:36.899104 dspygen-2024.5.7/README.md
--rw-r--r--   0        0        0     6806 2024-05-07 22:52:30.652088 dspygen-2024.5.7/pyproject.toml
--rw-r--r--   0        0        0     3048 2024-05-05 21:39:36.913212 dspygen-2024.5.7/src/dspygen/4www.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.913237 dspygen-2024.5.7/src/dspygen/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.913298 dspygen-2024.5.7/src/dspygen/agents/__init__.py
--rw-r--r--   0        0        0     4085 2024-05-05 21:39:36.913365 dspygen-2024.5.7/src/dspygen/agents/coder_agent.py
--rw-r--r--   0        0        0     3155 2024-05-05 21:39:36.913432 dspygen-2024.5.7/src/dspygen/agents/coder_agent_v2.py
--rw-r--r--   0        0        0     3854 2024-05-05 21:39:36.913478 dspygen-2024.5.7/src/dspygen/agents/coder_agent_v3.py
--rw-r--r--   0        0        0     4139 2024-05-07 03:32:57.110303 dspygen-2024.5.7/src/dspygen/agents/coder_agent_v4.py
--rw-r--r--   0        0        0     3706 2024-05-07 03:32:57.112778 dspygen-2024.5.7/src/dspygen/agents/pytest_agent.py
--rw-r--r--   0        0        0     6992 2024-05-06 00:43:13.492936 dspygen-2024.5.7/src/dspygen/agents/research_agent.py
--rw-r--r--   0        0        0     2278 2024-05-05 21:39:36.913588 dspygen-2024.5.7/src/dspygen/api.py
--rw-r--r--   0        0        0     1019 2024-05-05 21:39:36.913639 dspygen-2024.5.7/src/dspygen/app.py
--rw-r--r--   0        0        0      731 2024-05-05 21:39:36.913693 dspygen-2024.5.7/src/dspygen/async_typer.py
--rw-r--r--   0        0        0      216 2024-05-05 21:39:36.913914 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/book.toml
--rw-r--r--   0        0        0     2190 2024-05-05 21:39:36.913998 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/SUMMARY.md
--rw-r--r--   0        0        0       13 2024-05-05 21:39:36.914070 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/appendices/README.md
--rw-r--r--   0        0        0       18 2024-05-05 21:39:36.914111 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/appendices/further-reading.md
--rw-r--r--   0        0        0       11 2024-05-05 21:39:36.914156 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/appendices/glossary.md
--rw-r--r--   0        0        0       14 2024-05-05 21:39:36.914238 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/architecture/actor-model.md
--rw-r--r--   0        0        0       21 2024-05-05 21:39:36.914281 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/architecture/content-management.md
--rw-r--r--   0        0        0       15 2024-05-05 21:39:36.914327 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/architecture/domain-model.md
--rw-r--r--   0        0        0       28 2024-05-05 21:39:36.914368 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/architecture/event-driven.md
--rw-r--r--   0        0        0       22 2024-05-05 21:39:36.914421 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/architecture/feedback-generation.md
--rw-r--r--   0        0        0       22 2024-05-05 21:39:36.914464 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/architecture/question-generation.md
--rw-r--r--   0        0        0       19 2024-05-05 21:39:36.914527 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/architecture/student-modeling.md
--rw-r--r--   0        0        0       54 2024-05-05 21:39:36.914631 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/best-practices/collaboration.md
--rw-r--r--   0        0        0       29 2024-05-05 21:39:36.914698 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/best-practices/domain-modeling.md
--rw-r--r--   0        0        0       32 2024-05-05 21:39:36.914775 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/best-practices/error-handling.md
--rw-r--r--   0        0        0       22 2024-05-05 21:39:36.914925 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/best-practices/future-enhancements.md
--rw-r--r--   0        0        0       27 2024-05-05 21:39:36.915093 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/best-practices/performance.md
--rw-r--r--   0        0        0       12 2024-05-05 21:39:36.915154 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/chapter_1.md
--rw-r--r--   0        0        0       34 2024-05-05 21:39:36.915253 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/foundations/ddd.md
--rw-r--r--   0        0        0       22 2024-05-05 21:39:36.915521 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/foundations/language-models/in-context-learning.md
--rw-r--r--   0        0        0       21 2024-05-05 21:39:36.915581 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/foundations/language-models/prompt-engineering.md
--rw-r--r--   0        0        0       25 2024-05-05 21:39:36.915634 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/foundations/language-models/sparse-representations.md
--rw-r--r--   0        0        0       18 2024-05-05 21:39:36.915311 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/foundations/language-models.md
--rw-r--r--   0        0        0       24 2024-05-05 21:39:36.915686 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/foundations/reactive.md
--rw-r--r--   0        0        0       23 2024-05-05 21:39:36.915767 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/implementation/application-services.md
--rw-r--r--   0        0        0       33 2024-05-05 21:39:36.915825 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/implementation/code-generation.md
--rw-r--r--   0        0        0       18 2024-05-05 21:39:36.915877 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/implementation/domain-services.md
--rw-r--r--   0        0        0       18 2024-05-05 21:39:36.916029 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/implementation/infrastructure/message-brokers.md
--rw-r--r--   0        0        0       14 2024-05-05 21:39:36.916083 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/implementation/infrastructure/persistence.md
--rw-r--r--   0        0        0       17 2024-05-05 21:39:36.915933 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/implementation/infrastructure.md
--rw-r--r--   0        0        0       29 2024-05-05 21:39:36.916136 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/implementation/language-model-integration.md
--rw-r--r--   0        0        0       20 2024-05-05 21:39:36.916189 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/implementation/project-structure.md
--rw-r--r--   0        0        0       15 2024-05-05 21:39:36.916281 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/introduction/overview.md
--rw-r--r--   0        0        0       38 2024-05-05 21:39:36.916373 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/testing/ci-cd.md
--rw-r--r--   0        0        0       22 2024-05-05 21:39:36.916427 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/testing/integration-testing.md
--rw-r--r--   0        0        0       31 2024-05-05 21:39:36.916480 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/testing/monitoring.md
--rw-r--r--   0        0        0       15 2024-05-05 21:39:36.916538 dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/testing/unit-testing.md
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.916606 dspygen-2024.5.7/src/dspygen/bpel_diagrams/__init__.py
--rw-r--r--   0        0        0     5857 2024-05-05 21:39:36.916707 dspygen-2024.5.7/src/dspygen/bpel_diagrams/mermaid_multi_module_demo.py
--rw-r--r--   0        0        0       49 2024-05-05 21:39:36.916799 dspygen-2024.5.7/src/dspygen/bpel_models/__init__.py
--rw-r--r--   0        0        0    12392 2024-05-05 21:39:36.916873 dspygen-2024.5.7/src/dspygen/bpel_models/activities.py
--rw-r--r--   0        0        0     4328 2024-05-05 21:39:36.916958 dspygen-2024.5.7/src/dspygen/bpel_models/correlations.py
--rw-r--r--   0        0        0     2976 2024-05-05 21:39:36.917023 dspygen-2024.5.7/src/dspygen/bpel_models/event_handlers.py
--rw-r--r--   0        0        0     5007 2024-05-05 21:39:36.917095 dspygen-2024.5.7/src/dspygen/bpel_models/fault_handlers.py
--rw-r--r--   0        0        0     3787 2024-05-05 21:39:36.917161 dspygen-2024.5.7/src/dspygen/bpel_models/links.py
--rw-r--r--   0        0        0     1934 2024-05-05 21:39:36.917223 dspygen-2024.5.7/src/dspygen/bpel_models/partner_links.py
--rw-r--r--   0        0        0     2125 2024-05-05 21:39:36.917290 dspygen-2024.5.7/src/dspygen/bpel_models/process.py
--rw-r--r--   0        0        0     5256 2024-05-05 21:39:36.917366 dspygen-2024.5.7/src/dspygen/bpel_models/variables.py
--rw-r--r--   0        0        0       49 2024-05-05 21:39:36.917455 dspygen-2024.5.7/src/dspygen/bpmn_models/__init__.py
--rw-r--r--   0        0        0     1682 2024-05-05 21:39:36.917513 dspygen-2024.5.7/src/dspygen/bpmn_models/artifacts.py
--rw-r--r--   0        0        0     2236 2024-05-05 21:39:36.917572 dspygen-2024.5.7/src/dspygen/bpmn_models/connecting_objects.py
--rw-r--r--   0        0        0     2360 2024-05-05 21:39:36.917631 dspygen-2024.5.7/src/dspygen/bpmn_models/events.py
--rw-r--r--   0        0        0     1194 2024-05-05 21:39:36.917695 dspygen-2024.5.7/src/dspygen/bpmn_models/flow_objects.py
--rw-r--r--   0        0        0      807 2024-05-05 21:39:36.917755 dspygen-2024.5.7/src/dspygen/bpmn_models/gateways.py
--rw-r--r--   0        0        0     2604 2024-05-05 21:39:36.917811 dspygen-2024.5.7/src/dspygen/bpmn_models/other_entities.py
--rw-r--r--   0        0        0     1508 2024-05-05 21:39:36.917869 dspygen-2024.5.7/src/dspygen/bpmn_models/pools_and_lanes.py
--rw-r--r--   0        0        0      816 2024-05-05 21:39:36.917926 dspygen-2024.5.7/src/dspygen/bpmn_models/sub_processes.py
--rw-r--r--   0        0        0     7676 2024-05-05 21:39:36.918009 dspygen-2024.5.7/src/dspygen/cli.py
--rw-r--r--   0        0        0      469 2024-05-05 21:39:36.918078 dspygen-2024.5.7/src/dspygen/config.yaml
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.918138 dspygen-2024.5.7/src/dspygen/dsl/__init__.py
--rw-r--r--   0        0        0     1257 2024-05-05 21:39:36.918212 dspygen-2024.5.7/src/dspygen/dsl/dsl_dspy_assertion.py
--rw-r--r--   0        0        0     2732 2024-05-05 21:56:54.035475 dspygen-2024.5.7/src/dspygen/dsl/dsl_pipeline_executor.py
--rw-r--r--   0        0        0     5086 2024-05-05 21:39:36.918350 dspygen-2024.5.7/src/dspygen/dsl/dsl_predict_module.py
--rw-r--r--   0        0        0     6253 2024-05-05 21:39:36.918419 dspygen-2024.5.7/src/dspygen/dsl/dsl_pydantic_models.py
--rw-r--r--   0        0        0     3519 2024-05-05 21:39:36.918473 dspygen-2024.5.7/src/dspygen/dsl/dsl_step_module.py
--rw-r--r--   0        0        0      101 2024-05-05 21:39:36.918549 dspygen-2024.5.7/src/dspygen/dsl/examples/blog_pipeline.yaml
--rw-r--r--   0        0        0      745 2024-05-05 21:39:36.918601 dspygen-2024.5.7/src/dspygen/dsl/examples/example_pipeline.yaml
--rw-r--r--   0        0        0     1294 2024-05-05 21:39:36.918650 dspygen-2024.5.7/src/dspygen/dsl/examples/poem_pipeline.yaml
--rw-r--r--   0        0        0     1395 2024-05-05 21:39:36.918698 dspygen-2024.5.7/src/dspygen/dsl/examples/saltcorn_plugin_generator.yaml
--rw-r--r--   0        0        0      148 2024-05-05 21:39:36.918752 dspygen-2024.5.7/src/dspygen/dsl/examples/sql_to_nl.yaml
--rw-r--r--   0        0        0       55 2024-05-05 21:39:36.918799 dspygen-2024.5.7/src/dspygen/dsl/examples/text_signature_pipeline.yaml
--rw-r--r--   0        0        0       85 2024-05-05 21:39:36.918872 dspygen-2024.5.7/src/dspygen/dsl/modules/raw_to_structure_module.yaml
--rw-r--r--   0        0        0      361 2024-05-05 21:39:36.918946 dspygen-2024.5.7/src/dspygen/dsl/signature/sql_to_natural_signature.yaml
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.918997 dspygen-2024.5.7/src/dspygen/dsl/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.919028 dspygen-2024.5.7/src/dspygen/dsl/utils/dsl_assertions_utils.py
--rw-r--r--   0        0        0      566 2024-05-05 21:39:36.919099 dspygen-2024.5.7/src/dspygen/dsl/utils/dsl_language_model_utils.py
--rw-r--r--   0        0        0     2699 2024-05-05 21:39:36.919152 dspygen-2024.5.7/src/dspygen/dsl/utils/dsl_lm_module_utils.py
--rw-r--r--   0        0        0      852 2024-05-05 21:39:36.919205 dspygen-2024.5.7/src/dspygen/dsl/utils/dsl_retrieval_model_utils.py
--rw-r--r--   0        0        0     1108 2024-05-05 21:39:36.919270 dspygen-2024.5.7/src/dspygen/dsl/utils/dsl_rm_module_utils.py
--rw-r--r--   0        0        0     2517 2024-05-05 21:39:36.919338 dspygen-2024.5.7/src/dspygen/dsl/utils/dsl_signature_utils.py
--rw-r--r--   0        0        0     1344 2024-05-05 21:39:36.919405 dspygen-2024.5.7/src/dspygen/dspygen_app.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.919464 dspygen-2024.5.7/src/dspygen/experiments/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.919528 dspygen-2024.5.7/src/dspygen/experiments/bkgn/__init__.py
--rw-r--r--   0        0        0      667 2024-05-05 21:56:54.024131 dspygen-2024.5.7/src/dspygen/experiments/bkgn/chapter_draft.py
--rw-r--r--   0        0        0     2751 2024-05-05 21:56:54.036357 dspygen-2024.5.7/src/dspygen/experiments/bkgn/get_book_files.py
--rw-r--r--   0        0        0     2000 2024-05-05 21:56:54.022240 dspygen-2024.5.7/src/dspygen/experiments/bkgn/get_leaf.py
--rw-r--r--   0        0        0    10333 2024-05-05 21:56:54.020904 dspygen-2024.5.7/src/dspygen/experiments/bkgn/get_soc_files.py
--rw-r--r--   0        0        0     2011 2024-05-05 21:39:36.919837 dspygen-2024.5.7/src/dspygen/experiments/bkgn/quick_demo.py
--rw-r--r--   0        0        0     2586 2024-05-05 21:39:36.919920 dspygen-2024.5.7/src/dspygen/experiments/blog/Tetris_1.md
--rw-r--r--   0        0        0     3103 2024-05-05 21:39:36.919977 dspygen-2024.5.7/src/dspygen/experiments/blog/Tetris_LMStud_Llama3.py
--rw-r--r--   0        0        0     2531 2024-05-05 21:39:36.920031 dspygen-2024.5.7/src/dspygen/experiments/blog/Tetris_groq.py
--rw-r--r--   0        0        0     3302 2024-05-05 21:39:36.920084 dspygen-2024.5.7/src/dspygen/experiments/blog/Tetris_groq_llama3_80.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.920134 dspygen-2024.5.7/src/dspygen/experiments/bulk_code_generator/__init__.py
--rw-r--r--   0        0        0      788 2024-05-05 21:39:36.920202 dspygen-2024.5.7/src/dspygen/experiments/bulk_code_generator/main.py
--rw-r--r--   0        0        0      585 2024-05-05 21:56:54.037122 dspygen-2024.5.7/src/dspygen/experiments/business_patterns_for_devs.py
--rw-r--r--   0        0        0     1405 2024-05-05 21:39:36.920369 dspygen-2024.5.7/src/dspygen/experiments/done/CriticFeedbackGeneratorSignature_pipeline.yaml
--rw-r--r--   0        0        0      668 2024-05-05 21:39:36.920430 dspygen-2024.5.7/src/dspygen/experiments/done/WebsitePRD_pipeline.yaml
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.920451 dspygen-2024.5.7/src/dspygen/experiments/done/__init__.py
--rw-r--r--   0        0        0      331 2024-05-05 21:39:36.920511 dspygen-2024.5.7/src/dspygen/experiments/done/chatbots.py
--rw-r--r--   0        0        0      361 2024-05-05 21:39:36.920570 dspygen-2024.5.7/src/dspygen/experiments/done/code_generator_agent.py
--rw-r--r--   0        0        0     1790 2024-05-05 21:39:36.920626 dspygen-2024.5.7/src/dspygen/experiments/done/data_pipeline.yaml
--rw-r--r--   0        0        0      260 2024-05-05 21:39:36.920682 dspygen-2024.5.7/src/dspygen/experiments/done/file_path.py
--rw-r--r--   0        0        0      940 2024-05-05 21:39:36.920740 dspygen-2024.5.7/src/dspygen/experiments/done/first_step_with_user_input.py
--rw-r--r--   0        0        0     1720 2024-05-05 21:39:36.920794 dspygen-2024.5.7/src/dspygen/experiments/done/gen_dsl_instances.py
--rw-r--r--   0        0        0    14783 2024-05-05 21:39:36.920878 dspygen-2024.5.7/src/dspygen/experiments/done/gen_pydantic_class.py
--rw-r--r--   0        0        0     6076 2024-05-05 21:39:36.920951 dspygen-2024.5.7/src/dspygen/experiments/done/gherkin_parser.py
--rw-r--r--   0        0        0     3560 2024-05-05 21:39:36.921004 dspygen-2024.5.7/src/dspygen/experiments/done/lm_call.py
--rw-r--r--   0        0        0     1061 2024-05-05 21:39:36.921059 dspygen-2024.5.7/src/dspygen/experiments/done/openai_ror_cli.py
--rw-r--r--   0        0        0     1753 2024-05-05 21:39:36.921113 dspygen-2024.5.7/src/dspygen/experiments/done/python_to_elixir.py
--rw-r--r--   0        0        0       87 2024-05-05 21:39:36.921168 dspygen-2024.5.7/src/dspygen/experiments/done/raw_to_structure_module.yaml
--rw-r--r--   0        0        0      408 2024-05-05 21:39:36.921218 dspygen-2024.5.7/src/dspygen/experiments/done/saltcorn_plugin_generator.py
--rw-r--r--   0        0        0    15627 2024-05-05 21:39:36.921275 dspygen-2024.5.7/src/dspygen/experiments/done/saltcorn_plugin_generator_output.yaml
--rw-r--r--   0        0        0     1597 2024-05-05 21:39:36.921325 dspygen-2024.5.7/src/dspygen/experiments/done/socket_actor_system.py
--rw-r--r--   0        0        0      286 2024-05-05 21:39:36.921372 dspygen-2024.5.7/src/dspygen/experiments/done/sql_to_natural_signature.yaml
--rw-r--r--   0        0        0     1283 2024-05-05 21:39:36.921422 dspygen-2024.5.7/src/dspygen/experiments/done/test_openai_ror_cli.py
--rw-r--r--   0        0        0     1864 2024-05-05 21:39:36.921580 dspygen-2024.5.7/src/dspygen/experiments/done/two_steps_with_user_input.py
--rw-r--r--   0        0        0     1457 2024-05-05 21:39:36.921636 dspygen-2024.5.7/src/dspygen/experiments/done/understand_input_pipeline.yaml
--rw-r--r--   0        0        0     2554 2024-05-05 21:39:36.921704 dspygen-2024.5.7/src/dspygen/experiments/done/wizard.py
--rw-r--r--   0        0        0   884736 2024-05-05 21:39:36.922920 dspygen-2024.5.7/src/dspygen/experiments/function_calling/Chinook.db
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.922968 dspygen-2024.5.7/src/dspygen/experiments/function_calling/__init__.py
--rw-r--r--   0        0        0     1145 2024-05-05 21:39:36.923032 dspygen-2024.5.7/src/dspygen/experiments/function_calling/function_call.py
--rw-r--r--   0        0        0     1241 2024-05-05 21:39:36.923089 dspygen-2024.5.7/src/dspygen/experiments/function_calling/sql_calling_asserts.py
--rw-r--r--   0        0        0     1802 2024-05-05 21:39:36.923146 dspygen-2024.5.7/src/dspygen/experiments/function_calling/sql_optimization_function.py
--rw-r--r--   0        0        0      915 2024-05-05 21:39:36.923199 dspygen-2024.5.7/src/dspygen/experiments/function_calling/weather_function_calling_asserts.py
--rw-r--r--   0        0        0     1029 2024-05-05 21:39:36.923252 dspygen-2024.5.7/src/dspygen/experiments/function_calling/weather_functions.exs
--rw-r--r--   0        0        0        0 2024-05-06 16:37:21.090513 dspygen-2024.5.7/src/dspygen/experiments/mock_gen/__init__.py
--rw-r--r--   0        0        0     1679 2024-05-06 16:43:45.432058 dspygen-2024.5.7/src/dspygen/experiments/mock_gen/auto_pytest_mock_rover.py
--rw-r--r--   0        0        0     1397 2024-05-07 22:56:33.999148 dspygen-2024.5.7/src/dspygen/experiments/mock_gen/min_example.py
--rw-r--r--   0        0        0     5905 2024-05-07 22:57:40.654750 dspygen-2024.5.7/src/dspygen/experiments/mock_gen/mipro_example.py
--rw-r--r--   0        0        0    50545 2024-05-07 05:03:05.064147 dspygen-2024.5.7/src/dspygen/experiments/mock_gen/optimized_cot.json
--rw-r--r--   0        0        0    21085 2024-05-07 05:27:35.316795 dspygen-2024.5.7/src/dspygen/experiments/mock_gen/optimized_cot_sig.json
--rw-r--r--   0        0        0    50539 2024-05-07 16:42:15.979451 dspygen-2024.5.7/src/dspygen/experiments/mock_gen/optimized_cot_sig_1715100135.978442.json
--rw-r--r--   0        0        0     4572 2024-05-07 22:03:17.970194 dspygen-2024.5.7/src/dspygen/experiments/mock_gen/swe_bench.py
--rw-r--r--   0        0        0     2202 2024-05-07 16:39:55.859263 dspygen-2024.5.7/src/dspygen/experiments/mock_gen/swebench_example.py
--rw-r--r--   0        0        0     1635 2024-05-07 05:17:22.860325 dspygen-2024.5.7/src/dspygen/experiments/mock_gen/swebench_mipro_example.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.923304 dspygen-2024.5.7/src/dspygen/experiments/module_docstrings/__init__.py
--rw-r--r--   0        0        0      776 2024-05-05 21:39:36.923367 dspygen-2024.5.7/src/dspygen/experiments/module_docstrings/generate_docstring_exec.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.923414 dspygen-2024.5.7/src/dspygen/experiments/pomo_bud/__init__.py
--rw-r--r--   0        0        0      923 2024-05-05 21:39:36.923473 dspygen-2024.5.7/src/dspygen/experiments/pomo_bud/pomo_bud_dsl.yaml
--rw-r--r--   0        0        0     4975 2024-05-05 21:39:36.923541 dspygen-2024.5.7/src/dspygen/experiments/pomo_bud/pomo_bud_models.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.923596 dspygen-2024.5.7/src/dspygen/experiments/quiz/__init__.py
--rw-r--r--   0        0        0     7610 2024-05-05 21:39:36.923679 dspygen-2024.5.7/src/dspygen/experiments/quiz/quiz_input.py
--rw-r--r--   0        0        0     1037 2024-05-05 21:39:36.923733 dspygen-2024.5.7/src/dspygen/experiments/quiz/session_data.json
--rw-r--r--   0        0        0        0 2024-05-05 22:08:46.601395 dspygen-2024.5.7/src/dspygen/experiments/raga/__init__.py
--rw-r--r--   0        0        0     5955 2024-05-06 00:47:55.965499 dspygen-2024.5.7/src/dspygen/experiments/raga/chat_gpt_rag_retrevier.py
--rw-r--r--   0        0        0     1590 2024-05-05 22:18:40.646174 dspygen-2024.5.7/src/dspygen/experiments/raga/convo_loader.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.923780 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/__init__.py
--rw-r--r--   0        0        0     2380 2024-05-05 21:39:36.923845 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/api-for-document-management.tsx
--rw-r--r--   0        0        0      729 2024-05-05 21:39:36.923986 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/confirm-signature-placement.tsx
--rw-r--r--   0        0        0      634 2024-05-05 21:39:36.924039 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/custom-signing-instructions.tsx
--rw-r--r--   0        0        0     1555 2024-05-05 21:39:36.924169 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/data_gherkin_pipeline.yaml
--rw-r--r--   0        0        0      349 2024-05-05 21:39:36.924219 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/document-download.tsx
--rw-r--r--   0        0        0     3006 2024-05-05 21:39:36.924269 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/document-preview.tsx
--rw-r--r--   0        0        0     1100 2024-05-05 21:39:36.924324 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/document-upload.tsx
--rw-r--r--   0        0        0      518 2024-05-05 21:39:36.924459 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/drag-and-drop-document-upload.tsx
--rw-r--r--   0        0        0      601 2024-05-05 21:39:36.924515 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/email-confirmation-to-sender.tsx
--rw-r--r--   0        0        0     1222 2024-05-05 21:39:36.924571 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/email-link-to-signer.tsx
--rw-r--r--   0        0        0      165 2024-05-05 21:39:36.924617 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/feature_data_pipeline.yaml
--rw-r--r--   0        0        0     1034 2024-05-05 21:39:36.924678 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/generate-unique-signing-link.tsx
--rw-r--r--   0        0        0      938 2024-05-05 21:39:36.924814 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/generate_react_code_from_csv.py
--rw-r--r--   0        0        0     1425 2024-05-05 21:39:36.924955 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/gherkin_pipeline.yaml
--rw-r--r--   0        0        0     5785 2024-05-05 21:39:36.925028 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/hello-world.tsx
--rw-r--r--   0        0        0      591 2024-05-05 21:39:36.925088 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/link-expiration.tsx
--rw-r--r--   0        0        0     1965 2024-05-05 21:39:36.925260 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/mobile-responsive-design.tsx
--rw-r--r--   0        0        0      776 2024-05-05 21:39:36.925318 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/retrieve_and_generate_pipeline.py
--rw-r--r--   0        0        0      391 2024-05-05 21:39:36.925465 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/save-signature.tsx
--rw-r--r--   0        0        0      816 2024-05-05 21:39:36.925512 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/signature-capture.tsx
--rw-r--r--   0        0        0      786 2024-05-05 21:39:36.925562 dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/signature-validation.tsx
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.925608 dspygen-2024.5.7/src/dspygen/experiments/rfc5545/__init__.py
--rw-r--r--   0        0        0    11768 2024-05-05 21:39:36.925704 dspygen-2024.5.7/src/dspygen/experiments/rfc5545/calendar_cmd.py
--rw-r--r--   0        0        0     2819 2024-05-05 21:39:36.925768 dspygen-2024.5.7/src/dspygen/experiments/rfc5545/ical_crud.py
--rw-r--r--   0        0        0      270 2024-05-05 21:39:36.925824 dspygen-2024.5.7/src/dspygen/experiments/rfc5545/ical_data_ret.py
--rw-r--r--   0        0        0      442 2024-05-05 21:39:36.925879 dspygen-2024.5.7/src/dspygen/experiments/rfc5545/ical_db_session.py
--rw-r--r--   0        0        0    14826 2024-05-05 21:39:36.925935 dspygen-2024.5.7/src/dspygen/experiments/rfc5545/ical_models.py
--rw-r--r--   0        0        0      657 2024-05-05 21:39:36.925982 dspygen-2024.5.7/src/dspygen/experiments/rfc5545/ical_workbench.py
--rw-r--r--   0        0        0     3246 2024-05-05 21:39:36.926035 dspygen-2024.5.7/src/dspygen/experiments/rfc5545/journal_cmd.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926083 dspygen-2024.5.7/src/dspygen/experiments/self_coding/__init__.py
--rw-r--r--   0        0        0     3050 2024-05-05 21:39:36.926149 dspygen-2024.5.7/src/dspygen/experiments/self_coding/interview_processing.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926198 dspygen-2024.5.7/src/dspygen/experiments/soonify_groq/__init__.py
--rw-r--r--   0        0        0     2655 2024-05-05 21:39:36.926367 dspygen-2024.5.7/src/dspygen/experiments/soonify_groq/groq_pydantic.py
--rw-r--r--   0        0        0     4831 2024-05-05 21:39:36.926439 dspygen-2024.5.7/src/dspygen/experiments/soonify_groq/run_groq_soon.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926488 dspygen-2024.5.7/src/dspygen/experiments/spider/__init__.py
--rw-r--r--   0        0        0     2433 2024-05-05 21:39:36.926661 dspygen-2024.5.7/src/dspygen/experiments/spider/wiki_spider.py
--rw-r--r--   0        0        0     5987 2024-05-05 21:39:36.926725 dspygen-2024.5.7/src/dspygen/experiments/state_actor.txt
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926773 dspygen-2024.5.7/src/dspygen/experiments/tagee/.gitignore
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926803 dspygen-2024.5.7/src/dspygen/experiments/tagee/LICENSE
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926833 dspygen-2024.5.7/src/dspygen/experiments/tagee/README.md
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926924 dspygen-2024.5.7/src/dspygen/experiments/tagee/assets/images/.keep
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926979 dspygen-2024.5.7/src/dspygen/experiments/tagee/assets/sounds/.keep
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927044 dspygen-2024.5.7/src/dspygen/experiments/tagee/config/dev.json
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927074 dspygen-2024.5.7/src/dspygen/experiments/tagee/config/prod.json
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927103 dspygen-2024.5.7/src/dspygen/experiments/tagee/config/test.json
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927165 dspygen-2024.5.7/src/dspygen/experiments/tagee/docs/CurriculumAlignment.md
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927205 dspygen-2024.5.7/src/dspygen/experiments/tagee/docs/GettingStarted.md
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927247 dspygen-2024.5.7/src/dspygen/experiments/tagee/docs/TechnicalOverview.md
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927329 dspygen-2024.5.7/src/dspygen/experiments/tagee/lib/.keep
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927393 dspygen-2024.5.7/src/dspygen/experiments/tagee/scripts/deploy.sh
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927426 dspygen-2024.5.7/src/dspygen/experiments/tagee/scripts/maintenance.sh
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927456 dspygen-2024.5.7/src/dspygen/experiments/tagee/scripts/setup.sh
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927543 dspygen-2024.5.7/src/dspygen/experiments/tagee/src/core/education_module.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927572 dspygen-2024.5.7/src/dspygen/experiments/tagee/src/core/game_engine.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927601 dspygen-2024.5.7/src/dspygen/experiments/tagee/src/core/narrative_engine.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927688 dspygen-2024.5.7/src/dspygen/experiments/tagee/src/ui/modules/chatbot_view.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927719 dspygen-2024.5.7/src/dspygen/experiments/tagee/src/ui/modules/quiz_view.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927748 dspygen-2024.5.7/src/dspygen/experiments/tagee/src/ui/modules/story_view.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927804 dspygen-2024.5.7/src/dspygen/experiments/tagee/src/ui/utils/formatting_tools.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927837 dspygen-2024.5.7/src/dspygen/experiments/tagee/src/ui/utils/ui_helpers.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927943 dspygen-2024.5.7/src/dspygen/experiments/tagee/tests/integration/chatbot_integration_test.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927982 dspygen-2024.5.7/src/dspygen/experiments/tagee/tests/integration/quiz_integration_test.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928029 dspygen-2024.5.7/src/dspygen/experiments/tagee/tests/integration/story_integration_test.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928128 dspygen-2024.5.7/src/dspygen/experiments/tagee/tests/unit/education_module_test.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928168 dspygen-2024.5.7/src/dspygen/experiments/tagee/tests/unit/game_engine_test.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928213 dspygen-2024.5.7/src/dspygen/experiments/tagee/tests/unit/narrative_engine_test.py
--rw-r--r--   0        0        0     1367 2024-05-05 21:39:36.928339 dspygen-2024.5.7/src/dspygen/experiments/touch.sh
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928420 dspygen-2024.5.7/src/dspygen/experiments/txta/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928502 dspygen-2024.5.7/src/dspygen/experiments/wip/__init__.py
--rw-r--r--   0        0        0     2452 2024-05-05 21:56:54.030536 dspygen-2024.5.7/src/dspygen/experiments/wip/chatgpt_conversation_parser.py
--rw-r--r--   0        0        0      696 2024-05-05 21:39:36.928674 dspygen-2024.5.7/src/dspygen/experiments/wip/default_pipeline.yaml
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928733 dspygen-2024.5.7/src/dspygen/experiments/wip/models/__init__.py
--rw-r--r--   0        0        0    11258 2024-05-05 21:39:36.928863 dspygen-2024.5.7/src/dspygen/experiments/wip/models/dsl_project.py
--rw-r--r--   0        0        0     3117 2024-05-05 21:39:36.928929 dspygen-2024.5.7/src/dspygen/experiments/wip/one_shot_pipeline.py
--rw-r--r--   0        0        0     7582 2024-05-05 21:39:36.929009 dspygen-2024.5.7/src/dspygen/experiments/wip/self_evolving_business_logic.py
--rw-r--r--   0        0        0       23 2024-05-05 21:39:36.929096 dspygen-2024.5.7/src/dspygen/lm/__init__.py
--rw-r--r--   0        0        0     1645 2024-05-05 21:39:36.929153 dspygen-2024.5.7/src/dspygen/lm/groq_lm.py
--rw-r--r--   0        0        0     1860 2024-05-05 21:39:36.929219 dspygen-2024.5.7/src/dspygen/lm/ollama_lm.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.929272 dspygen-2024.5.7/src/dspygen/mixin/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.929329 dspygen-2024.5.7/src/dspygen/mixin/btrees/__init__.py
--rw-r--r--   0        0        0     4469 2024-05-05 21:39:36.929417 dspygen-2024.5.7/src/dspygen/mixin/btrees/bt_mixin_v2.py
--rw-r--r--   0        0        0     6856 2024-05-05 21:39:36.929495 dspygen-2024.5.7/src/dspygen/mixin/btrees/bt_ros_works.py
--rw-r--r--   0        0        0     2881 2024-05-05 21:39:36.929564 dspygen-2024.5.7/src/dspygen/mixin/btrees/bt_super.py
--rw-r--r--   0        0        0      952 2024-05-05 21:39:36.929622 dspygen-2024.5.7/src/dspygen/mixin/btrees/bt_traffic.py
--rw-r--r--   0        0        0     3717 2024-05-05 21:39:36.929689 dspygen-2024.5.7/src/dspygen/mixin/btrees/btree_mixin.py
--rw-r--r--   0        0        0     2075 2024-05-05 21:39:36.929872 dspygen-2024.5.7/src/dspygen/mixin/btrees/superhero_activities.dot
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.929951 dspygen-2024.5.7/src/dspygen/mixin/fsm/__init__.py
--rw-r--r--   0        0        0     1768 2024-05-05 21:39:36.930149 dspygen-2024.5.7/src/dspygen/mixin/fsm/employee_onboarding_fsm.py
--rw-r--r--   0        0        0     1556 2024-05-05 21:39:36.930333 dspygen-2024.5.7/src/dspygen/mixin/fsm/example.py
--rw-r--r--   0        0        0     2491 2024-05-05 21:39:36.930390 dspygen-2024.5.7/src/dspygen/mixin/fsm/fsm_gas.py
--rw-r--r--   0        0        0     3490 2024-05-06 00:31:25.538045 dspygen-2024.5.7/src/dspygen/mixin/fsm/fsm_mixin.py
--rw-r--r--   0        0        0    12039 2024-05-05 21:39:36.930562 dspygen-2024.5.7/src/dspygen/mixin/fsm/fsm_renderer.py
--rw-r--r--   0        0        0     8122 2024-05-05 21:39:36.930650 dspygen-2024.5.7/src/dspygen/mixin/fsm/order_processing_fsm.py
--rw-r--r--   0        0        0     1585 2024-05-05 21:39:36.930725 dspygen-2024.5.7/src/dspygen/mixin/fsm/traffic_light.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.930788 dspygen-2024.5.7/src/dspygen/mixin/hsm/__init__.py
--rw-r--r--   0        0        0     2662 2024-05-05 21:39:36.930966 dspygen-2024.5.7/src/dspygen/mixin/hsm/hsm_mixin.py
--rw-r--r--   0        0        0     1367 2024-05-05 21:39:36.931063 dspygen-2024.5.7/src/dspygen/models/BPMN.yaml
--rw-r--r--   0        0        0     1316 2024-05-05 21:39:36.931210 dspygen-2024.5.7/src/dspygen/models/CMMN.yaml
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.931235 dspygen-2024.5.7/src/dspygen/models/__init__.py
--rw-r--r--   0        0        0     2936 2024-05-05 21:39:36.931413 dspygen-2024.5.7/src/dspygen/models/bpm_plus_domain_models.py
--rw-r--r--   0        0        0     1569 2024-05-05 21:39:36.931476 dspygen-2024.5.7/src/dspygen/models/cmmn_shipping.yaml
--rw-r--r--   0        0        0      940 2024-05-05 21:39:36.931532 dspygen-2024.5.7/src/dspygen/models/dmn_shipping.yaml
--rw-r--r--   0        0        0       70 2024-05-05 21:39:36.931593 dspygen-2024.5.7/src/dspygen/module_docstring_writer.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.931654 dspygen-2024.5.7/src/dspygen/modules/__init__.py
--rw-r--r--   0        0        0     2149 2024-05-05 21:39:36.931743 dspygen-2024.5.7/src/dspygen/modules/arch_module.py
--rw-r--r--   0        0        0      782 2024-05-05 21:39:36.931810 dspygen-2024.5.7/src/dspygen/modules/bill_of_objects_module.py
--rw-r--r--   0        0        0     1359 2024-05-05 21:39:36.931867 dspygen-2024.5.7/src/dspygen/modules/binary_output_module.py
--rw-r--r--   0        0        0     2461 2024-05-05 21:39:36.931935 dspygen-2024.5.7/src/dspygen/modules/blog_module.py
--rw-r--r--   0        0        0     2103 2024-05-05 21:39:36.931995 dspygen-2024.5.7/src/dspygen/modules/book_appointment_module.py
--rw-r--r--   0        0        0     2186 2024-05-05 21:39:36.932054 dspygen-2024.5.7/src/dspygen/modules/bpmn2_bpel_module.py
--rw-r--r--   0        0        0     1116 2024-05-05 21:39:36.932115 dspygen-2024.5.7/src/dspygen/modules/business_dev_consultant.py
--rw-r--r--   0        0        0     2429 2024-05-05 21:39:36.932178 dspygen-2024.5.7/src/dspygen/modules/business_requirements.py
--rw-r--r--   0        0        0     1151 2024-05-05 21:39:36.932230 dspygen-2024.5.7/src/dspygen/modules/chat_bot_cli.py
--rw-r--r--   0        0        0     1920 2024-05-05 21:39:36.932278 dspygen-2024.5.7/src/dspygen/modules/chat_bot_module.py
--rw-r--r--   0        0        0     1058 2024-05-05 21:39:36.932332 dspygen-2024.5.7/src/dspygen/modules/checker_module.py
--rw-r--r--   0        0        0     4382 2024-05-05 21:39:36.932400 dspygen-2024.5.7/src/dspygen/modules/choose_function_module.py
--rw-r--r--   0        0        0      931 2024-05-05 21:39:36.932454 dspygen-2024.5.7/src/dspygen/modules/cli_bot_module.py
--rw-r--r--   0        0        0     1233 2024-05-05 21:39:36.932513 dspygen-2024.5.7/src/dspygen/modules/cobol_to_python_module.py
--rw-r--r--   0        0        0     2922 2024-05-06 00:19:09.661287 dspygen-2024.5.7/src/dspygen/modules/condition_sufficient_info_module.py
--rw-r--r--   0        0        0     4265 2024-05-05 21:39:36.932580 dspygen-2024.5.7/src/dspygen/modules/dflss_module.py
--rw-r--r--   0        0        0      751 2024-05-05 21:39:36.932646 dspygen-2024.5.7/src/dspygen/modules/dflss_output.txt
--rw-r--r--   0        0        0      859 2024-05-05 21:39:36.932709 dspygen-2024.5.7/src/dspygen/modules/dspygen_dsl_pipeline.py
--rw-r--r--   0        0        0     3530 2024-05-05 21:39:36.932771 dspygen-2024.5.7/src/dspygen/modules/dspygen_module.py
--rw-r--r--   0        0        0     5765 2024-05-05 21:39:36.932854 dspygen-2024.5.7/src/dspygen/modules/elite_module.py
--rw-r--r--   0        0        0     2039 2024-05-05 21:39:36.932915 dspygen-2024.5.7/src/dspygen/modules/exam_point_weight_module.py
--rw-r--r--   0        0        0     2160 2024-05-05 21:39:36.932964 dspygen-2024.5.7/src/dspygen/modules/faang_module.py
--rw-r--r--   0        0        0     2247 2024-05-05 21:39:36.933016 dspygen-2024.5.7/src/dspygen/modules/faang_sys_arch_nuxt_module.py
--rw-r--r--   0        0        0     1274 2024-05-05 21:39:36.933166 dspygen-2024.5.7/src/dspygen/modules/file_name_module.py
--rw-r--r--   0        0        0     2385 2024-05-05 21:39:36.933224 dspygen-2024.5.7/src/dspygen/modules/function_invoke_module.py
--rw-r--r--   0        0        0     4239 2024-05-05 21:39:36.933287 dspygen-2024.5.7/src/dspygen/modules/gen_cli_module.py
--rw-r--r--   0        0        0     2213 2024-05-05 21:39:36.933349 dspygen-2024.5.7/src/dspygen/modules/gen_dspy_module.py
--rw-r--r--   0        0        0     5363 2024-05-05 21:39:36.933416 dspygen-2024.5.7/src/dspygen/modules/gen_keyword_arguments_module.py
--rw-r--r--   0        0        0     1093 2024-05-05 21:39:36.933466 dspygen-2024.5.7/src/dspygen/modules/gen_message_module.py
--rw-r--r--   0        0        0     1901 2024-05-05 21:39:36.933513 dspygen-2024.5.7/src/dspygen/modules/gen_module.py
--rw-r--r--   0        0        0    14776 2024-05-05 21:39:36.933566 dspygen-2024.5.7/src/dspygen/modules/gen_pydantic_class.py
--rw-r--r--   0        0        0    10747 2024-05-05 21:39:36.933653 dspygen-2024.5.7/src/dspygen/modules/gen_pydantic_instance.py
--rw-r--r--   0        0        0     5555 2024-05-05 21:39:36.933725 dspygen-2024.5.7/src/dspygen/modules/gen_pydantic_instance_module.py
--rw-r--r--   0        0        0     3398 2024-05-05 21:50:16.283283 dspygen-2024.5.7/src/dspygen/modules/gen_python_primitive.py
--rw-r--r--   0        0        0     1266 2024-05-05 21:39:36.933824 dspygen-2024.5.7/src/dspygen/modules/gen_signature_module.py
--rw-r--r--   0        0        0     4595 2024-05-05 21:39:36.933885 dspygen-2024.5.7/src/dspygen/modules/get_selector_module.py
--rw-r--r--   0        0        0     1099 2024-05-05 21:39:36.934044 dspygen-2024.5.7/src/dspygen/modules/gusty_module.py
--rw-r--r--   0        0        0      137 2024-05-05 21:39:36.934096 dspygen-2024.5.7/src/dspygen/modules/hello_world_module.yaml
--rw-r--r--   0        0        0     1421 2024-05-05 21:39:36.934152 dspygen-2024.5.7/src/dspygen/modules/html_module.py
--rw-r--r--   0        0        0     1899 2024-05-05 21:39:36.934202 dspygen-2024.5.7/src/dspygen/modules/insight_tweet_module.py
--rw-r--r--   0        0        0     2869 2024-05-05 21:39:36.934253 dspygen-2024.5.7/src/dspygen/modules/js_to_fast_api_module.py
--rw-r--r--   0        0        0     4946 2024-05-05 21:39:36.934319 dspygen-2024.5.7/src/dspygen/modules/json_module.py
--rw-r--r--   0        0        0     1788 2024-05-05 21:39:36.934365 dspygen-2024.5.7/src/dspygen/modules/jsx_module.py
--rw-r--r--   0        0        0     1997 2024-05-05 21:39:36.934528 dspygen-2024.5.7/src/dspygen/modules/long_form_qa_module.py
--rw-r--r--   0        0        0     7742 2024-05-05 21:39:36.934598 dspygen-2024.5.7/src/dspygen/modules/md_book_summarizer_module.py
--rw-r--r--   0        0        0     2732 2024-05-05 21:39:36.934647 dspygen-2024.5.7/src/dspygen/modules/mermaid_js_module.py
--rw-r--r--   0        0        0     1337 2024-05-05 21:39:36.934693 dspygen-2024.5.7/src/dspygen/modules/message_module.py
--rw-r--r--   0        0        0     1239 2024-05-05 21:39:36.934739 dspygen-2024.5.7/src/dspygen/modules/module_docstring_module.py
--rw-r--r--   0        0        0      335 2024-05-05 21:39:36.934787 dspygen-2024.5.7/src/dspygen/modules/pipeline.yaml
--rw-r--r--   0        0        0     1787 2024-05-05 21:39:36.934844 dspygen-2024.5.7/src/dspygen/modules/product_bot_module.py
--rw-r--r--   0        0        0      819 2024-05-05 21:39:36.934900 dspygen-2024.5.7/src/dspygen/modules/prompt_function_call_module.py
--rw-r--r--   0        0        0     4048 2024-05-06 22:58:03.790452 dspygen-2024.5.7/src/dspygen/modules/pytest_module.py
--rw-r--r--   0        0        0     1781 2024-05-05 21:39:36.934946 dspygen-2024.5.7/src/dspygen/modules/python_expert_module.py
--rw-r--r--   0        0        0     1878 2024-05-06 03:10:48.896564 dspygen-2024.5.7/src/dspygen/modules/python_source_code_module.py
--rw-r--r--   0        0        0     1781 2024-05-05 21:39:36.935034 dspygen-2024.5.7/src/dspygen/modules/pyts_module.py
--rw-r--r--   0        0        0     2641 2024-05-06 00:40:47.401404 dspygen-2024.5.7/src/dspygen/modules/query_generator_module.py
--rw-r--r--   0        0        0     1261 2024-05-05 21:39:36.935080 dspygen-2024.5.7/src/dspygen/modules/rails_code_module.py
--rw-r--r--   0        0        0      849 2024-05-05 21:39:36.935127 dspygen-2024.5.7/src/dspygen/modules/react_jsx_module.py
--rw-r--r--   0        0        0     2717 2024-05-06 00:19:09.661560 dspygen-2024.5.7/src/dspygen/modules/refine_results_module.py
--rw-r--r--   0        0        0     1001 2024-05-05 21:39:36.935176 dspygen-2024.5.7/src/dspygen/modules/request_contract_module.py
--rw-r--r--   0        0        0     5828 2024-05-05 21:39:36.935242 dspygen-2024.5.7/src/dspygen/modules/signature_factory.py
--rw-r--r--   0        0        0     5969 2024-05-05 21:39:36.935312 dspygen-2024.5.7/src/dspygen/modules/signature_renderer.py
--rw-r--r--   0        0        0     1744 2024-05-05 21:39:36.935450 dspygen-2024.5.7/src/dspygen/modules/source_code_pep8_docs_module.py
--rw-r--r--   0        0        0     2658 2024-05-06 00:19:09.661691 dspygen-2024.5.7/src/dspygen/modules/source_selector_module.py
--rw-r--r--   0        0        0      969 2024-05-05 21:39:36.935497 dspygen-2024.5.7/src/dspygen/modules/sql_query_module.py
--rw-r--r--   0        0        0     2073 2024-05-05 21:39:36.935541 dspygen-2024.5.7/src/dspygen/modules/streamlit_bot_module.py
--rw-r--r--   0        0        0     2165 2024-05-05 21:39:36.935601 dspygen-2024.5.7/src/dspygen/modules/subject_destination_audience_newsletter_article_module.py
--rw-r--r--   0        0        0     1798 2024-05-05 21:39:36.935657 dspygen-2024.5.7/src/dspygen/modules/success_planner_module.py
--rw-r--r--   0        0        0     1052 2024-05-05 21:39:36.935707 dspygen-2024.5.7/src/dspygen/modules/tax_return_agent.py
--rw-r--r--   0        0        0      914 2024-05-05 21:39:36.935751 dspygen-2024.5.7/src/dspygen/modules/test.py
--rw-r--r--   0        0        0     1486 2024-05-05 21:39:36.935792 dspygen-2024.5.7/src/dspygen/modules/test_chat_bot_cli.py
--rw-r--r--   0        0        0      799 2024-05-05 21:39:36.935841 dspygen-2024.5.7/src/dspygen/modules/text_summary_module_module.py
--rw-r--r--   0        0        0     1767 2024-05-05 21:39:36.935889 dspygen-2024.5.7/src/dspygen/modules/to_elixir_module.py
--rw-r--r--   0        0        0     2330 2024-05-05 21:39:36.935933 dspygen-2024.5.7/src/dspygen/modules/usp_connect_ship_webhook.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.935980 dspygen-2024.5.7/src/dspygen/pages/__init__.py
--rw-r--r--   0        0        0      481 2024-05-05 21:39:36.936036 dspygen-2024.5.7/src/dspygen/pages/hello.py
--rw-r--r--   0        0        0     1407 2024-05-05 21:39:36.936082 dspygen-2024.5.7/src/dspygen/pages/mqtt_page.py
--rw-r--r--   0        0        0      481 2024-05-05 21:39:36.936129 dspygen-2024.5.7/src/dspygen/pages/remodeling.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.936177 dspygen-2024.5.7/src/dspygen/prototypes/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.936238 dspygen-2024.5.7/src/dspygen/prototypes/state_chat/__init__.py
--rw-r--r--   0        0        0     5029 2024-05-05 21:39:36.936310 dspygen-2024.5.7/src/dspygen/prototypes/state_chat/hello_world_convo_agent.py
--rw-r--r--   0        0        0     9821 2024-05-05 21:39:36.936392 dspygen-2024.5.7/src/dspygen/prototypes/state_chat/socrates_convo.py
--rw-r--r--   0        0        0       23 2024-05-05 21:39:36.936589 dspygen-2024.5.7/src/dspygen/rdddy/__init__.py
--rw-r--r--   0        0        0    17082 2024-05-05 21:39:36.936661 dspygen-2024.5.7/src/dspygen/rdddy/actor_system.py
--rw-r--r--   0        0        0    11050 2024-05-05 21:39:36.936745 dspygen-2024.5.7/src/dspygen/rdddy/base_actor.py
--rw-r--r--   0        0        0     1155 2024-05-05 21:39:36.936869 dspygen-2024.5.7/src/dspygen/rdddy/base_aggregate.py
--rw-r--r--   0        0        0      125 2024-05-05 21:39:36.936913 dspygen-2024.5.7/src/dspygen/rdddy/base_command.py
--rw-r--r--   0        0        0      113 2024-05-05 21:39:36.936957 dspygen-2024.5.7/src/dspygen/rdddy/base_event.py
--rw-r--r--   0        0        0     3539 2024-05-05 21:39:36.937019 dspygen-2024.5.7/src/dspygen/rdddy/base_message.py
--rw-r--r--   0        0        0      648 2024-05-05 21:39:36.937070 dspygen-2024.5.7/src/dspygen/rdddy/base_policy.py
--rw-r--r--   0        0        0      113 2024-05-05 21:39:36.937112 dspygen-2024.5.7/src/dspygen/rdddy/base_query.py
--rw-r--r--   0        0        0      165 2024-05-05 21:39:36.937159 dspygen-2024.5.7/src/dspygen/rdddy/base_read_model.py
--rw-r--r--   0        0        0     3123 2024-05-05 21:39:36.937210 dspygen-2024.5.7/src/dspygen/rdddy/base_repository.py
--rw-r--r--   0        0        0      522 2024-05-05 21:39:36.937338 dspygen-2024.5.7/src/dspygen/rdddy/base_saga.py
--rw-r--r--   0        0        0      446 2024-05-05 21:39:36.937387 dspygen-2024.5.7/src/dspygen/rdddy/base_task.py
--rw-r--r--   0        0        0      416 2024-05-05 21:39:36.937435 dspygen-2024.5.7/src/dspygen/rdddy/base_value_object.py
--rw-r--r--   0        0        0      405 2024-05-05 21:39:36.937483 dspygen-2024.5.7/src/dspygen/rdddy/base_view.py
--rw-r--r--   0        0        0       23 2024-05-05 21:39:36.937623 dspygen-2024.5.7/src/dspygen/rdddy/browser/__init__.py
--rw-r--r--   0        0        0     2435 2024-05-05 21:39:36.937681 dspygen-2024.5.7/src/dspygen/rdddy/browser/browser_domain.py
--rw-r--r--   0        0        0     4129 2024-05-05 21:39:36.937750 dspygen-2024.5.7/src/dspygen/rdddy/browser/browser_process_supervisor.py
--rw-r--r--   0        0        0     5541 2024-05-05 21:39:36.937819 dspygen-2024.5.7/src/dspygen/rdddy/browser/browser_worker.py
--rw-r--r--   0        0        0      118 2024-05-05 21:39:36.937952 dspygen-2024.5.7/src/dspygen/rdddy/browser/run_chatgpt.py
--rw-r--r--   0        0        0      425 2024-05-05 21:39:36.938003 dspygen-2024.5.7/src/dspygen/rdddy/domain_exception.py
--rw-r--r--   0        0        0     5148 2024-05-05 21:39:36.938069 dspygen-2024.5.7/src/dspygen/rdddy/event_storm_domain_specification_model.py
--rw-r--r--   0        0        0     1079 2024-05-05 21:39:36.938117 dspygen-2024.5.7/src/dspygen/rdddy/event_storm_model.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.938173 dspygen-2024.5.7/src/dspygen/rm/__init__.py
--rw-r--r--   0        0        0     8406 2024-05-06 16:16:54.869789 dspygen-2024.5.7/src/dspygen/rm/chatgpt_chromadb_retriever.py
--rw-r--r--   0        0        0     1106 2024-05-05 21:39:36.938356 dspygen-2024.5.7/src/dspygen/rm/chatgpt_string_retriever.py
--rw-r--r--   0        0        0     3985 2024-05-07 06:10:18.872098 dspygen-2024.5.7/src/dspygen/rm/chroma_retriever.py
--rw-r--r--   0        0        0     3529 2024-05-05 21:56:54.026813 dspygen-2024.5.7/src/dspygen/rm/code_retriever.py
--rw-r--r--   0        0        0     4577 2024-05-05 21:39:36.938481 dspygen-2024.5.7/src/dspygen/rm/data_retriever.py
--rw-r--r--   0        0        0     2692 2024-05-05 21:56:54.033125 dspygen-2024.5.7/src/dspygen/rm/doc_retriever.py
--rw-r--r--   0        0        0      316 2024-05-05 21:39:36.938580 dspygen-2024.5.7/src/dspygen/rm/natural_language_data_retriever.py
--rw-r--r--   0        0        0     3964 2024-05-05 21:39:36.938630 dspygen-2024.5.7/src/dspygen/rm/python_code_retriever.py
--rw-r--r--   0        0        0      424 2024-05-05 21:39:36.938678 dspygen-2024.5.7/src/dspygen/rm/web_retriever.py
--rw-r--r--   0        0        0       38 2024-05-05 21:39:36.938752 dspygen-2024.5.7/src/dspygen/signatures/__init__.py
--rw-r--r--   0        0        0      400 2024-05-05 21:39:36.938803 dspygen-2024.5.7/src/dspygen/signatures/blog_article.py
--rw-r--r--   0        0        0      425 2024-05-05 21:39:36.938849 dspygen-2024.5.7/src/dspygen/signatures/generate_answer.py
--rw-r--r--   0        0        0      635 2024-05-05 21:39:36.938909 dspygen-2024.5.7/src/dspygen/signatures/signature.yaml
--rw-r--r--   0        0        0     1972 2024-05-05 21:39:36.938960 dspygen-2024.5.7/src/dspygen/signatures/signature_dsl.py
--rw-r--r--   0        0        0       23 2024-05-05 21:39:36.939049 dspygen-2024.5.7/src/dspygen/subcommands/__init__.py
--rw-r--r--   0        0        0     2849 2024-05-05 21:39:36.939112 dspygen-2024.5.7/src/dspygen/subcommands/actor_cmd.py
--rw-r--r--   0        0        0     1890 2024-05-05 21:39:36.939170 dspygen-2024.5.7/src/dspygen/subcommands/assert_cmd.py
--rw-r--r--   0        0        0      993 2024-05-05 21:39:36.939225 dspygen-2024.5.7/src/dspygen/subcommands/browser_cmd.py
--rw-r--r--   0        0        0     2795 2024-05-05 21:39:36.939277 dspygen-2024.5.7/src/dspygen/subcommands/cmd_cmd.py
--rw-r--r--   0        0        0     1020 2024-05-05 21:39:36.939334 dspygen-2024.5.7/src/dspygen/subcommands/code_cmd.py
--rw-r--r--   0        0        0     2192 2024-05-05 21:39:36.939390 dspygen-2024.5.7/src/dspygen/subcommands/help.txt
--rw-r--r--   0        0        0     3654 2024-05-05 21:39:36.939445 dspygen-2024.5.7/src/dspygen/subcommands/help_cmd.py
--rw-r--r--   0        0        0      984 2024-05-05 21:39:36.939500 dspygen-2024.5.7/src/dspygen/subcommands/lm_cmd.py
--rw-r--r--   0        0        0     2167 2024-05-05 21:39:36.939559 dspygen-2024.5.7/src/dspygen/subcommands/module_cmd.py
--rw-r--r--   0        0        0     6944 2024-05-05 21:39:36.939625 dspygen-2024.5.7/src/dspygen/subcommands/pln_cmd.py
--rw-r--r--   0        0        0      258 2024-05-05 21:39:36.939677 dspygen-2024.5.7/src/dspygen/subcommands/poet_cmd.py
--rw-r--r--   0        0        0      810 2024-05-05 21:39:36.939725 dspygen-2024.5.7/src/dspygen/subcommands/rm_cmd.py
--rw-r--r--   0        0        0      763 2024-05-05 21:39:36.939777 dspygen-2024.5.7/src/dspygen/subcommands/sig_cmd.py
--rw-r--r--   0        0        0     2660 2024-05-05 21:39:36.939834 dspygen-2024.5.7/src/dspygen/subcommands/temp_assert.py
--rw-r--r--   0        0        0     7118 2024-05-05 21:56:54.028290 dspygen-2024.5.7/src/dspygen/subcommands/wkf_cmd.py
--rw-r--r--   0        0        0      786 2024-05-05 21:39:36.939937 dspygen-2024.5.7/src/dspygen/subcommands/wrt_cmd.py
--rw-r--r--   0        0        0      600 2024-05-05 21:39:36.940013 dspygen-2024.5.7/src/dspygen/templates/actor_template.j2
--rw-r--r--   0        0        0      187 2024-05-05 21:39:36.940062 dspygen-2024.5.7/src/dspygen/templates/dspy_module_cli_call.j2
--rw-r--r--   0        0        0      146 2024-05-05 21:39:36.940112 dspygen-2024.5.7/src/dspygen/templates/dspy_module_def_call.j2
--rw-r--r--   0        0        0      172 2024-05-05 21:39:36.940155 dspygen-2024.5.7/src/dspygen/templates/dspy_module_main.j2
--rw-r--r--   0        0        0      240 2024-05-05 21:39:36.940203 dspygen-2024.5.7/src/dspygen/templates/dspy_module_route.j2
--rw-r--r--   0        0        0      335 2024-05-05 21:39:36.940255 dspygen-2024.5.7/src/dspygen/templates/dspy_module_streamlit_input.j2
--rw-r--r--   0        0        0      378 2024-05-05 21:39:36.940304 dspygen-2024.5.7/src/dspygen/templates/signature_class_def.j2
--rw-r--r--   0        0        0     1622 2024-05-05 21:39:36.940350 dspygen-2024.5.7/src/dspygen/touch_models.sh
--rw-r--r--   0        0        0      577 2024-05-05 21:39:36.940421 dspygen-2024.5.7/src/dspygen/typetemp/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.940470 dspygen-2024.5.7/src/dspygen/typetemp/environment/__init__.py
--rw-r--r--   0        0        0     1043 2024-05-05 21:39:36.940532 dspygen-2024.5.7/src/dspygen/typetemp/environment/typed_environment.py
--rw-r--r--   0        0        0      979 2024-05-05 21:39:36.940581 dspygen-2024.5.7/src/dspygen/typetemp/environment/typed_native_environment.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.940636 dspygen-2024.5.7/src/dspygen/typetemp/extension/__init__.py
--rw-r--r--   0        0        0    24023 2024-05-05 21:39:36.940726 dspygen-2024.5.7/src/dspygen/typetemp/extension/faker_extension.py
--rw-r--r--   0        0        0     1098 2024-05-05 21:39:36.940777 dspygen-2024.5.7/src/dspygen/typetemp/extension/inflection_extension.py
--rw-r--r--   0        0        0     1812 2024-05-05 21:39:36.940830 dspygen-2024.5.7/src/dspygen/typetemp/functional.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.940880 dspygen-2024.5.7/src/dspygen/typetemp/template/__init__.py
--rw-r--r--   0        0        0     2454 2024-05-05 21:39:36.940938 dspygen-2024.5.7/src/dspygen/typetemp/template/async_render_mixin.py
--rw-r--r--   0        0        0    11207 2024-05-05 21:39:36.941024 dspygen-2024.5.7/src/dspygen/typetemp/template/dsl_project.py
--rw-r--r--   0        0        0      241 2024-05-05 21:39:36.941069 dspygen-2024.5.7/src/dspygen/typetemp/template/python
--rw-r--r--   0        0        0     1001 2024-05-05 21:39:36.941118 dspygen-2024.5.7/src/dspygen/typetemp/template/render_funcs.py
--rw-r--r--   0        0        0     2160 2024-05-05 21:39:36.941166 dspygen-2024.5.7/src/dspygen/typetemp/template/render_mixin.py
--rw-r--r--   0        0        0     3393 2024-05-05 21:39:36.941217 dspygen-2024.5.7/src/dspygen/typetemp/template/smart_template.py
--rw-r--r--   0        0        0     5497 2024-05-05 21:39:36.941279 dspygen-2024.5.7/src/dspygen/typetemp/template/typed_injector.py
--rw-r--r--   0        0        0     2348 2024-05-05 21:39:36.941329 dspygen-2024.5.7/src/dspygen/typetemp/template/typed_prompt.py
--rw-r--r--   0        0        0     2590 2024-05-05 21:39:36.941380 dspygen-2024.5.7/src/dspygen/typetemp/template/typed_python_source.py
--rw-r--r--   0        0        0     1042 2024-05-05 21:39:36.941532 dspygen-2024.5.7/src/dspygen/typetemp/template/typed_template.py
--rw-r--r--   0        0        0       23 2024-05-05 21:39:36.941613 dspygen-2024.5.7/src/dspygen/utils/MyData.yaml
--rw-r--r--   0        0        0       23 2024-05-05 21:39:36.941654 dspygen-2024.5.7/src/dspygen/utils/__init__.py
--rw-r--r--   0        0        0     1698 2024-05-05 21:39:36.941700 dspygen-2024.5.7/src/dspygen/utils/cli_tools.py
--rw-r--r--   0        0        0    12563 2024-05-05 21:56:54.031492 dspygen-2024.5.7/src/dspygen/utils/complete.py
--rw-r--r--   0        0        0     2961 2024-05-05 21:39:36.941807 dspygen-2024.5.7/src/dspygen/utils/compression_tools.py
--rw-r--r--   0        0        0       65 2024-05-05 21:39:36.941852 dspygen-2024.5.7/src/dspygen/utils/contact.yaml
--rw-r--r--   0        0        0    25532 2024-05-05 21:39:36.941940 dspygen-2024.5.7/src/dspygen/utils/create_prompts.py
--rw-r--r--   0        0        0     2197 2024-05-05 21:39:36.941997 dspygen-2024.5.7/src/dspygen/utils/crud_tools.py
--rw-r--r--   0        0        0     1620 2024-05-05 21:39:36.942051 dspygen-2024.5.7/src/dspygen/utils/date_tools.py
--rw-r--r--   0        0        0      678 2024-05-06 16:49:32.984810 dspygen-2024.5.7/src/dspygen/utils/dspy_tools.py
--rw-r--r--   0        0        0      118 2024-05-05 21:39:36.943767 dspygen-2024.5.7/src/dspygen/utils/example.py
--rw-r--r--   0        0        0     6772 2024-05-05 21:39:36.943890 dspygen-2024.5.7/src/dspygen/utils/file_tools.py
--rw-r--r--   0        0        0     1061 2024-05-05 21:39:36.943956 dspygen-2024.5.7/src/dspygen/utils/json_tools.py
--rw-r--r--   0        0        0     4684 2024-05-05 21:39:36.944032 dspygen-2024.5.7/src/dspygen/utils/models.py
--rw-r--r--   0        0        0     1641 2024-05-05 21:39:36.944085 dspygen-2024.5.7/src/dspygen/utils/module_tools.py
--rw-r--r--   0        0        0     1772 2024-05-05 21:39:36.944137 dspygen-2024.5.7/src/dspygen/utils/pydantic_tools.py
--rw-r--r--   0        0        0     3743 2024-05-07 22:44:34.036186 dspygen-2024.5.7/src/dspygen/utils/scraping_tools.py
--rw-r--r--   0        0        0     8227 2024-05-05 21:39:36.944228 dspygen-2024.5.7/src/dspygen/utils/yaml_tools.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.944282 dspygen-2024.5.7/src/dspygen/workflow/__init__.py
--rw-r--r--   0        0        0     1776 2024-05-05 21:39:36.944470 dspygen-2024.5.7/src/dspygen/workflow/control_flow_workflow.yaml
--rw-r--r--   0        0        0     1885 2024-05-05 21:39:36.944524 dspygen-2024.5.7/src/dspygen/workflow/control_flow_workflow_output_new.yaml
--rw-r--r--   0        0        0      923 2024-05-05 21:56:54.029489 dspygen-2024.5.7/src/dspygen/workflow/data_analysis_workflow.yaml
--rw-r--r--   0        0        0      912 2024-05-05 21:39:36.944640 dspygen-2024.5.7/src/dspygen/workflow/data_preparation_workflow.yaml
--rw-r--r--   0        0        0     2773 2024-05-05 21:56:54.024971 dspygen-2024.5.7/src/dspygen/workflow/workflow_engine.py
--rw-r--r--   0        0        0     3765 2024-05-05 21:39:36.944751 dspygen-2024.5.7/src/dspygen/workflow/workflow_executor.py
--rw-r--r--   0        0        0    10229 2024-05-05 21:39:36.944839 dspygen-2024.5.7/src/dspygen/workflow/workflow_models.py
--rw-r--r--   0        0        0     1697 2024-05-05 21:39:36.944898 dspygen-2024.5.7/src/dspygen/workflow/workflow_router.py
--rw-r--r--   0        0        0        0 2024-05-05 21:39:36.944953 dspygen-2024.5.7/src/dspygen/writer/__init__.py
--rw-r--r--   0        0        0      418 2024-05-05 21:39:36.945009 dspygen-2024.5.7/src/dspygen/writer/code_writer.py
--rw-r--r--   0        0        0     3755 2024-05-05 21:56:54.033929 dspygen-2024.5.7/src/dspygen/writer/data_writer.py
--rw-r--r--   0        0        0    13936 1970-01-01 00:00:00.000000 dspygen-2024.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-05 21:39:36.898989 dspygen-2024.5.8/LICENSE
+-rw-r--r--   0        0        0    11342 2024-05-05 21:39:36.899104 dspygen-2024.5.8/README.md
+-rw-r--r--   0        0        0     6806 2024-05-08 20:45:28.830116 dspygen-2024.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3048 2024-05-05 21:39:36.913212 dspygen-2024.5.8/src/dspygen/4www.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.913237 dspygen-2024.5.8/src/dspygen/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.913298 dspygen-2024.5.8/src/dspygen/agents/__init__.py
+-rw-r--r--   0        0        0     1963 2024-05-08 18:49:18.790552 dspygen-2024.5.8/src/dspygen/agents/analytics_agent.py
+-rw-r--r--   0        0        0     4085 2024-05-05 21:39:36.913365 dspygen-2024.5.8/src/dspygen/agents/coder_agent.py
+-rw-r--r--   0        0        0     3155 2024-05-05 21:39:36.913432 dspygen-2024.5.8/src/dspygen/agents/coder_agent_v2.py
+-rw-r--r--   0        0        0     3854 2024-05-05 21:39:36.913478 dspygen-2024.5.8/src/dspygen/agents/coder_agent_v3.py
+-rw-r--r--   0        0        0     4326 2024-05-08 19:20:56.844418 dspygen-2024.5.8/src/dspygen/agents/coder_agent_v4.py
+-rw-r--r--   0        0        0      614 2024-05-08 19:01:49.205349 dspygen-2024.5.8/src/dspygen/agents/idapr_adapter.py
+-rw-r--r--   0        0        0     1910 2024-05-08 19:05:27.394118 dspygen-2024.5.8/src/dspygen/agents/mock_dapr_adapter.py
+-rw-r--r--   0        0        0      123 2024-05-08 19:01:23.602497 dspygen-2024.5.8/src/dspygen/agents/order_payload.py
+-rw-r--r--   0        0        0     3706 2024-05-07 03:32:57.112778 dspygen-2024.5.8/src/dspygen/agents/pytest_agent.py
+-rw-r--r--   0        0        0     6992 2024-05-06 00:43:13.492936 dspygen-2024.5.8/src/dspygen/agents/research_agent.py
+-rw-r--r--   0        0        0     6135 2024-05-08 19:46:28.106496 dspygen-2024.5.8/src/dspygen/agents/workflow_agent.py
+-rw-r--r--   0        0        0     2278 2024-05-05 21:39:36.913588 dspygen-2024.5.8/src/dspygen/api.py
+-rw-r--r--   0        0        0     1019 2024-05-05 21:39:36.913639 dspygen-2024.5.8/src/dspygen/app.py
+-rw-r--r--   0        0        0      731 2024-05-05 21:39:36.913693 dspygen-2024.5.8/src/dspygen/async_typer.py
+-rw-r--r--   0        0        0      216 2024-05-05 21:39:36.913914 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/book.toml
+-rw-r--r--   0        0        0     2190 2024-05-05 21:39:36.913998 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/SUMMARY.md
+-rw-r--r--   0        0        0       13 2024-05-05 21:39:36.914070 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/appendices/README.md
+-rw-r--r--   0        0        0       18 2024-05-05 21:39:36.914111 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/appendices/further-reading.md
+-rw-r--r--   0        0        0       11 2024-05-05 21:39:36.914156 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/appendices/glossary.md
+-rw-r--r--   0        0        0       14 2024-05-05 21:39:36.914238 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/architecture/actor-model.md
+-rw-r--r--   0        0        0       21 2024-05-05 21:39:36.914281 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/architecture/content-management.md
+-rw-r--r--   0        0        0       15 2024-05-05 21:39:36.914327 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/architecture/domain-model.md
+-rw-r--r--   0        0        0       28 2024-05-05 21:39:36.914368 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/architecture/event-driven.md
+-rw-r--r--   0        0        0       22 2024-05-05 21:39:36.914421 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/architecture/feedback-generation.md
+-rw-r--r--   0        0        0       22 2024-05-05 21:39:36.914464 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/architecture/question-generation.md
+-rw-r--r--   0        0        0       19 2024-05-05 21:39:36.914527 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/architecture/student-modeling.md
+-rw-r--r--   0        0        0       54 2024-05-05 21:39:36.914631 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/best-practices/collaboration.md
+-rw-r--r--   0        0        0       29 2024-05-05 21:39:36.914698 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/best-practices/domain-modeling.md
+-rw-r--r--   0        0        0       32 2024-05-05 21:39:36.914775 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/best-practices/error-handling.md
+-rw-r--r--   0        0        0       22 2024-05-05 21:39:36.914925 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/best-practices/future-enhancements.md
+-rw-r--r--   0        0        0       27 2024-05-05 21:39:36.915093 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/best-practices/performance.md
+-rw-r--r--   0        0        0       12 2024-05-05 21:39:36.915154 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/chapter_1.md
+-rw-r--r--   0        0        0       34 2024-05-05 21:39:36.915253 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/foundations/ddd.md
+-rw-r--r--   0        0        0       22 2024-05-05 21:39:36.915521 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/foundations/language-models/in-context-learning.md
+-rw-r--r--   0        0        0       21 2024-05-05 21:39:36.915581 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/foundations/language-models/prompt-engineering.md
+-rw-r--r--   0        0        0       25 2024-05-05 21:39:36.915634 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/foundations/language-models/sparse-representations.md
+-rw-r--r--   0        0        0       18 2024-05-05 21:39:36.915311 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/foundations/language-models.md
+-rw-r--r--   0        0        0       24 2024-05-05 21:39:36.915686 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/foundations/reactive.md
+-rw-r--r--   0        0        0       23 2024-05-05 21:39:36.915767 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/implementation/application-services.md
+-rw-r--r--   0        0        0       33 2024-05-05 21:39:36.915825 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/implementation/code-generation.md
+-rw-r--r--   0        0        0       18 2024-05-05 21:39:36.915877 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/implementation/domain-services.md
+-rw-r--r--   0        0        0       18 2024-05-05 21:39:36.916029 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/implementation/infrastructure/message-brokers.md
+-rw-r--r--   0        0        0       14 2024-05-05 21:39:36.916083 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/implementation/infrastructure/persistence.md
+-rw-r--r--   0        0        0       17 2024-05-05 21:39:36.915933 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/implementation/infrastructure.md
+-rw-r--r--   0        0        0       29 2024-05-05 21:39:36.916136 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/implementation/language-model-integration.md
+-rw-r--r--   0        0        0       20 2024-05-05 21:39:36.916189 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/implementation/project-structure.md
+-rw-r--r--   0        0        0       15 2024-05-05 21:39:36.916281 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/introduction/overview.md
+-rw-r--r--   0        0        0       38 2024-05-05 21:39:36.916373 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/testing/ci-cd.md
+-rw-r--r--   0        0        0       22 2024-05-05 21:39:36.916427 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/testing/integration-testing.md
+-rw-r--r--   0        0        0       31 2024-05-05 21:39:36.916480 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/testing/monitoring.md
+-rw-r--r--   0        0        0       15 2024-05-05 21:39:36.916538 dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/testing/unit-testing.md
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.916606 dspygen-2024.5.8/src/dspygen/bpel_diagrams/__init__.py
+-rw-r--r--   0        0        0     5857 2024-05-05 21:39:36.916707 dspygen-2024.5.8/src/dspygen/bpel_diagrams/mermaid_multi_module_demo.py
+-rw-r--r--   0        0        0       49 2024-05-05 21:39:36.916799 dspygen-2024.5.8/src/dspygen/bpel_models/__init__.py
+-rw-r--r--   0        0        0    12392 2024-05-05 21:39:36.916873 dspygen-2024.5.8/src/dspygen/bpel_models/activities.py
+-rw-r--r--   0        0        0     4328 2024-05-05 21:39:36.916958 dspygen-2024.5.8/src/dspygen/bpel_models/correlations.py
+-rw-r--r--   0        0        0     2976 2024-05-05 21:39:36.917023 dspygen-2024.5.8/src/dspygen/bpel_models/event_handlers.py
+-rw-r--r--   0        0        0     5007 2024-05-05 21:39:36.917095 dspygen-2024.5.8/src/dspygen/bpel_models/fault_handlers.py
+-rw-r--r--   0        0        0     3787 2024-05-05 21:39:36.917161 dspygen-2024.5.8/src/dspygen/bpel_models/links.py
+-rw-r--r--   0        0        0     1934 2024-05-05 21:39:36.917223 dspygen-2024.5.8/src/dspygen/bpel_models/partner_links.py
+-rw-r--r--   0        0        0     2125 2024-05-05 21:39:36.917290 dspygen-2024.5.8/src/dspygen/bpel_models/process.py
+-rw-r--r--   0        0        0     5256 2024-05-05 21:39:36.917366 dspygen-2024.5.8/src/dspygen/bpel_models/variables.py
+-rw-r--r--   0        0        0       49 2024-05-05 21:39:36.917455 dspygen-2024.5.8/src/dspygen/bpmn_models/__init__.py
+-rw-r--r--   0        0        0     1682 2024-05-05 21:39:36.917513 dspygen-2024.5.8/src/dspygen/bpmn_models/artifacts.py
+-rw-r--r--   0        0        0     2236 2024-05-05 21:39:36.917572 dspygen-2024.5.8/src/dspygen/bpmn_models/connecting_objects.py
+-rw-r--r--   0        0        0     2360 2024-05-05 21:39:36.917631 dspygen-2024.5.8/src/dspygen/bpmn_models/events.py
+-rw-r--r--   0        0        0     1194 2024-05-05 21:39:36.917695 dspygen-2024.5.8/src/dspygen/bpmn_models/flow_objects.py
+-rw-r--r--   0        0        0      807 2024-05-05 21:39:36.917755 dspygen-2024.5.8/src/dspygen/bpmn_models/gateways.py
+-rw-r--r--   0        0        0     2604 2024-05-05 21:39:36.917811 dspygen-2024.5.8/src/dspygen/bpmn_models/other_entities.py
+-rw-r--r--   0        0        0     1508 2024-05-05 21:39:36.917869 dspygen-2024.5.8/src/dspygen/bpmn_models/pools_and_lanes.py
+-rw-r--r--   0        0        0      816 2024-05-05 21:39:36.917926 dspygen-2024.5.8/src/dspygen/bpmn_models/sub_processes.py
+-rw-r--r--   0        0        0     7676 2024-05-05 21:39:36.918009 dspygen-2024.5.8/src/dspygen/cli.py
+-rw-r--r--   0        0        0      469 2024-05-05 21:39:36.918078 dspygen-2024.5.8/src/dspygen/config.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.918138 dspygen-2024.5.8/src/dspygen/dsl/__init__.py
+-rw-r--r--   0        0        0     1257 2024-05-05 21:39:36.918212 dspygen-2024.5.8/src/dspygen/dsl/dsl_dspy_assertion.py
+-rw-r--r--   0        0        0     2732 2024-05-05 21:56:54.035475 dspygen-2024.5.8/src/dspygen/dsl/dsl_pipeline_executor.py
+-rw-r--r--   0        0        0     5086 2024-05-05 21:39:36.918350 dspygen-2024.5.8/src/dspygen/dsl/dsl_predict_module.py
+-rw-r--r--   0        0        0     6253 2024-05-05 21:39:36.918419 dspygen-2024.5.8/src/dspygen/dsl/dsl_pydantic_models.py
+-rw-r--r--   0        0        0     3519 2024-05-05 21:39:36.918473 dspygen-2024.5.8/src/dspygen/dsl/dsl_step_module.py
+-rw-r--r--   0        0        0      101 2024-05-05 21:39:36.918549 dspygen-2024.5.8/src/dspygen/dsl/examples/blog_pipeline.yaml
+-rw-r--r--   0        0        0      745 2024-05-05 21:39:36.918601 dspygen-2024.5.8/src/dspygen/dsl/examples/example_pipeline.yaml
+-rw-r--r--   0        0        0     1294 2024-05-05 21:39:36.918650 dspygen-2024.5.8/src/dspygen/dsl/examples/poem_pipeline.yaml
+-rw-r--r--   0        0        0     1395 2024-05-05 21:39:36.918698 dspygen-2024.5.8/src/dspygen/dsl/examples/saltcorn_plugin_generator.yaml
+-rw-r--r--   0        0        0      148 2024-05-05 21:39:36.918752 dspygen-2024.5.8/src/dspygen/dsl/examples/sql_to_nl.yaml
+-rw-r--r--   0        0        0       55 2024-05-05 21:39:36.918799 dspygen-2024.5.8/src/dspygen/dsl/examples/text_signature_pipeline.yaml
+-rw-r--r--   0        0        0       85 2024-05-05 21:39:36.918872 dspygen-2024.5.8/src/dspygen/dsl/modules/raw_to_structure_module.yaml
+-rw-r--r--   0        0        0      361 2024-05-05 21:39:36.918946 dspygen-2024.5.8/src/dspygen/dsl/signature/sql_to_natural_signature.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.918997 dspygen-2024.5.8/src/dspygen/dsl/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.919028 dspygen-2024.5.8/src/dspygen/dsl/utils/dsl_assertions_utils.py
+-rw-r--r--   0        0        0      566 2024-05-05 21:39:36.919099 dspygen-2024.5.8/src/dspygen/dsl/utils/dsl_language_model_utils.py
+-rw-r--r--   0        0        0     2699 2024-05-05 21:39:36.919152 dspygen-2024.5.8/src/dspygen/dsl/utils/dsl_lm_module_utils.py
+-rw-r--r--   0        0        0      852 2024-05-05 21:39:36.919205 dspygen-2024.5.8/src/dspygen/dsl/utils/dsl_retrieval_model_utils.py
+-rw-r--r--   0        0        0     1108 2024-05-05 21:39:36.919270 dspygen-2024.5.8/src/dspygen/dsl/utils/dsl_rm_module_utils.py
+-rw-r--r--   0        0        0     2517 2024-05-05 21:39:36.919338 dspygen-2024.5.8/src/dspygen/dsl/utils/dsl_signature_utils.py
+-rw-r--r--   0        0        0     1344 2024-05-05 21:39:36.919405 dspygen-2024.5.8/src/dspygen/dspygen_app.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.919464 dspygen-2024.5.8/src/dspygen/experiments/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.919528 dspygen-2024.5.8/src/dspygen/experiments/bkgn/__init__.py
+-rw-r--r--   0        0        0      667 2024-05-05 21:56:54.024131 dspygen-2024.5.8/src/dspygen/experiments/bkgn/chapter_draft.py
+-rw-r--r--   0        0        0     2751 2024-05-05 21:56:54.036357 dspygen-2024.5.8/src/dspygen/experiments/bkgn/get_book_files.py
+-rw-r--r--   0        0        0     2000 2024-05-05 21:56:54.022240 dspygen-2024.5.8/src/dspygen/experiments/bkgn/get_leaf.py
+-rw-r--r--   0        0        0    10333 2024-05-05 21:56:54.020904 dspygen-2024.5.8/src/dspygen/experiments/bkgn/get_soc_files.py
+-rw-r--r--   0        0        0     2011 2024-05-05 21:39:36.919837 dspygen-2024.5.8/src/dspygen/experiments/bkgn/quick_demo.py
+-rw-r--r--   0        0        0     2586 2024-05-05 21:39:36.919920 dspygen-2024.5.8/src/dspygen/experiments/blog/Tetris_1.md
+-rw-r--r--   0        0        0     3103 2024-05-05 21:39:36.919977 dspygen-2024.5.8/src/dspygen/experiments/blog/Tetris_LMStud_Llama3.py
+-rw-r--r--   0        0        0     2531 2024-05-05 21:39:36.920031 dspygen-2024.5.8/src/dspygen/experiments/blog/Tetris_groq.py
+-rw-r--r--   0        0        0     3302 2024-05-05 21:39:36.920084 dspygen-2024.5.8/src/dspygen/experiments/blog/Tetris_groq_llama3_80.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.920134 dspygen-2024.5.8/src/dspygen/experiments/bulk_code_generator/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-05 21:39:36.920202 dspygen-2024.5.8/src/dspygen/experiments/bulk_code_generator/main.py
+-rw-r--r--   0        0        0      585 2024-05-05 21:56:54.037122 dspygen-2024.5.8/src/dspygen/experiments/business_patterns_for_devs.py
+-rw-r--r--   0        0        0     1405 2024-05-05 21:39:36.920369 dspygen-2024.5.8/src/dspygen/experiments/done/CriticFeedbackGeneratorSignature_pipeline.yaml
+-rw-r--r--   0        0        0      668 2024-05-05 21:39:36.920430 dspygen-2024.5.8/src/dspygen/experiments/done/WebsitePRD_pipeline.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.920451 dspygen-2024.5.8/src/dspygen/experiments/done/__init__.py
+-rw-r--r--   0        0        0      331 2024-05-05 21:39:36.920511 dspygen-2024.5.8/src/dspygen/experiments/done/chatbots.py
+-rw-r--r--   0        0        0      361 2024-05-05 21:39:36.920570 dspygen-2024.5.8/src/dspygen/experiments/done/code_generator_agent.py
+-rw-r--r--   0        0        0     1790 2024-05-05 21:39:36.920626 dspygen-2024.5.8/src/dspygen/experiments/done/data_pipeline.yaml
+-rw-r--r--   0        0        0      260 2024-05-05 21:39:36.920682 dspygen-2024.5.8/src/dspygen/experiments/done/file_path.py
+-rw-r--r--   0        0        0      940 2024-05-05 21:39:36.920740 dspygen-2024.5.8/src/dspygen/experiments/done/first_step_with_user_input.py
+-rw-r--r--   0        0        0     1720 2024-05-05 21:39:36.920794 dspygen-2024.5.8/src/dspygen/experiments/done/gen_dsl_instances.py
+-rw-r--r--   0        0        0    14783 2024-05-05 21:39:36.920878 dspygen-2024.5.8/src/dspygen/experiments/done/gen_pydantic_class.py
+-rw-r--r--   0        0        0     6076 2024-05-05 21:39:36.920951 dspygen-2024.5.8/src/dspygen/experiments/done/gherkin_parser.py
+-rw-r--r--   0        0        0     3560 2024-05-05 21:39:36.921004 dspygen-2024.5.8/src/dspygen/experiments/done/lm_call.py
+-rw-r--r--   0        0        0     1061 2024-05-05 21:39:36.921059 dspygen-2024.5.8/src/dspygen/experiments/done/openai_ror_cli.py
+-rw-r--r--   0        0        0     1753 2024-05-05 21:39:36.921113 dspygen-2024.5.8/src/dspygen/experiments/done/python_to_elixir.py
+-rw-r--r--   0        0        0       87 2024-05-05 21:39:36.921168 dspygen-2024.5.8/src/dspygen/experiments/done/raw_to_structure_module.yaml
+-rw-r--r--   0        0        0      408 2024-05-05 21:39:36.921218 dspygen-2024.5.8/src/dspygen/experiments/done/saltcorn_plugin_generator.py
+-rw-r--r--   0        0        0    15627 2024-05-05 21:39:36.921275 dspygen-2024.5.8/src/dspygen/experiments/done/saltcorn_plugin_generator_output.yaml
+-rw-r--r--   0        0        0     1597 2024-05-05 21:39:36.921325 dspygen-2024.5.8/src/dspygen/experiments/done/socket_actor_system.py
+-rw-r--r--   0        0        0      286 2024-05-05 21:39:36.921372 dspygen-2024.5.8/src/dspygen/experiments/done/sql_to_natural_signature.yaml
+-rw-r--r--   0        0        0     1283 2024-05-05 21:39:36.921422 dspygen-2024.5.8/src/dspygen/experiments/done/test_openai_ror_cli.py
+-rw-r--r--   0        0        0     1864 2024-05-05 21:39:36.921580 dspygen-2024.5.8/src/dspygen/experiments/done/two_steps_with_user_input.py
+-rw-r--r--   0        0        0     1457 2024-05-05 21:39:36.921636 dspygen-2024.5.8/src/dspygen/experiments/done/understand_input_pipeline.yaml
+-rw-r--r--   0        0        0     2554 2024-05-05 21:39:36.921704 dspygen-2024.5.8/src/dspygen/experiments/done/wizard.py
+-rw-r--r--   0        0        0   884736 2024-05-05 21:39:36.922920 dspygen-2024.5.8/src/dspygen/experiments/function_calling/Chinook.db
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.922968 dspygen-2024.5.8/src/dspygen/experiments/function_calling/__init__.py
+-rw-r--r--   0        0        0     1145 2024-05-05 21:39:36.923032 dspygen-2024.5.8/src/dspygen/experiments/function_calling/function_call.py
+-rw-r--r--   0        0        0     1241 2024-05-05 21:39:36.923089 dspygen-2024.5.8/src/dspygen/experiments/function_calling/sql_calling_asserts.py
+-rw-r--r--   0        0        0     1802 2024-05-05 21:39:36.923146 dspygen-2024.5.8/src/dspygen/experiments/function_calling/sql_optimization_function.py
+-rw-r--r--   0        0        0      915 2024-05-05 21:39:36.923199 dspygen-2024.5.8/src/dspygen/experiments/function_calling/weather_function_calling_asserts.py
+-rw-r--r--   0        0        0     1029 2024-05-05 21:39:36.923252 dspygen-2024.5.8/src/dspygen/experiments/function_calling/weather_functions.exs
+-rw-r--r--   0        0        0        0 2024-05-06 16:37:21.090513 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/__init__.py
+-rw-r--r--   0        0        0     1679 2024-05-06 16:43:45.432058 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/auto_pytest_mock_rover.py
+-rw-r--r--   0        0        0     1397 2024-05-07 22:56:33.999148 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/min_example.py
+-rw-r--r--   0        0        0     5905 2024-05-07 22:57:40.654750 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/mipro_example.py
+-rw-r--r--   0        0        0     3887 2024-05-08 06:23:46.533401 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/mipro_swe_bench_example.py
+-rw-r--r--   0        0        0    50545 2024-05-07 05:03:05.064147 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/optimized_cot.json
+-rw-r--r--   0        0        0    21085 2024-05-07 05:27:35.316795 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/optimized_cot_sig.json
+-rw-r--r--   0        0        0    50539 2024-05-07 16:42:15.979451 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/optimized_cot_sig_1715100135.978442.json
+-rw-r--r--   0        0        0    50505 2024-05-08 04:56:07.618463 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/optimized_cot_sig_1715144167.617128.json
+-rw-r--r--   0        0        0    50505 2024-05-08 04:59:56.168140 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/optimized_cot_sig_1715144396.167356.json
+-rw-r--r--   0        0        0    50505 2024-05-08 05:03:01.270533 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/optimized_cot_sig_1715144581.270241.json
+-rw-r--r--   0        0        0     4545 2024-05-08 04:54:45.406715 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/swe_bench.py
+-rw-r--r--   0        0        0     3602 2024-05-08 05:58:28.723224 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/swebench_example.py
+-rw-r--r--   0        0        0     1635 2024-05-07 05:17:22.860325 dspygen-2024.5.8/src/dspygen/experiments/mock_gen/swebench_mipro_example.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.923304 dspygen-2024.5.8/src/dspygen/experiments/module_docstrings/__init__.py
+-rw-r--r--   0        0        0      776 2024-05-05 21:39:36.923367 dspygen-2024.5.8/src/dspygen/experiments/module_docstrings/generate_docstring_exec.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.923414 dspygen-2024.5.8/src/dspygen/experiments/pomo_bud/__init__.py
+-rw-r--r--   0        0        0      923 2024-05-05 21:39:36.923473 dspygen-2024.5.8/src/dspygen/experiments/pomo_bud/pomo_bud_dsl.yaml
+-rw-r--r--   0        0        0     4975 2024-05-05 21:39:36.923541 dspygen-2024.5.8/src/dspygen/experiments/pomo_bud/pomo_bud_models.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.923596 dspygen-2024.5.8/src/dspygen/experiments/quiz/__init__.py
+-rw-r--r--   0        0        0     7610 2024-05-05 21:39:36.923679 dspygen-2024.5.8/src/dspygen/experiments/quiz/quiz_input.py
+-rw-r--r--   0        0        0     1037 2024-05-05 21:39:36.923733 dspygen-2024.5.8/src/dspygen/experiments/quiz/session_data.json
+-rw-r--r--   0        0        0        0 2024-05-05 22:08:46.601395 dspygen-2024.5.8/src/dspygen/experiments/raga/__init__.py
+-rw-r--r--   0        0        0     5955 2024-05-06 00:47:55.965499 dspygen-2024.5.8/src/dspygen/experiments/raga/chat_gpt_rag_retrevier.py
+-rw-r--r--   0        0        0     1590 2024-05-05 22:18:40.646174 dspygen-2024.5.8/src/dspygen/experiments/raga/convo_loader.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.923780 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/__init__.py
+-rw-r--r--   0        0        0     2380 2024-05-05 21:39:36.923845 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/api-for-document-management.tsx
+-rw-r--r--   0        0        0      729 2024-05-05 21:39:36.923986 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/confirm-signature-placement.tsx
+-rw-r--r--   0        0        0      634 2024-05-05 21:39:36.924039 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/custom-signing-instructions.tsx
+-rw-r--r--   0        0        0     1555 2024-05-05 21:39:36.924169 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/data_gherkin_pipeline.yaml
+-rw-r--r--   0        0        0      349 2024-05-05 21:39:36.924219 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/document-download.tsx
+-rw-r--r--   0        0        0     3006 2024-05-05 21:39:36.924269 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/document-preview.tsx
+-rw-r--r--   0        0        0     1100 2024-05-05 21:39:36.924324 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/document-upload.tsx
+-rw-r--r--   0        0        0      518 2024-05-05 21:39:36.924459 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/drag-and-drop-document-upload.tsx
+-rw-r--r--   0        0        0      601 2024-05-05 21:39:36.924515 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/email-confirmation-to-sender.tsx
+-rw-r--r--   0        0        0     1222 2024-05-05 21:39:36.924571 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/email-link-to-signer.tsx
+-rw-r--r--   0        0        0      165 2024-05-05 21:39:36.924617 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/feature_data_pipeline.yaml
+-rw-r--r--   0        0        0     1034 2024-05-05 21:39:36.924678 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/generate-unique-signing-link.tsx
+-rw-r--r--   0        0        0      938 2024-05-05 21:39:36.924814 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/generate_react_code_from_csv.py
+-rw-r--r--   0        0        0     1425 2024-05-05 21:39:36.924955 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/gherkin_pipeline.yaml
+-rw-r--r--   0        0        0     5785 2024-05-05 21:39:36.925028 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/hello-world.tsx
+-rw-r--r--   0        0        0      591 2024-05-05 21:39:36.925088 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/link-expiration.tsx
+-rw-r--r--   0        0        0     1965 2024-05-05 21:39:36.925260 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/mobile-responsive-design.tsx
+-rw-r--r--   0        0        0      776 2024-05-05 21:39:36.925318 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/retrieve_and_generate_pipeline.py
+-rw-r--r--   0        0        0      391 2024-05-05 21:39:36.925465 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/save-signature.tsx
+-rw-r--r--   0        0        0      816 2024-05-05 21:39:36.925512 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/signature-capture.tsx
+-rw-r--r--   0        0        0      786 2024-05-05 21:39:36.925562 dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/signature-validation.tsx
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.925608 dspygen-2024.5.8/src/dspygen/experiments/rfc5545/__init__.py
+-rw-r--r--   0        0        0    11768 2024-05-05 21:39:36.925704 dspygen-2024.5.8/src/dspygen/experiments/rfc5545/calendar_cmd.py
+-rw-r--r--   0        0        0     2819 2024-05-05 21:39:36.925768 dspygen-2024.5.8/src/dspygen/experiments/rfc5545/ical_crud.py
+-rw-r--r--   0        0        0      270 2024-05-05 21:39:36.925824 dspygen-2024.5.8/src/dspygen/experiments/rfc5545/ical_data_ret.py
+-rw-r--r--   0        0        0      442 2024-05-05 21:39:36.925879 dspygen-2024.5.8/src/dspygen/experiments/rfc5545/ical_db_session.py
+-rw-r--r--   0        0        0    14826 2024-05-05 21:39:36.925935 dspygen-2024.5.8/src/dspygen/experiments/rfc5545/ical_models.py
+-rw-r--r--   0        0        0      657 2024-05-05 21:39:36.925982 dspygen-2024.5.8/src/dspygen/experiments/rfc5545/ical_workbench.py
+-rw-r--r--   0        0        0     3246 2024-05-05 21:39:36.926035 dspygen-2024.5.8/src/dspygen/experiments/rfc5545/journal_cmd.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926083 dspygen-2024.5.8/src/dspygen/experiments/self_coding/__init__.py
+-rw-r--r--   0        0        0     3050 2024-05-05 21:39:36.926149 dspygen-2024.5.8/src/dspygen/experiments/self_coding/interview_processing.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926198 dspygen-2024.5.8/src/dspygen/experiments/soonify_groq/__init__.py
+-rw-r--r--   0        0        0     2655 2024-05-05 21:39:36.926367 dspygen-2024.5.8/src/dspygen/experiments/soonify_groq/groq_pydantic.py
+-rw-r--r--   0        0        0     4831 2024-05-05 21:39:36.926439 dspygen-2024.5.8/src/dspygen/experiments/soonify_groq/run_groq_soon.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926488 dspygen-2024.5.8/src/dspygen/experiments/spider/__init__.py
+-rw-r--r--   0        0        0     2433 2024-05-05 21:39:36.926661 dspygen-2024.5.8/src/dspygen/experiments/spider/wiki_spider.py
+-rw-r--r--   0        0        0     5987 2024-05-05 21:39:36.926725 dspygen-2024.5.8/src/dspygen/experiments/state_actor.txt
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926773 dspygen-2024.5.8/src/dspygen/experiments/tagee/.gitignore
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926803 dspygen-2024.5.8/src/dspygen/experiments/tagee/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926833 dspygen-2024.5.8/src/dspygen/experiments/tagee/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926924 dspygen-2024.5.8/src/dspygen/experiments/tagee/assets/images/.keep
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.926979 dspygen-2024.5.8/src/dspygen/experiments/tagee/assets/sounds/.keep
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927044 dspygen-2024.5.8/src/dspygen/experiments/tagee/config/dev.json
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927074 dspygen-2024.5.8/src/dspygen/experiments/tagee/config/prod.json
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927103 dspygen-2024.5.8/src/dspygen/experiments/tagee/config/test.json
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927165 dspygen-2024.5.8/src/dspygen/experiments/tagee/docs/CurriculumAlignment.md
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927205 dspygen-2024.5.8/src/dspygen/experiments/tagee/docs/GettingStarted.md
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927247 dspygen-2024.5.8/src/dspygen/experiments/tagee/docs/TechnicalOverview.md
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927329 dspygen-2024.5.8/src/dspygen/experiments/tagee/lib/.keep
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927393 dspygen-2024.5.8/src/dspygen/experiments/tagee/scripts/deploy.sh
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927426 dspygen-2024.5.8/src/dspygen/experiments/tagee/scripts/maintenance.sh
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927456 dspygen-2024.5.8/src/dspygen/experiments/tagee/scripts/setup.sh
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927543 dspygen-2024.5.8/src/dspygen/experiments/tagee/src/core/education_module.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927572 dspygen-2024.5.8/src/dspygen/experiments/tagee/src/core/game_engine.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927601 dspygen-2024.5.8/src/dspygen/experiments/tagee/src/core/narrative_engine.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927688 dspygen-2024.5.8/src/dspygen/experiments/tagee/src/ui/modules/chatbot_view.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927719 dspygen-2024.5.8/src/dspygen/experiments/tagee/src/ui/modules/quiz_view.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927748 dspygen-2024.5.8/src/dspygen/experiments/tagee/src/ui/modules/story_view.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927804 dspygen-2024.5.8/src/dspygen/experiments/tagee/src/ui/utils/formatting_tools.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927837 dspygen-2024.5.8/src/dspygen/experiments/tagee/src/ui/utils/ui_helpers.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927943 dspygen-2024.5.8/src/dspygen/experiments/tagee/tests/integration/chatbot_integration_test.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.927982 dspygen-2024.5.8/src/dspygen/experiments/tagee/tests/integration/quiz_integration_test.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928029 dspygen-2024.5.8/src/dspygen/experiments/tagee/tests/integration/story_integration_test.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928128 dspygen-2024.5.8/src/dspygen/experiments/tagee/tests/unit/education_module_test.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928168 dspygen-2024.5.8/src/dspygen/experiments/tagee/tests/unit/game_engine_test.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928213 dspygen-2024.5.8/src/dspygen/experiments/tagee/tests/unit/narrative_engine_test.py
+-rw-r--r--   0        0        0     1367 2024-05-05 21:39:36.928339 dspygen-2024.5.8/src/dspygen/experiments/touch.sh
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928420 dspygen-2024.5.8/src/dspygen/experiments/txta/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928502 dspygen-2024.5.8/src/dspygen/experiments/wip/__init__.py
+-rw-r--r--   0        0        0     2452 2024-05-05 21:56:54.030536 dspygen-2024.5.8/src/dspygen/experiments/wip/chatgpt_conversation_parser.py
+-rw-r--r--   0        0        0      696 2024-05-05 21:39:36.928674 dspygen-2024.5.8/src/dspygen/experiments/wip/default_pipeline.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.928733 dspygen-2024.5.8/src/dspygen/experiments/wip/models/__init__.py
+-rw-r--r--   0        0        0    11258 2024-05-05 21:39:36.928863 dspygen-2024.5.8/src/dspygen/experiments/wip/models/dsl_project.py
+-rw-r--r--   0        0        0     3117 2024-05-05 21:39:36.928929 dspygen-2024.5.8/src/dspygen/experiments/wip/one_shot_pipeline.py
+-rw-r--r--   0        0        0     7582 2024-05-05 21:39:36.929009 dspygen-2024.5.8/src/dspygen/experiments/wip/self_evolving_business_logic.py
+-rw-r--r--   0        0        0       23 2024-05-05 21:39:36.929096 dspygen-2024.5.8/src/dspygen/lm/__init__.py
+-rw-r--r--   0        0        0     1645 2024-05-05 21:39:36.929153 dspygen-2024.5.8/src/dspygen/lm/groq_lm.py
+-rw-r--r--   0        0        0     1860 2024-05-05 21:39:36.929219 dspygen-2024.5.8/src/dspygen/lm/ollama_lm.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.929272 dspygen-2024.5.8/src/dspygen/mixin/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.929329 dspygen-2024.5.8/src/dspygen/mixin/btrees/__init__.py
+-rw-r--r--   0        0        0     4469 2024-05-05 21:39:36.929417 dspygen-2024.5.8/src/dspygen/mixin/btrees/bt_mixin_v2.py
+-rw-r--r--   0        0        0     6856 2024-05-05 21:39:36.929495 dspygen-2024.5.8/src/dspygen/mixin/btrees/bt_ros_works.py
+-rw-r--r--   0        0        0     2881 2024-05-05 21:39:36.929564 dspygen-2024.5.8/src/dspygen/mixin/btrees/bt_super.py
+-rw-r--r--   0        0        0      952 2024-05-05 21:39:36.929622 dspygen-2024.5.8/src/dspygen/mixin/btrees/bt_traffic.py
+-rw-r--r--   0        0        0     3717 2024-05-05 21:39:36.929689 dspygen-2024.5.8/src/dspygen/mixin/btrees/btree_mixin.py
+-rw-r--r--   0        0        0     2075 2024-05-05 21:39:36.929872 dspygen-2024.5.8/src/dspygen/mixin/btrees/superhero_activities.dot
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.929951 dspygen-2024.5.8/src/dspygen/mixin/fsm/__init__.py
+-rw-r--r--   0        0        0     1768 2024-05-05 21:39:36.930149 dspygen-2024.5.8/src/dspygen/mixin/fsm/employee_onboarding_fsm.py
+-rw-r--r--   0        0        0     1556 2024-05-05 21:39:36.930333 dspygen-2024.5.8/src/dspygen/mixin/fsm/example.py
+-rw-r--r--   0        0        0     2491 2024-05-05 21:39:36.930390 dspygen-2024.5.8/src/dspygen/mixin/fsm/fsm_gas.py
+-rw-r--r--   0        0        0     3755 2024-05-08 19:40:18.629065 dspygen-2024.5.8/src/dspygen/mixin/fsm/fsm_mixin.py
+-rw-r--r--   0        0        0    12039 2024-05-05 21:39:36.930562 dspygen-2024.5.8/src/dspygen/mixin/fsm/fsm_renderer.py
+-rw-r--r--   0        0        0     8122 2024-05-05 21:39:36.930650 dspygen-2024.5.8/src/dspygen/mixin/fsm/order_processing_fsm.py
+-rw-r--r--   0        0        0     1585 2024-05-05 21:39:36.930725 dspygen-2024.5.8/src/dspygen/mixin/fsm/traffic_light.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.930788 dspygen-2024.5.8/src/dspygen/mixin/hsm/__init__.py
+-rw-r--r--   0        0        0     2662 2024-05-05 21:39:36.930966 dspygen-2024.5.8/src/dspygen/mixin/hsm/hsm_mixin.py
+-rw-r--r--   0        0        0     1367 2024-05-05 21:39:36.931063 dspygen-2024.5.8/src/dspygen/models/BPMN.yaml
+-rw-r--r--   0        0        0     1316 2024-05-05 21:39:36.931210 dspygen-2024.5.8/src/dspygen/models/CMMN.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.931235 dspygen-2024.5.8/src/dspygen/models/__init__.py
+-rw-r--r--   0        0        0     2936 2024-05-05 21:39:36.931413 dspygen-2024.5.8/src/dspygen/models/bpm_plus_domain_models.py
+-rw-r--r--   0        0        0     1569 2024-05-05 21:39:36.931476 dspygen-2024.5.8/src/dspygen/models/cmmn_shipping.yaml
+-rw-r--r--   0        0        0      940 2024-05-05 21:39:36.931532 dspygen-2024.5.8/src/dspygen/models/dmn_shipping.yaml
+-rw-r--r--   0        0        0       70 2024-05-05 21:39:36.931593 dspygen-2024.5.8/src/dspygen/module_docstring_writer.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.931654 dspygen-2024.5.8/src/dspygen/modules/__init__.py
+-rw-r--r--   0        0        0     2149 2024-05-05 21:39:36.931743 dspygen-2024.5.8/src/dspygen/modules/arch_module.py
+-rw-r--r--   0        0        0     2933 2024-05-08 16:48:08.919887 dspygen-2024.5.8/src/dspygen/modules/base_model_module.py
+-rw-r--r--   0        0        0      782 2024-05-05 21:39:36.931810 dspygen-2024.5.8/src/dspygen/modules/bill_of_objects_module.py
+-rw-r--r--   0        0        0     1359 2024-05-05 21:39:36.931867 dspygen-2024.5.8/src/dspygen/modules/binary_output_module.py
+-rw-r--r--   0        0        0     2461 2024-05-05 21:39:36.931935 dspygen-2024.5.8/src/dspygen/modules/blog_module.py
+-rw-r--r--   0        0        0     2103 2024-05-05 21:39:36.931995 dspygen-2024.5.8/src/dspygen/modules/book_appointment_module.py
+-rw-r--r--   0        0        0     2186 2024-05-05 21:39:36.932054 dspygen-2024.5.8/src/dspygen/modules/bpmn2_bpel_module.py
+-rw-r--r--   0        0        0     1116 2024-05-05 21:39:36.932115 dspygen-2024.5.8/src/dspygen/modules/business_dev_consultant.py
+-rw-r--r--   0        0        0     2429 2024-05-05 21:39:36.932178 dspygen-2024.5.8/src/dspygen/modules/business_requirements.py
+-rw-r--r--   0        0        0     1151 2024-05-05 21:39:36.932230 dspygen-2024.5.8/src/dspygen/modules/chat_bot_cli.py
+-rw-r--r--   0        0        0     1920 2024-05-05 21:39:36.932278 dspygen-2024.5.8/src/dspygen/modules/chat_bot_module.py
+-rw-r--r--   0        0        0     1058 2024-05-05 21:39:36.932332 dspygen-2024.5.8/src/dspygen/modules/checker_module.py
+-rw-r--r--   0        0        0     4382 2024-05-05 21:39:36.932400 dspygen-2024.5.8/src/dspygen/modules/choose_function_module.py
+-rw-r--r--   0        0        0      931 2024-05-05 21:39:36.932454 dspygen-2024.5.8/src/dspygen/modules/cli_bot_module.py
+-rw-r--r--   0        0        0     1233 2024-05-05 21:39:36.932513 dspygen-2024.5.8/src/dspygen/modules/cobol_to_python_module.py
+-rw-r--r--   0        0        0     2922 2024-05-06 00:19:09.661287 dspygen-2024.5.8/src/dspygen/modules/condition_sufficient_info_module.py
+-rw-r--r--   0        0        0     4265 2024-05-05 21:39:36.932580 dspygen-2024.5.8/src/dspygen/modules/dflss_module.py
+-rw-r--r--   0        0        0      751 2024-05-05 21:39:36.932646 dspygen-2024.5.8/src/dspygen/modules/dflss_output.txt
+-rw-r--r--   0        0        0      859 2024-05-05 21:39:36.932709 dspygen-2024.5.8/src/dspygen/modules/dspygen_dsl_pipeline.py
+-rw-r--r--   0        0        0     3530 2024-05-05 21:39:36.932771 dspygen-2024.5.8/src/dspygen/modules/dspygen_module.py
+-rw-r--r--   0        0        0     5765 2024-05-05 21:39:36.932854 dspygen-2024.5.8/src/dspygen/modules/elite_module.py
+-rw-r--r--   0        0        0     2039 2024-05-05 21:39:36.932915 dspygen-2024.5.8/src/dspygen/modules/exam_point_weight_module.py
+-rw-r--r--   0        0        0     2160 2024-05-05 21:39:36.932964 dspygen-2024.5.8/src/dspygen/modules/faang_module.py
+-rw-r--r--   0        0        0     2247 2024-05-05 21:39:36.933016 dspygen-2024.5.8/src/dspygen/modules/faang_sys_arch_nuxt_module.py
+-rw-r--r--   0        0        0     1274 2024-05-05 21:39:36.933166 dspygen-2024.5.8/src/dspygen/modules/file_name_module.py
+-rw-r--r--   0        0        0     1666 2024-05-08 19:48:39.021848 dspygen-2024.5.8/src/dspygen/modules/fsm_trigger_module.py
+-rw-r--r--   0        0        0     2385 2024-05-05 21:39:36.933224 dspygen-2024.5.8/src/dspygen/modules/function_invoke_module.py
+-rw-r--r--   0        0        0     4239 2024-05-05 21:39:36.933287 dspygen-2024.5.8/src/dspygen/modules/gen_cli_module.py
+-rw-r--r--   0        0        0     2213 2024-05-05 21:39:36.933349 dspygen-2024.5.8/src/dspygen/modules/gen_dspy_module.py
+-rw-r--r--   0        0        0     5363 2024-05-05 21:39:36.933416 dspygen-2024.5.8/src/dspygen/modules/gen_keyword_arguments_module.py
+-rw-r--r--   0        0        0     1093 2024-05-05 21:39:36.933466 dspygen-2024.5.8/src/dspygen/modules/gen_message_module.py
+-rw-r--r--   0        0        0     1901 2024-05-05 21:39:36.933513 dspygen-2024.5.8/src/dspygen/modules/gen_module.py
+-rw-r--r--   0        0        0    14776 2024-05-05 21:39:36.933566 dspygen-2024.5.8/src/dspygen/modules/gen_pydantic_class.py
+-rw-r--r--   0        0        0    10747 2024-05-05 21:39:36.933653 dspygen-2024.5.8/src/dspygen/modules/gen_pydantic_instance.py
+-rw-r--r--   0        0        0     5555 2024-05-05 21:39:36.933725 dspygen-2024.5.8/src/dspygen/modules/gen_pydantic_instance_module.py
+-rw-r--r--   0        0        0     3398 2024-05-05 21:50:16.283283 dspygen-2024.5.8/src/dspygen/modules/gen_python_primitive.py
+-rw-r--r--   0        0        0     1266 2024-05-05 21:39:36.933824 dspygen-2024.5.8/src/dspygen/modules/gen_signature_module.py
+-rw-r--r--   0        0        0     4595 2024-05-05 21:39:36.933885 dspygen-2024.5.8/src/dspygen/modules/get_selector_module.py
+-rw-r--r--   0        0        0     1099 2024-05-05 21:39:36.934044 dspygen-2024.5.8/src/dspygen/modules/gusty_module.py
+-rw-r--r--   0        0        0      137 2024-05-05 21:39:36.934096 dspygen-2024.5.8/src/dspygen/modules/hello_world_module.yaml
+-rw-r--r--   0        0        0     1421 2024-05-05 21:39:36.934152 dspygen-2024.5.8/src/dspygen/modules/html_module.py
+-rw-r--r--   0        0        0     1899 2024-05-05 21:39:36.934202 dspygen-2024.5.8/src/dspygen/modules/insight_tweet_module.py
+-rw-r--r--   0        0        0     2869 2024-05-05 21:39:36.934253 dspygen-2024.5.8/src/dspygen/modules/js_to_fast_api_module.py
+-rw-r--r--   0        0        0     5027 2024-05-08 16:57:15.444460 dspygen-2024.5.8/src/dspygen/modules/json_module.py
+-rw-r--r--   0        0        0     1788 2024-05-05 21:39:36.934365 dspygen-2024.5.8/src/dspygen/modules/jsx_module.py
+-rw-r--r--   0        0        0     1997 2024-05-05 21:39:36.934528 dspygen-2024.5.8/src/dspygen/modules/long_form_qa_module.py
+-rw-r--r--   0        0        0     7742 2024-05-05 21:39:36.934598 dspygen-2024.5.8/src/dspygen/modules/md_book_summarizer_module.py
+-rw-r--r--   0        0        0     2732 2024-05-05 21:39:36.934647 dspygen-2024.5.8/src/dspygen/modules/mermaid_js_module.py
+-rw-r--r--   0        0        0     1337 2024-05-05 21:39:36.934693 dspygen-2024.5.8/src/dspygen/modules/message_module.py
+-rw-r--r--   0        0        0     1239 2024-05-05 21:39:36.934739 dspygen-2024.5.8/src/dspygen/modules/module_docstring_module.py
+-rw-r--r--   0        0        0      335 2024-05-05 21:39:36.934787 dspygen-2024.5.8/src/dspygen/modules/pipeline.yaml
+-rw-r--r--   0        0        0     1787 2024-05-05 21:39:36.934844 dspygen-2024.5.8/src/dspygen/modules/product_bot_module.py
+-rw-r--r--   0        0        0      819 2024-05-05 21:39:36.934900 dspygen-2024.5.8/src/dspygen/modules/prompt_function_call_module.py
+-rw-r--r--   0        0        0     4048 2024-05-06 22:58:03.790452 dspygen-2024.5.8/src/dspygen/modules/pytest_module.py
+-rw-r--r--   0        0        0     1781 2024-05-05 21:39:36.934946 dspygen-2024.5.8/src/dspygen/modules/python_expert_module.py
+-rw-r--r--   0        0        0     1878 2024-05-06 03:10:48.896564 dspygen-2024.5.8/src/dspygen/modules/python_source_code_module.py
+-rw-r--r--   0        0        0     1781 2024-05-05 21:39:36.935034 dspygen-2024.5.8/src/dspygen/modules/pyts_module.py
+-rw-r--r--   0        0        0     2641 2024-05-06 00:40:47.401404 dspygen-2024.5.8/src/dspygen/modules/query_generator_module.py
+-rw-r--r--   0        0        0     1261 2024-05-05 21:39:36.935080 dspygen-2024.5.8/src/dspygen/modules/rails_code_module.py
+-rw-r--r--   0        0        0      849 2024-05-05 21:39:36.935127 dspygen-2024.5.8/src/dspygen/modules/react_jsx_module.py
+-rw-r--r--   0        0        0     2717 2024-05-06 00:19:09.661560 dspygen-2024.5.8/src/dspygen/modules/refine_results_module.py
+-rw-r--r--   0        0        0     1001 2024-05-05 21:39:36.935176 dspygen-2024.5.8/src/dspygen/modules/request_contract_module.py
+-rw-r--r--   0        0        0     5828 2024-05-05 21:39:36.935242 dspygen-2024.5.8/src/dspygen/modules/signature_factory.py
+-rw-r--r--   0        0        0     5969 2024-05-05 21:39:36.935312 dspygen-2024.5.8/src/dspygen/modules/signature_renderer.py
+-rw-r--r--   0        0        0     1744 2024-05-05 21:39:36.935450 dspygen-2024.5.8/src/dspygen/modules/source_code_pep8_docs_module.py
+-rw-r--r--   0        0        0     2658 2024-05-06 00:19:09.661691 dspygen-2024.5.8/src/dspygen/modules/source_selector_module.py
+-rw-r--r--   0        0        0      969 2024-05-05 21:39:36.935497 dspygen-2024.5.8/src/dspygen/modules/sql_query_module.py
+-rw-r--r--   0        0        0     2073 2024-05-05 21:39:36.935541 dspygen-2024.5.8/src/dspygen/modules/streamlit_bot_module.py
+-rw-r--r--   0        0        0     2165 2024-05-05 21:39:36.935601 dspygen-2024.5.8/src/dspygen/modules/subject_destination_audience_newsletter_article_module.py
+-rw-r--r--   0        0        0     1798 2024-05-05 21:39:36.935657 dspygen-2024.5.8/src/dspygen/modules/success_planner_module.py
+-rw-r--r--   0        0        0     1052 2024-05-05 21:39:36.935707 dspygen-2024.5.8/src/dspygen/modules/tax_return_agent.py
+-rw-r--r--   0        0        0      914 2024-05-05 21:39:36.935751 dspygen-2024.5.8/src/dspygen/modules/test.py
+-rw-r--r--   0        0        0     1486 2024-05-05 21:39:36.935792 dspygen-2024.5.8/src/dspygen/modules/test_chat_bot_cli.py
+-rw-r--r--   0        0        0      799 2024-05-05 21:39:36.935841 dspygen-2024.5.8/src/dspygen/modules/text_summary_module_module.py
+-rw-r--r--   0        0        0     1767 2024-05-05 21:39:36.935889 dspygen-2024.5.8/src/dspygen/modules/to_elixir_module.py
+-rw-r--r--   0        0        0     2330 2024-05-05 21:39:36.935933 dspygen-2024.5.8/src/dspygen/modules/usp_connect_ship_webhook.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.935980 dspygen-2024.5.8/src/dspygen/pages/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-05 21:39:36.936036 dspygen-2024.5.8/src/dspygen/pages/hello.py
+-rw-r--r--   0        0        0     1407 2024-05-05 21:39:36.936082 dspygen-2024.5.8/src/dspygen/pages/mqtt_page.py
+-rw-r--r--   0        0        0      481 2024-05-05 21:39:36.936129 dspygen-2024.5.8/src/dspygen/pages/remodeling.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.936177 dspygen-2024.5.8/src/dspygen/prototypes/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.936238 dspygen-2024.5.8/src/dspygen/prototypes/state_chat/__init__.py
+-rw-r--r--   0        0        0     5029 2024-05-05 21:39:36.936310 dspygen-2024.5.8/src/dspygen/prototypes/state_chat/hello_world_convo_agent.py
+-rw-r--r--   0        0        0     9821 2024-05-05 21:39:36.936392 dspygen-2024.5.8/src/dspygen/prototypes/state_chat/socrates_convo.py
+-rw-r--r--   0        0        0       23 2024-05-05 21:39:36.936589 dspygen-2024.5.8/src/dspygen/rdddy/__init__.py
+-rw-r--r--   0        0        0    17082 2024-05-05 21:39:36.936661 dspygen-2024.5.8/src/dspygen/rdddy/actor_system.py
+-rw-r--r--   0        0        0    11050 2024-05-05 21:39:36.936745 dspygen-2024.5.8/src/dspygen/rdddy/base_actor.py
+-rw-r--r--   0        0        0     1155 2024-05-05 21:39:36.936869 dspygen-2024.5.8/src/dspygen/rdddy/base_aggregate.py
+-rw-r--r--   0        0        0      125 2024-05-05 21:39:36.936913 dspygen-2024.5.8/src/dspygen/rdddy/base_command.py
+-rw-r--r--   0        0        0      113 2024-05-05 21:39:36.936957 dspygen-2024.5.8/src/dspygen/rdddy/base_event.py
+-rw-r--r--   0        0        0     3539 2024-05-05 21:39:36.937019 dspygen-2024.5.8/src/dspygen/rdddy/base_message.py
+-rw-r--r--   0        0        0      648 2024-05-05 21:39:36.937070 dspygen-2024.5.8/src/dspygen/rdddy/base_policy.py
+-rw-r--r--   0        0        0      113 2024-05-05 21:39:36.937112 dspygen-2024.5.8/src/dspygen/rdddy/base_query.py
+-rw-r--r--   0        0        0      165 2024-05-05 21:39:36.937159 dspygen-2024.5.8/src/dspygen/rdddy/base_read_model.py
+-rw-r--r--   0        0        0     3123 2024-05-05 21:39:36.937210 dspygen-2024.5.8/src/dspygen/rdddy/base_repository.py
+-rw-r--r--   0        0        0      522 2024-05-05 21:39:36.937338 dspygen-2024.5.8/src/dspygen/rdddy/base_saga.py
+-rw-r--r--   0        0        0      446 2024-05-05 21:39:36.937387 dspygen-2024.5.8/src/dspygen/rdddy/base_task.py
+-rw-r--r--   0        0        0      416 2024-05-05 21:39:36.937435 dspygen-2024.5.8/src/dspygen/rdddy/base_value_object.py
+-rw-r--r--   0        0        0      405 2024-05-05 21:39:36.937483 dspygen-2024.5.8/src/dspygen/rdddy/base_view.py
+-rw-r--r--   0        0        0       23 2024-05-05 21:39:36.937623 dspygen-2024.5.8/src/dspygen/rdddy/browser/__init__.py
+-rw-r--r--   0        0        0     2435 2024-05-05 21:39:36.937681 dspygen-2024.5.8/src/dspygen/rdddy/browser/browser_domain.py
+-rw-r--r--   0        0        0     4129 2024-05-05 21:39:36.937750 dspygen-2024.5.8/src/dspygen/rdddy/browser/browser_process_supervisor.py
+-rw-r--r--   0        0        0     5541 2024-05-05 21:39:36.937819 dspygen-2024.5.8/src/dspygen/rdddy/browser/browser_worker.py
+-rw-r--r--   0        0        0      118 2024-05-05 21:39:36.937952 dspygen-2024.5.8/src/dspygen/rdddy/browser/run_chatgpt.py
+-rw-r--r--   0        0        0      425 2024-05-05 21:39:36.938003 dspygen-2024.5.8/src/dspygen/rdddy/domain_exception.py
+-rw-r--r--   0        0        0     5345 2024-05-08 04:47:32.013547 dspygen-2024.5.8/src/dspygen/rdddy/event_storm_domain_specification_model.py
+-rw-r--r--   0        0        0     1079 2024-05-05 21:39:36.938117 dspygen-2024.5.8/src/dspygen/rdddy/event_storm_model.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.938173 dspygen-2024.5.8/src/dspygen/rm/__init__.py
+-rw-r--r--   0        0        0     8406 2024-05-06 16:16:54.869789 dspygen-2024.5.8/src/dspygen/rm/chatgpt_chromadb_retriever.py
+-rw-r--r--   0        0        0     1106 2024-05-05 21:39:36.938356 dspygen-2024.5.8/src/dspygen/rm/chatgpt_string_retriever.py
+-rw-r--r--   0        0        0     3985 2024-05-07 06:10:18.872098 dspygen-2024.5.8/src/dspygen/rm/chroma_retriever.py
+-rw-r--r--   0        0        0     3529 2024-05-05 21:56:54.026813 dspygen-2024.5.8/src/dspygen/rm/code_retriever.py
+-rw-r--r--   0        0        0     4577 2024-05-05 21:39:36.938481 dspygen-2024.5.8/src/dspygen/rm/data_retriever.py
+-rw-r--r--   0        0        0     2692 2024-05-05 21:56:54.033125 dspygen-2024.5.8/src/dspygen/rm/doc_retriever.py
+-rw-r--r--   0        0        0      316 2024-05-05 21:39:36.938580 dspygen-2024.5.8/src/dspygen/rm/natural_language_data_retriever.py
+-rw-r--r--   0        0        0     3964 2024-05-05 21:39:36.938630 dspygen-2024.5.8/src/dspygen/rm/python_code_retriever.py
+-rw-r--r--   0        0        0      424 2024-05-05 21:39:36.938678 dspygen-2024.5.8/src/dspygen/rm/web_retriever.py
+-rw-r--r--   0        0        0       38 2024-05-05 21:39:36.938752 dspygen-2024.5.8/src/dspygen/signatures/__init__.py
+-rw-r--r--   0        0        0      400 2024-05-05 21:39:36.938803 dspygen-2024.5.8/src/dspygen/signatures/blog_article.py
+-rw-r--r--   0        0        0      425 2024-05-05 21:39:36.938849 dspygen-2024.5.8/src/dspygen/signatures/generate_answer.py
+-rw-r--r--   0        0        0      635 2024-05-05 21:39:36.938909 dspygen-2024.5.8/src/dspygen/signatures/signature.yaml
+-rw-r--r--   0        0        0     1972 2024-05-05 21:39:36.938960 dspygen-2024.5.8/src/dspygen/signatures/signature_dsl.py
+-rw-r--r--   0        0        0       23 2024-05-05 21:39:36.939049 dspygen-2024.5.8/src/dspygen/subcommands/__init__.py
+-rw-r--r--   0        0        0     2849 2024-05-05 21:39:36.939112 dspygen-2024.5.8/src/dspygen/subcommands/actor_cmd.py
+-rw-r--r--   0        0        0     1890 2024-05-05 21:39:36.939170 dspygen-2024.5.8/src/dspygen/subcommands/assert_cmd.py
+-rw-r--r--   0        0        0      993 2024-05-05 21:39:36.939225 dspygen-2024.5.8/src/dspygen/subcommands/browser_cmd.py
+-rw-r--r--   0        0        0     2795 2024-05-05 21:39:36.939277 dspygen-2024.5.8/src/dspygen/subcommands/cmd_cmd.py
+-rw-r--r--   0        0        0     1020 2024-05-05 21:39:36.939334 dspygen-2024.5.8/src/dspygen/subcommands/code_cmd.py
+-rw-r--r--   0        0        0     2192 2024-05-05 21:39:36.939390 dspygen-2024.5.8/src/dspygen/subcommands/help.txt
+-rw-r--r--   0        0        0     3654 2024-05-05 21:39:36.939445 dspygen-2024.5.8/src/dspygen/subcommands/help_cmd.py
+-rw-r--r--   0        0        0      984 2024-05-05 21:39:36.939500 dspygen-2024.5.8/src/dspygen/subcommands/lm_cmd.py
+-rw-r--r--   0        0        0     2167 2024-05-05 21:39:36.939559 dspygen-2024.5.8/src/dspygen/subcommands/module_cmd.py
+-rw-r--r--   0        0        0     6944 2024-05-05 21:39:36.939625 dspygen-2024.5.8/src/dspygen/subcommands/pln_cmd.py
+-rw-r--r--   0        0        0      258 2024-05-05 21:39:36.939677 dspygen-2024.5.8/src/dspygen/subcommands/poet_cmd.py
+-rw-r--r--   0        0        0      810 2024-05-05 21:39:36.939725 dspygen-2024.5.8/src/dspygen/subcommands/rm_cmd.py
+-rw-r--r--   0        0        0      763 2024-05-05 21:39:36.939777 dspygen-2024.5.8/src/dspygen/subcommands/sig_cmd.py
+-rw-r--r--   0        0        0     2660 2024-05-05 21:39:36.939834 dspygen-2024.5.8/src/dspygen/subcommands/temp_assert.py
+-rw-r--r--   0        0        0     7118 2024-05-05 21:56:54.028290 dspygen-2024.5.8/src/dspygen/subcommands/wkf_cmd.py
+-rw-r--r--   0        0        0      786 2024-05-05 21:39:36.939937 dspygen-2024.5.8/src/dspygen/subcommands/wrt_cmd.py
+-rw-r--r--   0        0        0      600 2024-05-05 21:39:36.940013 dspygen-2024.5.8/src/dspygen/templates/actor_template.j2
+-rw-r--r--   0        0        0      187 2024-05-05 21:39:36.940062 dspygen-2024.5.8/src/dspygen/templates/dspy_module_cli_call.j2
+-rw-r--r--   0        0        0      146 2024-05-05 21:39:36.940112 dspygen-2024.5.8/src/dspygen/templates/dspy_module_def_call.j2
+-rw-r--r--   0        0        0      172 2024-05-05 21:39:36.940155 dspygen-2024.5.8/src/dspygen/templates/dspy_module_main.j2
+-rw-r--r--   0        0        0      240 2024-05-05 21:39:36.940203 dspygen-2024.5.8/src/dspygen/templates/dspy_module_route.j2
+-rw-r--r--   0        0        0      335 2024-05-05 21:39:36.940255 dspygen-2024.5.8/src/dspygen/templates/dspy_module_streamlit_input.j2
+-rw-r--r--   0        0        0      378 2024-05-05 21:39:36.940304 dspygen-2024.5.8/src/dspygen/templates/signature_class_def.j2
+-rw-r--r--   0        0        0     1622 2024-05-05 21:39:36.940350 dspygen-2024.5.8/src/dspygen/touch_models.sh
+-rw-r--r--   0        0        0      577 2024-05-05 21:39:36.940421 dspygen-2024.5.8/src/dspygen/typetemp/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.940470 dspygen-2024.5.8/src/dspygen/typetemp/environment/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-05 21:39:36.940532 dspygen-2024.5.8/src/dspygen/typetemp/environment/typed_environment.py
+-rw-r--r--   0        0        0      979 2024-05-05 21:39:36.940581 dspygen-2024.5.8/src/dspygen/typetemp/environment/typed_native_environment.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.940636 dspygen-2024.5.8/src/dspygen/typetemp/extension/__init__.py
+-rw-r--r--   0        0        0    24023 2024-05-05 21:39:36.940726 dspygen-2024.5.8/src/dspygen/typetemp/extension/faker_extension.py
+-rw-r--r--   0        0        0     1098 2024-05-05 21:39:36.940777 dspygen-2024.5.8/src/dspygen/typetemp/extension/inflection_extension.py
+-rw-r--r--   0        0        0     1812 2024-05-05 21:39:36.940830 dspygen-2024.5.8/src/dspygen/typetemp/functional.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.940880 dspygen-2024.5.8/src/dspygen/typetemp/template/__init__.py
+-rw-r--r--   0        0        0     2454 2024-05-05 21:39:36.940938 dspygen-2024.5.8/src/dspygen/typetemp/template/async_render_mixin.py
+-rw-r--r--   0        0        0    11207 2024-05-05 21:39:36.941024 dspygen-2024.5.8/src/dspygen/typetemp/template/dsl_project.py
+-rw-r--r--   0        0        0      241 2024-05-05 21:39:36.941069 dspygen-2024.5.8/src/dspygen/typetemp/template/python
+-rw-r--r--   0        0        0     1001 2024-05-05 21:39:36.941118 dspygen-2024.5.8/src/dspygen/typetemp/template/render_funcs.py
+-rw-r--r--   0        0        0     2160 2024-05-05 21:39:36.941166 dspygen-2024.5.8/src/dspygen/typetemp/template/render_mixin.py
+-rw-r--r--   0        0        0     3393 2024-05-05 21:39:36.941217 dspygen-2024.5.8/src/dspygen/typetemp/template/smart_template.py
+-rw-r--r--   0        0        0     5497 2024-05-05 21:39:36.941279 dspygen-2024.5.8/src/dspygen/typetemp/template/typed_injector.py
+-rw-r--r--   0        0        0     2348 2024-05-05 21:39:36.941329 dspygen-2024.5.8/src/dspygen/typetemp/template/typed_prompt.py
+-rw-r--r--   0        0        0     2590 2024-05-05 21:39:36.941380 dspygen-2024.5.8/src/dspygen/typetemp/template/typed_python_source.py
+-rw-r--r--   0        0        0     1042 2024-05-05 21:39:36.941532 dspygen-2024.5.8/src/dspygen/typetemp/template/typed_template.py
+-rw-r--r--   0        0        0       23 2024-05-05 21:39:36.941613 dspygen-2024.5.8/src/dspygen/utils/MyData.yaml
+-rw-r--r--   0        0        0       23 2024-05-05 21:39:36.941654 dspygen-2024.5.8/src/dspygen/utils/__init__.py
+-rw-r--r--   0        0        0     1698 2024-05-05 21:39:36.941700 dspygen-2024.5.8/src/dspygen/utils/cli_tools.py
+-rw-r--r--   0        0        0    12563 2024-05-05 21:56:54.031492 dspygen-2024.5.8/src/dspygen/utils/complete.py
+-rw-r--r--   0        0        0     2961 2024-05-05 21:39:36.941807 dspygen-2024.5.8/src/dspygen/utils/compression_tools.py
+-rw-r--r--   0        0        0       65 2024-05-05 21:39:36.941852 dspygen-2024.5.8/src/dspygen/utils/contact.yaml
+-rw-r--r--   0        0        0    25532 2024-05-05 21:39:36.941940 dspygen-2024.5.8/src/dspygen/utils/create_prompts.py
+-rw-r--r--   0        0        0     2197 2024-05-05 21:39:36.941997 dspygen-2024.5.8/src/dspygen/utils/crud_tools.py
+-rw-r--r--   0        0        0     1620 2024-05-05 21:39:36.942051 dspygen-2024.5.8/src/dspygen/utils/date_tools.py
+-rw-r--r--   0        0        0      685 2024-05-08 04:30:20.380322 dspygen-2024.5.8/src/dspygen/utils/dspy_tools.py
+-rw-r--r--   0        0        0      118 2024-05-05 21:39:36.943767 dspygen-2024.5.8/src/dspygen/utils/example.py
+-rw-r--r--   0        0        0     6772 2024-05-05 21:39:36.943890 dspygen-2024.5.8/src/dspygen/utils/file_tools.py
+-rw-r--r--   0        0        0     1061 2024-05-05 21:39:36.943956 dspygen-2024.5.8/src/dspygen/utils/json_tools.py
+-rw-r--r--   0        0        0     4684 2024-05-05 21:39:36.944032 dspygen-2024.5.8/src/dspygen/utils/models.py
+-rw-r--r--   0        0        0     1641 2024-05-05 21:39:36.944085 dspygen-2024.5.8/src/dspygen/utils/module_tools.py
+-rw-r--r--   0        0        0     1772 2024-05-05 21:39:36.944137 dspygen-2024.5.8/src/dspygen/utils/pydantic_tools.py
+-rw-r--r--   0        0        0     3743 2024-05-07 22:44:34.036186 dspygen-2024.5.8/src/dspygen/utils/scraping_tools.py
+-rw-r--r--   0        0        0     8227 2024-05-05 21:39:36.944228 dspygen-2024.5.8/src/dspygen/utils/yaml_tools.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.944282 dspygen-2024.5.8/src/dspygen/workflow/__init__.py
+-rw-r--r--   0        0        0     1776 2024-05-05 21:39:36.944470 dspygen-2024.5.8/src/dspygen/workflow/control_flow_workflow.yaml
+-rw-r--r--   0        0        0     1885 2024-05-05 21:39:36.944524 dspygen-2024.5.8/src/dspygen/workflow/control_flow_workflow_output_new.yaml
+-rw-r--r--   0        0        0      923 2024-05-05 21:56:54.029489 dspygen-2024.5.8/src/dspygen/workflow/data_analysis_workflow.yaml
+-rw-r--r--   0        0        0      912 2024-05-05 21:39:36.944640 dspygen-2024.5.8/src/dspygen/workflow/data_preparation_workflow.yaml
+-rw-r--r--   0        0        0     2773 2024-05-05 21:56:54.024971 dspygen-2024.5.8/src/dspygen/workflow/workflow_engine.py
+-rw-r--r--   0        0        0     3765 2024-05-05 21:39:36.944751 dspygen-2024.5.8/src/dspygen/workflow/workflow_executor.py
+-rw-r--r--   0        0        0    10229 2024-05-05 21:39:36.944839 dspygen-2024.5.8/src/dspygen/workflow/workflow_models.py
+-rw-r--r--   0        0        0     1697 2024-05-05 21:39:36.944898 dspygen-2024.5.8/src/dspygen/workflow/workflow_router.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:39:36.944953 dspygen-2024.5.8/src/dspygen/writer/__init__.py
+-rw-r--r--   0        0        0      418 2024-05-05 21:39:36.945009 dspygen-2024.5.8/src/dspygen/writer/code_writer.py
+-rw-r--r--   0        0        0     3755 2024-05-05 21:56:54.033929 dspygen-2024.5.8/src/dspygen/writer/data_writer.py
+-rw-r--r--   0        0        0    13936 1970-01-01 00:00:00.000000 dspygen-2024.5.8/PKG-INFO
```

### Comparing `dspygen-2024.5.7/LICENSE` & `dspygen-2024.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/README.md` & `dspygen-2024.5.8/README.md`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/pyproject.toml` & `dspygen-2024.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "dspygen"
-version = "2024.5.7"
+version = "2024.5.8"
 description = "A Ruby on Rails style framework for the DSPy (Demonstrate, Search, Predict) project for Language Models like GPT, BERT, and LLama."
 authors = ["Sean Chatman <info@chatmangpt.com>"]
 readme = "README.md"
 repository = "https://github.com/seanchatmangpt/dspygen"
 
 [tool.poetry.scripts]  # https://python-poetry.org/docs/pyproject/#scripts
 dspygen = "dspygen.cli:app"
```

### Comparing `dspygen-2024.5.7/src/dspygen/4www.py` & `dspygen-2024.5.8/src/dspygen/4www.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/agents/coder_agent.py` & `dspygen-2024.5.8/src/dspygen/agents/coder_agent.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/agents/coder_agent_v2.py` & `dspygen-2024.5.8/src/dspygen/agents/coder_agent_v2.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/agents/coder_agent_v3.py` & `dspygen-2024.5.8/src/dspygen/agents/coder_agent_v3.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/agents/coder_agent_v4.py` & `dspygen-2024.5.8/src/dspygen/agents/coder_agent_v4.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     @trigger(source=CoderAgentState.TESTING_CODE, dest=CoderAgentState.HANDLING_ERRORS, conditions=['errors_detected'])
     def handle_errors(self):
         """Handle errors if any are detected during testing."""
         print("Handling coding errors.")
         self.errors.clear()
 
-    @trigger(source=CoderAgentState.HANDLING_ERRORS, dest=CoderAgentState.REFACTORING_CODE, conditions=['errors_resolved'])
+    @trigger(source=[CoderAgentState.TESTING_CODE, CoderAgentState.HANDLING_ERRORS], dest=CoderAgentState.REFACTORING_CODE, conditions=['errors_resolved'])
     def refactor_code(self):
         """Refactor code after errors are resolved."""
         self.code = "# Added by refactoring\n" + self.code
         print("Code after refactoring:\n", self.code)
         os.remove(self.filename)  # Clean up the original file
         self.filename = self.write_code_to_file(self.code)  # Write the refactored code back to disk
 
@@ -82,21 +82,22 @@
     def errors_resolved(self):
         """Check if the errors have been successfully resolved."""
         return len(self.errors) == 0
 
 
 def main():
     from dspygen.utils.dspy_tools import init_ol
+    from dspygen.modules.fsm_trigger_module import fsm_trigger_call
+
     init_ol(max_tokens=3000)
     agent = CoderAgent("Make a request to an API and return the response.")
     print("Initial state:", agent.state)
-    agent.start_coding()
-    agent.test_code()
-    if agent.errors_detected():
-        agent.handle_errors()
-        agent.refactor_code()
-    agent.complete_task()
+
+    fsm_trigger_call("I want you to start coding for me", agent)
+    fsm_trigger_call("I want you to test the code", agent)
+    fsm_trigger_call("I want you to refactor the code", agent)
+    fsm_trigger_call("I want you to complete the task", agent)
     print("Final state:", agent.state)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dspygen-2024.5.7/src/dspygen/agents/pytest_agent.py` & `dspygen-2024.5.8/src/dspygen/agents/pytest_agent.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/agents/research_agent.py` & `dspygen-2024.5.8/src/dspygen/agents/research_agent.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/api.py` & `dspygen-2024.5.8/src/dspygen/api.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/app.py` & `dspygen-2024.5.8/src/dspygen/app.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/async_typer.py` & `dspygen-2024.5.8/src/dspygen/async_typer.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/books/socratic_tutor/src/SUMMARY.md` & `dspygen-2024.5.8/src/dspygen/books/socratic_tutor/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpel_diagrams/mermaid_multi_module_demo.py` & `dspygen-2024.5.8/src/dspygen/bpel_diagrams/mermaid_multi_module_demo.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpel_models/activities.py` & `dspygen-2024.5.8/src/dspygen/bpel_models/activities.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpel_models/correlations.py` & `dspygen-2024.5.8/src/dspygen/bpel_models/correlations.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpel_models/event_handlers.py` & `dspygen-2024.5.8/src/dspygen/bpel_models/event_handlers.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpel_models/fault_handlers.py` & `dspygen-2024.5.8/src/dspygen/bpel_models/fault_handlers.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpel_models/links.py` & `dspygen-2024.5.8/src/dspygen/bpel_models/links.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpel_models/partner_links.py` & `dspygen-2024.5.8/src/dspygen/bpel_models/partner_links.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpel_models/process.py` & `dspygen-2024.5.8/src/dspygen/bpel_models/process.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpel_models/variables.py` & `dspygen-2024.5.8/src/dspygen/bpel_models/variables.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpmn_models/artifacts.py` & `dspygen-2024.5.8/src/dspygen/bpmn_models/artifacts.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpmn_models/connecting_objects.py` & `dspygen-2024.5.8/src/dspygen/bpmn_models/connecting_objects.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpmn_models/events.py` & `dspygen-2024.5.8/src/dspygen/bpmn_models/events.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpmn_models/flow_objects.py` & `dspygen-2024.5.8/src/dspygen/bpmn_models/flow_objects.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpmn_models/gateways.py` & `dspygen-2024.5.8/src/dspygen/bpmn_models/gateways.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpmn_models/other_entities.py` & `dspygen-2024.5.8/src/dspygen/bpmn_models/other_entities.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpmn_models/pools_and_lanes.py` & `dspygen-2024.5.8/src/dspygen/bpmn_models/pools_and_lanes.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/bpmn_models/sub_processes.py` & `dspygen-2024.5.8/src/dspygen/bpmn_models/sub_processes.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/cli.py` & `dspygen-2024.5.8/src/dspygen/cli.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/dsl_dspy_assertion.py` & `dspygen-2024.5.8/src/dspygen/dsl/dsl_dspy_assertion.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/dsl_pipeline_executor.py` & `dspygen-2024.5.8/src/dspygen/dsl/dsl_pipeline_executor.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/dsl_predict_module.py` & `dspygen-2024.5.8/src/dspygen/dsl/dsl_predict_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/dsl_pydantic_models.py` & `dspygen-2024.5.8/src/dspygen/dsl/dsl_pydantic_models.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/dsl_step_module.py` & `dspygen-2024.5.8/src/dspygen/dsl/dsl_step_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/examples/example_pipeline.yaml` & `dspygen-2024.5.8/src/dspygen/dsl/examples/example_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/examples/poem_pipeline.yaml` & `dspygen-2024.5.8/src/dspygen/dsl/examples/poem_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/examples/saltcorn_plugin_generator.yaml` & `dspygen-2024.5.8/src/dspygen/dsl/examples/saltcorn_plugin_generator.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/utils/dsl_language_model_utils.py` & `dspygen-2024.5.8/src/dspygen/dsl/utils/dsl_language_model_utils.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/utils/dsl_lm_module_utils.py` & `dspygen-2024.5.8/src/dspygen/dsl/utils/dsl_lm_module_utils.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/utils/dsl_retrieval_model_utils.py` & `dspygen-2024.5.8/src/dspygen/dsl/utils/dsl_retrieval_model_utils.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/utils/dsl_rm_module_utils.py` & `dspygen-2024.5.8/src/dspygen/dsl/utils/dsl_rm_module_utils.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dsl/utils/dsl_signature_utils.py` & `dspygen-2024.5.8/src/dspygen/dsl/utils/dsl_signature_utils.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/dspygen_app.py` & `dspygen-2024.5.8/src/dspygen/dspygen_app.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/bkgn/chapter_draft.py` & `dspygen-2024.5.8/src/dspygen/experiments/bkgn/chapter_draft.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/bkgn/get_book_files.py` & `dspygen-2024.5.8/src/dspygen/experiments/bkgn/get_book_files.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/bkgn/get_leaf.py` & `dspygen-2024.5.8/src/dspygen/experiments/bkgn/get_leaf.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/bkgn/get_soc_files.py` & `dspygen-2024.5.8/src/dspygen/experiments/bkgn/get_soc_files.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/bkgn/quick_demo.py` & `dspygen-2024.5.8/src/dspygen/experiments/bkgn/quick_demo.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/blog/Tetris_1.md` & `dspygen-2024.5.8/src/dspygen/experiments/blog/Tetris_1.md`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/blog/Tetris_LMStud_Llama3.py` & `dspygen-2024.5.8/src/dspygen/experiments/blog/Tetris_LMStud_Llama3.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/blog/Tetris_groq.py` & `dspygen-2024.5.8/src/dspygen/experiments/blog/Tetris_groq.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/blog/Tetris_groq_llama3_80.py` & `dspygen-2024.5.8/src/dspygen/experiments/blog/Tetris_groq_llama3_80.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/bulk_code_generator/main.py` & `dspygen-2024.5.8/src/dspygen/experiments/bulk_code_generator/main.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/business_patterns_for_devs.py` & `dspygen-2024.5.8/src/dspygen/experiments/business_patterns_for_devs.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/CriticFeedbackGeneratorSignature_pipeline.yaml` & `dspygen-2024.5.8/src/dspygen/experiments/done/CriticFeedbackGeneratorSignature_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/WebsitePRD_pipeline.yaml` & `dspygen-2024.5.8/src/dspygen/experiments/done/WebsitePRD_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/data_pipeline.yaml` & `dspygen-2024.5.8/src/dspygen/experiments/done/data_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/first_step_with_user_input.py` & `dspygen-2024.5.8/src/dspygen/experiments/done/first_step_with_user_input.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/gen_dsl_instances.py` & `dspygen-2024.5.8/src/dspygen/experiments/done/gen_dsl_instances.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/gen_pydantic_class.py` & `dspygen-2024.5.8/src/dspygen/experiments/done/gen_pydantic_class.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/gherkin_parser.py` & `dspygen-2024.5.8/src/dspygen/experiments/done/gherkin_parser.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/lm_call.py` & `dspygen-2024.5.8/src/dspygen/experiments/done/lm_call.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/openai_ror_cli.py` & `dspygen-2024.5.8/src/dspygen/experiments/done/openai_ror_cli.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/python_to_elixir.py` & `dspygen-2024.5.8/src/dspygen/experiments/done/python_to_elixir.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/saltcorn_plugin_generator_output.yaml` & `dspygen-2024.5.8/src/dspygen/experiments/done/saltcorn_plugin_generator_output.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/socket_actor_system.py` & `dspygen-2024.5.8/src/dspygen/experiments/done/socket_actor_system.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/test_openai_ror_cli.py` & `dspygen-2024.5.8/src/dspygen/experiments/done/test_openai_ror_cli.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/two_steps_with_user_input.py` & `dspygen-2024.5.8/src/dspygen/experiments/done/two_steps_with_user_input.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/understand_input_pipeline.yaml` & `dspygen-2024.5.8/src/dspygen/experiments/done/understand_input_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/done/wizard.py` & `dspygen-2024.5.8/src/dspygen/experiments/done/wizard.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/function_calling/Chinook.db` & `dspygen-2024.5.8/src/dspygen/experiments/function_calling/Chinook.db`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/function_calling/function_call.py` & `dspygen-2024.5.8/src/dspygen/experiments/function_calling/function_call.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/function_calling/sql_calling_asserts.py` & `dspygen-2024.5.8/src/dspygen/experiments/function_calling/sql_calling_asserts.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/function_calling/sql_optimization_function.py` & `dspygen-2024.5.8/src/dspygen/experiments/function_calling/sql_optimization_function.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/function_calling/weather_function_calling_asserts.py` & `dspygen-2024.5.8/src/dspygen/experiments/function_calling/weather_function_calling_asserts.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/function_calling/weather_functions.exs` & `dspygen-2024.5.8/src/dspygen/experiments/function_calling/weather_functions.exs`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/mock_gen/auto_pytest_mock_rover.py` & `dspygen-2024.5.8/src/dspygen/experiments/mock_gen/auto_pytest_mock_rover.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/mock_gen/min_example.py` & `dspygen-2024.5.8/src/dspygen/experiments/mock_gen/min_example.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/mock_gen/mipro_example.py` & `dspygen-2024.5.8/src/dspygen/experiments/mock_gen/mipro_example.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/mock_gen/optimized_cot.json` & `dspygen-2024.5.8/src/dspygen/experiments/mock_gen/optimized_cot.json`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/mock_gen/optimized_cot_sig.json` & `dspygen-2024.5.8/src/dspygen/experiments/mock_gen/optimized_cot_sig.json`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/mock_gen/optimized_cot_sig_1715100135.978442.json` & `dspygen-2024.5.8/src/dspygen/experiments/mock_gen/optimized_cot_sig_1715100135.978442.json`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/mock_gen/swe_bench.py` & `dspygen-2024.5.8/src/dspygen/experiments/mock_gen/swe_bench.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 
         hf_official_train = dataset['train']
         hf_official_test = dataset['test']
         official_train = []
         official_test = []
 
         for example in tqdm.tqdm(hf_official_train):
-            print(example)
             issue = f"{example['problem_statement']}\n\n{example['hints_text']}"
             patch = example['patch']
             test_patch = example['test_patch']
 
             official_train.append(dict(issue=issue, patch=patch, test_patch=test_patch))
 
         for example in tqdm.tqdm(hf_official_test):
```

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/mock_gen/swebench_example.py` & `dspygen-2024.5.8/src/dspygen/experiments/mock_gen/swebench_mipro_example.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,55 @@
 import dspy
+from dspy.teleprompt import MIPRO
 
 from dspygen.experiments.mock_gen.swe_bench import SWEBench
 from dspygen.utils.dspy_tools import init_ol
 
 
-class IssueToPatchSignature(dspy.Signature):
-    """Transforms software issues into actionable patches. In the style of a FAANG System Architect interview question solution."""
-    # Input field representing the issue to be addressed
-    issue = dspy.InputField(desc="Detailed description of the software issue.")
-
-    # Output field representing the patch
-    patch = dspy.OutputField(desc="Proposed patch to resolve the issue.")
-
-
 class CoT(dspy.Module):
     def __init__(self):
         super().__init__()
-        self.prog = dspy.ChainOfThought(IssueToPatchSignature)
+        self.prog = dspy.ChainOfThought("issue -> patch")
 
     def forward(self, issue):
         return self.prog(issue=issue)
 
 
 def main():
     """Main function"""
     from dspy.teleprompt import BootstrapFewShot
     # Set up the LM
     lm = init_ol()
 
     # Load the SWE-bench dataset
     swe_bench = SWEBench()
-    swe_bench_trainset, swe_bench_devset = swe_bench.train[:5], swe_bench.dev[:5]
+    swe_bench_trainset, swe_bench_devset = swe_bench.train[:25], swe_bench.dev[:25]
 
     print(swe_bench_trainset)
 
     # Set up the optimizer: we want to "bootstrap" (i.e., self-generate) 4-shot examples of our CoT program.
     config = dict(max_bootstrapped_demos=4, max_labeled_demos=4)
 
     # Define a custom metric for evaluating patches
     def swebench_metric(gold, pred, trace=None):
         # This is a placeholder metric; adjust based on actual evaluation needs
-        if gold.patch == pred.patch:
-            print(f"Gold: {gold.patch} matched with Pred: {pred.patch}")
         return gold.patch == pred.patch
 
-    teleprompter = BootstrapFewShot(metric=swebench_metric, **config)
+    teleprompter = MIPRO(metric=swebench_metric, **config)
     optimized_cot = teleprompter.compile(CoT(), trainset=swe_bench_trainset)
-    from time import time
-    optimized_cot.save(f"optimized_cot_sig_{str(time())}.json")
+    optimized_cot.save("optimized_cot.json")
 
     from dspy.evaluate import Evaluate
 
     # Set up the evaluator, which can be used multiple times.
     evaluate = Evaluate(devset=swe_bench_devset, metric=swebench_metric, num_threads=8, display_progress=True,
                         display_table=0)
 
     # Evaluate our `optimized_cot` program.
     evaluate(optimized_cot)
 
+
     lm.inspect_history(n=1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/module_docstrings/generate_docstring_exec.py` & `dspygen-2024.5.8/src/dspygen/experiments/module_docstrings/generate_docstring_exec.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/pomo_bud/pomo_bud_dsl.yaml` & `dspygen-2024.5.8/src/dspygen/experiments/pomo_bud/pomo_bud_dsl.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/pomo_bud/pomo_bud_models.py` & `dspygen-2024.5.8/src/dspygen/experiments/pomo_bud/pomo_bud_models.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/quiz/quiz_input.py` & `dspygen-2024.5.8/src/dspygen/experiments/quiz/quiz_input.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/quiz/session_data.json` & `dspygen-2024.5.8/src/dspygen/experiments/quiz/session_data.json`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/raga/chat_gpt_rag_retrevier.py` & `dspygen-2024.5.8/src/dspygen/experiments/raga/chat_gpt_rag_retrevier.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/raga/convo_loader.py` & `dspygen-2024.5.8/src/dspygen/experiments/raga/convo_loader.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/api-for-document-management.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/api-for-document-management.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/confirm-signature-placement.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/confirm-signature-placement.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/custom-signing-instructions.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/custom-signing-instructions.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/data_gherkin_pipeline.yaml` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/data_gherkin_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/document-preview.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/document-preview.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/document-upload.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/document-upload.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/drag-and-drop-document-upload.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/drag-and-drop-document-upload.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/email-confirmation-to-sender.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/email-confirmation-to-sender.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/email-link-to-signer.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/email-link-to-signer.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/generate-unique-signing-link.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/generate-unique-signing-link.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/generate_react_code_from_csv.py` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/generate_react_code_from_csv.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/gherkin_pipeline.yaml` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/gherkin_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/hello-world.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/hello-world.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/link-expiration.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/link-expiration.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/mobile-responsive-design.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/mobile-responsive-design.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/retrieve_and_generate_pipeline.py` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/retrieve_and_generate_pipeline.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/signature-capture.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/signature-capture.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/react_code_gen/signature-validation.tsx` & `dspygen-2024.5.8/src/dspygen/experiments/react_code_gen/signature-validation.tsx`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/rfc5545/calendar_cmd.py` & `dspygen-2024.5.8/src/dspygen/experiments/rfc5545/calendar_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/rfc5545/ical_crud.py` & `dspygen-2024.5.8/src/dspygen/experiments/rfc5545/ical_crud.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/rfc5545/ical_models.py` & `dspygen-2024.5.8/src/dspygen/experiments/rfc5545/ical_models.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/rfc5545/ical_workbench.py` & `dspygen-2024.5.8/src/dspygen/experiments/rfc5545/ical_workbench.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/rfc5545/journal_cmd.py` & `dspygen-2024.5.8/src/dspygen/experiments/rfc5545/journal_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/self_coding/interview_processing.py` & `dspygen-2024.5.8/src/dspygen/experiments/self_coding/interview_processing.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/soonify_groq/groq_pydantic.py` & `dspygen-2024.5.8/src/dspygen/experiments/soonify_groq/groq_pydantic.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/soonify_groq/run_groq_soon.py` & `dspygen-2024.5.8/src/dspygen/experiments/soonify_groq/run_groq_soon.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/spider/wiki_spider.py` & `dspygen-2024.5.8/src/dspygen/experiments/spider/wiki_spider.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/state_actor.txt` & `dspygen-2024.5.8/src/dspygen/experiments/state_actor.txt`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/touch.sh` & `dspygen-2024.5.8/src/dspygen/experiments/touch.sh`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/wip/chatgpt_conversation_parser.py` & `dspygen-2024.5.8/src/dspygen/experiments/wip/chatgpt_conversation_parser.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/wip/default_pipeline.yaml` & `dspygen-2024.5.8/src/dspygen/experiments/wip/default_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/wip/models/dsl_project.py` & `dspygen-2024.5.8/src/dspygen/experiments/wip/models/dsl_project.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/wip/one_shot_pipeline.py` & `dspygen-2024.5.8/src/dspygen/experiments/wip/one_shot_pipeline.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/experiments/wip/self_evolving_business_logic.py` & `dspygen-2024.5.8/src/dspygen/experiments/wip/self_evolving_business_logic.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/lm/groq_lm.py` & `dspygen-2024.5.8/src/dspygen/lm/groq_lm.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/lm/ollama_lm.py` & `dspygen-2024.5.8/src/dspygen/lm/ollama_lm.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/btrees/bt_mixin_v2.py` & `dspygen-2024.5.8/src/dspygen/mixin/btrees/bt_mixin_v2.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/btrees/bt_ros_works.py` & `dspygen-2024.5.8/src/dspygen/mixin/btrees/bt_ros_works.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/btrees/bt_super.py` & `dspygen-2024.5.8/src/dspygen/mixin/btrees/bt_super.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/btrees/bt_traffic.py` & `dspygen-2024.5.8/src/dspygen/mixin/btrees/bt_traffic.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/btrees/btree_mixin.py` & `dspygen-2024.5.8/src/dspygen/mixin/btrees/btree_mixin.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/btrees/superhero_activities.dot` & `dspygen-2024.5.8/src/dspygen/mixin/btrees/superhero_activities.dot`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/fsm/employee_onboarding_fsm.py` & `dspygen-2024.5.8/src/dspygen/mixin/fsm/employee_onboarding_fsm.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/fsm/example.py` & `dspygen-2024.5.8/src/dspygen/mixin/fsm/example.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/fsm/fsm_gas.py` & `dspygen-2024.5.8/src/dspygen/mixin/fsm/fsm_gas.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/fsm/fsm_mixin.py` & `dspygen-2024.5.8/src/dspygen/mixin/fsm/fsm_mixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 
 from transitions import Machine
 from transitions.core import State
+from dspygen.modules.fsm_trigger_module import fsm_trigger_call
 
 import functools
 
 
 def trigger(source, dest, conditions=None, unless=None, before=None, after=None, prepare=None):
     def decorator(func):
         if not hasattr(func, '_transitions'):
@@ -51,14 +52,19 @@
 
         return wrapper
 
     return decorator
 
 
 class FSMMixin:
+    def __init__(self):
+        self.states = []
+        self.machine = None
+        self.state = None
+
     def setup_fsm(self, state_enum, initial=None):
         self.states = [State(state.name) for state in state_enum]
 
         if initial is None:
             initial = [state for state in state_enum][0]
 
         self.machine = Machine(model=self, states=self.states, initial=initial, auto_transitions=False)
@@ -82,12 +88,15 @@
     def possible_transitions(self):
         return state_transition_possibilities(self)
 
     def possible_triggers(self):
         # Get possible destination states from the current state
         return self.machine.get_triggers(self.state)
 
+    def prompt(self, prompt, **kwargs):
+        return fsm_trigger_call(prompt, self, **kwargs)
+
 
 def state_transition_possibilities(fsm):
     current_state = fsm.state
     transitions = fsm.machine.get_transitions()
     return [transition.dest for transition in transitions if transition.source == current_state]
```

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/fsm/fsm_renderer.py` & `dspygen-2024.5.8/src/dspygen/mixin/fsm/fsm_renderer.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/fsm/order_processing_fsm.py` & `dspygen-2024.5.8/src/dspygen/mixin/fsm/order_processing_fsm.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/fsm/traffic_light.py` & `dspygen-2024.5.8/src/dspygen/mixin/fsm/traffic_light.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/mixin/hsm/hsm_mixin.py` & `dspygen-2024.5.8/src/dspygen/mixin/hsm/hsm_mixin.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/models/BPMN.yaml` & `dspygen-2024.5.8/src/dspygen/models/BPMN.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/models/CMMN.yaml` & `dspygen-2024.5.8/src/dspygen/models/CMMN.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/models/bpm_plus_domain_models.py` & `dspygen-2024.5.8/src/dspygen/models/bpm_plus_domain_models.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/models/cmmn_shipping.yaml` & `dspygen-2024.5.8/src/dspygen/models/cmmn_shipping.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/models/dmn_shipping.yaml` & `dspygen-2024.5.8/src/dspygen/models/dmn_shipping.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/arch_module.py` & `dspygen-2024.5.8/src/dspygen/modules/arch_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/bill_of_objects_module.py` & `dspygen-2024.5.8/src/dspygen/modules/bill_of_objects_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/binary_output_module.py` & `dspygen-2024.5.8/src/dspygen/modules/binary_output_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/blog_module.py` & `dspygen-2024.5.8/src/dspygen/modules/blog_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/book_appointment_module.py` & `dspygen-2024.5.8/src/dspygen/modules/book_appointment_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/bpmn2_bpel_module.py` & `dspygen-2024.5.8/src/dspygen/modules/bpmn2_bpel_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/business_dev_consultant.py` & `dspygen-2024.5.8/src/dspygen/modules/business_dev_consultant.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/business_requirements.py` & `dspygen-2024.5.8/src/dspygen/modules/business_requirements.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/chat_bot_cli.py` & `dspygen-2024.5.8/src/dspygen/modules/chat_bot_cli.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/chat_bot_module.py` & `dspygen-2024.5.8/src/dspygen/modules/chat_bot_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/checker_module.py` & `dspygen-2024.5.8/src/dspygen/modules/checker_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/choose_function_module.py` & `dspygen-2024.5.8/src/dspygen/modules/choose_function_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/cli_bot_module.py` & `dspygen-2024.5.8/src/dspygen/modules/cli_bot_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/cobol_to_python_module.py` & `dspygen-2024.5.8/src/dspygen/modules/cobol_to_python_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/condition_sufficient_info_module.py` & `dspygen-2024.5.8/src/dspygen/modules/condition_sufficient_info_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/dflss_module.py` & `dspygen-2024.5.8/src/dspygen/modules/dflss_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/dflss_output.txt` & `dspygen-2024.5.8/src/dspygen/modules/dflss_output.txt`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/dspygen_dsl_pipeline.py` & `dspygen-2024.5.8/src/dspygen/modules/dspygen_dsl_pipeline.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/dspygen_module.py` & `dspygen-2024.5.8/src/dspygen/modules/dspygen_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/elite_module.py` & `dspygen-2024.5.8/src/dspygen/modules/elite_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/exam_point_weight_module.py` & `dspygen-2024.5.8/src/dspygen/modules/exam_point_weight_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/faang_module.py` & `dspygen-2024.5.8/src/dspygen/modules/faang_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/faang_sys_arch_nuxt_module.py` & `dspygen-2024.5.8/src/dspygen/modules/faang_sys_arch_nuxt_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/file_name_module.py` & `dspygen-2024.5.8/src/dspygen/modules/file_name_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/function_invoke_module.py` & `dspygen-2024.5.8/src/dspygen/modules/function_invoke_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/gen_cli_module.py` & `dspygen-2024.5.8/src/dspygen/modules/gen_cli_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/gen_dspy_module.py` & `dspygen-2024.5.8/src/dspygen/modules/gen_dspy_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/gen_keyword_arguments_module.py` & `dspygen-2024.5.8/src/dspygen/modules/gen_keyword_arguments_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/gen_message_module.py` & `dspygen-2024.5.8/src/dspygen/modules/gen_message_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/gen_module.py` & `dspygen-2024.5.8/src/dspygen/modules/gen_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/gen_pydantic_class.py` & `dspygen-2024.5.8/src/dspygen/modules/gen_pydantic_class.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/gen_pydantic_instance.py` & `dspygen-2024.5.8/src/dspygen/modules/gen_pydantic_instance.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/gen_pydantic_instance_module.py` & `dspygen-2024.5.8/src/dspygen/modules/gen_pydantic_instance_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/gen_python_primitive.py` & `dspygen-2024.5.8/src/dspygen/modules/gen_python_primitive.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/gen_signature_module.py` & `dspygen-2024.5.8/src/dspygen/modules/gen_signature_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/get_selector_module.py` & `dspygen-2024.5.8/src/dspygen/modules/get_selector_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/gusty_module.py` & `dspygen-2024.5.8/src/dspygen/modules/gusty_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/html_module.py` & `dspygen-2024.5.8/src/dspygen/modules/html_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/insight_tweet_module.py` & `dspygen-2024.5.8/src/dspygen/modules/insight_tweet_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/js_to_fast_api_module.py` & `dspygen-2024.5.8/src/dspygen/modules/js_to_fast_api_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/json_module.py` & `dspygen-2024.5.8/src/dspygen/modules/json_module.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-"""
-
-"""
 import json
+import typing
 from datetime import datetime, timedelta
 
-import dspy
 from pydantic import BaseModel
 
-from dspygen.utils.dspy_tools import init_dspy
-
-import dspy
+from dspygen.utils.dspy_tools import init_dspy, init_ol
 
 import dspy
 
 from dspygen.utils.json_tools import extract
-from dspygen.utils.pydantic_tools import extract_valid_dicts
+
+
+Model = typing.TypeVar('Model', bound='BaseModel')
 
 
 class GenerateJSONFromText(dspy.Signature):
     """
     [INST] Convert provided structured or unstructured text information into a valid JSON object.
     Ensure the conversion process intelligently identifies key-value pairs, lists, and other relevant
     structures from the text and formats them into JSON. This task should be completed by
@@ -55,15 +52,16 @@
 
     # Text information provided by the user, expected to be transformed into JSON format.
     # This can include both structured and unstructured data.
     json_schema = dspy.InputField(desc="JSON schema to validate the JSON object. YOUR RESPONSE MUST ADHERE TO THIS SCHEMA.")
     text_information = dspy.InputField(desc="Text information in structured or unstructured format. To be converted into a JSON object.")
 
     # The output JSON object, as a string, based on the processed text information.
-    json_object = dspy.OutputField(desc="YOUR ONLY OUTPUT IS THE JSON OBJECT. Ensure it adheres to the provided JSON schema. Do not include the schema in the output.")
+    json_object = dspy.OutputField(desc="YOUR ONLY OUTPUT IS THE JSON OBJECT. Ensure it adheres to the provided JSON schema. Do not include the schema in the output.",
+                                   prefix="Only return the JSON object based on the provided text information and schema.\n\n```json\n")
 
 
 # RFC 5545 VEvent
 class VEvent(BaseModel):
     dtstart: str
     dtend: str
     summary: str
@@ -86,40 +84,41 @@
         other.pipe(self.output)
 
         return other
 
     def forward(self, text, schema):
         pred = dspy.Predict(GenerateJSONFromText)
         self.output = pred(json_schema=str(schema), text_information=text).json_object
+        self.output = extract(self.output)
         return self.output
         
     def pipe(self, input_str):
         raise NotImplementedError("Please implement the pipe method for DSL support.")
         # Replace TODO with a keyword from you forward method
         # return self.forward(TODO=input_str)
         # VEvent.
 
 
-def json_call(schema, text):
-    json_mod = JsonModule()
-    return json_mod.forward(schema=schema, text=text)
+def json_call(model: type[Model], text: str) -> Model:
+    """Takes the JSON schema and text and returns the JSON object as a string."""
+    json_module = JsonModule()
+    model_dict = json_module.forward(schema=model.model_json_schema(), text=text)
+    instance = model.model_validate(model_dict)
+    return instance
 
 
 def main():
-    from dspygen.lm.groq_lm import Groq
-    # init_dspy(Groq, 1000, "mixtral-8x7b-32768")
-    init_dspy(Groq, max_tokens=1000, model= "llama3-70b-8192") # for Groq you must pass an Groq provided model
+    init_ol()
     # Create fake data
     import faker
     fake = faker.Faker()
     # text = f"{fake.date_time()} {fake.date_time()}{fake.date_time()} {fake.date_time()}{fake.date_time()} {fake.date_time()}{fake.date_time()} {fake.date_time()}{fake.date_time()} {fake.date_time()} {fake.sentence()} {fake.address()} {fake.text()}"
     # Mock VEvent in confusing email
     text = (f"Hi Jane, I hope you are doing well. I wanted to remind you about our meeting tomorrow at 10:00 AM. "
             f"Today:{datetime.now()} Tomorrow:{datetime.now() + timedelta(days=1)} "
             f"Location: {fake.address()} Description: {fake.text()}")
-    result = json_call(schema=VEvent.model_json_schema(), text=text)
-    res_dict = extract(result)
-    print(VEvent.model_validate_json(json.dumps(res_dict)))
+    result = json_call(VEvent, text=text)
+    print(result)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `dspygen-2024.5.7/src/dspygen/modules/jsx_module.py` & `dspygen-2024.5.8/src/dspygen/modules/jsx_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/long_form_qa_module.py` & `dspygen-2024.5.8/src/dspygen/modules/long_form_qa_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/md_book_summarizer_module.py` & `dspygen-2024.5.8/src/dspygen/modules/md_book_summarizer_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/mermaid_js_module.py` & `dspygen-2024.5.8/src/dspygen/modules/mermaid_js_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/message_module.py` & `dspygen-2024.5.8/src/dspygen/modules/message_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/module_docstring_module.py` & `dspygen-2024.5.8/src/dspygen/modules/module_docstring_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/product_bot_module.py` & `dspygen-2024.5.8/src/dspygen/modules/product_bot_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/prompt_function_call_module.py` & `dspygen-2024.5.8/src/dspygen/modules/prompt_function_call_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/pytest_module.py` & `dspygen-2024.5.8/src/dspygen/modules/pytest_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/python_expert_module.py` & `dspygen-2024.5.8/src/dspygen/modules/python_expert_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/python_source_code_module.py` & `dspygen-2024.5.8/src/dspygen/modules/python_source_code_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/pyts_module.py` & `dspygen-2024.5.8/src/dspygen/modules/pyts_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/query_generator_module.py` & `dspygen-2024.5.8/src/dspygen/modules/query_generator_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/rails_code_module.py` & `dspygen-2024.5.8/src/dspygen/modules/rails_code_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/react_jsx_module.py` & `dspygen-2024.5.8/src/dspygen/modules/react_jsx_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/refine_results_module.py` & `dspygen-2024.5.8/src/dspygen/modules/refine_results_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/request_contract_module.py` & `dspygen-2024.5.8/src/dspygen/modules/request_contract_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/signature_factory.py` & `dspygen-2024.5.8/src/dspygen/modules/signature_factory.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/signature_renderer.py` & `dspygen-2024.5.8/src/dspygen/modules/signature_renderer.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/source_code_pep8_docs_module.py` & `dspygen-2024.5.8/src/dspygen/modules/source_code_pep8_docs_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/source_selector_module.py` & `dspygen-2024.5.8/src/dspygen/modules/source_selector_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/sql_query_module.py` & `dspygen-2024.5.8/src/dspygen/modules/sql_query_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/streamlit_bot_module.py` & `dspygen-2024.5.8/src/dspygen/modules/streamlit_bot_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/subject_destination_audience_newsletter_article_module.py` & `dspygen-2024.5.8/src/dspygen/modules/subject_destination_audience_newsletter_article_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/success_planner_module.py` & `dspygen-2024.5.8/src/dspygen/modules/success_planner_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/tax_return_agent.py` & `dspygen-2024.5.8/src/dspygen/modules/tax_return_agent.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/test.py` & `dspygen-2024.5.8/src/dspygen/modules/test.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/test_chat_bot_cli.py` & `dspygen-2024.5.8/src/dspygen/modules/test_chat_bot_cli.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/text_summary_module_module.py` & `dspygen-2024.5.8/src/dspygen/modules/text_summary_module_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/to_elixir_module.py` & `dspygen-2024.5.8/src/dspygen/modules/to_elixir_module.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/modules/usp_connect_ship_webhook.py` & `dspygen-2024.5.8/src/dspygen/modules/usp_connect_ship_webhook.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/pages/mqtt_page.py` & `dspygen-2024.5.8/src/dspygen/pages/mqtt_page.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/prototypes/state_chat/hello_world_convo_agent.py` & `dspygen-2024.5.8/src/dspygen/prototypes/state_chat/hello_world_convo_agent.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/prototypes/state_chat/socrates_convo.py` & `dspygen-2024.5.8/src/dspygen/prototypes/state_chat/socrates_convo.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/actor_system.py` & `dspygen-2024.5.8/src/dspygen/rdddy/actor_system.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/base_actor.py` & `dspygen-2024.5.8/src/dspygen/rdddy/base_actor.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/base_aggregate.py` & `dspygen-2024.5.8/src/dspygen/rdddy/base_aggregate.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/base_message.py` & `dspygen-2024.5.8/src/dspygen/rdddy/base_message.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/base_policy.py` & `dspygen-2024.5.8/src/dspygen/rdddy/base_policy.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/base_repository.py` & `dspygen-2024.5.8/src/dspygen/rdddy/base_repository.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/base_saga.py` & `dspygen-2024.5.8/src/dspygen/rdddy/base_saga.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/browser/browser_domain.py` & `dspygen-2024.5.8/src/dspygen/rdddy/browser/browser_domain.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/browser/browser_process_supervisor.py` & `dspygen-2024.5.8/src/dspygen/rdddy/browser/browser_process_supervisor.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/browser/browser_worker.py` & `dspygen-2024.5.8/src/dspygen/rdddy/browser/browser_worker.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/event_storm_domain_specification_model.py` & `dspygen-2024.5.8/src/dspygen/rdddy/event_storm_domain_specification_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pydantic import BaseModel, Field
 
 from dspygen.modules.gen_pydantic_instance_module import GenPydanticInstance
-from dspygen.utils.dspy_tools import init_dspy
+from dspygen.utils.dspy_tools import init_dspy, init_ol
+
 
 class EventStormingDomainSpecificationModel(BaseModel):
     """Integrates Event Storming with RDDDY and DFLSS to capture and analyze domain complexities through events, commands,
     and queries, using Hoare logic for correctness. It serves as a repository for interactions identified in
     Event Storming, enhancing system responsiveness and process efficiency. This model educates on designing and
     verifying systems aligned with domain requirements and operational excellence. CamelCase only.
     """
@@ -85,23 +86,28 @@
 
 requirements = """The project must integrated the shippiing labels produced by USP ConnectShip shipping station with the certification number generated by the decision tree questionnaire.
 
 At the time of the shipping lable being produced, the event should halt moving to the next screen of the lable pritning process and invoke the browser.  The browser loads order specific questionnariere described as a decision tree and allow technician t provide answers about the order being packaed.
 
 Once the questionnaire is complete, the browser s closed, the questionnare cerificate id be posted and included to be printed to shipping label.
 
-The decision tree selection is based on types of products in the order and should be managed / created by business analysts."""
-
+The decision tree selection is based on types of products in the order and should be managed / created by business analysts.
 
-def main():
-    init_dspy(model="gpt-4")
+"""
 
-    pred = GenPydanticInstance(root_model=EventStormingDomainSpecificationModel)
 
-    model = pred(requirements)
+def main():
+    # init_ol(model="llama3")
+    init_ol()
 
-    print(model)
+    from dspygen.modules.gen_pydantic_instance import instance
+    inst = instance(EventStormingDomainSpecificationModel, requirements)
+    print(inst)
+
+    # from dspygen.modules.json_module import json_call
+    # mdl = json_call(EventStormingDomainSpecificationModel, requirements)
+    # print(mdl)
 
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `dspygen-2024.5.7/src/dspygen/rdddy/event_storm_model.py` & `dspygen-2024.5.8/src/dspygen/rdddy/event_storm_model.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rm/chatgpt_chromadb_retriever.py` & `dspygen-2024.5.8/src/dspygen/rm/chatgpt_chromadb_retriever.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rm/chatgpt_string_retriever.py` & `dspygen-2024.5.8/src/dspygen/rm/chatgpt_string_retriever.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rm/chroma_retriever.py` & `dspygen-2024.5.8/src/dspygen/rm/chroma_retriever.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rm/code_retriever.py` & `dspygen-2024.5.8/src/dspygen/rm/code_retriever.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rm/data_retriever.py` & `dspygen-2024.5.8/src/dspygen/rm/data_retriever.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rm/doc_retriever.py` & `dspygen-2024.5.8/src/dspygen/rm/doc_retriever.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/rm/python_code_retriever.py` & `dspygen-2024.5.8/src/dspygen/rm/python_code_retriever.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/signatures/signature.yaml` & `dspygen-2024.5.8/src/dspygen/signatures/signature.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/signatures/signature_dsl.py` & `dspygen-2024.5.8/src/dspygen/signatures/signature_dsl.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/actor_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/actor_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/assert_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/assert_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/browser_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/browser_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/cmd_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/cmd_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/code_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/code_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/help.txt` & `dspygen-2024.5.8/src/dspygen/subcommands/help.txt`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/help_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/help_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/lm_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/lm_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/module_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/module_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/pln_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/pln_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/rm_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/rm_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/sig_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/sig_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/temp_assert.py` & `dspygen-2024.5.8/src/dspygen/subcommands/temp_assert.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/wkf_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/wkf_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/subcommands/wrt_cmd.py` & `dspygen-2024.5.8/src/dspygen/subcommands/wrt_cmd.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/templates/actor_template.j2` & `dspygen-2024.5.8/src/dspygen/templates/actor_template.j2`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/touch_models.sh` & `dspygen-2024.5.8/src/dspygen/touch_models.sh`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/__init__.py` & `dspygen-2024.5.8/src/dspygen/typetemp/__init__.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/environment/typed_environment.py` & `dspygen-2024.5.8/src/dspygen/typetemp/environment/typed_environment.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/environment/typed_native_environment.py` & `dspygen-2024.5.8/src/dspygen/typetemp/environment/typed_native_environment.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/extension/faker_extension.py` & `dspygen-2024.5.8/src/dspygen/typetemp/extension/faker_extension.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/extension/inflection_extension.py` & `dspygen-2024.5.8/src/dspygen/typetemp/extension/inflection_extension.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/functional.py` & `dspygen-2024.5.8/src/dspygen/typetemp/functional.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/template/async_render_mixin.py` & `dspygen-2024.5.8/src/dspygen/typetemp/template/async_render_mixin.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/template/dsl_project.py` & `dspygen-2024.5.8/src/dspygen/typetemp/template/dsl_project.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/template/render_funcs.py` & `dspygen-2024.5.8/src/dspygen/typetemp/template/render_funcs.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/template/render_mixin.py` & `dspygen-2024.5.8/src/dspygen/typetemp/template/render_mixin.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/template/smart_template.py` & `dspygen-2024.5.8/src/dspygen/typetemp/template/smart_template.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/template/typed_injector.py` & `dspygen-2024.5.8/src/dspygen/typetemp/template/typed_injector.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/template/typed_prompt.py` & `dspygen-2024.5.8/src/dspygen/typetemp/template/typed_prompt.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/template/typed_python_source.py` & `dspygen-2024.5.8/src/dspygen/typetemp/template/typed_python_source.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/typetemp/template/typed_template.py` & `dspygen-2024.5.8/src/dspygen/typetemp/template/typed_template.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/cli_tools.py` & `dspygen-2024.5.8/src/dspygen/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/complete.py` & `dspygen-2024.5.8/src/dspygen/utils/complete.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/compression_tools.py` & `dspygen-2024.5.8/src/dspygen/utils/compression_tools.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/create_prompts.py` & `dspygen-2024.5.8/src/dspygen/utils/create_prompts.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/crud_tools.py` & `dspygen-2024.5.8/src/dspygen/utils/crud_tools.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/date_tools.py` & `dspygen-2024.5.8/src/dspygen/utils/date_tools.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/dspy_tools.py` & `dspygen-2024.5.8/src/dspygen/utils/dspy_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         return lm_instance
     else:
         lm = lm_class( max_tokens=max_tokens, model=model)
         dspy.settings.configure(lm=lm)
         return lm
 
 
-def init_ol(lm_class=dspy.OllamaLocal, model: str = "llama3", max_tokens: int = 800, lm_instance=None):
+def init_ol(lm_class=dspy.OllamaLocal, model: str = "phi3:instruct", max_tokens: int = 800, lm_instance=None):
     if lm_instance:
         dspy.settings.configure(lm=lm_instance)
         return lm_instance
     else:
         lm = lm_class(model=model, max_tokens=max_tokens)
         dspy.settings.configure(lm=lm)
         return lm
```

### Comparing `dspygen-2024.5.7/src/dspygen/utils/file_tools.py` & `dspygen-2024.5.8/src/dspygen/utils/file_tools.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/json_tools.py` & `dspygen-2024.5.8/src/dspygen/utils/json_tools.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/models.py` & `dspygen-2024.5.8/src/dspygen/utils/models.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/module_tools.py` & `dspygen-2024.5.8/src/dspygen/utils/module_tools.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/pydantic_tools.py` & `dspygen-2024.5.8/src/dspygen/utils/pydantic_tools.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/scraping_tools.py` & `dspygen-2024.5.8/src/dspygen/utils/scraping_tools.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/utils/yaml_tools.py` & `dspygen-2024.5.8/src/dspygen/utils/yaml_tools.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/workflow/control_flow_workflow.yaml` & `dspygen-2024.5.8/src/dspygen/workflow/control_flow_workflow.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/workflow/control_flow_workflow_output_new.yaml` & `dspygen-2024.5.8/src/dspygen/workflow/control_flow_workflow_output_new.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/workflow/data_analysis_workflow.yaml` & `dspygen-2024.5.8/src/dspygen/workflow/data_analysis_workflow.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/workflow/data_preparation_workflow.yaml` & `dspygen-2024.5.8/src/dspygen/workflow/data_preparation_workflow.yaml`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/workflow/workflow_engine.py` & `dspygen-2024.5.8/src/dspygen/workflow/workflow_engine.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/workflow/workflow_executor.py` & `dspygen-2024.5.8/src/dspygen/workflow/workflow_executor.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/workflow/workflow_models.py` & `dspygen-2024.5.8/src/dspygen/workflow/workflow_models.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/workflow/workflow_router.py` & `dspygen-2024.5.8/src/dspygen/workflow/workflow_router.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/src/dspygen/writer/data_writer.py` & `dspygen-2024.5.8/src/dspygen/writer/data_writer.py`

 * *Files identical despite different names*

### Comparing `dspygen-2024.5.7/PKG-INFO` & `dspygen-2024.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspygen
-Version: 2024.5.7
+Version: 2024.5.8
 Summary: A Ruby on Rails style framework for the DSPy (Demonstrate, Search, Predict) project for Language Models like GPT, BERT, and LLama.
 Home-page: https://github.com/seanchatmangpt/dspygen
 Author: Sean Chatman
 Author-email: info@chatmangpt.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

