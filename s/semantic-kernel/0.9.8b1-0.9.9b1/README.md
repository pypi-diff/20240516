# Comparing `tmp/semantic_kernel-0.9.8b1.tar.gz` & `tmp/semantic_kernel-0.9.9b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.9.8b1.tar", max compression
+gzip compressed data, was "semantic_kernel-0.9.9b1.tar", max compression
```

## Comparing `semantic_kernel-0.9.8b1.tar` & `semantic_kernel-0.9.9b1.tar`

### file list

```diff
@@ -1,217 +1,232 @@
--rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-0.9.8b1/pip/README.md
--rw-r--r--   0        0        0     5406 2024-05-09 23:07:37.255180 semantic_kernel-0.9.8b1/pyproject.toml
--rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/__init__.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     3223 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0      437 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0     7538 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/function_call_behavior.py
--rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/__init__.py
--rw-r--r--   0        0        0     1795 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
--rw-r--r--   0        0        0     9646 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
--rw-r--r--   0        0        0     3821 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
--rw-r--r--   0        0        0     2191 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
--rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     1169 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
--rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
--rw-r--r--   0        0        0     6662 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2119 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/__init__.py
--rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
--rw-r--r--   0        0        0     8403 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
--rw-r--r--   0        0        0     3962 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
--rw-r--r--   0        0        0     1805 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
--rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/utils.py
--rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0      246 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/const.py
--rw-r--r--   0        0        0     2464 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/contents/function_call.py
--rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
--rw-r--r--   0        0        0     3817 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
--rw-r--r--   0        0        0     4147 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
--rw-r--r--   0        0        0    16094 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     5364 2024-03-20 18:24:28.763758 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
--rw-r--r--   0        0        0     8276 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     4815 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     4731 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0    19477 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
--rw-r--r--   0        0        0     3719 2024-03-20 18:24:28.763758 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
--rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
--rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
--rw-r--r--   0        0        0     4797 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     6342 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
--rw-r--r--   0        0        0     3016 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
--rw-r--r--   0        0        0     2908 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/utils.py
--rw-r--r--   0        0        0     3908 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/prompt_execution_settings.py
--rw-r--r--   0        0        0     1720 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/__init__.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/__init__.py
--rw-r--r--   0        0        0     6718 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/astra_client.py
--rw-r--r--   0        0        0    11819 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
--rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/utils.py
--rw-r--r--   0        0        0      242 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0    15787 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      213 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
--rw-r--r--   0        0        0    10299 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
--rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
--rw-r--r--   0        0        0     1592 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
--rw-r--r--   0        0        0    13020 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
--rw-r--r--   0        0        0      159 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0    12786 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
--rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
--rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    14991 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    20518 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
--rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/README.md
--rw-r--r--   0        0        0      178 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/__init__.py
--rw-r--r--   0        0        0    15281 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
--rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/utils.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/usearch/__init__.py
--rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
--rw-r--r--   0        0        0      188 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/weaviate/__init__.py
--rw-r--r--   0        0        0    11001 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/__init__.py
--rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
--rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
--rw-r--r--   0        0        0     1011 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/openai_utils.py
--rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openapi_plugin/__init__.py
--rw-r--r--   0        0        0     1241 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
--rw-r--r--   0        0        0    13518 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
--rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     2648 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-0.9.8b1/semantic_kernel/connectors/telemetry.py
--rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/connectors/utils/__init__.py
--rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/connectors/utils/document_loader.py
--rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/__init__.py
--rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/author_role.py
--rw-r--r--   0        0        0    13781 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/chat_history.py
--rw-r--r--   0        0        0    12276 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/chat_message_content.py
--rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/const.py
--rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/contents/finish_reason.py
--rw-r--r--   0        0        0     3729 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/function_call_content.py
--rw-r--r--   0        0        0     3913 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/function_result_content.py
--rw-r--r--   0        0        0      772 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/kernel_content.py
--rw-r--r--   0        0        0    11084 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_chat_message_content.py
--rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_content_mixin.py
--rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_text_content.py
--rw-r--r--   0        0        0     1957 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/text_content.py
--rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/types.py
--rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/__init__.py
--rw-r--r--   0        0        0     3452 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/conversation_summary_plugin.py
--rw-r--r--   0        0        0     4069 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/http_plugin.py
--rw-r--r--   0        0        0     2474 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/math_plugin.py
--rw-r--r--   0        0        0     5868 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/README.md
--rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
--rw-r--r--   0        0        0     9409 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
--rw-r--r--   0        0        0     1106 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
--rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
--rw-r--r--   0        0        0     3783 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/text_memory_plugin.py
--rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/text_plugin.py
--rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/time_plugin.py
--rw-r--r--   0        0        0     1163 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/wait_plugin.py
--rw-r--r--   0        0        0     1789 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/web_search_engine_plugin.py
--rw-r--r--   0        0        0      316 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/events/__init__.py
--rw-r--r--   0        0        0     2068 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/events/function_invoked_event_args.py
--rw-r--r--   0        0        0     1420 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/events/function_invoking_event_args.py
--rw-r--r--   0        0        0     1725 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/events/kernel_events_args.py
--rw-r--r--   0        0        0      537 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/__init__.py
--rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/content_exceptions.py
--rw-r--r--   0        0        0     1176 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/function_exceptions.py
--rw-r--r--   0        0        0     1319 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/kernel_exceptions.py
--rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/planner_exceptions.py
--rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/service_exceptions.py
--rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/template_engine_exceptions.py
--rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/functions/__init__.py
--rw-r--r--   0        0        0     2455 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/function_result.py
--rw-r--r--   0        0        0     1601 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_arguments.py
--rw-r--r--   0        0        0     9539 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function.py
--rw-r--r--   0        0        0     5517 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_decorator.py
--rw-r--r--   0        0        0     7585 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_from_method.py
--rw-r--r--   0        0        0    17568 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_from_prompt.py
--rw-r--r--   0        0        0     1912 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_metadata.py
--rw-r--r--   0        0        0      559 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_parameter_metadata.py
--rw-r--r--   0        0        0    23557 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_plugin.py
--rw-r--r--   0        0        0      791 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/prompt_rendering_result.py
--rw-r--r--   0        0        0      260 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/types.py
--rw-r--r--   0        0        0    41973 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/kernel.py
--rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/kernel_pydantic.py
--rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6521 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     3619 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/planners/__init__.py
--rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
--rw-r--r--   0        0        0    11592 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
--rw-r--r--   0        0        0     1675 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
--rw-r--r--   0        0        0      928 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
--rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
--rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
--rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/planners/plan.py
--rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/planners/planner_extensions.py
--rw-r--r--   0        0        0      592 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/planners/planner_options.py
--rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
--rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
--rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/__init__.py
--rw-r--r--   0        0        0     5899 2024-05-09 23:07:37.275180 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner.py
--rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
--rw-r--r--   0        0        0     4720 2024-05-09 23:07:37.275180 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0        0        0     4987 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
--rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/__init__.py
--rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/const.py
--rw-r--r--   0        0        0     4128 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/handlebars_prompt_template.py
--rw-r--r--   0        0        0      340 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/input_variable.py
--rw-r--r--   0        0        0     4750 2024-05-09 23:07:37.275180 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/jinja2_prompt_template.py
--rw-r--r--   0        0        0     7935 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/kernel_prompt_template.py
--rw-r--r--   0        0        0      623 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/prompt_template_base.py
--rw-r--r--   0        0        0     4762 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/prompt_template_config.py
--rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/__init__.py
--rw-r--r--   0        0        0     4585 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
--rw-r--r--   0        0        0     2476 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
--rw-r--r--   0        0        0     1701 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/template_function_helpers.py
--rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/py.typed
--rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/services/__init__.py
--rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/services/ai_service_client_base.py
--rw-r--r--   0        0        0     2648 2024-05-09 23:07:37.275180 semantic_kernel-0.9.8b1/semantic_kernel/services/ai_service_selector.py
--rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     7402 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/named_arg_block.py
--rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/utils/chat.py
--rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/utils/logging.py
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/utils/naming.py
--rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0    12623 2024-05-09 23:07:37.275180 semantic_kernel-0.9.8b1/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 semantic_kernel-0.9.8b1/PKG-INFO
+-rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-0.9.9b1/pip/README.md
+-rw-r--r--   0        0        0     5410 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     3250 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0      437 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0     7538 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/function_call_behavior.py
+-rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/__init__.py
+-rw-r--r--   0        0        0     1795 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
+-rw-r--r--   0        0        0    10535 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
+-rw-r--r--   0        0        0     4676 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
+-rw-r--r--   0        0        0     3118 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
+-rw-r--r--   0        0        0     1866 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py
+-rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     1169 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
+-rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
+-rw-r--r--   0        0        0     6683 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2119 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/__init__.py
+-rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
+-rw-r--r--   0        0        0     8451 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
+-rw-r--r--   0        0        0     3983 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
+-rw-r--r--   0        0        0     1805 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
+-rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/utils.py
+-rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/const.py
+-rw-r--r--   0        0        0     2464 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/contents/function_call.py
+-rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
+-rw-r--r--   0        0        0     3817 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
+-rw-r--r--   0        0        0     4147 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
+-rw-r--r--   0        0        0    11081 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     5364 2024-03-20 18:24:28.763758 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
+-rw-r--r--   0        0        0     6087 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     6075 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     3614 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0    19750 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
+-rw-r--r--   0        0        0     3719 2024-03-20 18:24:28.763758 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
+-rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
+-rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
+-rw-r--r--   0        0        0     3823 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     6363 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
+-rw-r--r--   0        0        0     3663 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
+-rw-r--r--   0        0        0     2908 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/utils.py
+-rw-r--r--   0        0        0     4169 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py
+-rw-r--r--   0        0        0     2060 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py
+-rw-r--r--   0        0        0     3908 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/prompt_execution_settings.py
+-rw-r--r--   0        0        0     1741 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/__init__.py
+-rw-r--r--   0        0        0     6718 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/astra_client.py
+-rw-r--r--   0        0        0    13347 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
+-rw-r--r--   0        0        0      735 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/astradb_settings.py
+-rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/utils.py
+-rw-r--r--   0        0        0      383 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0     1160 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py
+-rw-r--r--   0        0        0    16963 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      345 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
+-rw-r--r--   0        0        0    11118 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
+-rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
+-rw-r--r--   0        0        0      538 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py
+-rw-r--r--   0        0        0     1592 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
+-rw-r--r--   0        0        0    13020 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      560 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/memory_settings_base.py
+-rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
+-rw-r--r--   0        0        0      336 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0    13131 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
+-rw-r--r--   0        0        0      518 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py
+-rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
+-rw-r--r--   0        0        0      309 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    15618 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0      460 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py
+-rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      300 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    21145 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      494 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/postgres/postgres_settings.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/README.md
+-rw-r--r--   0        0        0      276 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/__init__.py
+-rw-r--r--   0        0        0    15880 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
+-rw-r--r--   0        0        0      486 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/redis_settings.py
+-rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/utils.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/usearch/__init__.py
+-rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
+-rw-r--r--   0        0        0      298 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/weaviate/__init__.py
+-rw-r--r--   0        0        0    12496 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      908 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py
+-rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
+-rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
+-rw-r--r--   0        0        0     1011 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/openai_utils.py
+-rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openapi_plugin/__init__.py
+-rw-r--r--   0        0        0     1268 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
+-rw-r--r--   0        0        0    28989 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
+-rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     3425 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0     1165 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/bing_connector_settings.py
+-rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-0.9.9b1/semantic_kernel/connectors/telemetry.py
+-rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/connectors/utils/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/connectors/utils/document_loader.py
+-rw-r--r--   0        0        0      123 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/const.py
+-rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/__init__.py
+-rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/author_role.py
+-rw-r--r--   0        0        0    14167 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/chat_history.py
+-rw-r--r--   0        0        0    12594 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/chat_message_content.py
+-rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/const.py
+-rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/contents/finish_reason.py
+-rw-r--r--   0        0        0     4032 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/function_call_content.py
+-rw-r--r--   0        0        0     4509 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/function_result_content.py
+-rw-r--r--   0        0        0      772 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/kernel_content.py
+-rw-r--r--   0        0        0    10964 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_chat_message_content.py
+-rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_content_mixin.py
+-rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_text_content.py
+-rw-r--r--   0        0        0     2011 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/text_content.py
+-rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/types.py
+-rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3452 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/conversation_summary_plugin.py
+-rw-r--r--   0        0        0     4069 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/http_plugin.py
+-rw-r--r--   0        0        0     2474 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/math_plugin.py
+-rw-r--r--   0        0        0     5812 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/README.md
+-rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
+-rw-r--r--   0        0        0     9954 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
+-rw-r--r--   0        0        0     1919 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
+-rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
+-rw-r--r--   0        0        0     3783 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/text_memory_plugin.py
+-rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/text_plugin.py
+-rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/time_plugin.py
+-rw-r--r--   0        0        0     1163 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/wait_plugin.py
+-rw-r--r--   0        0        0     1789 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/web_search_engine_plugin.py
+-rw-r--r--   0        0        0      316 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/events/__init__.py
+-rw-r--r--   0        0        0     2068 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/events/function_invoked_event_args.py
+-rw-r--r--   0        0        0     1420 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/events/function_invoking_event_args.py
+-rw-r--r--   0        0        0     1725 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/events/kernel_events_args.py
+-rw-r--r--   0        0        0      626 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/__init__.py
+-rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/content_exceptions.py
+-rw-r--r--   0        0        0     1176 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/function_exceptions.py
+-rw-r--r--   0        0        0     1319 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/kernel_exceptions.py
+-rw-r--r--   0        0        0      467 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/memory_connector_exceptions.py
+-rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/planner_exceptions.py
+-rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/service_exceptions.py
+-rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/template_engine_exceptions.py
+-rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/functions/__init__.py
+-rw-r--r--   0        0        0     2455 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/functions/function_result.py
+-rw-r--r--   0        0        0     1750 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_arguments.py
+-rw-r--r--   0        0        0     9648 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function.py
+-rw-r--r--   0        0        0     6170 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_decorator.py
+-rw-r--r--   0        0        0     8258 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_from_method.py
+-rw-r--r--   0        0        0    17761 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_from_prompt.py
+-rw-r--r--   0        0        0     1991 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_metadata.py
+-rw-r--r--   0        0        0      559 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_parameter_metadata.py
+-rw-r--r--   0        0        0    24196 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_plugin.py
+-rw-r--r--   0        0        0      791 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/functions/prompt_rendering_result.py
+-rw-r--r--   0        0        0      260 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/functions/types.py
+-rw-r--r--   0        0        0    42096 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/kernel_pydantic.py
+-rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6521 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3619 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/planners/__init__.py
+-rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
+-rw-r--r--   0        0        0    11604 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
+-rw-r--r--   0        0        0     1675 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
+-rw-r--r--   0        0        0      928 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
+-rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
+-rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
+-rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/planners/plan.py
+-rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/planners/planner_extensions.py
+-rw-r--r--   0        0        0      592 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/planners/planner_options.py
+-rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     5978 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     4720 2024-05-09 23:07:37.275180 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     4987 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/const.py
+-rw-r--r--   0        0        0     4760 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/handlebars_prompt_template.py
+-rw-r--r--   0        0        0      893 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/input_variable.py
+-rw-r--r--   0        0        0     4945 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/jinja2_prompt_template.py
+-rw-r--r--   0        0        0     6785 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/kernel_prompt_template.py
+-rw-r--r--   0        0        0     2991 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/prompt_template_base.py
+-rw-r--r--   0        0        0     5586 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/prompt_template_config.py
+-rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/__init__.py
+-rw-r--r--   0        0        0     4592 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
+-rw-r--r--   0        0        0     2483 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
+-rw-r--r--   0        0        0     1894 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/template_function_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/py.typed
+-rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/services/__init__.py
+-rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/services/ai_service_client_base.py
+-rw-r--r--   0        0        0     2648 2024-05-09 23:07:37.275180 semantic_kernel-0.9.9b1/semantic_kernel/services/ai_service_selector.py
+-rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     7474 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/named_arg_block.py
+-rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/utils/chat.py
+-rw-r--r--   0        0        0      838 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/utils/experimental_decorator.py
+-rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/utils/logging.py
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/utils/naming.py
+-rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     5104 1970-01-01 00:00:00.000000 semantic_kernel-0.9.9b1/PKG-INFO
```

### Comparing `semantic_kernel-0.9.8b1/pip/README.md` & `semantic_kernel-0.9.9b1/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/pyproject.toml` & `semantic_kernel-0.9.9b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.9.8b1"
+version = "0.9.9b1"
 description = "Semantic Kernel Python SDK"
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.13"
@@ -20,19 +20,19 @@
 ]
 grpcio = [
     { version = ">=1.40.0", python = "3.8" },
     { version = ">=1.50.0", python = ">=3.9" },
     { version = ">=1.60.0", python = ">=3.12" }
 ]
 openai = ">=1.0"
-python-dotenv = "^1.0.1"
 regex = "^2023.6.3"
 openapi_core = ">=0.18,<0.20"
 prance = "^23.6.21.0"
 pydantic = "^2"
+pydantic-settings = "^2.2.1"
 motor = "^3.3.2"
 defusedxml = "^0.7.1"
 pybars4 = "^0.9.13"
 jinja2 = "^3.1.3"
 nest-asyncio = "^1.6.0"
 eval_type_backport = { version = "^0.1.3", markers = "python_version < '3.10'" }
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     from semantic_kernel.contents.chat_history import ChatHistory
     from semantic_kernel.contents.chat_message_content import ChatMessageContent
     from semantic_kernel.contents.streaming_chat_message_content import StreamingChatMessageContent
 
 
 class ChatCompletionClientBase(AIServiceClientBase, ABC):
     @abstractmethod
-    async def complete_chat(
+    async def get_chat_message_contents(
         self,
         chat_history: "ChatHistory",
         settings: "PromptExecutionSettings",
         **kwargs: Any,
     ) -> list["ChatMessageContent"]:
         """
         This is the method that is called from the kernel to get a response from a chat-optimized LLM.
@@ -32,15 +32,15 @@
 
         Returns:
             Union[str, List[str]] -- A string or list of strings representing the response(s) from the LLM.
         """
         pass
 
     @abstractmethod
-    def complete_chat_stream(
+    def get_streaming_chat_message_contents(
         self,
         chat_history: "ChatHistory",
         settings: "PromptExecutionSettings",
         **kwargs: Any,
     ) -> AsyncGenerator[list["StreamingChatMessageContent"], Any]:
         """
         This is the method that is called from the kernel to get a stream response from a chat-optimized LLM.
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/function_call_behavior.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/function_call_behavior.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-import sys
-from typing import Any, List, Optional, Tuple
-
-if sys.version_info >= (3, 9):
-    from typing import Annotated
-else:
-    from typing_extensions import Annotated
+from typing import Annotated, Any, List, Tuple
 
 import google.generativeai as palm
 from google.generativeai.types import ChatResponse, MessageDict
-from pydantic import PrivateAttr, StringConstraints
+from pydantic import PrivateAttr, StringConstraints, ValidationError
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
 from semantic_kernel.connectors.ai.google_palm.gp_prompt_execution_settings import (
     GooglePalmChatPromptExecutionSettings,
     GooglePalmPromptExecutionSettings,
 )
+from semantic_kernel.connectors.ai.google_palm.settings.google_palm_settings import GooglePalmSettings
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
 from semantic_kernel.contents.author_role import AuthorRole
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
 from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import ServiceInvalidRequestError, ServiceResponseException
@@ -29,40 +24,58 @@
 logger: logging.Logger = logging.getLogger(__name__)
 
 int_to_role = {1: AuthorRole.USER, 2: AuthorRole.SYSTEM, 3: AuthorRole.ASSISTANT, 4: AuthorRole.TOOL}
 
 
 class GooglePalmChatCompletion(ChatCompletionClientBase, TextCompletionClientBase):
     api_key: Annotated[str, StringConstraints(strip_whitespace=True, min_length=1)]
-    _message_history: Optional[ChatHistory] = PrivateAttr()
-    service_id: Optional[str] = None
+    _message_history: ChatHistory | None = PrivateAttr()
+    service_id: str | None = None
 
     def __init__(
         self,
         ai_model_id: str,
-        api_key: str,
-        message_history: Optional[ChatHistory] = None,
+        api_key: str | None = None,
+        message_history: ChatHistory | None = None,
+        env_file_path: str | None = None,
     ):
         """
         Initializes a new instance of the GooglePalmChatCompletion class.
 
         Arguments:
             ai_model_id {str} -- GooglePalm model name, see
                 https://developers.generativeai.google/models/language
-            api_key {str} -- GooglePalm API key, see
-                https://developers.generativeai.google/products/palm
-            message_history {Optional[ChatHistory]} -- The message history to use for context. (Optional)
-        """
+            api_key {str | None} -- The optional API key to use. If not provided, will be read from either
+                the env vars or the .env settings file
+            message_history {ChatHistory | None} -- The message history to use for context. (Optional)
+            env_file_path {str | None} -- Use the environment settings file as a fallback to
+                environment variables. (Optional)
+        """
+        google_palm_settings = None
+        try:
+            google_palm_settings = GooglePalmSettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.warning(f"Error loading Google Palm pydantic settings: {e}")
+
+        api_key = api_key or (
+            google_palm_settings.api_key.get_secret_value()
+            if google_palm_settings and google_palm_settings.api_key
+            else None
+        )
+        ai_model_id = ai_model_id or (
+            google_palm_settings.chat_model_id if google_palm_settings and google_palm_settings.chat_model_id else None
+        )
+
         super().__init__(
             ai_model_id=ai_model_id,
             api_key=api_key,
         )
         self._message_history = message_history
 
-    async def complete_chat(
+    async def get_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: GooglePalmPromptExecutionSettings,
         **kwargs: Any,
     ) -> List[ChatMessageContent]:
         """
         This is the method that is called from the kernel to get a response from a chat-optimized LLM.
@@ -105,23 +118,23 @@
             inner_content=response,
             ai_model_id=self.ai_model_id,
             metadata=metadata,
             role=int_to_role[int(candidate.get("author"))],  # TODO: why is author coming back as '1'?
             content=candidate.get("content"),
         )
 
-    async def complete_chat_stream(
+    async def get_streaming_chat_message_contents(
         self,
         messages: List[Tuple[str, str]],
         settings: GooglePalmPromptExecutionSettings,
         **kwargs: Any,
     ):
         raise NotImplementedError("Google Palm API does not currently support streaming")
 
-    async def complete(
+    async def get_text_contents(
         self,
         prompt: str,
         settings: GooglePalmPromptExecutionSettings,
     ) -> List[TextContent]:
         """
         This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
@@ -152,15 +165,15 @@
         return TextContent(
             inner_content=response,
             ai_model_id=self.ai_model_id,
             metadata=metadata,
             text=candidate.get("content"),
         )
 
-    async def complete_stream(
+    async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: GooglePalmPromptExecutionSettings,
     ):
         raise NotImplementedError("Google Palm API does not currently support streaming")
 
     async def _send_chat_request(
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,97 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-import sys
-from typing import List
+from abc import ABC
+from typing import List, Union
 
-if sys.version_info >= (3, 9):
-    from typing import Annotated
-else:
-    from typing_extensions import Annotated
-
-import google.generativeai as palm
-from google.generativeai.types import Completion
-from google.generativeai.types.text_types import TextCompletion
-from pydantic import StringConstraints
-
-from semantic_kernel.connectors.ai.google_palm.gp_prompt_execution_settings import GooglePalmTextPromptExecutionSettings
-from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
-from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
-from semantic_kernel.contents.text_content import TextContent
+from numpy import array, ndarray
+from openai import AsyncOpenAI, AsyncStream, BadRequestError
+from openai.types import Completion
+from openai.types.chat import ChatCompletion, ChatCompletionChunk
+
+from semantic_kernel.connectors.ai.open_ai.exceptions.content_filter_ai_exception import (
+    ContentFilterAIException,
+)
+from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
+    OpenAIEmbeddingPromptExecutionSettings,
+    OpenAIPromptExecutionSettings,
+)
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_model_types import (
+    OpenAIModelTypes,
+)
 from semantic_kernel.exceptions import ServiceResponseException
+from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-class GooglePalmTextCompletion(TextCompletionClientBase):
-    api_key: Annotated[str, StringConstraints(strip_whitespace=True, min_length=1)]
+class OpenAIHandler(KernelBaseModel, ABC):
+    """Internal class for calls to OpenAI API's."""
 
-    def __init__(self, ai_model_id: str, api_key: str):
-        """
-        Initializes a new instance of the GooglePalmTextCompletion class.
-
-        Arguments:
-            ai_model_id {str} -- GooglePalm model name, see
-                https://developers.generativeai.google/models/language
-            api_key {str} -- GooglePalm API key, see
-                https://developers.generativeai.google/products/palm
-        """
-        super().__init__(ai_model_id=ai_model_id, api_key=api_key)
+    client: AsyncOpenAI
+    ai_model_type: OpenAIModelTypes = OpenAIModelTypes.CHAT
+    prompt_tokens: int = 0
+    completion_tokens: int = 0
+    total_tokens: int = 0
 
-    async def complete(self, prompt: str, settings: GooglePalmTextPromptExecutionSettings) -> List[TextContent]:
+    async def _send_request(
+        self,
+        request_settings: OpenAIPromptExecutionSettings,
+    ) -> Union[ChatCompletion, Completion, AsyncStream[ChatCompletionChunk], AsyncStream[Completion]]:
         """
-        This is the method that is called from the kernel to get a response from a text-optimized LLM.
+        Completes the given prompt. Returns a single string completion.
+        Cannot return multiple completions. Cannot return logprobs.
 
         Arguments:
-            prompt {str} -- The prompt to send to the LLM.
-            settings {GooglePalmTextPromptExecutionSettings} -- Settings for the request.
+            prompt {str} -- The prompt to complete.
+            messages {List[Tuple[str, str]]} -- A list of tuples, where each tuple is a role and content set.
+            request_settings {OpenAIPromptExecutionSettings} -- The request settings.
+            stream {bool} -- Whether to stream the response.
 
         Returns:
-            List[TextContent] -- A list of TextContent objects representing the response(s) from the LLM.
+            ChatCompletion, Completion, AsyncStream[Completion | ChatCompletionChunk] -- The completion response.
         """
-        settings.prompt = prompt
-        if not settings.ai_model_id:
-            settings.ai_model_id = self.ai_model_id
+
         try:
-            palm.configure(api_key=self.api_key)
+            if self.ai_model_type == OpenAIModelTypes.CHAT:
+                response = await self.client.chat.completions.create(**request_settings.prepare_settings_dict())
+            else:
+                response = await self.client.completions.create(**request_settings.prepare_settings_dict())
+            self.store_usage(response)
+            return response
+        except BadRequestError as ex:
+            if ex.code == "content_filter":
+                raise ContentFilterAIException(
+                    f"{type(self)} service encountered a content error",
+                    ex,
+                )
+            raise ServiceResponseException(
+                f"{type(self)} service failed to complete the prompt",
+                ex,
+            ) from ex
         except Exception as ex:
-            raise PermissionError(
-                "Google PaLM service failed to configure. Invalid API key provided.",
+            raise ServiceResponseException(
+                f"{type(self)} service failed to complete the prompt",
                 ex,
-            )
+            ) from ex
+
+    async def _send_embedding_request(self, settings: OpenAIEmbeddingPromptExecutionSettings) -> List[ndarray]:
         try:
-            response = palm.generate_text(**settings.prepare_settings_dict())
+            response = await self.client.embeddings.create(**settings.prepare_settings_dict())
+            self.store_usage(response)
+            # make numpy arrays from the response
+            # TODO: the openai response is cast to a list[float], could be used instead of ndarray
+            return [array(x.embedding) for x in response.data]
         except Exception as ex:
             raise ServiceResponseException(
-                "Google PaLM service failed to complete the prompt",
+                f"{type(self)} service failed to generate embeddings",
                 ex,
             ) from ex
-        return [self._create_text_content(response, candidate) for candidate in response.candidates]
-
-    def _create_text_content(self, response: Completion, candidate: TextCompletion) -> TextContent:
-        """Create a text content object from a candidate."""
-        return TextContent(
-            inner_content=response,
-            ai_model_id=self.ai_model_id,
-            text=candidate.get("output"),
-            metadata={
-                "filters": response.filters,
-                "safety_feedback": response.safety_feedback,
-                "citation_metadata": candidate.get("citation_metadata"),
-                "safety_ratings": candidate.get("safety_ratings"),
-            },
-        )
 
-    async def complete_stream(
-        self,
-        prompt: str,
-        settings: GooglePalmTextPromptExecutionSettings,
-    ):
-        raise NotImplementedError("Google Palm API does not currently support streaming")
-
-    def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
-        """Create a request settings object."""
-        return GooglePalmTextPromptExecutionSettings
+    def store_usage(self, response):
+        if not isinstance(response, AsyncStream):
+            logger.info(f"OpenAI usage: {response.usage}")
+            self.prompt_tokens += response.usage.prompt_tokens
+            self.total_tokens += response.usage.total_tokens
+            if hasattr(response.usage, "completion_tokens"):
+                self.completion_tokens += response.usage.completion_tokens
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-
-import sys
-from typing import Any, List
-
-if sys.version_info >= (3, 9):
-    from typing import Annotated
-else:
-    from typing_extensions import Annotated
+import logging
+from typing import Annotated, Any, List
 
 import google.generativeai as palm
 from numpy import array, ndarray
-from pydantic import StringConstraints
+from pydantic import StringConstraints, ValidationError
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
+from semantic_kernel.connectors.ai.google_palm.settings.google_palm_settings import GooglePalmSettings
 from semantic_kernel.exceptions import ServiceInvalidAuthError, ServiceResponseException
 
+logger: logging.Logger = logging.getLogger(__name__)
+
 
 class GooglePalmTextEmbedding(EmbeddingGeneratorBase):
     api_key: Annotated[str, StringConstraints(strip_whitespace=True, min_length=1)]
 
-    def __init__(self, ai_model_id: str, api_key: str) -> None:
+    def __init__(self, ai_model_id: str, api_key: str | None = None, env_file_path: str | None = None) -> None:
         """
         Initializes a new instance of the GooglePalmTextEmbedding class.
 
         Arguments:
             ai_model_id {str} -- GooglePalm model name, see
-            https://developers.generativeai.google/models/language
-            api_key {str} -- GooglePalm API key, see
-            https://developers.generativeai.google/products/palm
+                https://developers.generativeai.google/models/language
+            api_key {str | None} -- The optional API key to use. If not provided, will be
+                read from either the env vars or the .env settings file.
+            env_file_path {str | None} -- Use the environment settings file
+                as a fallback to environment variables. (Optional)
         """
+        try:
+            google_palm_settings = GooglePalmSettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.error(f"Error loading Google Palm pydantic settings: {e}")
+
+        api_key = api_key or (
+            google_palm_settings.api_key.get_secret_value()
+            if google_palm_settings and google_palm_settings.api_key
+            else None
+        )
+        ai_model_id = ai_model_id or (
+            google_palm_settings.embedding_model_id
+            if google_palm_settings and google_palm_settings.embedding_model_id
+            else None
+        )
         super().__init__(ai_model_id=ai_model_id, api_key=api_key)
 
     async def generate_embeddings(self, texts: List[str], **kwargs: Any) -> ndarray:
         """
         Generates embeddings for a list of texts.
 
         Arguments:
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             service_id=service_id,
             ai_model_id=ai_model_id,
             task=task,
             device=(f"cuda:{device}" if device >= 0 and torch.cuda.is_available() else "cpu"),
             generator=generator,
         )
 
-    async def complete(
+    async def get_text_contents(
         self,
         prompt: str,
         settings: HuggingFacePromptExecutionSettings,
     ) -> List[TextContent]:
         """
         This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
@@ -99,15 +99,15 @@
     def _create_text_content(self, response: Any, candidate: Dict[str, str]) -> TextContent:
         return TextContent(
             inner_content=response,
             ai_model_id=self.ai_model_id,
             text=candidate["summary_text" if self.task == "summarization" else "generated_text"],
         )
 
-    async def complete_stream(
+    async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: HuggingFacePromptExecutionSettings,
     ) -> AsyncGenerator[List[StreamingTextContent], Any]:
         """
         Streams a text completion using a Hugging Face model.
         Note that this method does not support multiple responses.
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         url {Optional[Union[str, HttpUrl]]} -- URL of the Ollama server, defaults to http://localhost:11434/api/chat
         session {Optional[aiohttp.ClientSession]} -- Optional client session to use for requests.
     """
 
     url: HttpUrl = "http://localhost:11434/api/chat"
     session: Optional[aiohttp.ClientSession] = None
 
-    async def complete_chat(
+    async def get_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: OllamaChatPromptExecutionSettings,
         **kwargs: Any,
     ) -> List[ChatMessageContent]:
         """
         This is the method that is called from the kernel to get a response from a chat-optimized LLM.
@@ -66,15 +66,15 @@
                         inner_content=response_object,
                         ai_model_id=self.ai_model_id,
                         role="assistant",
                         content=response_object.get("message", {"content": None}).get("content", None),
                     )
                 ]
 
-    async def complete_chat_stream(
+    async def get_streaming_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: OllamaChatPromptExecutionSettings,
         **kwargs: Any,
     ) -> AsyncGenerator[List[StreamingChatMessageContent], Any]:
         """
         Streams a text completion using a Ollama model.
@@ -108,15 +108,15 @@
                             ai_model_id=self.ai_model_id,
                             content=body.get("message", {"content": None}).get("content", None),
                         )
                     ]
                     if body.get("done"):
                         break
 
-    async def complete(
+    async def get_text_contents(
         self,
         prompt: str,
         settings: OllamaChatPromptExecutionSettings,
     ) -> List[TextContent]:
         """
         This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
@@ -139,15 +139,15 @@
                     TextContent(
                         inner_content=response_object,
                         ai_model_id=self.ai_model_id,
                         text=response_object.get("message", {"content": None}).get("content", None),
                     )
                 ]
 
-    async def complete_stream(
+    async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: OllamaChatPromptExecutionSettings,
     ) -> AsyncGenerator[List[StreamingTextContent], Any]:
         """
         Streams a text completion using a Ollama model.
         Note that this method does not support multiple responses.
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         ai_model_id {str} -- Ollama model name, see https://ollama.ai/library
         url {Optional[Union[str, HttpUrl]]} -- URL of the Ollama server, defaults to http://localhost:11434/api/generate
     """
 
     url: HttpUrl = "http://localhost:11434/api/generate"
     session: Optional[aiohttp.ClientSession] = None
 
-    async def complete(
+    async def get_text_contents(
         self,
         prompt: str,
         settings: OllamaTextPromptExecutionSettings,
     ) -> List[TextContent]:
         """
         This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
@@ -52,15 +52,15 @@
         async with AsyncSession(self.session) as session:
             async with session.post(self.url, json=settings.prepare_settings_dict()) as response:
                 response.raise_for_status()
                 inner_content = await response.json()
                 text = inner_content["response"]
                 return [TextContent(inner_content=inner_content, ai_model_id=self.ai_model_id, text=text)]
 
-    async def complete_stream(
+    async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: OllamaTextPromptExecutionSettings,
     ) -> AsyncGenerator[List[StreamingTextContent], Any]:
         """
         Streams a text completion using a Ollama model.
         Note that this method does not support multiple responses,
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/contents/function_call.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/contents/function_call.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,117 +1,136 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 
 import logging
-from typing import Dict, Mapping, Optional, overload
+from typing import Mapping
 
 from openai import AsyncAzureOpenAI
 from openai.lib.azure import AsyncAzureADTokenProvider
+from pydantic import ValidationError
 
 from semantic_kernel.connectors.ai.open_ai.const import DEFAULT_AZURE_API_VERSION
 from semantic_kernel.connectors.ai.open_ai.services.azure_config_base import (
     AzureOpenAIConfigBase,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
     OpenAIModelTypes,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding_base import (
     OpenAITextEmbeddingBase,
 )
+from semantic_kernel.connectors.ai.open_ai.settings.azure_open_ai_settings import AzureOpenAISettings
+from semantic_kernel.exceptions.service_exceptions import ServiceInitializationError
+from semantic_kernel.kernel_pydantic import HttpsUrl
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class AzureTextEmbedding(AzureOpenAIConfigBase, OpenAITextEmbeddingBase):
     """Azure Text Embedding class."""
 
-    @overload
     def __init__(
         self,
-        deployment_name: str,
-        async_client: AsyncAzureOpenAI,
-        service_id: Optional[str] = None,
+        service_id: str | None = None,
+        api_key: str | None = None,
+        deployment_name: str | None = None,
+        endpoint: str | None = None,
+        base_url: str | None = None,
+        api_version: str | None = None,
+        ad_token: str | None = None,
+        ad_token_provider: AsyncAzureADTokenProvider | None = None,
+        default_headers: Mapping[str, str] | None = None,
+        async_client: AsyncAzureOpenAI | None = None,
+        env_file_path: str | None = None,
     ) -> None:
         """
-        Initialize an AzureChatCompletion service.
+        Initialize an AzureTextEmbedding service.
 
-        Arguments:
-            deployment_name: The name of the Azure deployment. This value
-                will correspond to the custom name you chose for your deployment
-                when you deployed a model. This value can be found under
-                Resource Management > Deployments in the Azure portal or, alternatively,
-                under Management > Deployments in Azure OpenAI Studio.
-            async_client {AsyncAzureOpenAI} -- An existing client to use.
-        """
+        service_id: The service ID. (Optional)
+        api_key  {str | None}: The optional api key. If provided, will override the value in the
+                env vars or .env file.
+        deployment_name  {str | None}: The optional deployment. If provided, will override the value
+            (text_deployment_name) in the env vars or .env file.
+        endpoint {str | None}: The optional deployment endpoint. If provided will override the value
+            in the env vars or .env file.
+        base_url {str | None}: The optional deployment base_url. If provided will override the value
+            in the env vars or .env file.
+        api_version {str | None}: The optional deployment api version. If provided will override the value
+            in the env vars or .env file.
+        ad_token {str | None}: The Azure AD token for authentication. (Optional)
+        ad_auth {AsyncAzureADTokenProvider | None}: Whether to use Azure Active Directory authentication.
+            (Optional) The default value is False.
+        default_headers: The default headers mapping of string keys to
+                string values for HTTP requests. (Optional)
+        async_client {Optional[AsyncAzureOpenAI]} -- An existing client to use. (Optional)
+        env_file_path {str | None} -- Use the environment settings file as a fallback to
+            environment variables. (Optional)
+        """
+        azure_openai_settings = None
+        try:
+            azure_openai_settings = AzureOpenAISettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.warning(f"Failed to load AzureOpenAI pydantic settings: {e}")
 
-    def __init__(
-        self,
-        deployment_name: str,
-        endpoint: Optional[str] = None,
-        api_version: str = DEFAULT_AZURE_API_VERSION,
-        service_id: Optional[str] = None,
-        api_key: Optional[str] = None,
-        ad_token: Optional[str] = None,
-        ad_token_provider: Optional[AsyncAzureADTokenProvider] = None,
-        default_headers: Optional[Mapping[str, str]] = None,
-        async_client: Optional[AsyncAzureOpenAI] = None,
-    ) -> None:
-        """
-        Initialize an AzureTextEmbedding service.
+        base_url = base_url or (
+            str(azure_openai_settings.base_url) if azure_openai_settings and azure_openai_settings.base_url else None
+        )
+        endpoint = endpoint or (
+            str(azure_openai_settings.endpoint) if azure_openai_settings and azure_openai_settings.endpoint else None
+        )
+        deployment_name = deployment_name or (
+            azure_openai_settings.embedding_deployment_name if azure_openai_settings else None
+        )
+        api_version = api_version or (azure_openai_settings.api_version if azure_openai_settings else None)
+        api_key = api_key or (
+            azure_openai_settings.api_key.get_secret_value()
+            if azure_openai_settings and azure_openai_settings.api_key
+            else None
+        )
 
-        You must provide:
-        - A deployment_name, endpoint, and api_key (plus, optionally: ad_auth)
+        if api_version is None:
+            api_version = DEFAULT_AZURE_API_VERSION
 
-        :param deployment_name: The name of the Azure deployment. This value
-            will correspond to the custom name you chose for your deployment
-            when you deployed a model. This value can be found under
-            Resource Management > Deployments in the Azure portal or, alternatively,
-            under Management > Deployments in Azure OpenAI Studio.
-        :param endpoint: The endpoint of the Azure deployment. This value
-            can be found in the Keys & Endpoint section when examining
-            your resource from the Azure portal.
-        :param api_version: The API version to use. (Optional)
-            The default value is "2023-05-15".
-        :param api_key: The API key for the Azure deployment. This value can be
-            found in the Keys & Endpoint section when examining your resource in
-            the Azure portal. You can use either KEY1 or KEY2.
-        :param ad_token : The Azure AD token for authentication. (Optional)
-        :param ad_auth: Whether to use Azure Active Directory authentication.
-            (Optional) The default value is False.
-        :param default_headers: The default headers mapping of string keys to
-            string values for HTTP requests. (Optional)
-        :param async_client: An existing client to use. (Optional)
+        if not base_url and not endpoint:
+            raise ServiceInitializationError("At least one of base_url or endpoint must be provided.")
+
+        if base_url and isinstance(base_url, str):
+            base_url = HttpsUrl(base_url)
+        if endpoint and deployment_name:
+            base_url = HttpsUrl(f"{str(endpoint).rstrip('/')}/openai/deployments/{deployment_name}")
 
-        """
         super().__init__(
             deployment_name=deployment_name,
-            endpoint=endpoint,
+            endpoint=endpoint if not isinstance(endpoint, str) else HttpsUrl(endpoint),
+            base_url=base_url,
             api_version=api_version,
             service_id=service_id,
             api_key=api_key,
             ad_token=ad_token,
             ad_token_provider=ad_token_provider,
             default_headers=default_headers,
             ai_model_type=OpenAIModelTypes.EMBEDDING,
             async_client=async_client,
         )
 
     @classmethod
-    def from_dict(cls, settings: Dict[str, str]) -> "AzureTextEmbedding":
+    def from_dict(cls, settings: dict[str, str]) -> "AzureTextEmbedding":
         """
         Initialize an Azure OpenAI service from a dictionary of settings.
 
         Arguments:
             settings: A dictionary of settings for the service.
                 should contains keys: deployment_name, endpoint, api_key
                 and optionally: api_version, ad_auth
         """
         return AzureTextEmbedding(
-            deployment_name=settings["deployment_name"],
-            endpoint=settings["endpoint"],
-            api_key=settings["api_key"],
-            api_version=settings.get("api_version", DEFAULT_AZURE_API_VERSION),
             service_id=settings.get("service_id"),
+            api_key=settings.get("api_key", None),
+            deployment_name=settings.get("deployment_name", None),
+            endpoint=settings.get("endpoint", None),
+            base_url=settings.get("base_url", None),
+            api_version=settings.get("api_version", None),
             ad_token=settings.get("ad_token"),
             ad_token_provider=settings.get("ad_token_provider"),
             default_headers=settings.get("default_headers"),
+            env_file_path=settings.get("env_file_path", None),
         )
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # most of the methods are overridden from the ChatCompletionClientBase class, otherwise it is mentioned
 
     # override from AIServiceClientBase
     def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
         """Create a request settings object."""
         return OpenAIChatPromptExecutionSettings
 
-    async def complete_chat(
+    async def get_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: OpenAIChatPromptExecutionSettings,
         **kwargs: Any,
     ) -> List["ChatMessageContent"]:
         """Executes a chat completion request and returns the result.
 
@@ -96,15 +96,15 @@
             ):
                 return completions
             await self._process_chat_response_with_tool_call(
                 completions=completions, chat_history=chat_history, kernel=kernel, arguments=arguments
             )
             settings = self._prepare_settings(settings, chat_history, stream_request=False, kernel=kernel)
 
-    async def complete_chat_stream(
+    async def get_streaming_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: OpenAIChatPromptExecutionSettings,
         **kwargs: Any,
     ) -> AsyncGenerator[List[StreamingChatMessageContent], Any]:
         """Executes a streaming chat completion request and returns the result.
 
@@ -420,16 +420,21 @@
             )
             chat_history.add_message(message=frc.to_chat_message_content())
             return
         logger.info(f"Calling {func.name} function with args: {func.arguments}")
         try:
             func_result = await kernel.invoke(**func.split_name_dict(), arguments=args_cloned)
         except Exception as exc:
-            logger.exception(f"Error occurred while invoking function {func.name}")
-            raise ServiceInvalidResponseError(f"Error occurred while invoking function {func.name}") from exc
+            logger.exception(f"Exception occurred while invoking function {func.name}, exception: {exc}")
+            frc = FunctionResultContent.from_function_call_content_and_result(
+                function_call_content=result,
+                result=f"Exception occurred while invoking function {func.name}, exception: {exc}",
+            )
+            chat_history.add_message(message=frc.to_chat_message_content())
+            return
         frc = FunctionResultContent.from_function_call_content_and_result(
             function_call_content=result, result=func_result
         )
         chat_history.add_message(message=frc.to_chat_message_content())
 
 
 # endregion
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,115 +1,73 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
 import logging
-from typing import Dict, Mapping, Optional, overload
+from typing import Dict, Mapping, Optional
 
 from openai import AsyncOpenAI
+from pydantic import ValidationError
 
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_config_base import (
     OpenAIConfigBase,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
     OpenAIModelTypes,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_completion_base import (
     OpenAITextCompletionBase,
 )
+from semantic_kernel.connectors.ai.open_ai.settings.open_ai_settings import OpenAISettings
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class OpenAITextCompletion(OpenAITextCompletionBase, OpenAIConfigBase):
     """OpenAI Text Completion class."""
 
-    @overload
     def __init__(
         self,
-        ai_model_id: str,
-        async_client: AsyncOpenAI,
-        service_id: Optional[str] = None,
-    ) -> None:
-        """
-        Initialize an OpenAITextCompletion service.
-
-        Arguments:
-            ai_model_id {str} -- OpenAI model name, see
-                https://platform.openai.com/docs/models
-            async_client {AsyncOpenAI} -- An existing client to use.
-        """
-
-    @overload
-    def __init__(
-        self,
-        ai_model_id: str,
-        api_key: Optional[str] = None,
-        org_id: Optional[str] = None,
-        service_id: Optional[str] = None,
-        default_headers: Optional[Mapping[str, str]] = None,
-    ) -> None:
-        """
-        Initialize an OpenAITextCompletion service.
-
-        Arguments:
-            ai_model_id {str} -- OpenAI model name, see
-                https://platform.openai.com/docs/models
-            api_key {Optional[str]} -- OpenAI API key, see
-                https://platform.openai.com/account/api-keys (Optional)
-            org_id {Optional[str]} -- OpenAI organization ID.
-                This is usually optional unless your
-                account belongs to multiple organizations.
-            default_headers: The default headers mapping of string keys to
-                string values for HTTP requests. (Optional)
-        """
-
-    @overload
-    def __init__(
-        self,
-        ai_model_id: str,
-        api_key: Optional[str] = None,
-        service_id: Optional[str] = None,
-        default_headers: Optional[Mapping[str, str]] = None,
-    ) -> None:
-        """
-        Initialize an OpenAITextCompletion service.
-
-        Arguments:
-            ai_model_id {str} -- OpenAI model name, see
-                https://platform.openai.com/docs/models
-            api_key {Optional[str]} -- OpenAI API key, see
-                https://platform.openai.com/account/api-keys (Optional)
-            default_headers: The default headers mapping of string keys to
-                string values for HTTP requests. (Optional)
-        """
-
-    def __init__(
-        self,
-        ai_model_id: str,
-        api_key: Optional[str] = None,
-        org_id: Optional[str] = None,
+        ai_model_id: str | None = None,
+        api_key: str | None = None,
+        org_id: str | None = None,
         service_id: Optional[str] = None,
         default_headers: Optional[Mapping[str, str]] = None,
         async_client: Optional[AsyncOpenAI] = None,
+        env_file_path: str | None = None,
     ) -> None:
         """
         Initialize an OpenAITextCompletion service.
 
         Arguments:
-            ai_model_id {str} -- OpenAI model name, see
+            ai_model_id {str | None} -- OpenAI model name, see
                 https://platform.openai.com/docs/models
-            api_key {Optional[str]} -- OpenAI API key, see
-                https://platform.openai.com/account/api-keys (Optional)
-            org_id {Optional[str]} -- OpenAI organization ID.
-                This is usually optional unless your
-                account belongs to multiple organizations.
+            service_id {str | None} -- Service ID tied to the execution settings.
+            api_key {str | None} -- The optional API key to use. If provided will override,
+                the env vars or .env file value.
+            org_id {str | None} -- The optional org ID to use. If provided will override,
+                the env vars or .env file value.
             default_headers: The default headers mapping of string keys to
                 string values for HTTP requests. (Optional)
             async_client {Optional[AsyncOpenAI]} -- An existing client to use. (Optional)
+            env_file_path {str | None} -- Use the environment settings file as a fallback to
+                environment variables. (Optional)
         """
+        try:
+            openai_settings = OpenAISettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.warning(f"Failed to load OpenAI pydantic settings: {e}")
+
+        api_key = api_key or (
+            openai_settings.api_key.get_secret_value() if openai_settings and openai_settings.api_key else None
+        )
+        org_id = org_id or (openai_settings.org_id if openai_settings and openai_settings.org_id else None)
+        ai_model_id = ai_model_id or (
+            openai_settings.text_model_id if openai_settings and openai_settings.text_model_id else None
+        )
+
         super().__init__(
             ai_model_id=ai_model_id,
             api_key=api_key,
             org_id=org_id,
             service_id=service_id,
             ai_model_type=OpenAIModelTypes.TEXT,
             default_headers=default_headers,
@@ -123,13 +81,14 @@
 
         Arguments:
             settings: A dictionary of settings for the service.
         """
         if "default_headers" in settings and isinstance(settings["default_headers"], str):
             settings["default_headers"] = json.loads(settings["default_headers"])
         return OpenAITextCompletion(
-            ai_model_id=settings["ai_model_id"],
-            api_key=settings["api_key"],
-            org_id=settings.get("org_id"),
+            ai_model_id=settings.get("ai_model_id", None),
+            api_key=settings.get("api_key", None),
+            org_id=settings.get("org_id", None),
             service_id=settings.get("service_id"),
             default_headers=settings.get("default_headers"),
+            env_file_path=settings.get("env_file_path", None),
         )
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 class OpenAITextCompletionBase(OpenAIHandler, TextCompletionClientBase):
     def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
         """Create a request settings object."""
         return OpenAITextPromptExecutionSettings
 
-    async def complete(
+    async def get_text_contents(
         self,
         prompt: str,
         settings: "OpenAIPromptExecutionSettings",
     ) -> List["TextContent"]:
         """Executes a completion request and returns the result.
 
         Arguments:
@@ -68,15 +68,15 @@
         return TextContent(
             inner_content=response,
             ai_model_id=self.ai_model_id,
             text=text,
             metadata=choice_metadata,
         )
 
-    async def complete_stream(
+    async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: "OpenAIPromptExecutionSettings",
     ) -> AsyncGenerator[List["StreamingTextContent"], Any]:
         """
         Executes a completion request and streams the result.
         Supports both chat completion and text completion.
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Dict, Mapping, Optional, overload
+from typing import Dict, Mapping, Optional
 
 from openai import AsyncOpenAI
+from pydantic import ValidationError
 
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_config_base import (
     OpenAIConfigBase,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
     OpenAIModelTypes,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding_base import (
     OpenAITextEmbeddingBase,
 )
+from semantic_kernel.connectors.ai.open_ai.settings.open_ai_settings import OpenAISettings
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class OpenAITextEmbedding(OpenAIConfigBase, OpenAITextEmbeddingBase):
     """OpenAI Text Embedding class."""
 
-    @overload
     def __init__(
         self,
         ai_model_id: str,
-        async_client: AsyncOpenAI,
-        service_id: Optional[str] = None,
-    ) -> None:
-        """
-        Initialize an OpenAITextEmbedding service.
-
-        Arguments:
-            ai_model_id {str} -- OpenAI model name, see
-                https://platform.openai.com/docs/models
-            async_client {AsyncOpenAI} -- An existing client to use.
-        """
-
-    def __init__(
-        self,
-        ai_model_id: str,
-        api_key: Optional[str] = None,
-        org_id: Optional[str] = None,
+        api_key: str | None = None,
+        org_id: str | None = None,
         service_id: Optional[str] = None,
         default_headers: Optional[Mapping[str, str]] = None,
         async_client: Optional[AsyncOpenAI] = None,
+        env_file_path: str | None = None,
     ) -> None:
         """
         Initializes a new instance of the OpenAITextCompletion class.
 
         Arguments:
             ai_model_id {str} -- OpenAI model name, see
                 https://platform.openai.com/docs/models
-            api_key {str} -- OpenAI API key, see
-                https://platform.openai.com/account/api-keys
-            org_id {Optional[str]} -- OpenAI organization ID.
-                This is usually optional unless your
-                account belongs to multiple organizations.
+            service_id {str | None} -- Service ID tied to the execution settings.
+            api_key {str | None} -- The optional API key to use. If provided will override,
+                the env vars or .env file value.
+            org_id {str | None} -- The optional org ID to use. If provided will override,
+                the env vars or .env file value.
             default_headers {Optional[Mapping[str,str]]}: The default headers mapping of string keys to
                 string values for HTTP requests. (Optional)
             async_client {Optional[AsyncOpenAI]} -- An existing client to use. (Optional)
+            env_file_path {str | None} -- Use the environment settings file as
+                a fallback to environment variables. (Optional)
         """
+        try:
+            openai_settings = OpenAISettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.warning(f"Failed to load OpenAI pydantic settings: {e}")
+
+        api_key = api_key or (
+            openai_settings.api_key.get_secret_value() if openai_settings and openai_settings.api_key else None
+        )
+        org_id = org_id or (openai_settings.org_id if openai_settings and openai_settings.org_id else None)
+        ai_model_id = ai_model_id or (
+            openai_settings.embedding_model_id if openai_settings and openai_settings.embedding_model_id else None
+        )
+
         super().__init__(
             ai_model_id=ai_model_id,
             api_key=api_key,
             ai_model_type=OpenAIModelTypes.EMBEDDING,
             org_id=org_id,
             service_id=service_id,
             default_headers=default_headers,
@@ -78,12 +80,13 @@
 
         Arguments:
             settings: A dictionary of settings for the service.
         """
 
         return OpenAITextEmbedding(
             ai_model_id=settings["ai_model_id"],
-            api_key=settings["api_key"],
-            org_id=settings.get("org_id"),
+            api_key=settings.get("api_key", None),
+            org_id=settings.get("org_id", None),
             service_id=settings.get("service_id"),
             default_headers=settings.get("default_headers"),
+            env_file_path=settings.get("env_file_path", None),
         )
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/utils.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/prompt_execution_settings.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     from semantic_kernel.contents import StreamingTextContent, TextContent
 
 
 class TextCompletionClientBase(AIServiceClientBase, ABC):
     """Base class for text completion AI services."""
 
     @abstractmethod
-    async def complete(
+    async def get_text_contents(
         self,
         prompt: str,
         settings: "PromptExecutionSettings",
     ) -> list["TextContent"]:
         """
         This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
@@ -28,15 +28,15 @@
             settings {PromptExecutionSettings} -- Settings for the request.
 
             Returns:
             list[TextContent] -- A string or list of strings representing the response(s) from the LLM.
         """
 
     @abstractmethod
-    def complete_stream(
+    def get_streaming_text_contents(
         self,
         prompt: str,
         settings: "PromptExecutionSettings",
     ) -> AsyncGenerator[list["StreamingTextContent"], Any]:
         """
         This is the method that is called from the kernel to get a stream response from a text-optimized LLM.
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/astra_client.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/astra_client.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,304 +1,367 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-import asyncio
 import logging
-from typing import List, Optional, Tuple
+from typing import TYPE_CHECKING, List, Optional, Tuple
 
-import aiohttp
-from numpy import ndarray
+from numpy import array, ndarray
 
-from semantic_kernel.connectors.memory.astradb.astra_client import AstraClient
-from semantic_kernel.connectors.memory.astradb.utils import (
-    build_payload,
-    parse_payload,
-)
-from semantic_kernel.exceptions import ServiceInitializationError
+from semantic_kernel.connectors.memory.chroma.utils import chroma_compute_similarity_scores, query_results_to_records
+from semantic_kernel.exceptions import ServiceInitializationError, ServiceResourceNotFoundError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 
-MAX_DIMENSIONALITY = 20000
-MAX_UPSERT_BATCH_SIZE = 100
-MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE = 10000
-MAX_QUERY_WITH_METADATA_BATCH_SIZE = 1000
-MAX_FETCH_BATCH_SIZE = 1000
-MAX_DELETE_BATCH_SIZE = 1000
+if TYPE_CHECKING:
+    import chromadb
+    import chromadb.config
+    from chromadb.api.models.Collection import Collection
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-class AstraDBMemoryStore(MemoryStoreBase):
-    """A memory store that uses Astra database as the backend."""
+class ChromaMemoryStore(MemoryStoreBase):
+    _client: "chromadb.Client"
 
     def __init__(
         self,
-        astra_application_token: str,
-        astra_id: str,
-        astra_region: str,
-        keyspace_name: str,
-        embedding_dim: int,
-        similarity: str,
-        session: Optional[aiohttp.ClientSession] = None,
+        persist_directory: Optional[str] = None,
+        client_settings: Optional["chromadb.config.Settings"] = None,
+        **kwargs,
     ) -> None:
-        """Initializes a new instance of the AstraDBMemoryStore class.
-
-        Arguments:
-            astra_application_token {str} -- The Astra application token.
-            astra_id {str} -- The Astra id of database.
-            astra_region {str} -- The Astra region
-            keyspace_name {str} -- The Astra keyspace
-            embedding_dim {int} -- The dimensionality to use for new collections.
-            similarity {str} -- TODO
-            session -- Optional session parameter
-        """
-        self._embedding_dim = embedding_dim
-        self._similarity = similarity
-        self._session = session
+        """
+        ChromaMemoryStore provides an interface to store and retrieve data using ChromaDB.
+        Collection names with uppercase characters are not supported by ChromaDB, they will be automatically converted.
 
-        if self._embedding_dim > MAX_DIMENSIONALITY:
-            raise ServiceInitializationError(
-                f"Dimensionality of {self._embedding_dim} exceeds "
-                + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
+        Args:
+            persist_directory (Optional[str], optional): Path to the directory where data will be persisted.
+                Defaults to None, which means the default settings for ChromaDB will be used.
+            client_settings (Optional["chromadb.config.Settings"], optional): A Settings instance to configure
+                the ChromaDB client. Defaults to None, which means the default settings for ChromaDB will be used.
+            similarity_fetch_limit (int, optional): The maximum number of results to calculate cosine-similarity.
+        Example:
+            # Create a ChromaMemoryStore with a local specified directory for data persistence
+            chroma_local_data_store = ChromaMemoryStore(persist_directory='/path/to/persist/directory')
+            # Create a ChromaMemoryStore with a custom Settings instance
+            chroma_remote_data_store = ChromaMemoryStore(
+                client_settings=Settings(
+                    chroma_api_impl="rest",
+                    chroma_server_host="xxx.xxx.xxx.xxx",
+                    chroma_server_http_port="8000"
+                )
             )
-
-        self._client = AstraClient(
-            astra_id=astra_id,
-            astra_region=astra_region,
-            astra_application_token=astra_application_token,
-            keyspace_name=keyspace_name,
-            embedding_dim=embedding_dim,
-            similarity_function=similarity,
-            session=self._session,
-        )
-
-    async def get_collections(self) -> List[str]:
-        """Gets the list of collections.
-
-        Returns:
-            List[str] -- The list of collections.
         """
-        return await self._client.find_collections(False)
+        try:
+            import chromadb
+            import chromadb.config
 
-    async def create_collection(
-        self,
-        collection_name: str,
-        dimension_num: Optional[int] = None,
-        distance_type: Optional[str] = "cosine",
-    ) -> None:
-        """Creates a new collection in Astra if it does not exist.
+        except ImportError as exc:
+            raise ServiceInitializationError(
+                "Could not import chromadb python package. " "Please install it with `pip install chromadb`."
+            ) from exc
+
+        if client_settings:
+            self._client_settings = client_settings
+        else:
+            self._client_settings = chromadb.config.Settings()
+            if persist_directory is not None:
+                self._client_settings = chromadb.config.Settings(
+                    is_persistent=True, persist_directory=persist_directory
+                )
+        self._client = chromadb.Client(self._client_settings)
+        self._persist_directory = persist_directory
+        self._default_query_includes = ["embeddings", "metadatas", "documents"]
+
+    async def create_collection(self, collection_name: str) -> None:
+        """Creates a new collection in Chroma if it does not exist.
+            To prevent downloading model file from embedding_function,
+            embedding_function is set to "DoNotUseChromaEmbeddingFunction".
 
         Arguments:
             collection_name {str} -- The name of the collection to create.
-            dimension_num {int} -- The dimension of the vectors to be stored in this collection.
-            distance_type {str} -- Specifies the similarity metric to be used when querying or comparing vectors within
-            this collection. The available options are dot_product, euclidean, and cosine.
+            The name of the collection will be converted to snake case.
+
         Returns:
             None
         """
-        dimension_num = dimension_num if dimension_num is not None else self._embedding_dim
-        distance_type = distance_type if distance_type is not None else self._similarity
+        self._client.create_collection(name=collection_name)
 
-        if dimension_num > MAX_DIMENSIONALITY:
-            raise ValueError(
-                f"Dimensionality of {dimension_num} exceeds " + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
-            )
+    async def get_collection(self, collection_name: str) -> Optional["Collection"]:
+        try:
+            # Current version of ChromeDB rejects camel case collection names.
+            return self._client.get_collection(name=collection_name)
+        except ValueError:
+            return None
+
+    async def get_collections(self) -> List[str]:
+        """Gets the list of collections.
 
-        result = await self._client.create_collection(collection_name, dimension_num, distance_type)
-        if result is True:
-            logger.info(f"Collection {collection_name} created.")
+        Returns:
+            List[str] -- The list of collections.
+        """
+        return [collection.name for collection in self._client.list_collections()]
 
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection.
 
         Arguments:
             collection_name {str} -- The name of the collection to delete.
 
         Returns:
             None
         """
-        result = await self._client.delete_collection(collection_name)
-        logger.log(
-            logging.INFO if result is True else logging.WARNING,
-            f"Collection {collection_name} {'deleted.' if result is True else 'does not exist.'}",
-        )
+        self._client.delete_collection(name=collection_name)
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to check.
 
         Returns:
             bool -- True if the collection exists; otherwise, False.
         """
-        return await self._client.find_collection(collection_name)
+        if await self.get_collection(collection_name) is None:
+            return False
+        else:
+            return True
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
-        """Upserts a memory record into the data store. Does not guarantee that the collection exists.
-            If the record already exists, it will be updated.
-            If the record does not exist, it will be created.
+        """Upserts a single MemoryRecord.
 
         Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            record {MemoryRecord} -- The memory record to upsert.
+            collection_name {str} -- The name of the collection to upsert the record into.
+            records {MemoryRecord} -- The record to upsert.
 
         Returns:
-            str -- The unique identifier for the memory record.
+            List[str] -- The unique database key of the record.
         """
-        filter = {"_id": record._id}
-        update = {"$set": build_payload(record)}
-        status = await self._client.update_document(collection_name, filter, update, True)
-
-        return status["upsertedId"] if "upsertedId" in status else record._id
+        collection = await self.get_collection(collection_name)
+        if collection is None:
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+
+        record._key = record._id
+        metadata = {
+            "timestamp": record._timestamp or "",
+            "is_reference": str(record._is_reference),
+            "external_source_name": record._external_source_name or "",
+            "description": record._description or "",
+            "additional_metadata": record._additional_metadata or "",
+            "id": record._id or "",
+        }
+
+        collection.add(
+            metadatas=metadata,
+            # by providing embeddings, we can skip the chroma's embedding function call
+            embeddings=record.embedding.tolist(),
+            documents=record._text,
+            ids=record._key,
+        )
+        return record._key
 
     async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
-        """Upserts a batch of memory records into the data store. Does not guarantee that the collection exists.
-            If the record already exists, it will be updated.
-            If the record does not exist, it will be created.
+        """Upserts a batch of records.
 
         Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            records {List[MemoryRecord]} -- The memory records to upsert.
+            collection_name {str} -- The name of the collection to upsert the records into.
+            records {List[MemoryRecord]} -- The records to upsert.
 
         Returns:
-            List[str] -- The unique identifiers for the memory record.
+            List[str] -- The unique database keys of the records. In Pinecone, these are the record IDs.
         """
-        return await asyncio.gather(*[self.upsert(collection_name, record) for record in records])
+        # upsert is checking collection existence
+        return [await self.upsert(collection_name, record) for record in records]
 
-    async def get(self, collection_name: str, key: str, with_embedding: bool = False) -> MemoryRecord:
-        """Gets a record. Does not guarantee that the collection exists.
+    async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
+        """Gets a record.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the record from.
             key {str} -- The unique database key of the record.
             with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
 
         Returns:
             MemoryRecord -- The record.
         """
-        filter = {"_id": key}
-        documents = await self._client.find_documents(
-            collection_name=collection_name,
-            filter=filter,
-            include_vector=with_embedding,
-        )
-
-        if len(documents) == 0:
-            raise KeyError(f"Record with key '{key}' does not exist")
+        records = await self.get_batch(collection_name, [key], with_embedding)
+        try:
+            return records[0]
+        except IndexError as exc:
+            raise ServiceResourceNotFoundError(
+                f"Record with key '{key}' does not exist in collection '{collection_name}'"
+            ) from exc
 
-        return parse_payload(documents[0])
-
-    async def get_batch(
-        self, collection_name: str, keys: List[str], with_embeddings: bool = False
-    ) -> List[MemoryRecord]:
-        """Gets a batch of records. Does not guarantee that the collection exists.
+    async def get_batch(self, collection_name: str, keys: List[str], with_embeddings: bool) -> List[MemoryRecord]:
+        """Gets a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the records from.
             keys {List[str]} -- The unique database keys of the records.
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
         Returns:
             List[MemoryRecord] -- The records.
         """
-
-        filter = {"_id": {"$in": keys}}
-        documents = await self._client.find_documents(
-            collection_name=collection_name,
-            filter=filter,
-            include_vector=with_embeddings,
-        )
-        return [parse_payload(document) for document in documents]
+        collection = await self.get_collection(collection_name)
+        if collection is None:
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+
+        query_includes = ["embeddings", "metadatas", "documents"] if with_embeddings else ["metadatas", "documents"]
+
+        value = collection.get(ids=keys, include=query_includes)
+        record = query_results_to_records(value, with_embeddings)
+        return record
 
     async def remove(self, collection_name: str, key: str) -> None:
-        """Removes a memory record from the data store. Does not guarantee that the collection exists.
+        """Removes a record.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the record from.
-            key {str} -- The unique id associated with the memory record to remove.
+            key {str} -- The unique database key of the record to remove.
 
         Returns:
             None
         """
-        filter = {"_id": key}
-        await self._client.delete_documents(collection_name, filter)
+        await self.remove_batch(collection_name, [key])
 
     async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
-        """Removes a batch of records. Does not guarantee that the collection exists.
+        """Removes a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the records from.
-            keys {List[str]} -- The unique ids associated with the memory records to remove.
+            keys {List[str]} -- The unique database keys of the records to remove.
 
         Returns:
             None
         """
-        filter = {"_id": {"$in": keys}}
-        await self._client.delete_documents(collection_name, filter)
+        collection = await self.get_collection(collection_name=collection_name)
+        if collection is not None:
+            collection.delete(ids=keys)
 
-    async def get_nearest_match(
+    async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
+        limit: int,
         min_relevance_score: float = 0.0,
-        with_embedding: bool = False,
-    ) -> Tuple[MemoryRecord, float]:
-        """Gets the nearest match to an embedding using cosine similarity.
+        with_embeddings: bool = True,
+    ) -> List[Tuple[MemoryRecord, float]]:
+        """Gets the nearest matches to an embedding using cosine similarity.
+
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest matches from.
             embedding {ndarray} -- The embedding to find the nearest matches to.
+            limit {int} -- The maximum number of matches to return.
             min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            Tuple[MemoryRecord, float] -- The record and the relevance score.
+            List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
         """
-        matches = await self.get_nearest_matches(
-            collection_name=collection_name,
-            embedding=embedding,
-            limit=1,
-            min_relevance_score=min_relevance_score,
-            with_embeddings=with_embedding,
+        if with_embeddings is False:
+            logger.warning(
+                "Chroma returns distance score not cosine similarity score.\
+                So embeddings are automatically queried from database for calculation."
+            )
+        collection = await self.get_collection(collection_name)
+        if collection is None:
+            return []
+
+        query_results = collection.query(
+            query_embeddings=embedding.tolist(),
+            n_results=limit,
+            include=self._default_query_includes,
         )
-        return matches[0]
 
-    async def get_nearest_matches(
+        # Convert the collection of embeddings into a numpy array (stacked)
+        embedding_array = array(query_results["embeddings"][0])
+        embedding_array = embedding_array.reshape(embedding_array.shape[0], -1)
+
+        # If the query embedding has shape (1, embedding_size),
+        # reshape it to (embedding_size,)
+        if len(embedding.shape) == 2:
+            embedding = embedding.reshape(
+                embedding.shape[1],
+            )
+
+        similarity_score = chroma_compute_similarity_scores(embedding, embedding_array)
+
+        # Convert query results into memory records
+        record_list = [
+            (record, distance)
+            for record, distance in zip(
+                query_results_to_records(query_results, with_embeddings),
+                similarity_score,
+            )
+        ]
+
+        sorted_results = sorted(
+            record_list,
+            key=lambda x: x[1],
+            reverse=True,
+        )
+
+        filtered_results = [x for x in sorted_results if x[1] >= min_relevance_score]
+        top_results = filtered_results[:limit]
+
+        return top_results
+
+    async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
-        limit: int,
         min_relevance_score: float = 0.0,
-        with_embeddings: bool = False,
-    ) -> List[Tuple[MemoryRecord, float]]:
-        """Gets the nearest matches to an embedding using cosine similarity.
+        with_embedding: bool = True,
+    ) -> Tuple[MemoryRecord, float]:
+        """Gets the nearest match to an embedding using cosine similarity.
+
         Arguments:
-            collection_name {str} -- The name of the collection to get the nearest matches from.
-            embedding {ndarray} -- The embedding to find the nearest matches to.
-            limit {int} -- The maximum number of matches to return.
-            min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
+            collection_name {str} -- The name of the collection to get the nearest match from.
+            embedding {ndarray} -- The embedding to find the nearest match to.
+            min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
+            with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
 
         Returns:
-            List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
+            Tuple[MemoryRecord, float] -- The record and the relevance score.
         """
-        matches = await self._client.find_documents(
+        results = await self.get_nearest_matches(
             collection_name=collection_name,
-            vector=embedding.tolist(),
-            limit=limit,
-            include_similarity=True,
-            include_vector=with_embeddings,
+            embedding=embedding,
+            limit=1,
+            min_relevance_score=min_relevance_score,
+            with_embeddings=with_embedding,
         )
+        return results[0]
 
-        if min_relevance_score:
-            matches = [match for match in matches if match["$similarity"] >= min_relevance_score]
 
-        return (
-            [
-                (
-                    parse_payload(match),
-                    match["$similarity"],
-                )
-                for match in matches
-            ]
-            if len(matches) > 0
-            else []
-        )
+if __name__ == "__main__":
+    import asyncio
+
+    import numpy as np
+
+    memory = ChromaMemoryStore()
+    memory_record1 = MemoryRecord(
+        id="test_id1",
+        text="sample text1",
+        is_reference=False,
+        embedding=np.array([0.5, 0.5]),
+        description="description",
+        external_source_name="external source",
+        timestamp="timestamp",
+    )
+    memory_record2 = MemoryRecord(
+        id="test_id2",
+        text="sample text2",
+        is_reference=False,
+        embedding=np.array([0.25, 0.75]),
+        description="description",
+        external_source_name="external source",
+        timestamp="timestamp",
+    )
+
+    asyncio.run(memory.create_collection("test_collection"))
+    collection = asyncio.run(memory.get_collection("test_collection"))
+
+    asyncio.run(memory.upsert_batch(collection.name, [memory_record1, memory_record2]))
+
+    result = asyncio.run(memory.get(collection.name, "test_id1", True))
+    results = asyncio.run(memory.get_nearest_match("test_collection", np.array([0.5, 0.5])))
+    print(results)
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/utils.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,63 +14,85 @@
     SearchIndex,
     SearchResourceEncryptionKey,
     VectorSearch,
     VectorSearchProfile,
 )
 from azure.search.documents.models import VectorizedQuery
 from numpy import ndarray
+from pydantic import ValidationError
 
 from semantic_kernel.connectors.memory.azure_cognitive_search.utils import (
     SEARCH_FIELD_EMBEDDING,
     SEARCH_FIELD_ID,
     dict_to_memory_record,
     encode_id,
     get_field_selection,
     get_index_schema,
     get_search_index_async_client,
     memory_record_to_search_record,
 )
-from semantic_kernel.exceptions import ServiceInitializationError, ServiceResourceNotFoundError
+from semantic_kernel.exceptions import MemoryConnectorInitializationError, MemoryConnectorResourceNotFound
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class AzureCognitiveSearchMemoryStore(MemoryStoreBase):
     _search_index_client: SearchIndexClient = None
     _vector_size: int = None
 
     def __init__(
         self,
         vector_size: int,
-        search_endpoint: Optional[str] = None,
-        admin_key: Optional[str] = None,
-        azure_credentials: Optional[AzureKeyCredential] = None,
-        token_credentials: Optional[TokenCredential] = None,
-        **kwargs,
+        search_endpoint: str | None = None,
+        admin_key: str | None = None,
+        azure_credentials: AzureKeyCredential | None = None,
+        token_credentials: TokenCredential | None = None,
+        env_file_path: str | None = None,
     ) -> None:
         """Initializes a new instance of the AzureCognitiveSearchMemoryStore class.
 
         Arguments:
             vector_size {int}                                -- Embedding vector size.
-            search_endpoint {Optional[str]}                  -- The endpoint of the Azure Cognitive Search service
+            search_endpoint {str | None}                  -- The endpoint of the Azure Cognitive Search service
                                                                 (default: {None}).
-            admin_key {Optional[str]}                        -- Azure Cognitive Search API key (default: {None}).
-            azure_credentials {Optional[AzureKeyCredential]} -- Azure Cognitive Search credentials (default: {None}).
-            token_credentials {Optional[TokenCredential]}    -- Azure Cognitive Search token credentials
+            admin_key {str | None}                        -- Azure Cognitive Search API key (default: {None}).
+            azure_credentials {AzureKeyCredential | None} -- Azure Cognitive Search credentials (default: {None}).
+            token_credentials {TokenCredential | None}    -- Azure Cognitive Search token credentials
                                                                 (default: {None}).
+            env_file_path {str | None}                  -- Use the environment settings file as a fallback
+                                                                to environment variables
 
         Instantiate using Async Context Manager:
             async with AzureCognitiveSearchMemoryStore(<...>) as memory:
                 await memory.<...>
         """
+        from semantic_kernel.connectors.memory.azure_cognitive_search import AzureAISearchSettings
+
+        acs_memory_settings = None
+        try:
+            acs_memory_settings = AzureAISearchSettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.warning(f"Failed to load AzureAISearch pydantic settings: {e}")
+
+        admin_key = admin_key or (
+            acs_memory_settings.api_key.get_secret_value()
+            if acs_memory_settings and acs_memory_settings.api_key
+            else None
+        )
+        assert admin_key, "The ACS admin_key is required to connect to Azure Cognitive Search."
+        search_endpoint = search_endpoint or (
+            acs_memory_settings.endpoint if acs_memory_settings and acs_memory_settings.endpoint else None
+        )
+        assert search_endpoint, "The ACS endpoint is required to connect to Azure Cognitive Search."
+
         self._vector_size = vector_size
         self._search_index_client = get_search_index_async_client(
-            search_endpoint, admin_key, azure_credentials, token_credentials
+            str(search_endpoint), admin_key, azure_credentials, token_credentials
         )
 
     async def close(self):
         """Async close connection, invoked by MemoryStoreBase.__aexit__()"""
         if self._search_index_client is not None:
             await self._search_index_client.close()
 
@@ -118,15 +140,15 @@
                             metric="cosine",  # Can be "cosine", "dotProduct", or "euclidean"
                         ),
                     )
                 ],
             )
 
         if not self._search_index_client:
-            raise ServiceInitializationError("Error: self._search_index_client not set 1.")
+            raise MemoryConnectorInitializationError("Error: self._search_index_client not set 1.")
 
         # Check to see if collection exists
         collection_index = None
         try:
             collection_index = await self._search_index_client.get_index(collection_name.lower())
         except ResourceNotFoundError:
             pass
@@ -260,15 +282,15 @@
 
         try:
             search_result = await search_client.get_document(
                 key=encode_id(key), selected_fields=get_field_selection(with_embedding)
             )
         except ResourceNotFoundError as exc:
             await search_client.close()
-            raise ServiceResourceNotFoundError("Memory record not found") from exc
+            raise MemoryConnectorResourceNotFound("Memory record not found") from exc
 
         await search_client.close()
 
         # Create Memory record from document
         return dict_to_memory_record(search_result, with_embedding)
 
     async def get_batch(
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # Copyright (c) Microsoft. All rights reserved.
+
+import logging
 from typing import List, Tuple
 
 from numpy import ndarray
+from pydantic import ValidationError
 
 from semantic_kernel.connectors.memory.azure_cosmosdb.azure_cosmos_db_store_api import AzureCosmosDBStoreApi
+from semantic_kernel.connectors.memory.azure_cosmosdb.azure_cosmosdb_settings import AzureCosmosDBSettings
 from semantic_kernel.connectors.memory.azure_cosmosdb.cosmosdb_utils import (
     CosmosDBSimilarityType,
     CosmosDBVectorSearchType,
     get_mongodb_search_client,
 )
 from semantic_kernel.connectors.memory.azure_cosmosdb.mongo_vcore_store_api import MongoStoreApi
-from semantic_kernel.exceptions import ServiceInitializationError
+from semantic_kernel.exceptions import MemoryConnectorInitializationError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 
+logger: logging.Logger = logging.getLogger(__name__)
+
 
 class AzureCosmosDBMemoryStore(MemoryStoreBase):
     """A memory store that uses AzureCosmosDB for MongoDB vCore, to perform vector similarity search on a fully
     managed MongoDB compatible database service.
     https://learn.microsoft.com/en-us/azure/cosmos-db/mongodb/vcore/vector-search"""
 
     # Right now this only supports Mongo, but set up to support more later.
@@ -44,21 +50,21 @@
         similarity: CosmosDBSimilarityType = CosmosDBSimilarityType.COS,
         kind: CosmosDBVectorSearchType = CosmosDBVectorSearchType.VECTOR_HNSW,
         m: int = 16,
         ef_construction: int = 64,
         ef_search: int = 40,
     ):
         if vector_dimensions <= 0:
-            raise ServiceInitializationError("Vector dimensions must be a positive number.")
+            raise MemoryConnectorInitializationError("Vector dimensions must be a positive number.")
         # if connection_string is None:
         #     raise ValueError("Connection String cannot be empty.")
         if database_name is None:
-            raise ServiceInitializationError("Database Name cannot be empty.")
+            raise MemoryConnectorInitializationError("Database Name cannot be empty.")
         if index_name is None:
-            raise ServiceInitializationError("Index Name cannot be empty.")
+            raise MemoryConnectorInitializationError("Index Name cannot be empty.")
 
         self.cosmosStore = cosmosStore
         self.index_name = index_name
         self.num_lists = num_lists
         self.similarity = similarity
         self.kind = kind
         self.m = m
@@ -76,19 +82,33 @@
         vector_dimensions,
         num_lists,
         similarity,
         kind,
         m,
         ef_construction,
         ef_search,
+        env_file_path: str | None = None,
     ) -> MemoryStoreBase:
         """Creates the underlying data store based on the API definition"""
         # Right now this only supports Mongo, but set up to support more later.
         apiStore: AzureCosmosDBStoreApi = None
         if cosmos_api == "mongo-vcore":
+
+            cosmosdb_settings = None
+            try:
+                cosmosdb_settings = AzureCosmosDBSettings.create(env_file_path=env_file_path)
+            except ValidationError as e:
+                logger.warning(f"Failed to load AzureCosmosDB pydantic settings: {e}")
+
+            cosmos_connstr = cosmos_connstr or (
+                cosmosdb_settings.connection_string.get_secret_value()
+                if cosmosdb_settings and cosmosdb_settings.connection_string
+                else None
+            )
+
             mongodb_client = get_mongodb_search_client(cosmos_connstr, application_name)
             database = mongodb_client[database_name]
             apiStore = MongoStoreApi(
                 collection_name=collection_name,
                 index_name=index_name,
                 vector_dimensions=vector_dimensions,
                 num_lists=num_lists,
@@ -96,15 +116,15 @@
                 database=database,
                 kind=kind,
                 m=m,
                 ef_construction=ef_construction,
                 ef_search=ef_search,
             )
         else:
-            raise NotImplementedError(f"API type {cosmos_api} is not supported.")
+            raise MemoryConnectorInitializationError(f"API type {cosmos_api} is not supported.")
 
         store = AzureCosmosDBMemoryStore(
             apiStore,
             database_name,
             index_name,
             vector_dimensions,
             num_lists,
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,367 +1,398 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING, List, Optional, Tuple
+from typing import List, NamedTuple, Optional, Tuple
 
-from numpy import array, ndarray
-
-from semantic_kernel.connectors.memory.chroma.utils import chroma_compute_similarity_scores, query_results_to_records
-from semantic_kernel.exceptions import ServiceInitializationError, ServiceResourceNotFoundError
+from numpy import ndarray
+from pinecone import FetchResponse, IndexDescription, IndexList, Pinecone, ServerlessSpec
+from pydantic import ValidationError
+
+from semantic_kernel.connectors.memory.pinecone.pinecone_settings import PineconeSettings
+from semantic_kernel.connectors.memory.pinecone.utils import (
+    build_payload,
+    parse_payload,
+)
+from semantic_kernel.exceptions import (
+    ServiceInitializationError,
+    ServiceInvalidRequestError,
+    ServiceResourceNotFoundError,
+    ServiceResponseException,
+)
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 
-if TYPE_CHECKING:
-    import chromadb
-    import chromadb.config
-    from chromadb.api.models.Collection import Collection
+# Limitations set by Pinecone at https://docs.pinecone.io/reference/known-limitations
+MAX_DIMENSIONALITY = 20000
+MAX_UPSERT_BATCH_SIZE = 100
+MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE = 10000
+MAX_QUERY_WITH_METADATA_BATCH_SIZE = 1000
+MAX_FETCH_BATCH_SIZE = 1000
+MAX_DELETE_BATCH_SIZE = 1000
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-class ChromaMemoryStore(MemoryStoreBase):
-    _client: "chromadb.Client"
+class PineconeMemoryStore(MemoryStoreBase):
+    """A memory store that uses Pinecone as the backend."""
+
+    _pinecone_api_key: str
+    _default_dimensionality: int
+
+    DEFAULT_INDEX_SPEC: ServerlessSpec = ServerlessSpec(
+        cloud="aws",
+        region="us-east-1",
+    )
 
     def __init__(
         self,
-        persist_directory: Optional[str] = None,
-        client_settings: Optional["chromadb.config.Settings"] = None,
-        **kwargs,
+        api_key: str,
+        default_dimensionality: int,
+        env_file_path: str | None = None,
     ) -> None:
-        """
-        ChromaMemoryStore provides an interface to store and retrieve data using ChromaDB.
-        Collection names with uppercase characters are not supported by ChromaDB, they will be automatically converted.
+        """Initializes a new instance of the PineconeMemoryStore class.
 
-        Args:
-            persist_directory (Optional[str], optional): Path to the directory where data will be persisted.
-                Defaults to None, which means the default settings for ChromaDB will be used.
-            client_settings (Optional["chromadb.config.Settings"], optional): A Settings instance to configure
-                the ChromaDB client. Defaults to None, which means the default settings for ChromaDB will be used.
-            similarity_fetch_limit (int, optional): The maximum number of results to calculate cosine-similarity.
-        Example:
-            # Create a ChromaMemoryStore with a local specified directory for data persistence
-            chroma_local_data_store = ChromaMemoryStore(persist_directory='/path/to/persist/directory')
-            # Create a ChromaMemoryStore with a custom Settings instance
-            chroma_remote_data_store = ChromaMemoryStore(
-                client_settings=Settings(
-                    chroma_api_impl="rest",
-                    chroma_server_host="xxx.xxx.xxx.xxx",
-                    chroma_server_http_port="8000"
-                )
-            )
+        Arguments:
+            pinecone_api_key {str} -- The Pinecone API key.
+            default_dimensionality {int} -- The default dimensionality to use for new collections.
+            env_file_path {str | None} -- Use the environment settings file as a fallback
+                to environment variables. (Optional)
         """
+        if default_dimensionality > MAX_DIMENSIONALITY:
+            raise ServiceInitializationError(
+                f"Dimensionality of {default_dimensionality} exceeds "
+                + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
+            )
+
+        pinecone_settings = None
         try:
-            import chromadb
-            import chromadb.config
+            pinecone_settings = PineconeSettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.warning(f"Failed to load the Pinecone pydantic settings: {e}")
 
-        except ImportError as exc:
-            raise ServiceInitializationError(
-                "Could not import chromadb python package. " "Please install it with `pip install chromadb`."
-            ) from exc
+        api_key = api_key or (
+            pinecone_settings.api_key.get_secret_value() if pinecone_settings and pinecone_settings.api_key else None
+        )
+        assert api_key, "The Pinecone api_key cannot be None."
 
-        if client_settings:
-            self._client_settings = client_settings
-        else:
-            self._client_settings = chromadb.config.Settings()
-            if persist_directory is not None:
-                self._client_settings = chromadb.config.Settings(
-                    is_persistent=True, persist_directory=persist_directory
-                )
-        self._client = chromadb.Client(self._client_settings)
-        self._persist_directory = persist_directory
-        self._default_query_includes = ["embeddings", "metadatas", "documents"]
-
-    async def create_collection(self, collection_name: str) -> None:
-        """Creates a new collection in Chroma if it does not exist.
-            To prevent downloading model file from embedding_function,
-            embedding_function is set to "DoNotUseChromaEmbeddingFunction".
+        self._pinecone_api_key = api_key
+        self._default_dimensionality = default_dimensionality
+
+        self.pinecone = Pinecone(api_key=self._pinecone_api_key)
+        self.collection_names_cache = set()
+
+    async def create_collection(
+        self,
+        collection_name: str,
+        dimension_num: Optional[int] = None,
+        distance_type: Optional[str] = "cosine",
+        index_spec: NamedTuple = DEFAULT_INDEX_SPEC,
+    ) -> None:
+        """Creates a new collection in Pinecone if it does not exist.
+            This function creates an index, by default the following index
+            settings are used: metric = cosine, cloud = aws, region = us-east-1.
 
         Arguments:
             collection_name {str} -- The name of the collection to create.
-            The name of the collection will be converted to snake case.
+            In Pinecone, a collection is represented as an index. The concept
+            of "collection" in Pinecone is just a static copy of an index.
 
         Returns:
             None
         """
-        self._client.create_collection(name=collection_name)
+        if dimension_num is None:
+            dimension_num = self._default_dimensionality
+        if dimension_num > MAX_DIMENSIONALITY:
+            raise ServiceInitializationError(
+                f"Dimensionality of {dimension_num} exceeds " + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
+            )
 
-    async def get_collection(self, collection_name: str) -> Optional["Collection"]:
-        try:
-            # Current version of ChromeDB rejects camel case collection names.
-            return self._client.get_collection(name=collection_name)
-        except ValueError:
-            return None
+        if not await self.does_collection_exist(collection_name):
+            self.pinecone.create_index(
+                name=collection_name, dimension=dimension_num, metric=distance_type, spec=index_spec
+            )
+            self.collection_names_cache.add(collection_name)
+
+    async def describe_collection(self, collection_name: str) -> Optional[IndexDescription]:
+        """Gets the description of the index.
+        Arguments:
+            collection_name {str} -- The name of the index to get.
+        Returns:
+            Optional[dict] -- The index.
+        """
+        if await self.does_collection_exist(collection_name):
+            return self.pinecone.describe_index(collection_name)
+        return None
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(
+        self,
+    ) -> IndexList:
         """Gets the list of collections.
 
         Returns:
-            List[str] -- The list of collections.
+            IndexList -- The list of collections.
         """
-        return [collection.name for collection in self._client.list_collections()]
+        return self.pinecone.list_indexes()
 
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection.
 
         Arguments:
             collection_name {str} -- The name of the collection to delete.
 
         Returns:
             None
         """
-        self._client.delete_collection(name=collection_name)
+        if await self.does_collection_exist(collection_name):
+            self.pinecone.delete_index(collection_name)
+            self.collection_names_cache.discard(collection_name)
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to check.
 
         Returns:
             bool -- True if the collection exists; otherwise, False.
         """
-        if await self.get_collection(collection_name) is None:
-            return False
-        else:
+        if collection_name in self.collection_names_cache:
             return True
 
+        index_collection_names = self.pinecone.list_indexes().names()
+        self.collection_names_cache |= set(index_collection_names)
+
+        return collection_name in index_collection_names
+
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
-        """Upserts a single MemoryRecord.
+        """Upserts a record.
 
         Arguments:
             collection_name {str} -- The name of the collection to upsert the record into.
-            records {MemoryRecord} -- The record to upsert.
+            record {MemoryRecord} -- The record to upsert.
 
         Returns:
-            List[str] -- The unique database key of the record.
+            str -- The unique database key of the record. In Pinecone, this is the record ID.
         """
-        collection = await self.get_collection(collection_name)
-        if collection is None:
+        if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        record._key = record._id
-        metadata = {
-            "timestamp": record._timestamp or "",
-            "is_reference": str(record._is_reference),
-            "external_source_name": record._external_source_name or "",
-            "description": record._description or "",
-            "additional_metadata": record._additional_metadata or "",
-            "id": record._id or "",
-        }
-
-        collection.add(
-            metadatas=metadata,
-            # by providing embeddings, we can skip the chroma's embedding function call
-            embeddings=record.embedding.tolist(),
-            documents=record._text,
-            ids=record._key,
+        collection = self.pinecone.Index(collection_name)
+
+        upsert_response = collection.upsert(
+            vectors=[(record._id, record.embedding.tolist(), build_payload(record))],
+            namespace="",
         )
-        return record._key
+
+        if upsert_response.upserted_count is None:
+            raise ServiceResponseException(f"Error upserting record: {upsert_response.message}")
+
+        return record._id
 
     async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
         """Upserts a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to upsert the records into.
             records {List[MemoryRecord]} -- The records to upsert.
 
         Returns:
-            List[str] -- The unique database keys of the records. In Pinecone, these are the record IDs.
+            List[str] -- The unique database keys of the records.
         """
-        # upsert is checking collection existence
-        return [await self.upsert(collection_name, record) for record in records]
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+
+        collection = self.pinecone.Index(collection_name)
+
+        vectors = [
+            (
+                record._id,
+                record.embedding.tolist(),
+                build_payload(record),
+            )
+            for record in records
+        ]
+
+        upsert_response = collection.upsert(vectors, namespace="", batch_size=MAX_UPSERT_BATCH_SIZE)
+
+        if upsert_response.upserted_count is None:
+            raise ServiceResponseException(f"Error upserting record: {upsert_response.message}")
+        else:
+            return [record._id for record in records]
 
-    async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
+    async def get(self, collection_name: str, key: str, with_embedding: bool = False) -> MemoryRecord:
         """Gets a record.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the record from.
             key {str} -- The unique database key of the record.
             with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
 
         Returns:
             MemoryRecord -- The record.
         """
-        records = await self.get_batch(collection_name, [key], with_embedding)
-        try:
-            return records[0]
-        except IndexError as exc:
-            raise ServiceResourceNotFoundError(
-                f"Record with key '{key}' does not exist in collection '{collection_name}'"
-            ) from exc
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+
+        collection = self.pinecone.Index(collection_name)
+        fetch_response = collection.fetch([key])
 
-    async def get_batch(self, collection_name: str, keys: List[str], with_embeddings: bool) -> List[MemoryRecord]:
+        if len(fetch_response.vectors) == 0:
+            raise ServiceResourceNotFoundError(f"Record with key '{key}' does not exist")
+
+        return parse_payload(fetch_response.vectors[key], with_embedding)
+
+    async def get_batch(
+        self, collection_name: str, keys: List[str], with_embeddings: bool = False
+    ) -> List[MemoryRecord]:
         """Gets a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the records from.
             keys {List[str]} -- The unique database keys of the records.
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
         Returns:
             List[MemoryRecord] -- The records.
         """
-        collection = await self.get_collection(collection_name)
-        if collection is None:
+        if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        query_includes = ["embeddings", "metadatas", "documents"] if with_embeddings else ["metadatas", "documents"]
-
-        value = collection.get(ids=keys, include=query_includes)
-        record = query_results_to_records(value, with_embeddings)
-        return record
+        fetch_response = await self.__get_batch(collection_name, keys, with_embeddings)
+        return [parse_payload(fetch_response.vectors[key], with_embeddings) for key in fetch_response.vectors.keys()]
 
     async def remove(self, collection_name: str, key: str) -> None:
         """Removes a record.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the record from.
             key {str} -- The unique database key of the record to remove.
 
         Returns:
             None
         """
-        await self.remove_batch(collection_name, [key])
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+
+        collection = self.pinecone.Index(collection_name)
+        collection.delete([key])
 
     async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
         """Removes a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the records from.
             keys {List[str]} -- The unique database keys of the records to remove.
 
         Returns:
             None
         """
-        collection = await self.get_collection(collection_name=collection_name)
-        if collection is not None:
-            collection.delete(ids=keys)
-
-    async def get_nearest_matches(
-        self,
-        collection_name: str,
-        embedding: ndarray,
-        limit: int,
-        min_relevance_score: float = 0.0,
-        with_embeddings: bool = True,
-    ) -> List[Tuple[MemoryRecord, float]]:
-        """Gets the nearest matches to an embedding using cosine similarity.
-
-        Arguments:
-            collection_name {str} -- The name of the collection to get the nearest matches from.
-            embedding {ndarray} -- The embedding to find the nearest matches to.
-            limit {int} -- The maximum number of matches to return.
-            min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
-
-        Returns:
-            List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
-        """
-        if with_embeddings is False:
-            logger.warning(
-                "Chroma returns distance score not cosine similarity score.\
-                So embeddings are automatically queried from database for calculation."
-            )
-        collection = await self.get_collection(collection_name)
-        if collection is None:
-            return []
-
-        query_results = collection.query(
-            query_embeddings=embedding.tolist(),
-            n_results=limit,
-            include=self._default_query_includes,
-        )
-
-        # Convert the collection of embeddings into a numpy array (stacked)
-        embedding_array = array(query_results["embeddings"][0])
-        embedding_array = embedding_array.reshape(embedding_array.shape[0], -1)
-
-        # If the query embedding has shape (1, embedding_size),
-        # reshape it to (embedding_size,)
-        if len(embedding.shape) == 2:
-            embedding = embedding.reshape(
-                embedding.shape[1],
-            )
-
-        similarity_score = chroma_compute_similarity_scores(embedding, embedding_array)
-
-        # Convert query results into memory records
-        record_list = [
-            (record, distance)
-            for record, distance in zip(
-                query_results_to_records(query_results, with_embeddings),
-                similarity_score,
-            )
-        ]
-
-        sorted_results = sorted(
-            record_list,
-            key=lambda x: x[1],
-            reverse=True,
-        )
-
-        filtered_results = [x for x in sorted_results if x[1] >= min_relevance_score]
-        top_results = filtered_results[:limit]
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        return top_results
+        collection = self.pinecone.Index(collection_name)
+        for i in range(0, len(keys), MAX_DELETE_BATCH_SIZE):
+            collection.delete(keys[i : i + MAX_DELETE_BATCH_SIZE])
+        collection.delete(keys)
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
-        with_embedding: bool = True,
+        with_embedding: bool = False,
     ) -> Tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using cosine similarity.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest match from.
             embedding {ndarray} -- The embedding to find the nearest match to.
             min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
             with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
 
         Returns:
             Tuple[MemoryRecord, float] -- The record and the relevance score.
         """
-        results = await self.get_nearest_matches(
+        matches = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
             limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
         )
-        return results[0]
-
+        return matches[0]
 
-if __name__ == "__main__":
-    import asyncio
+    async def get_nearest_matches(
+        self,
+        collection_name: str,
+        embedding: ndarray,
+        limit: int,
+        min_relevance_score: float = 0.0,
+        with_embeddings: bool = False,
+    ) -> List[Tuple[MemoryRecord, float]]:
+        """Gets the nearest matches to an embedding using cosine similarity.
 
-    import numpy as np
+        Arguments:
+            collection_name {str} -- The name of the collection to get the nearest matches from.
+            embedding {ndarray} -- The embedding to find the nearest matches to.
+            limit {int} -- The maximum number of matches to return.
+            min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
+            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
-    memory = ChromaMemoryStore()
-    memory_record1 = MemoryRecord(
-        id="test_id1",
-        text="sample text1",
-        is_reference=False,
-        embedding=np.array([0.5, 0.5]),
-        description="description",
-        external_source_name="external source",
-        timestamp="timestamp",
-    )
-    memory_record2 = MemoryRecord(
-        id="test_id2",
-        text="sample text2",
-        is_reference=False,
-        embedding=np.array([0.25, 0.75]),
-        description="description",
-        external_source_name="external source",
-        timestamp="timestamp",
-    )
+        Returns:
+            List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
+        """
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-    asyncio.run(memory.create_collection("test_collection"))
-    collection = asyncio.run(memory.get_collection("test_collection"))
+        collection = self.pinecone.Index(collection_name)
 
-    asyncio.run(memory.upsert_batch(collection.name, [memory_record1, memory_record2]))
+        if limit > MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE:
+            raise ServiceInvalidRequestError(
+                "Limit must be less than or equal to " + f"{MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE}"
+            )
+        elif limit > MAX_QUERY_WITH_METADATA_BATCH_SIZE:
+            query_response = collection.query(
+                vector=embedding.tolist(),
+                top_k=limit,
+                include_values=False,
+                include_metadata=False,
+            )
+            keys = [match.id for match in query_response.matches]
+            fetch_response = await self.__get_batch(collection_name, keys, with_embeddings)
+            vectors = fetch_response.vectors
+            for match in query_response.matches:
+                vectors[match.id].update(match)
+            matches = [vectors[key] for key in vectors.keys()]
+        else:
+            query_response = collection.query(
+                vector=embedding.tolist(),
+                top_k=limit,
+                include_values=with_embeddings,
+                include_metadata=True,
+            )
+            matches = query_response.matches
+        if min_relevance_score is not None:
+            matches = [match for match in matches if match.score >= min_relevance_score]
+        return (
+            [
+                (
+                    parse_payload(match, with_embeddings),
+                    match["score"],
+                )
+                for match in matches
+            ]
+            if len(matches) > 0
+            else []
+        )
 
-    result = asyncio.run(memory.get(collection.name, "test_id1", True))
-    results = asyncio.run(memory.get_nearest_match("test_collection", np.array([0.5, 0.5])))
-    print(results)
+    async def __get_batch(
+        self, collection_name: str, keys: List[str], with_embeddings: bool = False
+    ) -> "FetchResponse":
+        index = self.pinecone.Index(collection_name)
+        if len(keys) > MAX_FETCH_BATCH_SIZE:
+            fetch_response = index.fetch(keys[0:MAX_FETCH_BATCH_SIZE])
+            for i in range(MAX_FETCH_BATCH_SIZE, len(keys), MAX_FETCH_BATCH_SIZE):
+                fetch_response.vectors.update(index.fetch(keys[i : i + MAX_FETCH_BATCH_SIZE]).vectors)
+        else:
+            fetch_response = index.fetch(keys)
+        return fetch_response
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 from importlib import metadata
-from typing import Any, List, Mapping, Optional, Tuple
+from typing import Any, List, Mapping, Tuple
 
 from motor import core, motor_asyncio
 from numpy import ndarray
+from pydantic import ValidationError
 from pymongo import DeleteOne, ReadPreference, UpdateOne, results
 from pymongo.driver_info import DriverInfo
 
 from semantic_kernel.connectors.memory.mongodb_atlas.utils import (
     DEFAULT_DB_NAME,
     DEFAULT_SEARCH_INDEX_NAME,
     MONGODB_FIELD_EMBEDDING,
@@ -18,15 +19,14 @@
     NUM_CANDIDATES_SCALAR,
     document_to_memory_record,
     memory_record_to_mongo_document,
 )
 from semantic_kernel.exceptions import ServiceResourceNotFoundError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
-from semantic_kernel.utils.settings import mongodb_atlas_settings_from_dot_env
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class MongoDBAtlasMemoryStore(MemoryStoreBase):
     """Memory Store for MongoDB Atlas Vector Search Connections"""
 
@@ -34,24 +34,36 @@
 
     _mongo_client: motor_asyncio.AsyncIOMotorClient
     __database_name: str
     __index_name: str
 
     def __init__(
         self,
-        index_name: Optional[str] = None,
-        connection_string: Optional[str] = None,
-        database_name: Optional[str] = None,
-        read_preference: Optional[ReadPreference] = ReadPreference.PRIMARY,
-        **kwargs,
+        index_name: str | None = None,
+        connection_string: str | None = None,
+        database_name: str | None = None,
+        read_preference: ReadPreference | None = ReadPreference.PRIMARY,
+        env_file_path: str | None = None,
     ):
-        if kwargs.get("logger"):
-            logger.warning("The `logger` parameter is deprecated. Please use the `logging` module instead.")
+        from semantic_kernel.connectors.memory.mongodb_atlas import MongoDBAtlasSettings
+
+        mongodb_settings = None
+        try:
+            mongodb_settings = MongoDBAtlasSettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.warning(f"Failed to load the MongoDBAtlas pydantic settings: {e}")
+
+        connection_string = connection_string or (
+            mongodb_settings.connection_string.get_secret_value()
+            if mongodb_settings and mongodb_settings.connection_string
+            else None
+        )
+
         self._mongo_client = motor_asyncio.AsyncIOMotorClient(
-            connection_string or mongodb_atlas_settings_from_dot_env(),
+            connection_string,
             read_preference=read_preference,
             driver=DriverInfo("Microsoft Semantic Kernel", metadata.version("semantic-kernel")),
         )
         self.__database_name = database_name or DEFAULT_DB_NAME
         self.__index_name = index_name or DEFAULT_SEARCH_INDEX_NAME
 
     @property
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,303 +1,284 @@
 # Copyright (c) Microsoft. All rights reserved.
 
+import asyncio
 import logging
-from typing import List, NamedTuple, Optional, Tuple
+from typing import List, Optional, Tuple
 
+import aiohttp
 from numpy import ndarray
-from pinecone import FetchResponse, IndexDescription, IndexList, Pinecone, ServerlessSpec
+from pydantic import ValidationError
 
-from semantic_kernel.connectors.memory.pinecone.utils import (
+from semantic_kernel.connectors.memory.astradb.astra_client import AstraClient
+from semantic_kernel.connectors.memory.astradb.astradb_settings import AstraDBSettings
+from semantic_kernel.connectors.memory.astradb.utils import (
     build_payload,
     parse_payload,
 )
-from semantic_kernel.exceptions import (
-    ServiceInitializationError,
-    ServiceInvalidRequestError,
-    ServiceResourceNotFoundError,
-    ServiceResponseException,
-)
+from semantic_kernel.exceptions import MemoryConnectorInitializationError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 
-# Limitations set by Pinecone at https://docs.pinecone.io/reference/known-limitations
 MAX_DIMENSIONALITY = 20000
 MAX_UPSERT_BATCH_SIZE = 100
 MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE = 10000
 MAX_QUERY_WITH_METADATA_BATCH_SIZE = 1000
 MAX_FETCH_BATCH_SIZE = 1000
 MAX_DELETE_BATCH_SIZE = 1000
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-class PineconeMemoryStore(MemoryStoreBase):
-    """A memory store that uses Pinecone as the backend."""
-
-    _pinecone_api_key: str
-    _default_dimensionality: int
-
-    DEFAULT_INDEX_SPEC: ServerlessSpec = ServerlessSpec(
-        cloud="aws",
-        region="us-east-1",
-    )
+class AstraDBMemoryStore(MemoryStoreBase):
+    """A memory store that uses Astra database as the backend."""
 
     def __init__(
         self,
-        api_key: str,
-        default_dimensionality: int,
-        **kwargs,
+        astra_application_token: str,
+        astra_id: str,
+        astra_region: str,
+        keyspace_name: str,
+        embedding_dim: int,
+        similarity: str,
+        session: aiohttp.ClientSession | None = None,
+        env_file_path: str | None = None,
     ) -> None:
-        """Initializes a new instance of the PineconeMemoryStore class.
+        """Initializes a new instance of the AstraDBMemoryStore class.
 
         Arguments:
-            pinecone_api_key {str} -- The Pinecone API key.
-            default_dimensionality {int} -- The default dimensionality to use for new collections.
-        """
-        if kwargs.get("logger"):
-            logger.warning("The `logger` parameter is deprecated. Please use the `logging` module instead.")
-        if default_dimensionality > MAX_DIMENSIONALITY:
-            raise ServiceInitializationError(
-                f"Dimensionality of {default_dimensionality} exceeds "
+            astra_application_token {str} -- The Astra application token.
+            astra_id {str} -- The Astra id of database.
+            astra_region {str} -- The Astra region
+            keyspace_name {str} -- The Astra keyspace
+            embedding_dim {int} -- The dimensionality to use for new collections.
+            similarity {str} -- TODO
+            session -- Optional session parameter
+            env_file_path {str | None} -- Use the environment settings file as a
+                fallback to environment variables. (Optional)
+        """
+        astradb_settings = None
+        try:
+            astradb_settings = AstraDBSettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.warning(f"Failed to load AstraDB pydantic settings: {e}")
+
+        # Load the settings and validate
+        astra_application_token = astra_application_token or (
+            astradb_settings.app_token.get_secret_value() if astradb_settings and astradb_settings.app_token else None
+        )
+        assert astra_application_token is not None, "The astra_application_token cannot be None."
+        astra_id = astra_id or (astradb_settings.db_id if astradb_settings and astradb_settings.db_id else None)
+        assert astra_id is not None, "The astra_id cannot be None."
+        astra_region = astra_region or (
+            astradb_settings.region if astradb_settings and astradb_settings.region else None
+        )
+        assert astra_region is not None, "The astra_region cannot be None."
+        keyspace_name = keyspace_name or (
+            astradb_settings.keyspace if astradb_settings and astradb_settings.keyspace else None
+        )
+        assert keyspace_name is not None, "The keyspace_name cannot be None."
+
+        self._embedding_dim = embedding_dim
+        self._similarity = similarity
+        self._session = session
+
+        if self._embedding_dim > MAX_DIMENSIONALITY:
+            raise MemoryConnectorInitializationError(
+                f"Dimensionality of {self._embedding_dim} exceeds "
                 + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
             )
-        self._pinecone_api_key = api_key
-        self._default_dimensionality = default_dimensionality
 
-        self.pinecone = Pinecone(api_key=self._pinecone_api_key)
-        self.collection_names_cache = set()
+        self._client = AstraClient(
+            astra_id=astra_id,
+            astra_region=astra_region,
+            astra_application_token=astra_application_token,
+            keyspace_name=keyspace_name,
+            embedding_dim=embedding_dim,
+            similarity_function=similarity,
+            session=self._session,
+        )
+
+    async def get_collections(self) -> List[str]:
+        """Gets the list of collections.
+
+        Returns:
+            List[str] -- The list of collections.
+        """
+        return await self._client.find_collections(False)
 
     async def create_collection(
         self,
         collection_name: str,
         dimension_num: Optional[int] = None,
         distance_type: Optional[str] = "cosine",
-        index_spec: NamedTuple = DEFAULT_INDEX_SPEC,
     ) -> None:
-        """Creates a new collection in Pinecone if it does not exist.
-            This function creates an index, by default the following index
-            settings are used: metric = cosine, cloud = aws, region = us-east-1.
+        """Creates a new collection in Astra if it does not exist.
 
         Arguments:
             collection_name {str} -- The name of the collection to create.
-            In Pinecone, a collection is represented as an index. The concept
-            of "collection" in Pinecone is just a static copy of an index.
-
+            dimension_num {int} -- The dimension of the vectors to be stored in this collection.
+            distance_type {str} -- Specifies the similarity metric to be used when querying or comparing vectors within
+            this collection. The available options are dot_product, euclidean, and cosine.
         Returns:
             None
         """
-        if dimension_num is None:
-            dimension_num = self._default_dimensionality
+        dimension_num = dimension_num if dimension_num is not None else self._embedding_dim
+        distance_type = distance_type if distance_type is not None else self._similarity
+
         if dimension_num > MAX_DIMENSIONALITY:
-            raise ServiceInitializationError(
+            raise ValueError(
                 f"Dimensionality of {dimension_num} exceeds " + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
             )
 
-        if not await self.does_collection_exist(collection_name):
-            self.pinecone.create_index(
-                name=collection_name, dimension=dimension_num, metric=distance_type, spec=index_spec
-            )
-            self.collection_names_cache.add(collection_name)
-
-    async def describe_collection(self, collection_name: str) -> Optional[IndexDescription]:
-        """Gets the description of the index.
-        Arguments:
-            collection_name {str} -- The name of the index to get.
-        Returns:
-            Optional[dict] -- The index.
-        """
-        if await self.does_collection_exist(collection_name):
-            return self.pinecone.describe_index(collection_name)
-        return None
-
-    async def get_collections(
-        self,
-    ) -> IndexList:
-        """Gets the list of collections.
-
-        Returns:
-            IndexList -- The list of collections.
-        """
-        return self.pinecone.list_indexes()
+        result = await self._client.create_collection(collection_name, dimension_num, distance_type)
+        if result is True:
+            logger.info(f"Collection {collection_name} created.")
 
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection.
 
         Arguments:
             collection_name {str} -- The name of the collection to delete.
 
         Returns:
             None
         """
-        if await self.does_collection_exist(collection_name):
-            self.pinecone.delete_index(collection_name)
-            self.collection_names_cache.discard(collection_name)
+        result = await self._client.delete_collection(collection_name)
+        logger.log(
+            logging.INFO if result is True else logging.WARNING,
+            f"Collection {collection_name} {'deleted.' if result is True else 'does not exist.'}",
+        )
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to check.
 
         Returns:
             bool -- True if the collection exists; otherwise, False.
         """
-        if collection_name in self.collection_names_cache:
-            return True
-
-        index_collection_names = self.pinecone.list_indexes().names()
-        self.collection_names_cache |= set(index_collection_names)
-
-        return collection_name in index_collection_names
+        return await self._client.find_collection(collection_name)
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
-        """Upserts a record.
+        """Upserts a memory record into the data store. Does not guarantee that the collection exists.
+            If the record already exists, it will be updated.
+            If the record does not exist, it will be created.
 
         Arguments:
-            collection_name {str} -- The name of the collection to upsert the record into.
-            record {MemoryRecord} -- The record to upsert.
+            collection_name {str} -- The name associated with a collection of embeddings.
+            record {MemoryRecord} -- The memory record to upsert.
 
         Returns:
-            str -- The unique database key of the record. In Pinecone, this is the record ID.
+            str -- The unique identifier for the memory record.
         """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+        filter = {"_id": record._id}
+        update = {"$set": build_payload(record)}
+        status = await self._client.update_document(collection_name, filter, update, True)
 
-        collection = self.pinecone.Index(collection_name)
-
-        upsert_response = collection.upsert(
-            vectors=[(record._id, record.embedding.tolist(), build_payload(record))],
-            namespace="",
-        )
-
-        if upsert_response.upserted_count is None:
-            raise ServiceResponseException(f"Error upserting record: {upsert_response.message}")
-
-        return record._id
+        return status["upsertedId"] if "upsertedId" in status else record._id
 
     async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
-        """Upserts a batch of records.
+        """Upserts a batch of memory records into the data store. Does not guarantee that the collection exists.
+            If the record already exists, it will be updated.
+            If the record does not exist, it will be created.
 
         Arguments:
-            collection_name {str} -- The name of the collection to upsert the records into.
-            records {List[MemoryRecord]} -- The records to upsert.
+            collection_name {str} -- The name associated with a collection of embeddings.
+            records {List[MemoryRecord]} -- The memory records to upsert.
 
         Returns:
-            List[str] -- The unique database keys of the records.
+            List[str] -- The unique identifiers for the memory record.
         """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
-
-        collection = self.pinecone.Index(collection_name)
-
-        vectors = [
-            (
-                record._id,
-                record.embedding.tolist(),
-                build_payload(record),
-            )
-            for record in records
-        ]
-
-        upsert_response = collection.upsert(vectors, namespace="", batch_size=MAX_UPSERT_BATCH_SIZE)
-
-        if upsert_response.upserted_count is None:
-            raise ServiceResponseException(f"Error upserting record: {upsert_response.message}")
-        else:
-            return [record._id for record in records]
+        return await asyncio.gather(*[self.upsert(collection_name, record) for record in records])
 
     async def get(self, collection_name: str, key: str, with_embedding: bool = False) -> MemoryRecord:
-        """Gets a record.
+        """Gets a record. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the record from.
             key {str} -- The unique database key of the record.
             with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
 
         Returns:
             MemoryRecord -- The record.
         """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
-
-        collection = self.pinecone.Index(collection_name)
-        fetch_response = collection.fetch([key])
+        filter = {"_id": key}
+        documents = await self._client.find_documents(
+            collection_name=collection_name,
+            filter=filter,
+            include_vector=with_embedding,
+        )
 
-        if len(fetch_response.vectors) == 0:
-            raise ServiceResourceNotFoundError(f"Record with key '{key}' does not exist")
+        if len(documents) == 0:
+            raise KeyError(f"Record with key '{key}' does not exist")
 
-        return parse_payload(fetch_response.vectors[key], with_embedding)
+        return parse_payload(documents[0])
 
     async def get_batch(
         self, collection_name: str, keys: List[str], with_embeddings: bool = False
     ) -> List[MemoryRecord]:
-        """Gets a batch of records.
+        """Gets a batch of records. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the records from.
             keys {List[str]} -- The unique database keys of the records.
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
         Returns:
             List[MemoryRecord] -- The records.
         """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        fetch_response = await self.__get_batch(collection_name, keys, with_embeddings)
-        return [parse_payload(fetch_response.vectors[key], with_embeddings) for key in fetch_response.vectors.keys()]
+        filter = {"_id": {"$in": keys}}
+        documents = await self._client.find_documents(
+            collection_name=collection_name,
+            filter=filter,
+            include_vector=with_embeddings,
+        )
+        return [parse_payload(document) for document in documents]
 
     async def remove(self, collection_name: str, key: str) -> None:
-        """Removes a record.
+        """Removes a memory record from the data store. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the record from.
-            key {str} -- The unique database key of the record to remove.
+            key {str} -- The unique id associated with the memory record to remove.
 
         Returns:
             None
         """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
-
-        collection = self.pinecone.Index(collection_name)
-        collection.delete([key])
+        filter = {"_id": key}
+        await self._client.delete_documents(collection_name, filter)
 
     async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
-        """Removes a batch of records.
+        """Removes a batch of records. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the records from.
-            keys {List[str]} -- The unique database keys of the records to remove.
+            keys {List[str]} -- The unique ids associated with the memory records to remove.
 
         Returns:
             None
         """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
-
-        collection = self.pinecone.Index(collection_name)
-        for i in range(0, len(keys), MAX_DELETE_BATCH_SIZE):
-            collection.delete(keys[i : i + MAX_DELETE_BATCH_SIZE])
-        collection.delete(keys)
+        filter = {"_id": {"$in": keys}}
+        await self._client.delete_documents(collection_name, filter)
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
     ) -> Tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using cosine similarity.
-
         Arguments:
-            collection_name {str} -- The name of the collection to get the nearest match from.
-            embedding {ndarray} -- The embedding to find the nearest match to.
-            min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
-            with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
+            collection_name {str} -- The name of the collection to get the nearest matches from.
+            embedding {ndarray} -- The embedding to find the nearest matches to.
+            min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
+            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
         Returns:
             Tuple[MemoryRecord, float] -- The record and the relevance score.
         """
         matches = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
@@ -312,73 +293,39 @@
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
     ) -> List[Tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using cosine similarity.
-
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest matches from.
             embedding {ndarray} -- The embedding to find the nearest matches to.
             limit {int} -- The maximum number of matches to return.
             min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
         Returns:
             List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
         """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+        matches = await self._client.find_documents(
+            collection_name=collection_name,
+            vector=embedding.tolist(),
+            limit=limit,
+            include_similarity=True,
+            include_vector=with_embeddings,
+        )
 
-        collection = self.pinecone.Index(collection_name)
+        if min_relevance_score:
+            matches = [match for match in matches if match["$similarity"] >= min_relevance_score]
 
-        if limit > MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE:
-            raise ServiceInvalidRequestError(
-                "Limit must be less than or equal to " + f"{MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE}"
-            )
-        elif limit > MAX_QUERY_WITH_METADATA_BATCH_SIZE:
-            query_response = collection.query(
-                vector=embedding.tolist(),
-                top_k=limit,
-                include_values=False,
-                include_metadata=False,
-            )
-            keys = [match.id for match in query_response.matches]
-            fetch_response = await self.__get_batch(collection_name, keys, with_embeddings)
-            vectors = fetch_response.vectors
-            for match in query_response.matches:
-                vectors[match.id].update(match)
-            matches = [vectors[key] for key in vectors.keys()]
-        else:
-            query_response = collection.query(
-                vector=embedding.tolist(),
-                top_k=limit,
-                include_values=with_embeddings,
-                include_metadata=True,
-            )
-            matches = query_response.matches
-        if min_relevance_score is not None:
-            matches = [match for match in matches if match.score >= min_relevance_score]
         return (
             [
                 (
-                    parse_payload(match, with_embeddings),
-                    match["score"],
+                    parse_payload(match),
+                    match["$similarity"],
                 )
                 for match in matches
             ]
             if len(matches) > 0
             else []
         )
-
-    async def __get_batch(
-        self, collection_name: str, keys: List[str], with_embeddings: bool = False
-    ) -> "FetchResponse":
-        index = self.pinecone.Index(collection_name)
-        if len(keys) > MAX_FETCH_BATCH_SIZE:
-            fetch_response = index.fetch(keys[0:MAX_FETCH_BATCH_SIZE])
-            for i in range(MAX_FETCH_BATCH_SIZE, len(keys), MAX_FETCH_BATCH_SIZE):
-                fetch_response.vectors.update(index.fetch(keys[i : i + MAX_FETCH_BATCH_SIZE]).vectors)
-        else:
-            fetch_response = index.fetch(keys)
-        return fetch_response
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from typing import List, Optional, Tuple
 
 import numpy as np
 from numpy import ndarray
 from psycopg import Cursor
 from psycopg.sql import SQL, Identifier
 from psycopg_pool import ConnectionPool
+from pydantic import ValidationError
 
+from semantic_kernel.connectors.memory.postgres.postgres_settings import PostgresSettings
 from semantic_kernel.exceptions import (
     ServiceInitializationError,
     ServiceResourceNotFoundError,
     ServiceResponseException,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
@@ -37,29 +39,41 @@
     def __init__(
         self,
         connection_string: str,
         default_dimensionality: int,
         min_pool: int,
         max_pool: int,
         schema: str = DEFAULT_SCHEMA,
-        **kwargs,
+        env_file_path: str | None = None,
     ) -> None:
         """Initializes a new instance of the PostgresMemoryStore class.
 
         Arguments:
             connection_string {str} -- The connection string to the Postgres database.\n
             default_dimensionality {int} -- The default dimensionality of the embeddings.\n
             min_pool {int} -- The minimum number of connections in the connection pool.\n
             max_pool {int} -- The maximum number of connections in the connection pool.\n
             schema {str} -- The schema to use. (default: {"public"})\n
             timezone_offset {Optional[str]} -- The timezone offset to use. (default: {None})
-            Expected format '-7:00'. Uses the local timezone offset when not provided.\n
+                Expected format '-7:00'. Uses the local timezone offset when not provided.\n
+            env_file_path {str | None} -- Use the environment settings file as a fallback
+                to environment variables. (Optional)
         """
-        if kwargs.get("logger"):
-            logger.warning("The `logger` parameter is deprecated. Please use the `logging` module instead.")
+        postgres_settings = None
+        try:
+            postgres_settings = PostgresSettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.warning(f"Failed to load Postgres pydantic settings: {e}")
+
+        connection_string = connection_string or (
+            postgres_settings.connection_string.get_secret_value()
+            if postgres_settings and postgres_settings.connection_string
+            else None
+        )
+
         self._check_dimensionality(default_dimensionality)
 
         self._connection_string = connection_string
         self._default_dimensionality = default_dimensionality
         self._connection_pool = ConnectionPool(self._connection_string, min_size=min_pool, max_size=max_pool)
         self._schema = schema
         atexit.register(self._connection_pool.close)
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/README.md` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 import logging
 from typing import List, Tuple
 
 import numpy as np
 import redis
 from numpy import ndarray
+from pydantic import ValidationError
 from redis.commands.search.field import TextField, VectorField
 from redis.commands.search.indexDefinition import IndexDefinition, IndexType
 from redis.commands.search.query import Query
 from redis.exceptions import ResponseError
 
+from semantic_kernel.connectors.memory.redis.redis_settings import RedisSettings
 from semantic_kernel.connectors.memory.redis.utils import (
     deserialize_document_to_record,
     deserialize_redis_to_record,
     get_redis_key,
     serialize_record_to_redis,
 )
 from semantic_kernel.exceptions import (
@@ -46,32 +48,43 @@
         self,
         connection_string: str,
         vector_size: int = 1536,
         vector_distance_metric: str = "COSINE",
         vector_type: str = "FLOAT32",
         vector_index_algorithm: str = "HNSW",
         query_dialect: int = 2,
-        **kwargs,
+        env_file_path: str | None = None,
     ) -> None:
         """
         RedisMemoryStore is an abstracted interface to interact with a Redis node connection.
         See documentation about connections: https://redis-py.readthedocs.io/en/stable/connections.html
         See documentation about vector attributes: https://redis.io/docs/stack/search/reference/vectors
 
         Arguments:
             connection_string {str} -- Provide connection URL to a Redis instance
             vector_size {str} -- Size of vectors, defaults to 1536
             vector_distance_metric {str} -- Metric for measuring vector distances, defaults to COSINE
             vector_type {str} -- Vector type, defaults to FLOAT32
             vector_index_algorithm {str} -- Indexing algorithm for vectors, defaults to HNSW
             query_dialect {int} -- Query dialect, must be 2 or greater for vector similarity searching, defaults to 2
-
+            env_file_path {str | None} -- Use the environment settings file as a fallback to
+                environment variables, defaults to False
         """
-        if kwargs.get("logger"):
-            logger.warning("The `logger` parameter is deprecated. Please use the `logging` module instead.")
+        redis_settings = None
+        try:
+            redis_settings = RedisSettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.warning(f"Failed to load Redis pydantic settings: {e}")
+
+        connection_string = connection_string or (
+            redis_settings.connection_string.get_secret_value()
+            if redis_settings and redis_settings.connection_string
+            else None
+        )
+
         if vector_size <= 0:
             raise ServiceInitializationError("Vector dimension must be a positive integer")
 
         self._database = redis.Redis.from_url(connection_string)
         self._ft = self._database.ft
 
         self._query_dialect = query_dialect
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/utils.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import asyncio
 import logging
 from dataclasses import dataclass
 from typing import List, Tuple
 
 import numpy as np
 import weaviate
-from weaviate.embedded import EmbeddedOptions
+from pydantic import ValidationError
 
-from semantic_kernel.exceptions import ServiceInitializationError
+from semantic_kernel.connectors.memory.weaviate.weaviate_settings import WeaviateSettings
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 SCHEMA = {
     "class": "MemoryRecord",
@@ -111,33 +111,67 @@
         @classmethod
         def remove_underscore_prefix(cls, sk_dict):
             """
             Used to initialize a MemoryRecord from a SK's dict of private attribute-values.
             """
             return {key.lstrip("_"): value for key, value in sk_dict.items()}
 
-    def __init__(self, config: WeaviateConfig, **kwargs):
-        if kwargs.get("logger"):
-            logger.warning("The `logger` parameter is deprecated. Please use the `logging` module instead.")
-        self.config = config
-        self.client = self._initialize_client()
+    def __init__(self, config: WeaviateConfig | None = None, env_file_path: str | None = None):
+        """Initializes a new instance of the WeaviateMemoryStore
+
+        Optional parameters:
+        - env_file_path {str | None} -- Whether to use the environment settings (.env) file. Defaults to False.
+        """
 
-    def _initialize_client(self):
-        if self.config.use_embed:
-            return weaviate.Client(embedded_options=EmbeddedOptions())
-        elif self.config.url:
-            if self.config.api_key:
-                return weaviate.Client(
-                    url=self.config.url,
-                    auth_client_secret=weaviate.auth.AuthApiKey(api_key=self.config.api_key),
-                )
-            else:
-                return weaviate.Client(url=self.config.url)
+        # Initialize settings from environment variables or defaults defined in WeaviateSettings
+        weaviate_settings = None
+        try:
+            weaviate_settings = WeaviateSettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.warning(f"Failed to load WeaviateSettings pydantic settings: {e}")
+
+        # Override settings with provided config if available
+        if config:
+            self.settings = self.merge_settings(weaviate_settings, config)
         else:
-            raise ServiceInitializationError("Weaviate config must have either url or use_embed set")
+            self.settings = weaviate_settings
+
+        self.settings.validate_settings()
+        self.client = self._initialize_client()
+
+    def merge_settings(self, default_settings: WeaviateSettings, config: WeaviateConfig) -> WeaviateSettings:
+        """
+        Merges default settings with configuration provided through WeaviateConfig.
+
+        This function allows for manual overriding of settings from the config parameter.
+        """
+        return WeaviateSettings(
+            url=config.url or (str(default_settings.url) if default_settings and default_settings.url else None),
+            api_key=config.api_key
+            or (default_settings.api_key.get_secret_value() if default_settings and default_settings.api_key else None),
+            use_embed=(
+                config.use_embed
+                if config.use_embed is not None
+                else (default_settings.use_embed if default_settings and default_settings.use_embed else False)
+            ),
+        )
+
+    def _initialize_client(self) -> weaviate.Client:
+        """
+        Initializes the Weaviate client based on the combined settings.
+        """
+        if self.settings.use_embed:
+            return weaviate.Client(embedded_options=weaviate.EmbeddedOptions())
+
+        if self.settings.api_key:
+            return weaviate.Client(
+                url=self.settings.url, auth_client_secret=weaviate.auth.AuthApiKey(api_key=self.settings.api_key)
+            )
+
+        return weaviate.Client(url=self.settings.url)
 
     async def create_collection(self, collection_name: str) -> None:
         schema = SCHEMA.copy()
         schema["class"] = collection_name
         await asyncio.get_running_loop().run_in_executor(None, self.client.schema.create_class, schema)
 
     async def get_collections(self) -> List[str]:
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/openai_utils.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/openai_utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from __future__ import annotations
 
 from typing import Any, Awaitable, Callable, List
 from urllib.parse import urlparse
 
+import httpx
 from pydantic import Field
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 AuthCallbackType = Callable[..., Awaitable[Any]]
 
 
 class OpenAPIFunctionExecutionParameters(KernelBaseModel):
     """OpenAPI function execution parameters."""
 
-    http_client: Any | None = None
+    http_client: httpx.AsyncClient | None = None
     auth_callback: AuthCallbackType | None = None
     server_url_override: str | None = None
     ignore_non_compliant_errors: bool = False
     user_agent: str | None = None
     enable_dynamic_payload: bool = True
     enable_payload_namespacing: bool = False
     operations_to_exclude: List[str] = Field(default_factory=list)
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,64 +8,70 @@
 
 from semantic_kernel.connectors.search_engine.connector import ConnectorBase
 from semantic_kernel.exceptions import ServiceInitializationError, ServiceInvalidRequestError
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-class BingConnector(ConnectorBase):
+class GoogleConnector(ConnectorBase):
     """
-    A search engine connector that uses the Bing Search API to perform a web search
+    A search engine connector that uses the Google Custom Search API to perform a web search.
     """
 
     _api_key: str
+    _search_engine_id: str
 
-    def __init__(self, api_key: str) -> None:
+    def __init__(self, api_key: str, search_engine_id: str) -> None:
         self._api_key = api_key
+        self._search_engine_id = search_engine_id
 
         if not self._api_key:
-            raise ServiceInitializationError(
-                "Bing API key cannot be null. Please set environment variable BING_API_KEY."
-            )
+            raise ServiceInitializationError("Google Custom Search API key cannot be null.")
+
+        if not self._search_engine_id:
+            raise ServiceInitializationError("Google search engine ID cannot be null.")
 
     async def search(self, query: str, num_results: int = 1, offset: int = 0) -> List[str]:
         """
-        Returns the search results of the query provided by pinging the Bing web search API.
+        Returns the search results of the query provided by pinging the Google Custom search API.
         Returns `num_results` results and ignores the first `offset`.
 
         :param query: search query
         :param num_results: the number of search results to return
         :param offset: the number of search results to ignore
         :return: list of search results
         """
         if not query:
             raise ServiceInvalidRequestError("query cannot be 'None' or empty.")
 
         if num_results <= 0:
             raise ServiceInvalidRequestError("num_results value must be greater than 0.")
-        if num_results >= 50:
-            raise ServiceInvalidRequestError("num_results value must be less than 50.")
+        if num_results > 10:
+            raise ServiceInvalidRequestError("num_results value must be less than or equal to 10.")
 
         if offset < 0:
             raise ServiceInvalidRequestError("offset must be greater than 0.")
 
         logger.info(
-            f"Received request for bing web search with \
+            f"Received request for google search with \
                 params:\nquery: {query}\nnum_results: {num_results}\noffset: {offset}"
         )
 
-        _base_url = "https://api.bing.microsoft.com/v7.0/search"
-        _request_url = f"{_base_url}?q={urllib.parse.quote_plus(query)}&count={num_results}&offset={offset}"
-
-        logger.info(f"Sending GET request to {_request_url}")
+        _base_url = "https://www.googleapis.com/customsearch/v1"
+        _request_url = (
+            f"{_base_url}?q={urllib.parse.quote_plus(query)}"
+            f"&key={self._api_key}&cx={self._search_engine_id}"
+            f"&num={num_results}&start={offset}"
+        )
 
-        headers = {"Ocp-Apim-Subscription-Key": self._api_key}
+        logger.info("Sending GET request to Google Search API.")
 
         async with aiohttp.ClientSession() as session:
-            async with session.get(_request_url, headers=headers, raise_for_status=True) as response:
+            async with session.get(_request_url, raise_for_status=True) as response:
                 if response.status == 200:
                     data = await response.json()
-                    pages = data.get("webPages", {}).get("value")
-                    if pages:
-                        return list(map(lambda x: x["snippet"], pages)) or []
+                    logger.info("Request successful.")
+                    logger.info(f"API Response: {data}")
+                    return [x["snippet"] for x in data["items"]]
                 else:
+                    logger.error(f"Request to Google Search API failed with status code: {response.status}.")
                     return []
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/telemetry.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/telemetry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/connectors/utils/document_loader.py` & `semantic_kernel-0.9.9b1/semantic_kernel/connectors/utils/document_loader.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/contents/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/contents/chat_history.py` & `semantic_kernel-0.9.9b1/semantic_kernel/contents/chat_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 from functools import singledispatchmethod
+from html import unescape
 from typing import Any, Generator
 from xml.etree.ElementTree import Element, tostring
 
 from defusedxml.ElementTree import XML, ParseError
 from pydantic import field_validator
 
 from semantic_kernel.contents.author_role import AuthorRole
@@ -216,14 +217,21 @@
     def __str__(self) -> str:
         """Return a string representation of the history."""
         chat_history_xml = Element(CHAT_HISTORY_TAG)
         for message in self.messages:
             chat_history_xml.append(message.to_element())
         return tostring(chat_history_xml, encoding="unicode", short_empty_elements=True)
 
+    def to_prompt(self) -> str:
+        """Return a string representation of the history."""
+        chat_history_xml = Element(CHAT_HISTORY_TAG)
+        for message in self.messages:
+            chat_history_xml.append(message.to_element())
+        return tostring(chat_history_xml, encoding="unicode", short_empty_elements=True)
+
     def __iter__(self) -> Generator[ChatMessageContent, None, None]:  # type: ignore
         """Return an iterator over the messages in the history."""
         yield from self.messages
 
     def __eq__(self, other: Any) -> bool:
         """Check if two ChatHistory instances are equal."""
         if not isinstance(other, ChatHistory):
@@ -238,32 +246,32 @@
 
         Args:
             rendered_prompt (str): The rendered prompt to convert to a ChatHistory instance.
 
         Returns:
             ChatHistory: The ChatHistory instance created from the rendered prompt.
         """
-        prompt_tag = "prompt"
+        prompt_tag = "root"
         messages: list["ChatMessageContent"] = []
         prompt = rendered_prompt.strip()
         try:
             xml_prompt = XML(text=f"<{prompt_tag}>{prompt}</{prompt_tag}>")
         except ParseError:
             logger.info(f"Could not parse prompt {prompt} as xml, treating as text")
-            return cls(messages=[ChatMessageContent(role=AuthorRole.USER, content=prompt)])
+            return cls(messages=[ChatMessageContent(role=AuthorRole.USER, content=unescape(prompt))])
         if xml_prompt.text and xml_prompt.text.strip():
-            messages.append(ChatMessageContent(role=AuthorRole.SYSTEM, content=xml_prompt.text.strip()))
+            messages.append(ChatMessageContent(role=AuthorRole.SYSTEM, content=unescape(xml_prompt.text.strip())))
         for item in xml_prompt:
             if item.tag == CHAT_MESSAGE_CONTENT_TAG:
                 messages.append(ChatMessageContent.from_element(item))
             elif item.tag == CHAT_HISTORY_TAG:
                 for message in item:
                     messages.append(ChatMessageContent.from_element(message))
             if item.tail and item.tail.strip():
-                messages.append(ChatMessageContent(role=AuthorRole.USER, content=item.tail.strip()))
+                messages.append(ChatMessageContent(role=AuthorRole.USER, content=unescape(item.tail.strip())))
         if len(messages) == 1 and messages[0].role == AuthorRole.SYSTEM:
             messages[0].role = AuthorRole.USER
         return cls(messages=messages)
 
     def serialize(self) -> str:
         """
         Serializes the ChatHistory instance to a JSON string.
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/contents/chat_message_content.py` & `semantic_kernel-0.9.9b1/semantic_kernel/contents/chat_message_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 from enum import Enum
+from html import unescape
 from typing import Any, Union, overload
 from xml.etree.ElementTree import Element
 
 from defusedxml import ElementTree
 from pydantic import Field
 
 from semantic_kernel.contents.author_role import AuthorRole
@@ -237,25 +238,29 @@
             element: Element - The XML Element to create the ChatMessageContent from.
 
         Returns:
             ChatMessageContent - The new instance of ChatMessageContent or a subclass.
         """
         kwargs: dict[str, Any] = {key: value for key, value in element.items()}
         items: list[KernelContent] = []
+        if element.text:
+            items.append(TextContent(text=unescape(element.text)))
         for child in element:
             if child.tag not in TAG_CONTENT_MAP:
                 logger.warning('Unknown tag "%s" in ChatMessageContent, treating as text', child.tag)
                 text = ElementTree.tostring(child, encoding="unicode", short_empty_elements=False)
-                items.append(TextContent(text=text or ""))
+                items.append(TextContent(text=unescape(text) or ""))
             else:
                 items.append(TAG_CONTENT_MAP[child.tag].from_element(child))  # type: ignore
-        if items:
+        if len(items) == 1 and isinstance(items[0], TextContent):
+            kwargs["content"] = items[0].text
+        elif all(isinstance(item, TextContent) for item in items):
+            kwargs["content"] = "".join(item.text for item in items)  # type: ignore
+        else:
             kwargs["items"] = items
-        if element.text:
-            kwargs["content"] = element.text
         if "choice_index" in kwargs and cls is ChatMessageContent:
             logger.warning(
                 "Seems like you are trying to create a StreamingChatMessageContent, "
                 "use StreamingChatMessageContent.from_element instead, ignoring that field "
                 " and creating a ChatMessageContent instance."
             )
             kwargs.pop("choice_index")
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/contents/function_call_content.py` & `semantic_kernel-0.9.9b1/semantic_kernel/contents/function_call_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import json
 import logging
+from functools import cached_property
 from typing import TYPE_CHECKING, Any
 from xml.etree.ElementTree import Element
 
 from semantic_kernel.contents.const import FUNCTION_CALL_CONTENT_TAG
 from semantic_kernel.contents.kernel_content import KernelContent
 from semantic_kernel.exceptions import FunctionCallInvalidArgumentsException, FunctionCallInvalidNameException
 
@@ -20,14 +21,24 @@
     """Class to hold a function call response."""
 
     id: str | None
     index: int | None = None
     name: str | None = None
     arguments: str | None = None
 
+    @cached_property
+    def function_name(self) -> str:
+        """Get the function name."""
+        return self.split_name()[1]
+
+    @cached_property
+    def plugin_name(self) -> str | None:
+        """Get the plugin name."""
+        return self.split_name()[0]
+
     def __str__(self) -> str:
         return f"{self.name}({self.arguments})"
 
     def __add__(self, other: "FunctionCallContent | None") -> "FunctionCallContent":
         """Add two function calls together, combines the arguments, ignores the name."""
         if not other:
             return self
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/contents/function_result_content.py` & `semantic_kernel-0.9.9b1/semantic_kernel/contents/function_result_content.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
+from functools import cached_property
 from typing import TYPE_CHECKING, Any
 from xml.etree.ElementTree import Element
 
 from pydantic import field_validator
 
 from semantic_kernel.contents.const import FUNCTION_RESULT_CONTENT_TAG, TEXT_CONTENT_TAG
 from semantic_kernel.contents.kernel_content import KernelContent
@@ -40,14 +41,24 @@
     """
 
     id: str
     name: str | None = None
     result: str
     encoding: str | None = None
 
+    @cached_property
+    def function_name(self) -> str:
+        """Get the function name."""
+        return self.split_name()[1]
+
+    @cached_property
+    def plugin_name(self) -> str | None:
+        """Get the plugin name."""
+        return self.split_name()[0]
+
     @field_validator("result", mode="before")
     @classmethod
     def _validate_result(cls, result: Any):
         if not isinstance(result, str):
             result = str(result)
         return result
 
@@ -97,7 +108,15 @@
 
     def to_dict(self) -> dict[str, str]:
         """Convert the instance to a dictionary."""
         return {
             "tool_call_id": self.id,
             "content": self.result,
         }
+
+    def split_name(self) -> list[str]:
+        """Split the name into a plugin and function name."""
+        if not self.name:
+            raise ValueError("Name is not set.")
+        if "-" not in self.name:
+            return ["", self.name]
+        return self.name.split("-", maxsplit=1)
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/contents/kernel_content.py` & `semantic_kernel-0.9.9b1/semantic_kernel/contents/kernel_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_chat_message_content.py` & `semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_chat_message_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,10 +230,7 @@
                 value = value.value
             if isinstance(value, int):
                 value = str(value)
             root.set(field, value)
         for index, item in enumerate(self.items):
             root.insert(index, item.to_element())
         return root
-        for index, item in enumerate(self.items):
-            root.insert(index, item.to_element())
-        return root
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_content_mixin.py` & `semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_content_mixin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_text_content.py` & `semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_text_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/contents/text_content.py` & `semantic_kernel-0.9.9b1/semantic_kernel/contents/text_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
+from html import unescape
 from xml.etree.ElementTree import Element
 
 from semantic_kernel.contents.const import TEXT_CONTENT_TAG
 from semantic_kernel.contents.kernel_content import KernelContent
 
 
 class TextContent(KernelContent):
@@ -42,12 +43,12 @@
 
     @classmethod
     def from_element(cls, element: Element) -> "TextContent":
         """Create an instance from an Element."""
         if element.tag != TEXT_CONTENT_TAG:
             raise ValueError(f"Element tag is not {TEXT_CONTENT_TAG}")
 
-        return TextContent(text=element.text or "", encoding=element.get("encoding", None))
+        return TextContent(text=unescape(element.text) if element.text else "", encoding=element.get("encoding", None))
 
     def to_dict(self) -> dict[str, str]:
         """Convert the instance to a dictionary."""
         return {"type": "text", "text": self.text}
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/contents/types.py` & `semantic_kernel-0.9.9b1/semantic_kernel/contents/types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/conversation_summary_plugin.py` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/conversation_summary_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/http_plugin.py` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/http_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/math_plugin.py` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/math_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/README.md` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 service_id = "azure_oai"
 chat_service = AzureChatCompletion(
     service_id=service_id, **azure_openai_settings_from_dot_env_as_dict(include_api_version=True)
 )
 kernel.add_service(chat_service)
 
 python_code_interpreter = SessionsPythonTool(
-    **azure_container_apps_settings_from_dot_env_as_dict(), auth_callback=auth_callback
+    auth_callback=auth_callback
 )
 
 sessions_tool = kernel.add_plugin(python_code_interpreter, "PythonCodeInterpreter")
 
 code = "import json\n\ndef add_numbers(a, b):\n    return a + b\n\nargs = '{\"a\": 1, \"b\": 1}'\nargs_dict = json.loads(args)\nprint(add_numbers(args_dict['a'], args_dict['b']))"
 result = await kernel.invoke(sessions_tool["execute_code"], code=code)
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 import logging
 import os
 import re
 from io import BufferedReader, BytesIO
 from typing import Annotated, Any, Awaitable, Callable
 
 import httpx
-from pydantic import field_validator
+from pydantic import ValidationError, field_validator
 
 from semantic_kernel.connectors.ai.open_ai.const import USER_AGENT
 from semantic_kernel.connectors.telemetry import HTTP_USER_AGENT, version_info
 from semantic_kernel.core_plugins.sessions_python_tool.sessions_python_settings import (
+    ACASessionsSettings,
     SessionsPythonSettings,
 )
 from semantic_kernel.core_plugins.sessions_python_tool.sessions_remote_file_metadata import SessionsRemoteFileMetadata
 from semantic_kernel.exceptions.function_exceptions import FunctionExecutionException
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
@@ -33,38 +34,49 @@
     pool_management_endpoint: str
     settings: SessionsPythonSettings | None = None
     auth_callback: Callable[..., Awaitable[Any]]
     http_client: httpx.AsyncClient | None = None
 
     def __init__(
         self,
-        pool_management_endpoint: str,
         auth_callback: Callable[..., Awaitable[Any]],
+        pool_management_endpoint: str | None = None,
         settings: SessionsPythonSettings | None = None,
         http_client: httpx.AsyncClient | None = None,
+        env_file_path: str | None = None,
         **kwargs,
     ):
         """Initializes a new instance of the SessionsPythonTool class."""
         if not settings:
             settings = SessionsPythonSettings()
 
         if not http_client:
             http_client = httpx.AsyncClient()
 
+        try:
+            aca_settings = ACASessionsSettings.create(env_file_path=env_file_path)
+        except ValidationError as e:
+            logger.error(f"Failed to load the ACASessionsSettings with message: {str(e)}")
+            raise FunctionExecutionException(f"Failed to load the ACASessionsSettings with message: {str(e)}") from e
+
+        endpoint = pool_management_endpoint or aca_settings.pool_management_endpoint
+
         super().__init__(
-            pool_management_endpoint=pool_management_endpoint,
+            pool_management_endpoint=endpoint,
             auth_callback=auth_callback,
             settings=settings,
             http_client=http_client,
             **kwargs,
         )
 
     @field_validator("pool_management_endpoint", mode="before")
     @classmethod
     def _validate_endpoint(cls, endpoint: str):
+        endpoint = str(endpoint)
+
         """Validates the pool management endpoint."""
         if "/python/execute" in endpoint:
             # Remove '/python/execute/' and ensure the endpoint ends with a '/'
             endpoint = endpoint.replace("/python/execute", "").rstrip("/") + "/"
         if not endpoint.endswith("/"):
             # Ensure the endpoint ends with a '/'
             endpoint = endpoint + "/"
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/text_memory_plugin.py` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/text_memory_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/text_plugin.py` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/text_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/time_plugin.py` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/time_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/wait_plugin.py` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/wait_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/web_search_engine_plugin.py` & `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/web_search_engine_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/events/function_invoked_event_args.py` & `semantic_kernel-0.9.9b1/semantic_kernel/events/function_invoked_event_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/events/function_invoking_event_args.py` & `semantic_kernel-0.9.9b1/semantic_kernel/events/function_invoking_event_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/events/kernel_events_args.py` & `semantic_kernel-0.9.9b1/semantic_kernel/events/kernel_events_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from semantic_kernel.exceptions.content_exceptions import *  # noqa: F401, F403
 from semantic_kernel.exceptions.function_exceptions import *  # noqa: F401, F403
 from semantic_kernel.exceptions.kernel_exceptions import *  # noqa: F401, F403
+from semantic_kernel.exceptions.memory_connector_exceptions import *  # noqa: F401, F403
 from semantic_kernel.exceptions.planner_exceptions import *  # noqa: F401, F403
 from semantic_kernel.exceptions.service_exceptions import *  # noqa: F401, F403
 from semantic_kernel.exceptions.template_engine_exceptions import *  # noqa: F401, F403
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/content_exceptions.py` & `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/content_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/function_exceptions.py` & `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/function_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/kernel_exceptions.py` & `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/kernel_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/planner_exceptions.py` & `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/planner_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/service_exceptions.py` & `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/service_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/template_engine_exceptions.py` & `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/template_engine_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/functions/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/functions/function_result.py` & `semantic_kernel-0.9.9b1/semantic_kernel/functions/function_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_arguments.py` & `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_arguments.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 if TYPE_CHECKING:
     from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 
 
 class KernelArguments(dict):
     def __init__(
         self,
-        settings: "PromptExecutionSettings" | list["PromptExecutionSettings"] | None = None,
+        settings: (
+            "PromptExecutionSettings" | list["PromptExecutionSettings"] | dict[str, "PromptExecutionSettings"] | None
+        ) = None,
         **kwargs: Any,
     ):
         """Initializes a new instance of the KernelArguments class,
         this is a dict-like class with the additional field for the execution_settings.
 
         This class is derived from a dict, hence behaves the same way,
         just adds the execution_settings as a dict, with service_id and the settings.
@@ -26,12 +28,14 @@
                 as that is used as the key for the dict.
             **kwargs (dict[str, Any]) -- The arguments for the function invocation, works similar to a regular dict.
         """
         super().__init__(**kwargs)
         settings_dict = None
         if settings:
             settings_dict = {}
-            if isinstance(settings, list):
+            if isinstance(settings, dict):
+                settings_dict = settings
+            elif isinstance(settings, list):
                 settings_dict = {s.service_id or "default": s for s in settings}
             else:
                 settings_dict = {settings.service_id or "default": settings}
         self.execution_settings: dict[str, "PromptExecutionSettings"] | None = settings_dict
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function.py` & `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import logging
 from abc import abstractmethod
 from collections.abc import AsyncGenerator
 from copy import copy, deepcopy
 from typing import TYPE_CHECKING, Any, Callable
 
+from semantic_kernel.const import METADATA_EXCEPTION_KEY
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.prompt_template.const import (
     HANDLEBARS_TEMPLATE_FORMAT_NAME,
@@ -188,15 +189,15 @@
         if arguments is None:
             arguments = KernelArguments(**kwargs)
         try:
             return await self._invoke_internal(kernel, arguments)
         except Exception as exc:
             logger.error(f"Error occurred while invoking function {self.name}: {exc}")
             return FunctionResult(
-                function=self.metadata, value=None, metadata={"exception": exc, "arguments": arguments}
+                function=self.metadata, value=None, metadata={METADATA_EXCEPTION_KEY: exc, "arguments": arguments}
             )
 
     @abstractmethod
     def _invoke_internal_stream(
         self,
         kernel: Kernel,
         arguments: KernelArguments,
@@ -230,15 +231,17 @@
         if arguments is None:
             arguments = KernelArguments(**kwargs)
         try:
             async for partial_result in self._invoke_internal_stream(kernel, arguments):
                 yield partial_result
         except Exception as e:
             logger.error(f"Error occurred while invoking function {self.name}: {e}")
-            yield FunctionResult(function=self.metadata, value=None, metadata={"exception": e, "arguments": arguments})
+            yield FunctionResult(
+                function=self.metadata, value=None, metadata={METADATA_EXCEPTION_KEY: e, "arguments": arguments}
+            )
 
     def function_copy(self, plugin_name: str | None = None) -> KernelFunction:
         """Copy the function, can also override the plugin_name.
 
         Args:
             plugin_name (str): The new plugin name.
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_decorator.py` & `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_decorator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
-from functools import wraps
-from inspect import Parameter, Signature, isasyncgenfunction, isgeneratorfunction, signature
-from typing import Any, Callable
+from inspect import get_annotations, isasyncgenfunction, isclass, isgeneratorfunction, signature
+from typing import Any, Callable, ForwardRef
 
 NoneType = type(None)
 logger = logging.getLogger(__name__)
 
 
 def kernel_function(
     func: Callable[..., object] | None = None,
     name: str | None = None,
     description: str | None = None,
-) -> Callable[..., object]:
+) -> Callable[..., Any]:
     """
-    Decorator for kernel functions.
+    Decorator for kernel functions, can be used directly as @kernel_function
+    or with parameters @kernel_function(name='function', description='I am a function.').
 
     This decorator is used to mark a function as a kernel function. It also provides metadata for the function.
     The name and description can be left empty, and then the function name and docstring will be used.
 
     The parameters are parsed from the function signature, use typing.Annotated to provide a description for the
     parameter, in python 3.8, use typing_extensions.Annotated.
 
@@ -33,91 +33,102 @@
     and that is stored in __kernel_function_return_type__, __kernel_function_return_description__
     and __kernel_function_return_required__.
 
     It also checks if the function is a streaming type (generator or iterable, async or not),
     and that is stored as a bool in __kernel_function_streaming__.
 
     Args:
-        name (Optional[str]) -- The name of the function, if not supplied, the function name will be used.
-        description (Optional[str]) -- The description of the function,
+        name (str | None) -- The name of the function, if not supplied, the function name will be used.
+        description (str | None) -- The description of the function,
             if not supplied, the function docstring will be used, can be None.
 
     """
 
-    @wraps(wrapped=func)  # type: ignore
     def decorator(func: Callable[..., object]) -> Callable[..., object]:
-        func.__kernel_function__ = True  # type: ignore
-        func.__kernel_function_description__ = description or func.__doc__  # type: ignore
-        func.__kernel_function_name__ = name or func.__name__  # type: ignore
-        func.__kernel_function_streaming__ = isasyncgenfunction(func) or isgeneratorfunction(func)  # type: ignore
-        logger.debug(f"Parsing decorator for function: {func.__kernel_function_name__}")  # type: ignore
-
+        setattr(func, "__kernel_function__", True)
+        setattr(func, "__kernel_function_description__", description or func.__doc__)
+        setattr(func, "__kernel_function_name__", name or getattr(func, "__name__", "unknown"))
+        setattr(func, "__kernel_function_streaming__", isasyncgenfunction(func) or isgeneratorfunction(func))
+        logger.debug(f"Parsing decorator for function: {getattr(func, '__kernel_function_name__')}")
         func_sig = signature(func)
-        logger.debug(f"{func_sig=}")
-        func.__kernel_function_parameters__ = [  # type: ignore
-            _parse_parameter(param) for param in func_sig.parameters.values() if param.name != "self"
-        ]
+        annotations = {name: None for name, _ in func_sig.parameters.items() if name != "self"}
+        try:
+            annotations.update(get_annotations(func, eval_str=True))
+        except Exception as ex:
+            logger.error(f"Failed to get annotations for function {func.__name__}: {ex}")
+        logger.debug(f"{annotations=}")
+        setattr(
+            func,
+            "__kernel_function_parameters__",
+            [_parse_parameter(name, param) for name, param in annotations.items() if name != "return"],
+        )
+        defaults = getattr(func, "__defaults__", None)
+        logger.debug(f"{defaults=}")
+        assert hasattr(func, "__kernel_function_parameters__")
+        if defaults:
+            for index, default in enumerate(defaults):
+                if default is None:
+                    continue
+                if func.__kernel_function_parameters__[index]:
+                    func.__kernel_function_parameters__[index]["default_value"] = default
+                    func.__kernel_function_parameters__[index]["is_required"] = False
         return_param_dict = {}
-        if func_sig.return_annotation != Signature.empty:
-            return_param_dict = _parse_annotation(func_sig.return_annotation)
-        func.__kernel_function_return_type__ = return_param_dict.get("type_", "None")  # type: ignore
-        func.__kernel_function_return_description__ = return_param_dict.get("description", "")  # type: ignore
-        func.__kernel_function_return_required__ = return_param_dict.get("is_required", False)  # type: ignore
+        if "return" in annotations:
+            return_param_dict = _parse_parameter("return", annotations["return"])
+        setattr(func, "__kernel_function_return_type__", return_param_dict.get("type_", "None"))
+        setattr(func, "__kernel_function_return_description__", return_param_dict.get("description", ""))
+        setattr(func, "__kernel_function_return_required__", return_param_dict.get("is_required", False))
         return func
 
     if func:
         return decorator(func)
-    return decorator  # type: ignore
-
-
-def _parse_parameter(param: Parameter) -> dict[str, Any]:
-    logger.debug(f"Parsing param: {param}")
-    ret = {}
-    if param != Parameter.empty:
-        ret = _parse_annotation(param.annotation)
-    ret["name"] = param.name
-    if param.default != Parameter.empty:
-        ret["default_value"] = param.default
-    return ret
-
+    return decorator
 
-def _parse_annotation(annotation: Parameter) -> dict[str, Any]:
-    logger.debug(f"Parsing annotation: {annotation}")
-    if annotation == Signature.empty:
-        return {"type_": "Any", "is_required": True}
-    if isinstance(annotation, str):
-        return {"type_": annotation, "is_required": True}
-    logger.debug(f"{annotation=}")
-    ret = _parse_internal_annotation(annotation, True)
-    if hasattr(annotation, "__metadata__") and annotation.__metadata__:  # type: ignore
-        ret["description"] = annotation.__metadata__[0]  # type: ignore
-    return ret
 
-
-def _parse_internal_annotation(annotation: Parameter, required: bool) -> dict[str, Any]:
-    logger.debug(f"Internal {annotation=}")
-    if hasattr(annotation, "__forward_arg__"):
-        return {"type_": annotation.__forward_arg__, "is_required": required}  # type: ignore
-    if getattr(annotation, "__name__", None) == "Optional":
-        required = False
-    if hasattr(annotation, "__args__"):
-        results = [_parse_internal_annotation(arg, required) for arg in annotation.__args__]  # type: ignore
-        type_objects = [
-            result["type_object"]
-            for result in results
-            if "type_object" in result and result["type_object"] is not NoneType
-        ]
-        str_results = [result["type_"] for result in results]
-        if "NoneType" in str_results:
-            str_results.remove("NoneType")
-            required = False
-        else:
-            required = not (any(not result["is_required"] for result in results))
-        ret = {"type_": ", ".join(str_results), "is_required": required}
-        if type_objects and len(type_objects) == 1:
-            ret["type_object"] = type_objects[0]
+def _parse_parameter(name: str, param: Any) -> dict[str, Any]:
+    logger.debug(f"Parsing param: {name}")
+    logger.debug(f"Parsing annotation: {param}")
+    ret: dict[str, Any] = {"name": name}
+    if not param:
+        ret["type_"] = "Any"
+        ret["is_required"] = True
         return ret
-    return {
-        "type_": getattr(annotation, "__name__", ""),
-        "type_object": annotation,
-        "is_required": required,
-    }
+    if not isinstance(param, str):
+        if hasattr(param, "default"):
+            ret["default_value"] = param.default
+            ret["is_required"] = False
+        else:
+            ret["is_required"] = True
+        if hasattr(param, "__metadata__"):
+            ret["description"] = param.__metadata__[0]
+        if hasattr(param, "__origin__"):
+            ret.update(_parse_parameter(name, param.__origin__))
+        if hasattr(param, "__args__"):
+            args = []
+            for arg in param.__args__:
+                if arg == NoneType:
+                    ret["is_required"] = False
+                    ret["default_value"] = None
+                    continue
+                if isinstance(arg, ForwardRef):
+                    arg = arg.__forward_arg__
+                args.append(_parse_parameter(name, arg))
+            if ret.get("type_") in ["list", "dict"]:
+                ret["type_"] = f"{ret['type_']}[{', '.join([arg['type_'] for arg in args])}]"
+            elif len(args) > 1:
+                ret["type_"] = ", ".join([arg["type_"] for arg in args])
+            else:
+                ret["type_"] = args[0]["type_"]
+                ret["type_object"] = args[0].get("type_object", None)
+                if def_value := args[0].get("default_value", None):
+                    ret["default_value"] = def_value
+        elif isclass(param):
+            ret["type_"] = param.__name__
+            ret["type_object"] = param
+        else:
+            ret["type_"] = str(param).replace(" |", ",")
+    else:
+        if "|" in param:
+            param = param.replace(" |", ",")
+        ret["type_"] = param
+        ret["is_required"] = True
+    return ret
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_from_method.py` & `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_from_method.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,51 +31,60 @@
     stream_method: Callable[..., Any] | None = None
 
     def __init__(
         self,
         method: Callable[..., Any],
         plugin_name: str | None = None,
         stream_method: Callable[..., Any] | None = None,
+        parameters: list[KernelParameterMetadata] | None = None,
+        return_parameter: KernelParameterMetadata | None = None,
+        additional_metadata: dict[str, Any] | None = None,
     ) -> None:
         """
         Initializes a new instance of the KernelFunctionFromMethod class
 
         Args:
             method (Callable[..., Any]): The method to be called
-            plugin_name (Optional[str]): The name of the plugin
-            stream_method (Optional[Callable[..., Any]]): The stream method for the function
+            plugin_name (str | None): The name of the plugin
+            stream_method (Callable[..., Any] | None): The stream method for the function
+            parameters (list[KernelParameterMetadata] | None): The parameters of the function
+            return_parameter (KernelParameterMetadata | None): The return parameter of the function
+            additional_metadata (dict[str, Any] | None): Additional metadata for the function
         """
         if method is None:
             raise FunctionInitializationError("Method cannot be `None`")
 
         if not hasattr(method, "__kernel_function__") or method.__kernel_function__ is None:
             raise FunctionInitializationError("Method is not a Kernel function")
 
         # all these fields are created when the kernel function decorator is used,
         # so no need to check before using, will raise an exception if not set
         function_name = method.__kernel_function_name__  # type: ignore
         description = method.__kernel_function_description__  # type: ignore
-        parameters = [KernelParameterMetadata(**param) for param in method.__kernel_function_parameters__]  # type: ignore
-        return_param = KernelParameterMetadata(
-            name="return",
-            description=method.__kernel_function_return_description__,  # type: ignore
-            default_value=None,
-            type=method.__kernel_function_return_type__,  # type: ignore
-            is_required=method.__kernel_function_return_required__,  # type: ignore
-        )
+        if parameters is None:
+            parameters = [KernelParameterMetadata(**param) for param in method.__kernel_function_parameters__]  # type: ignore
+        if return_parameter is None:
+            return_param = KernelParameterMetadata(
+                name="return",
+                description=method.__kernel_function_return_description__,  # type: ignore
+                default_value=None,
+                type=method.__kernel_function_return_type__,  # type: ignore
+                is_required=method.__kernel_function_return_required__,  # type: ignore
+            )
 
         try:
             metadata = KernelFunctionMetadata(
                 name=function_name,
                 description=description,
                 parameters=parameters,
                 return_parameter=return_param,
                 is_prompt=False,
                 is_asynchronous=isasyncgenfunction(method) or iscoroutinefunction(method),
                 plugin_name=plugin_name,
+                additional_properties=additional_metadata if additional_metadata is not None else {},
             )
         except ValidationError as exc:
             # reraise the exception to clarify it comes from KernelFunction init
             raise FunctionInitializationError("Failed to create KernelFunctionMetadata") from exc
 
         args: dict[str, Any] = {
             "metadata": metadata,
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_from_prompt.py` & `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_from_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 import os
+from html import unescape
 from typing import TYPE_CHECKING, Any, AsyncGenerator
 
 import yaml
 from pydantic import Field, ValidationError, model_validator
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
+from semantic_kernel.const import METADATA_EXCEPTION_KEY
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
 from semantic_kernel.contents.streaming_chat_message_content import StreamingChatMessageContent
 from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
 from semantic_kernel.contents.streaming_text_content import StreamingTextContent
 from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import FunctionExecutionException, FunctionInitializationError
@@ -184,15 +186,15 @@
         # pass the kernel in for auto function calling
         kwargs: dict[str, Any] = {}
         if hasattr(execution_settings, "function_call_behavior"):
             kwargs["kernel"] = kernel
             kwargs["arguments"] = arguments
 
         try:
-            completions = await service.complete_chat(
+            completions = await service.get_chat_message_contents(
                 chat_history=chat_history,
                 settings=execution_settings,
                 **kwargs,
             )
             if not completions:
                 raise FunctionExecutionException(f"No completions returned while invoking function {self.name}")
 
@@ -205,15 +207,15 @@
         service: TextCompletionClientBase,
         execution_settings: PromptExecutionSettings,
         prompt: str,
         arguments: KernelArguments,
     ) -> FunctionResult:
         """Handles the text service call."""
         try:
-            completions = await service.complete(prompt, execution_settings)
+            completions = await service.get_text_contents(unescape(prompt), execution_settings)
             return self._create_function_result(completions=completions, arguments=arguments, prompt=prompt)
         except Exception as exc:
             raise FunctionExecutionException(f"Error occurred while invoking function {self.name}: {exc}") from exc
 
     def _create_function_result(
         self,
         completions: list[ChatMessageContent] | list[TextContent],
@@ -282,40 +284,42 @@
         kwargs: dict[str, Any] = {}
         if hasattr(execution_settings, "function_call_behavior"):
             kwargs["kernel"] = kernel
             kwargs["arguments"] = arguments
 
         chat_history = ChatHistory.from_rendered_prompt(prompt)
         try:
-            async for partial_content in service.complete_chat_stream(
+            async for partial_content in service.get_streaming_chat_message_contents(
                 chat_history=chat_history,
                 settings=execution_settings,
                 **kwargs,
             ):
                 yield partial_content
 
             return  # Exit after processing all iterations
         except Exception as e:
             logger.error(f"Error occurred while invoking function {self.name}: {e}")
-            yield FunctionResult(function=self.metadata, value=None, metadata={"exception": e})
+            yield FunctionResult(function=self.metadata, value=None, metadata={METADATA_EXCEPTION_KEY: e})
 
     async def _handle_complete_text_stream(
         self,
         service: TextCompletionClientBase,
         execution_settings: PromptExecutionSettings,
         prompt: str,
     ) -> AsyncGenerator[FunctionResult | list[StreamingTextContent], Any]:
         """Handles the text service call."""
         try:
-            async for partial_content in service.complete_stream(prompt=prompt, settings=execution_settings):
+            async for partial_content in service.get_streaming_text_contents(
+                prompt=prompt, settings=execution_settings
+            ):
                 yield partial_content
             return
         except Exception as e:
             logger.error(f"Error occurred while invoking function {self.name}: {e}")
-            yield FunctionResult(function=self.metadata, value=None, metadata={"exception": e})
+            yield FunctionResult(function=self.metadata, value=None, metadata={METADATA_EXCEPTION_KEY: e})
 
     def add_default_values(self, arguments: KernelArguments) -> KernelArguments:
         """Gathers the function parameters from the arguments."""
         for parameter in self.prompt_template.prompt_template_config.input_variables:
             if parameter.name not in arguments and parameter.default not in {None, "", False, 0}:
                 arguments[parameter.name] = parameter.default
         return arguments
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_metadata.py` & `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from pydantic import Field
 
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.utils.validation import FUNCTION_NAME_REGEX, PLUGIN_NAME_REGEX
 
@@ -14,14 +14,15 @@
     name: str = Field(pattern=FUNCTION_NAME_REGEX)
     plugin_name: Optional[str] = Field(None, pattern=PLUGIN_NAME_REGEX)
     description: Optional[str] = Field(default=None)
     parameters: List[KernelParameterMetadata] = Field(default_factory=list)
     is_prompt: bool
     is_asynchronous: Optional[bool] = Field(default=True)
     return_parameter: Optional[KernelParameterMetadata] = None
+    additional_properties: Optional[dict[str, Any]] = Field(default=None)
 
     @property
     def fully_qualified_name(self) -> str:
         """
         Get the fully qualified name of the function.
 
         Returns:
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_parameter_metadata.py` & `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_parameter_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_plugin.py` & `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,30 +134,51 @@
             description=description,
             functions=self._validate_functions(functions=functions, plugin_name=name),
         )
 
     # region Dict-like methods
 
     def __setitem__(self, key: str, value: KERNEL_FUNCTION_TYPE) -> None:
+        """Set a function in the plugin.
+
+        This function uses plugin[function_name] = function syntax.
+
+        Args:
+            key (str): The name of the function.
+            value (KernelFunction): The function to set.
+
+        """
         self.functions[key] = KernelPlugin._parse_or_copy(value, self.name)
 
     def set(self, key: str, value: KERNEL_FUNCTION_TYPE) -> None:
         """Set a function in the plugin.
 
+        This function uses plugin.set(function_name, function) syntax.
+
         Args:
             key (str): The name of the function.
             value (KernelFunction): The function to set.
 
         """
         self[key] = value
 
     def __getitem__(self, key: str) -> KernelFunction:
+        """Get a function from the plugin.
+
+        Using plugin[function_name] syntax.
+        """
         return self.functions[key]
 
     def get(self, key: str, default: KernelFunction | None = None) -> KernelFunction | None:
+        """Get a function from the plugin.
+
+        Args:
+            key (str): The name of the function.
+            default (KernelFunction, optional): The default function to return if the key is not found.
+        """
         return self.functions.get(key, default)
 
     def update(self, *args: Any, **kwargs: KernelFunction) -> None:
         """Update the plugin with the functions from another.
 
         Args:
             *args: The functions to update the plugin with, can be a dict, list or KernelPlugin.
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/functions/prompt_rendering_result.py` & `semantic_kernel-0.9.9b1/semantic_kernel/functions/prompt_rendering_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/kernel.py` & `semantic_kernel-0.9.9b1/semantic_kernel/kernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from copy import copy
 from functools import singledispatchmethod
 from typing import TYPE_CHECKING, Any, AsyncGenerator, AsyncIterable, Callable, Literal, Type, TypeVar, Union
 
 from pydantic import Field, field_validator
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
+from semantic_kernel.const import METADATA_EXCEPTION_KEY
 from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
 from semantic_kernel.events import FunctionInvokedEventArgs, FunctionInvokingEventArgs
 from semantic_kernel.exceptions import (
     KernelFunctionAlreadyExistsError,
     KernelFunctionNotFoundError,
     KernelInvokeException,
     KernelPluginNotFoundError,
@@ -46,14 +47,15 @@
     from semantic_kernel.functions.kernel_function import KernelFunction
     from semantic_kernel.functions.types import KERNEL_FUNCTION_TYPE
 
 T = TypeVar("T")
 
 ALL_SERVICE_TYPES = Union["TextCompletionClientBase", "ChatCompletionClientBase", "EmbeddingGeneratorBase"]
 
+
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class Kernel(KernelBaseModel):
     """
     The Kernel class is the main entry point for the Semantic Kernel. It provides the ability to run
     semantic/native functions, and manage plugins, memory, and AI services.
@@ -195,15 +197,15 @@
                 f"Execution was skipped on function invoking event of function: {function.fully_qualified_name}."
             )
             return
         function_result: list[list["StreamingContentMixin"] | Any] = []
 
         async for stream_message in function.invoke_stream(self, arguments):
             if isinstance(stream_message, FunctionResult) and (
-                exception := stream_message.metadata.get("exception", None)
+                exception := stream_message.metadata.get(METADATA_EXCEPTION_KEY, None)
             ):
                 raise KernelInvokeException(
                     f"Error occurred while invoking function: '{function.fully_qualified_name}'"
                 ) from exception
             function_result.append(stream_message)
             yield stream_message
 
@@ -391,15 +393,15 @@
             template_format=template_format,
         )
 
         function_result: list[list["StreamingContentMixin"] | Any] = []
 
         async for stream_message in self.invoke_stream(function=function, arguments=arguments):
             if isinstance(stream_message, FunctionResult) and (
-                exception := stream_message.metadata.get("exception", None)
+                exception := stream_message.metadata.get(METADATA_EXCEPTION_KEY, None)
             ):
                 raise KernelInvokeException(
                     f"Error occurred while invoking function: '{function.fully_qualified_name}'"
                 ) from exception
             function_result.append(stream_message)
             yield stream_message
 
@@ -426,15 +428,17 @@
         exception: Exception | None = None,
     ) -> FunctionInvokedEventArgs:
         # TODO: include logic that uses function_result
         args = FunctionInvokedEventArgs(
             kernel_function_metadata=kernel_function_metadata,
             arguments=arguments,
             function_result=function_result,
-            exception=exception or function_result.metadata.get("exception", None) if function_result else None,
+            exception=(
+                exception or function_result.metadata.get(METADATA_EXCEPTION_KEY, None) if function_result else None
+            ),
         )
         if self.function_invoked_handlers:
             for handler in self.function_invoked_handlers.values():
                 handler(self, args)
         return args
 
     def on_function_invoking(
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/kernel_pydantic.py` & `semantic_kernel-0.9.9b1/semantic_kernel/kernel_pydantic.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.9.9b1/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.9.9b1/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.9.9b1/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.9.9b1/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         )
         for i in range(self.options.max_iterations):
             # sleep for a bit to avoid rate limiting
             if i > 0:
                 await asyncio.sleep(self.options.min_iteration_time_ms / 1000.0)  # convert ms to sec
             # For each step, request another completion to select a function for that step
             chat_history_for_steps.add_user_message(STEPWISE_USER_MESSAGE)
-            chat_result = await chat_completion.complete_chat(
+            chat_result = await chat_completion.get_chat_message_contents(
                 chat_history=chat_history_for_steps,
                 settings=prompt_execution_settings,
                 kernel=cloned_kernel,
             )
             chat_result = chat_result[0]
             chat_history_for_steps.add_message(chat_result)
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/plan.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/plan.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/planner_extensions.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/planner_options.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/planner_options.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import os
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
+from semantic_kernel.const import METADATA_EXCEPTION_KEY
 from semantic_kernel.exceptions import PlannerCreatePlanError, PlannerException, PlannerInvalidGoalError
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.kernel import Kernel
 from semantic_kernel.planners.plan import Plan
 from semantic_kernel.planners.sequential_planner.sequential_planner_config import SequentialPlannerConfig
@@ -96,18 +97,18 @@
             self._kernel, self._arguments, goal, self.config
         )
         self._arguments["available_functions"] = relevant_function_manual
         self._arguments["input"] = goal
 
         plan_result = await self._function_flow_function.invoke(self._kernel, self._arguments)
 
-        if isinstance(plan_result, FunctionResult) and "exception" in plan_result.metadata:
+        if isinstance(plan_result, FunctionResult) and METADATA_EXCEPTION_KEY in plan_result.metadata:
             raise PlannerCreatePlanError(
                 f"Error creating plan for goal: {plan_result.metadata['exception']}",
-            ) from plan_result.metadata["exception"]
+            ) from plan_result.metadata[METADATA_EXCEPTION_KEY]
 
         plan_result_string = str(plan_result).strip()
 
         try:
             plan = SequentialPlanParser.to_plan_from_xml(
                 xml_string=plan_result_string,
                 goal=goal,
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py` & `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/__init__.py` & `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/const.py` & `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/const.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/handlebars_prompt_template.py` & `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/handlebars_prompt_template.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any, Callable, Optional
 
 from pybars import Compiler, PybarsError
 from pydantic import PrivateAttr, field_validator
 
 from semantic_kernel.exceptions import HandlebarsTemplateRenderException, HandlebarsTemplateSyntaxError
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.prompt_template.const import HANDLEBARS_TEMPLATE_FORMAT_NAME
@@ -24,16 +24,19 @@
 
     Handlebars are parsed as a whole and therefore do not have variables that can be extracted,
     also with handlebars there is no distinction in syntax between a variable and a value,
     a value that is encountered is tried to resolve with the arguments and the functions,
     if not found, the literal value is returned.
 
     Args:
-        PromptTemplateConfig: The prompt template configuration
+        prompt_template_config (PromptTemplateConfig): The prompt template configuration
             This is checked if the template format is 'handlebars'
+        allow_dangerously_set_content (bool = False): Allow content without encoding throughout, this overrides
+            the same settings in the prompt template config and input variables.
+            This reverts the behavior to unencoded input.
 
     Raises:
         ValueError: If the template format is not 'handlebars'
         HandlebarsTemplateSyntaxError: If the handlebars template has a syntax error
     """
 
     _template_compiler: Any = PrivateAttr()
@@ -70,27 +73,38 @@
         Returns:
             The prompt template ready to be used for an AI request
         """
         if not self._template_compiler:
             return ""
         if arguments is None:
             arguments = KernelArguments()
-        helpers = {}
+
+        arguments = self._get_trusted_arguments(arguments)
+        allow_unsafe_function_output = self._get_allow_unsafe_function_output()
+        helpers: dict[str, Callable[..., Any]] = {}
         for plugin in kernel.plugins.values():
             helpers.update(
                 {
                     function.fully_qualified_name: create_template_helper_from_function(
-                        function, kernel, arguments, self.prompt_template_config.template_format
+                        function,
+                        kernel,
+                        arguments,
+                        self.prompt_template_config.template_format,
+                        allow_unsafe_function_output,
                     )
                     for function in plugin
                 }
             )
         helpers.update(HANDLEBAR_SYSTEM_HELPERS)
+
         try:
-            return self._template_compiler(arguments, helpers=helpers)
+            return self._template_compiler(
+                arguments,
+                helpers=helpers,
+            )
         except PybarsError as exc:
             logger.error(
                 f"Error rendering prompt template: {self.prompt_template_config.template} with arguments: {arguments}"
             )
             raise HandlebarsTemplateRenderException(
                 f"Error rendering prompt template: {self.prompt_template_config.template} "
                 f"with arguments: {arguments}: error: {exc}"
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/jinja2_prompt_template.py` & `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/jinja2_prompt_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any, Callable, Optional
 
 from jinja2 import BaseLoader, TemplateError
 from jinja2.sandbox import ImmutableSandboxedEnvironment
 from pydantic import PrivateAttr, field_validator
 
-from semantic_kernel.exceptions import Jinja2TemplateRenderException, Jinja2TemplateSyntaxError
+from semantic_kernel.exceptions import Jinja2TemplateRenderException
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.prompt_template.const import JINJA2_TEMPLATE_FORMAT_NAME
 from semantic_kernel.prompt_template.prompt_template_base import PromptTemplateBase
 from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
 from semantic_kernel.prompt_template.utils import JINJA2_SYSTEM_HELPERS, create_template_helper_from_function
 
 if TYPE_CHECKING:
@@ -31,17 +31,20 @@
     and arguments.
 
     Note that the fully qualified function name (in the form of "plugin-function") is not allowed
     in Jinja2 because of the hyphen. Therefore, the function name is replaced with an underscore,
     which are allowed in Python function names.
 
     Args:
-        template_config (PromptTemplateConfig): The configuration object for the prompt template.
+        prompt_template_config (PromptTemplateConfig): The configuration object for the prompt template.
             This should specify the template format as 'jinja2' and include any necessary
             configuration details required for rendering the template.
+        allow_dangerously_set_content (bool = False): Allow content without encoding throughout, this overrides
+            the same settings in the prompt template config and input variables.
+            This reverts the behavior to unencoded input.
 
     Raises:
         ValueError: If the template format specified in the configuration is not 'jinja2'.
         Jinja2TemplateSyntaxError: If there is a syntax error in the Jinja2 template.
     """
 
     _env: ImmutableSandboxedEnvironment = PrivateAttr()
@@ -49,23 +52,19 @@
     @field_validator("prompt_template_config")
     @classmethod
     def validate_template_format(cls, v: "PromptTemplateConfig") -> "PromptTemplateConfig":
         if v.template_format != JINJA2_TEMPLATE_FORMAT_NAME:
             raise ValueError(f"Invalid prompt template format: {v.template_format}. Expected: jinja2")
         return v
 
-    def model_post_init(self, __context: Any) -> None:
+    def model_post_init(self, _: Any) -> None:
         if not self.prompt_template_config.template:
             self._env = None
             return
-        try:
-            self._env = ImmutableSandboxedEnvironment(loader=BaseLoader())
-        except TemplateError as e:
-            logger.error(f"Invalid jinja2 template: {self.prompt_template_config.template}")
-            raise Jinja2TemplateSyntaxError(f"Invalid jinja2 template: {self.prompt_template_config.template}") from e
+        self._env = ImmutableSandboxedEnvironment(loader=BaseLoader())
 
     async def render(self, kernel: "Kernel", arguments: Optional["KernelArguments"] = None) -> str:
         """
         Using the prompt template, replace the variables with their values
         and execute the functions replacing their reference with the
         function result.
 
@@ -76,31 +75,36 @@
         Returns:
             The prompt template ready to be used for an AI request
         """
         if not self._env:
             return ""
         if arguments is None:
             arguments = KernelArguments()
-        helpers = {}
+
+        arguments = self._get_trusted_arguments(arguments)
+        allow_unsafe_function_output = self._get_allow_unsafe_function_output()
+        helpers: dict[str, Callable[..., Any]] = {}
         helpers.update(JINJA2_SYSTEM_HELPERS)
         for plugin in kernel.plugins.values():
             helpers.update(
                 {
                     function.fully_qualified_name.replace("-", "_"): create_template_helper_from_function(
                         function,
                         kernel,
                         arguments,
                         self.prompt_template_config.template_format,
+                        allow_unsafe_function_output,
                     )
                     for function in plugin
                 }
             )
         try:
             template = self._env.from_string(self.prompt_template_config.template, globals=helpers)
             return template.render(**arguments)
+
         except TemplateError as exc:
             logger.error(
                 f"Error rendering prompt template: {self.prompt_template_config.template} with arguments: {arguments}"
             )
             raise Jinja2TemplateRenderException(
                 f"Error rendering prompt template: {self.prompt_template_config.template} with "
                 f"arguments: {arguments}: error: {exc}"
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/kernel_prompt_template.py` & `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/kernel_prompt_template.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
+from html import escape
 from typing import TYPE_CHECKING, Any, List, Optional
 
 from pydantic import PrivateAttr, field_validator
 
 from semantic_kernel.exceptions import CodeBlockRenderException, TemplateRenderException
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.prompt_template.const import KERNEL_TEMPLATE_FORMAT_NAME
@@ -18,14 +19,28 @@
     from semantic_kernel.kernel import Kernel
     from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class KernelPromptTemplate(PromptTemplateBase):
+    """Create a Kernel prompt template.
+
+    Arguments:
+        prompt_template_config (PromptTemplateConfig): The prompt template configuration
+            This includes the actual template to use.
+        allow_dangerously_set_content (bool = False): Allow content without encoding throughout, this overrides
+            the same settings in the prompt template config and input variables.
+            This reverts the behavior to unencoded input.
+
+    Raises:
+        ValueError: If the template format is not 'semantic-kernel'
+        TemplateSyntaxError: If the template has a syntax error
+    """
+
     _blocks: List[Block] = PrivateAttr(default_factory=list)
 
     @field_validator("prompt_template_config")
     @classmethod
     def validate_template_format(cls, v: "PromptTemplateConfig") -> "PromptTemplateConfig":
         if v.template_format != KERNEL_TEMPLATE_FORMAT_NAME:
             raise ValueError(f"Invalid prompt template format: {v.template_format}. Expected: semantic-kernel")
@@ -105,68 +120,24 @@
         :return: The prompt template ready to be used for an AI request
         """
         from semantic_kernel.template_engine.protocols.code_renderer import CodeRenderer
         from semantic_kernel.template_engine.protocols.text_renderer import TextRenderer
 
         logger.debug(f"Rendering list of {len(blocks)} blocks")
         rendered_blocks: List[str] = []
+
+        arguments = self._get_trusted_arguments(arguments)
+        allow_unsafe_function_output = self._get_allow_unsafe_function_output()
         for block in blocks:
             if isinstance(block, TextRenderer):
                 rendered_blocks.append(block.render(kernel, arguments))
                 continue
             if isinstance(block, CodeRenderer):
                 try:
-                    rendered_blocks.append(await block.render_code(kernel, arguments))
+                    rendered = await block.render_code(kernel, arguments)
                 except CodeBlockRenderException as exc:
                     logger.error(f"Error rendering code block: {exc}")
                     raise TemplateRenderException(f"Error rendering code block: {exc}") from exc
+                rendered_blocks.append(rendered if allow_unsafe_function_output else escape(rendered))
         prompt = "".join(rendered_blocks)
         logger.debug(f"Rendered prompt: {prompt}")
         return prompt
-
-    def render_variables(
-        self, blocks: List[Block], kernel: "Kernel", arguments: Optional["KernelArguments"] = None
-    ) -> List[Block]:
-        """
-        Given a list of blocks, render the Variable Blocks, replacing
-        placeholders with the actual value in memory.
-
-        :param blocks: List of blocks, typically all the blocks found in a template
-        :param variables: Container of all the temporary variables known to the kernel
-        :return: An updated list of blocks where Variable Blocks have rendered to
-            Text Blocks
-        """
-        from semantic_kernel.template_engine.blocks.text_block import TextBlock
-
-        logger.debug("Rendering variables")
-
-        rendered_blocks: List[Block] = []
-        for block in blocks:
-            if block.type == BlockTypes.VARIABLE:
-                rendered_blocks.append(TextBlock.from_text(block.render(kernel, arguments)))
-                continue
-            rendered_blocks.append(block)
-
-        return rendered_blocks
-
-    async def render_code(self, blocks: List[Block], kernel: "Kernel", arguments: "KernelArguments") -> List[Block]:
-        """
-        Given a list of blocks, render the Code Blocks, executing the
-        functions and replacing placeholders with the functions result.
-
-        :param blocks: List of blocks, typically all the blocks found in a template
-        :param execution_context: Access into the current kernel execution context
-        :return: An updated list of blocks where Code Blocks have rendered to
-            Text Blocks
-        """
-        from semantic_kernel.template_engine.blocks.text_block import TextBlock
-
-        logger.debug("Rendering code")
-
-        rendered_blocks: List[Block] = []
-        for block in blocks:
-            if block.type == BlockTypes.CODE:
-                rendered_blocks.append(TextBlock.from_text(await block.render_code(kernel, arguments)))
-                continue
-            rendered_blocks.append(block)
-
-        return rendered_blocks
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/prompt_template_config.py` & `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/prompt_template_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,55 @@
 # Copyright (c) Microsoft. All rights reserved.
-import json
 import logging
 from typing import Dict, List, Optional, TypeVar, Union
 
-from pydantic import Field, field_validator
+from pydantic import Field, field_validator, model_validator
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.prompt_template.const import KERNEL_TEMPLATE_FORMAT_NAME, TEMPLATE_FORMAT_TYPES
 from semantic_kernel.prompt_template.input_variable import InputVariable
 
 PromptExecutionSettingsT = TypeVar("PromptExecutionSettingsT", bound=PromptExecutionSettings)
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class PromptTemplateConfig(KernelBaseModel):
+    """Configuration for a prompt template.
+
+    Args:
+        name: The name of the prompt template.
+        description: The description of the prompt template.
+        template: The template for the prompt.
+        template_format: The format of the template, should be 'semantic-kernel', 'jinja2' or 'handlebars'.
+        input_variables: The input variables for the prompt.
+        allow_dangerously_set_content (default: false): Allow content without encoding, this controls
+            if the output of functions called in the template is encoded before use.
+        execution_settings: The execution settings for the prompt.
+
+    """
+
     name: str = ""
     description: Optional[str] = ""
     template: Optional[str] = None
     template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME
     input_variables: List[InputVariable] = Field(default_factory=list)
+    allow_dangerously_set_content: bool = False
     execution_settings: Dict[str, PromptExecutionSettings] = Field(default_factory=dict)
 
+    @model_validator(mode="after")
+    def check_input_variables(self):
+        """Verify that input variable default values are string only"""
+        for variable in self.input_variables:
+            if variable.default and not isinstance(variable.default, str):
+                raise ValueError(f"Default value for input variable {variable.name} must be a string.")
+        return self
+
     @field_validator("execution_settings", mode="before")
     @classmethod
     def rewrite_execution_settings(
         cls,
         settings: Optional[
             Union[PromptExecutionSettings, List[PromptExecutionSettings], Dict[str, PromptExecutionSettings]]
         ],
@@ -62,40 +84,32 @@
         ]
 
     @classmethod
     def from_json(cls, json_str: str) -> "PromptTemplateConfig":
         """Create a PromptTemplateConfig instance from a JSON string."""
         if not json_str:
             raise ValueError("json_str is empty")
-
         try:
-            parsed_json = json.loads(json_str)
-            config = PromptTemplateConfig(**parsed_json)
+            return cls.model_validate_json(json_str)
         except Exception as e:
             raise ValueError(
                 "Unable to deserialize PromptTemplateConfig from the "
                 f"specified JSON string: {json_str} with exception: {e}"
             )
 
-        # Verify that input variable default values are string only
-        for variable in config.input_variables:
-            if variable.default and not isinstance(variable.default, str):
-                raise ValueError(f"Default value for input variable {variable.name} must be a string for {config.name}")
-
-        return config
-
     @classmethod
     def restore(
         cls,
         name: str,
         description: str,
         template: str,
         template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME,
         input_variables: List[InputVariable] = [],
         execution_settings: Dict[str, PromptExecutionSettings] = {},
+        allow_dangerously_set_content: bool = False,
     ) -> "PromptTemplateConfig":
         """Restore a PromptTemplateConfig instance from the specified parameters.
 
         Args:
             name: The name of the prompt template.
             description: The description of the prompt template.
             template: The template for the prompt.
@@ -108,8 +122,9 @@
         return cls(
             name=name,
             description=description,
             template=template,
             template_format=template_format,
             input_variables=input_variables,
             execution_settings=execution_settings,
+            allow_dangerously_set_content=allow_dangerously_set_content,
         )
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py` & `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def _messages(this, options, *args, **kwargs):
     from semantic_kernel.contents.chat_history import ChatHistory
 
     if not isinstance(this.context["chat_history"], ChatHistory):
         return ""
-    return str(this.context["chat_history"])
+    return this.context["chat_history"].to_prompt()
 
 
 def _message_to_prompt(this, *args, **kwargs):
     from semantic_kernel.contents.chat_message_content import ChatMessageContent
 
     if isinstance(this.context, ChatMessageContent):
         return str(this.context.to_prompt())
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py` & `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def _messages(chat_history):
     from semantic_kernel.contents.chat_history import ChatHistory
 
     if not isinstance(chat_history, ChatHistory):
         return ""
-    return str(chat_history)
+    return chat_history.to_prompt()
 
 
 def _message_to_prompt(context):
     from semantic_kernel.contents.chat_message_content import ChatMessageContent
 
     if isinstance(context, ChatMessageContent):
         return str(context.to_prompt())
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/template_function_helpers.py` & `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/template_function_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import asyncio
 import logging
-from typing import TYPE_CHECKING, Callable, Literal
+from html import escape
+from typing import TYPE_CHECKING, Any, Callable, Literal
 
 import nest_asyncio
 
 from semantic_kernel.prompt_template.const import HANDLEBARS_TEMPLATE_FORMAT_NAME
 
 if TYPE_CHECKING:
     from semantic_kernel.functions.kernel_arguments import KernelArguments
@@ -18,15 +19,16 @@
 
 
 def create_template_helper_from_function(
     function: "KernelFunction",
     kernel: "Kernel",
     base_arguments: "KernelArguments",
     template_format: Literal["handlebars", "jinja2"],
-) -> Callable:
+    allow_dangerously_set_content: bool = False,
+) -> Callable[..., Any]:
     """Create a helper function for both the Handlebars and Jinja2 templating engines from a kernel function."""
     if not getattr(asyncio, "_nest_patched", False):
         nest_asyncio.apply()
 
     def func(*args, **kwargs):
         arguments = base_arguments.copy()
         arguments.update(kwargs)
@@ -44,10 +46,13 @@
             logger.debug("Jinja2 context or Handlebars context without `this`")
 
         logger.debug(
             f"Invoking function {function.metadata.fully_qualified_name} "
             f"with args: {actual_args} and kwargs: {kwargs} and this: {this}."
         )
 
-        return asyncio.run(function.invoke(kernel=kernel, arguments=arguments))
+        result = asyncio.run(function.invoke(kernel=kernel, arguments=arguments))
+        if allow_dangerously_set_content:
+            return result
+        return escape(str(result))
 
     return func
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.9.9b1/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.9.9b1/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/services/ai_service_client_base.py` & `semantic_kernel-0.9.9b1/semantic_kernel/services/ai_service_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/services/ai_service_selector.py` & `semantic_kernel-0.9.9b1/semantic_kernel/services/ai_service_selector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from copy import copy
 from typing import TYPE_CHECKING, Any, ClassVar, List
 
 from pydantic import Field, field_validator, model_validator
 
+from semantic_kernel.const import METADATA_EXCEPTION_KEY
 from semantic_kernel.exceptions import CodeBlockRenderException, CodeBlockTokenError
 from semantic_kernel.exceptions.kernel_exceptions import KernelFunctionNotFoundError, KernelPluginNotFoundError
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 from semantic_kernel.template_engine.code_tokenizer import CodeTokenizer
 
@@ -122,15 +123,15 @@
             raise CodeBlockRenderException(error_msg) from exc
 
         arguments_clone = copy(arguments)
         if len(self.tokens) > 1:
             arguments_clone = self._enrich_function_arguments(kernel, arguments_clone, function.metadata)
 
         result = await function.invoke(kernel, arguments_clone)
-        if exc := result.metadata.get("error", None):
+        if exc := result.metadata.get(METADATA_EXCEPTION_KEY, None):
             raise CodeBlockRenderException(f"Error rendering function: {function.metadata} with error: {exc}") from exc
 
         return str(result) if result else ""
 
     def _enrich_function_arguments(
         self,
         kernel: "Kernel",
```

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/named_arg_block.py` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/named_arg_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.9.9b1/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.9.9b1/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/utils/naming.py` & `semantic_kernel-0.9.9b1/semantic_kernel/utils/naming.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/utils/null_logger.py` & `semantic_kernel-0.9.9b1/semantic_kernel/utils/null_logger.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/semantic_kernel/utils/validation.py` & `semantic_kernel-0.9.9b1/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.8b1/PKG-INFO` & `semantic_kernel-0.9.9b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.9.8b1
+Version: 0.9.9b1
 Summary: Semantic Kernel Python SDK
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -47,17 +47,17 @@
 Requires-Dist: openapi_core (>=0.18,<0.20)
 Requires-Dist: pinecone-client (>=3.0.0) ; extra == "pinecone" or extra == "all"
 Requires-Dist: prance (>=23.6.21.0,<24.0.0.0)
 Requires-Dist: psycopg[binary,pool] (>=3.1.9,<4.0.0) ; extra == "postgres" or extra == "all"
 Requires-Dist: pyarrow (>=12.0.1,<16.0.0) ; extra == "usearch" or extra == "all"
 Requires-Dist: pybars4 (>=0.9.13,<0.10.0)
 Requires-Dist: pydantic (>=2,<3)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pymilvus (>=2.2,<2.3) ; (python_version == "3.8") and (extra == "milvus" or extra == "all")
 Requires-Dist: pymilvus (>=2.3,<2.3.8) ; (python_version > "3.8") and (extra == "milvus" or extra == "all")
-Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: qdrant-client (>=1.6,<2.0) ; (python_version == "3.8") and (extra == "qdrant" or extra == "all")
 Requires-Dist: qdrant-client (>=1.7) ; (python_full_version > "3.9.0") and (extra == "qdrant" or extra == "all")
 Requires-Dist: redis (>=4.6.0,<5.0.0) ; extra == "redis" or extra == "all"
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: scipy (>=1.12.0) ; python_version >= "3.12"
 Requires-Dist: scipy (>=1.5.0) ; python_version < "3.12"
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "hugging-face" or extra == "all"
```

