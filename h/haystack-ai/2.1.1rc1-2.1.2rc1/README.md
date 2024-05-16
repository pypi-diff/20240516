# Comparing `tmp/haystack_ai-2.1.1rc1.tar.gz` & `tmp/haystack_ai-2.1.2rc1.tar.gz`

## Comparing `haystack_ai-2.1.1rc1.tar` & `haystack_ai-2.1.2rc1.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/VERSION.txt
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/errors.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/lazy_imports.py
--rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/logging.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/__init__.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/audio/__init__.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/audio/whisper_local.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/audio/whisper_remote.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/builders/__init__.py
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/builders/answer_builder.py
--rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/builders/dynamic_chat_prompt_builder.py
--rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/builders/dynamic_prompt_builder.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/builders/prompt_builder.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/caching/__init__.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/caching/cache_checker.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/classifiers/__init__.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/classifiers/document_language_classifier.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/connectors/__init__.py
--rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/connectors/openapi_service.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/__init__.py
--rw-r--r--   0        0        0    24642 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/azure.py
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/html.py
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/markdown.py
--rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/openapi_functions.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/output_adapter.py
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/pdfminer.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/pypdf.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/tika.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/txt.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/utils.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/__init__.py
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/azure_document_embedder.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/azure_text_embedder.py
--rw-r--r--   0        0        0    10902 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_api_document_embedder.py
--rw-r--r--   0        0        0     8005 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_api_text_embedder.py
--rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py
--rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/openai_document_embedder.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/openai_text_embedder.py
--rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/sentence_transformers_document_embedder.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/sentence_transformers_text_embedder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/backends/__init__.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/backends/sentence_transformers_backend.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/__init__.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/answer_exact_match.py
--rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/context_relevance.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/document_map.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/document_mrr.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/document_recall.py
--rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/faithfulness.py
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/llm_evaluator.py
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/sas_evaluator.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/extractors/__init__.py
--rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/extractors/named_entity_extractor.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/fetchers/__init__.py
--rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/fetchers/link_content.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/__init__.py
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/azure.py
--rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_api.py
--rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_local.py
--rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_tgi.py
--rw-r--r--   0        0        0    13449 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/openai.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/utils.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/__init__.py
--rw-r--r--   0        0        0     9791 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/azure.py
--rw-r--r--   0        0        0    11191 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_api.py
--rw-r--r--   0        0        0    17793 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_local.py
--rw-r--r--   0        0        0    15851 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_tgi.py
--rw-r--r--   0        0        0    16934 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/openai.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/joiners/__init__.py
--rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/joiners/document_joiner.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/others/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/others/multiplexer.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/preprocessors/__init__.py
--rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/preprocessors/document_cleaner.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/preprocessors/document_splitter.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/preprocessors/text_cleaner.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/rankers/__init__.py
--rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/rankers/lost_in_the_middle.py
--rw-r--r--   0        0        0    17048 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/rankers/meta_field.py
--rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/rankers/sentence_transformers_diversity.py
--rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/rankers/transformers_similarity.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/readers/__init__.py
--rw-r--r--   0        0        0    28699 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/readers/extractive.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/retrievers/__init__.py
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/retrievers/filter_retriever.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/retrievers/in_memory/__init__.py
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/retrievers/in_memory/bm25_retriever.py
--rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/retrievers/in_memory/embedding_retriever.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/__init__.py
--rw-r--r--   0        0        0    10151 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/conditional_router.py
--rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/file_type_router.py
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/metadata_router.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/text_language_router.py
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/zero_shot_text_router.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/samplers/__init__.py
--rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/samplers/top_p.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/validators/__init__.py
--rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/validators/json_schema.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/websearch/__init__.py
--rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/websearch/searchapi.py
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/websearch/serper_dev.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/writers/__init__.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/writers/document_writer.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/errors.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/serialization.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/type_utils.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/component/__init__.py
--rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/component/component.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/component/sockets.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/component/types.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/__init__.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/descriptions.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/draw.py
--rw-r--r--   0        0        0    56764 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/pipeline.py
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/template.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/__init__.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/answer.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/byte_stream.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/chat_message.py
--rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/document.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/sparse_embedding.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/streaming_chunk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/errors/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/errors/errors.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/in_memory/__init__.py
--rw-r--r--   0        0        0    15577 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/in_memory/document_store.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/types/policy.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/types/protocol.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/evaluation/__init__.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/evaluation/eval_run_result.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/marshal/__init__.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/marshal/protocol.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/marshal/yaml.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/telemetry/__init__.py
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/telemetry/_environment.py
--rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/telemetry/_telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/__init__.py
--rw-r--r--   0        0        0    63152 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/document_store.py
--rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/factory.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/test_utils.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/accumulate.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/add_value.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/concatenate.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/double.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/fstring.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/greet.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/hello.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/joiner.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/parity.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/remainder.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/repeat.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/self_loop.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/subtract.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/sum.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/text_splitter.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/threshold.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/tracing/__init__.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/tracing/datadog.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/tracing/opentelemetry.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/tracing/tracer.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/tracing/utils.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/__init__.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/auth.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/callable_serialization.py
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/device.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/expit.py
--rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/filters.py
--rw-r--r--   0        0        0    15510 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/hf.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/jupyter.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/requests_utils.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/type_serialization.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/url_validation.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/LICENSE
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/README.md
--rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/pyproject.toml
--rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/VERSION.txt
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/errors.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/lazy_imports.py
+-rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/logging.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/__init__.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/audio/__init__.py
+-rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/audio/whisper_local.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/audio/whisper_remote.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/builders/__init__.py
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/builders/answer_builder.py
+-rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/builders/dynamic_chat_prompt_builder.py
+-rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/builders/dynamic_prompt_builder.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/builders/prompt_builder.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/caching/__init__.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/caching/cache_checker.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/classifiers/__init__.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/classifiers/document_language_classifier.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/connectors/__init__.py
+-rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/connectors/openapi_service.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/__init__.py
+-rw-r--r--   0        0        0    24642 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/azure.py
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/html.py
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/markdown.py
+-rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/openapi_functions.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/output_adapter.py
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/pdfminer.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/pypdf.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/tika.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/txt.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/utils.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/__init__.py
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/azure_document_embedder.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/azure_text_embedder.py
+-rw-r--r--   0        0        0    10902 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_api_document_embedder.py
+-rw-r--r--   0        0        0     8005 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_api_text_embedder.py
+-rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py
+-rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/openai_document_embedder.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/openai_text_embedder.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/sentence_transformers_document_embedder.py
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/sentence_transformers_text_embedder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/backends/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/backends/sentence_transformers_backend.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/__init__.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/answer_exact_match.py
+-rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/context_relevance.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/document_map.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/document_mrr.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/document_recall.py
+-rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/faithfulness.py
+-rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/llm_evaluator.py
+-rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/sas_evaluator.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/extractors/__init__.py
+-rw-r--r--   0        0        0    16393 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/extractors/named_entity_extractor.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/fetchers/__init__.py
+-rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/fetchers/link_content.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/__init__.py
+-rw-r--r--   0        0        0     9100 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/azure.py
+-rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_api.py
+-rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_local.py
+-rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_tgi.py
+-rw-r--r--   0        0        0    13449 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/openai.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/utils.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/__init__.py
+-rw-r--r--   0        0        0     9813 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/azure.py
+-rw-r--r--   0        0        0    11191 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_api.py
+-rw-r--r--   0        0        0    17793 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_local.py
+-rw-r--r--   0        0        0    15851 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_tgi.py
+-rw-r--r--   0        0        0    16934 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/openai.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/joiners/__init__.py
+-rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/joiners/document_joiner.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/others/__init__.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/others/multiplexer.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/preprocessors/__init__.py
+-rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/preprocessors/document_cleaner.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/preprocessors/document_splitter.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/preprocessors/text_cleaner.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/rankers/__init__.py
+-rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/rankers/lost_in_the_middle.py
+-rw-r--r--   0        0        0    17048 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/rankers/meta_field.py
+-rw-r--r--   0        0        0    10902 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/rankers/sentence_transformers_diversity.py
+-rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/rankers/transformers_similarity.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/readers/__init__.py
+-rw-r--r--   0        0        0    28699 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/readers/extractive.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/retrievers/__init__.py
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/retrievers/filter_retriever.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/retrievers/in_memory/__init__.py
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/retrievers/in_memory/bm25_retriever.py
+-rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/retrievers/in_memory/embedding_retriever.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/__init__.py
+-rw-r--r--   0        0        0    10151 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/conditional_router.py
+-rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/file_type_router.py
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/metadata_router.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/text_language_router.py
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/zero_shot_text_router.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/samplers/__init__.py
+-rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/samplers/top_p.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/validators/__init__.py
+-rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/validators/json_schema.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/websearch/__init__.py
+-rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/websearch/searchapi.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/websearch/serper_dev.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/writers/__init__.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/writers/document_writer.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/errors.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/serialization.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/type_utils.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/component/__init__.py
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/component/component.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/component/sockets.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/component/types.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/__init__.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/descriptions.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/draw.py
+-rw-r--r--   0        0        0    57180 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/pipeline.py
+-rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/template.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/__init__.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/answer.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/byte_stream.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/chat_message.py
+-rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/document.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/sparse_embedding.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/streaming_chunk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/errors/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/errors/errors.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/in_memory/__init__.py
+-rw-r--r--   0        0        0    15577 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/in_memory/document_store.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/types/policy.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/types/protocol.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/evaluation/__init__.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/evaluation/eval_run_result.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/marshal/__init__.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/marshal/protocol.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/marshal/yaml.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/telemetry/__init__.py
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/telemetry/_environment.py
+-rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/telemetry/_telemetry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/__init__.py
+-rw-r--r--   0        0        0    63152 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/document_store.py
+-rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/factory.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/test_utils.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/accumulate.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/add_value.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/concatenate.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/double.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/fstring.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/greet.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/hello.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/joiner.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/parity.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/remainder.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/repeat.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/self_loop.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/subtract.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/sum.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/text_splitter.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/threshold.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/tracing/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/tracing/datadog.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/tracing/opentelemetry.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/tracing/tracer.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/tracing/utils.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/__init__.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/auth.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/callable_serialization.py
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/device.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/expit.py
+-rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/filters.py
+-rw-r--r--   0        0        0    15510 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/hf.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/jupyter.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/requests_utils.py
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/type_serialization.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/url_validation.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/LICENSE
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/README.md
+-rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/PKG-INFO
```

### Comparing `haystack_ai-2.1.1rc1/haystack/__init__.py` & `haystack_ai-2.1.2rc1/haystack/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/lazy_imports.py` & `haystack_ai-2.1.2rc1/haystack/lazy_imports.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/logging.py` & `haystack_ai-2.1.2rc1/haystack/logging.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/audio/whisper_local.py` & `haystack_ai-2.1.2rc1/haystack/components/audio/whisper_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,17 +82,17 @@
         Deserializes the component from a dictionary.
 
         :param data:
             The dictionary to deserialize from.
         :returns:
             The deserialized component.
         """
-        serialized_device = data["init_parameters"]["device"]
-        data["init_parameters"]["device"] = ComponentDevice.from_dict(serialized_device)
-
+        init_params = data["init_parameters"]
+        if init_params["device"] is not None:
+            init_params["device"] = ComponentDevice.from_dict(init_params["device"])
         return default_from_dict(cls, data)
 
     @component.output_types(documents=List[Document])
     def run(self, sources: List[Union[str, Path, ByteStream]], whisper_params: Optional[Dict[str, Any]] = None):
         """
         Transcribes the audio files into a list of Documents, one for each input file.
```

### Comparing `haystack_ai-2.1.1rc1/haystack/components/audio/whisper_remote.py` & `haystack_ai-2.1.2rc1/haystack/components/audio/whisper_remote.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/builders/answer_builder.py` & `haystack_ai-2.1.2rc1/haystack/components/builders/answer_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/builders/dynamic_chat_prompt_builder.py` & `haystack_ai-2.1.2rc1/haystack/components/builders/dynamic_chat_prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/builders/dynamic_prompt_builder.py` & `haystack_ai-2.1.2rc1/haystack/components/builders/dynamic_prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/builders/prompt_builder.py` & `haystack_ai-2.1.2rc1/haystack/components/builders/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/caching/cache_checker.py` & `haystack_ai-2.1.2rc1/haystack/components/caching/cache_checker.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/classifiers/document_language_classifier.py` & `haystack_ai-2.1.2rc1/haystack/components/classifiers/document_language_classifier.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/connectors/openapi_service.py` & `haystack_ai-2.1.2rc1/haystack/components/connectors/openapi_service.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/converters/__init__.py` & `haystack_ai-2.1.2rc1/haystack/components/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/converters/azure.py` & `haystack_ai-2.1.2rc1/haystack/components/converters/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/converters/html.py` & `haystack_ai-2.1.2rc1/haystack/components/converters/html.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/converters/markdown.py` & `haystack_ai-2.1.2rc1/haystack/components/converters/markdown.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/converters/openapi_functions.py` & `haystack_ai-2.1.2rc1/haystack/components/converters/openapi_functions.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/converters/output_adapter.py` & `haystack_ai-2.1.2rc1/haystack/components/converters/output_adapter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/converters/pdfminer.py` & `haystack_ai-2.1.2rc1/haystack/components/converters/pdfminer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/converters/pypdf.py` & `haystack_ai-2.1.2rc1/haystack/components/converters/pypdf.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/converters/tika.py` & `haystack_ai-2.1.2rc1/haystack/components/converters/tika.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/converters/txt.py` & `haystack_ai-2.1.2rc1/haystack/components/converters/txt.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/converters/utils.py` & `haystack_ai-2.1.2rc1/haystack/components/converters/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/__init__.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/azure_document_embedder.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/azure_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/azure_text_embedder.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/azure_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_api_document_embedder.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_api_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_api_text_embedder.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_api_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/openai_document_embedder.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/openai_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/openai_text_embedder.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/openai_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/sentence_transformers_document_embedder.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/sentence_transformers_document_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,17 @@
         Deserializes the component from a dictionary.
 
         :param data:
             Dictionary to deserialize from.
         :returns:
             Deserialized component.
         """
-        serialized_device = data["init_parameters"]["device"]
-        data["init_parameters"]["device"] = ComponentDevice.from_dict(serialized_device)
-
+        init_params = data["init_parameters"]
+        if init_params["device"] is not None:
+            init_params["device"] = ComponentDevice.from_dict(init_params["device"])
         deserialize_secrets_inplace(data["init_parameters"], keys=["token"])
         return default_from_dict(cls, data)
 
     def warm_up(self):
         """
         Initializes the component.
         """
```

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/sentence_transformers_text_embedder.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/sentence_transformers_text_embedder.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,17 +107,17 @@
         Deserializes the component from a dictionary.
 
         :param data:
             Dictionary to deserialize from.
         :returns:
             Deserialized component.
         """
-        serialized_device = data["init_parameters"]["device"]
-        data["init_parameters"]["device"] = ComponentDevice.from_dict(serialized_device)
-
+        init_params = data["init_parameters"]
+        if init_params["device"] is not None:
+            init_params["device"] = ComponentDevice.from_dict(init_params["device"])
         deserialize_secrets_inplace(data["init_parameters"], keys=["token"])
         return default_from_dict(cls, data)
 
     def warm_up(self):
         """
         Initializes the component.
         """
```

### Comparing `haystack_ai-2.1.1rc1/haystack/components/embedders/backends/sentence_transformers_backend.py` & `haystack_ai-2.1.2rc1/haystack/components/embedders/backends/sentence_transformers_backend.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/evaluators/__init__.py` & `haystack_ai-2.1.2rc1/haystack/components/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/evaluators/answer_exact_match.py` & `haystack_ai-2.1.2rc1/haystack/components/evaluators/answer_exact_match.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/evaluators/context_relevance.py` & `haystack_ai-2.1.2rc1/haystack/components/evaluators/context_relevance.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,18 @@
                 - `individual_scores`: A list of context relevance scores for each input question.
                 - `results`: A list of dictionaries with `statements` and `statement_scores` for each input context.
         """
         result = super().run(questions=questions, contexts=contexts)
 
         # calculate average statement relevance score per query
         for res in result["results"]:
-            res["score"] = np_mean(res["statement_scores"])
+            if not res["statements"]:
+                res["score"] = 0
+            else:
+                res["score"] = np_mean(res["statement_scores"])
 
         # calculate average context relevance score over all queries
         result["score"] = np_mean([res["score"] for res in result["results"]])
         result["individual_scores"] = [res["score"] for res in result["results"]]
 
         return result
```

### Comparing `haystack_ai-2.1.1rc1/haystack/components/evaluators/document_map.py` & `haystack_ai-2.1.2rc1/haystack/components/evaluators/document_map.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/evaluators/document_mrr.py` & `haystack_ai-2.1.2rc1/haystack/components/evaluators/document_mrr.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/evaluators/document_recall.py` & `haystack_ai-2.1.2rc1/haystack/components/evaluators/document_recall.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/evaluators/faithfulness.py` & `haystack_ai-2.1.2rc1/haystack/components/evaluators/faithfulness.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,18 @@
                 - `individual_scores`: A list of faithfulness scores for each input answer.
                 - `results`: A list of dictionaries with `statements` and `statement_scores` for each input answer.
         """
         result = super().run(questions=questions, contexts=contexts, predicted_answers=predicted_answers)
 
         # calculate average statement faithfulness score per query
         for res in result["results"]:
-            res["score"] = np_mean(res["statement_scores"])
+            if not res["statements"]:
+                res["score"] = 0
+            else:
+                res["score"] = np_mean(res["statement_scores"])
 
         # calculate average answer faithfulness score over all queries
         result["score"] = np_mean([res["score"] for res in result["results"]])
         result["individual_scores"] = [res["score"] for res in result["results"]]
 
         return result
```

### Comparing `haystack_ai-2.1.1rc1/haystack/components/evaluators/llm_evaluator.py` & `haystack_ai-2.1.2rc1/haystack/components/evaluators/llm_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,17 @@
         self.inputs = inputs
         self.outputs = outputs
         self.examples = examples
         self.api = api
         self.api_key = api_key
 
         if api == "openai":
-            self.generator = OpenAIGenerator(api_key=api_key)
+            self.generator = OpenAIGenerator(
+                api_key=api_key, generation_kwargs={"response_format": {"type": "json_object"}}
+            )
         else:
             raise ValueError(f"Unsupported API: {api}")
 
         template = self.prepare_template()
         self.builder = PromptBuilder(template=template)
 
         component.set_input_types(self, **dict(inputs))
```

### Comparing `haystack_ai-2.1.1rc1/haystack/components/evaluators/sas_evaluator.py` & `haystack_ai-2.1.2rc1/haystack/components/evaluators/sas_evaluator.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/extractors/named_entity_extractor.py` & `haystack_ai-2.1.2rc1/haystack/components/extractors/named_entity_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
-            backend=self._backend.type,
+            backend=self._backend.type.name,
             model=self._backend.model_name,
             device=self._backend.device.to_dict(),
             pipeline_kwargs=self._backend._pipeline_kwargs,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "NamedEntityExtractor":
@@ -207,15 +207,17 @@
         :param data:
             Dictionary to deserialize from.
         :returns:
             Deserialized component.
         """
         try:
             init_params = data["init_parameters"]
-            init_params["device"] = ComponentDevice.from_dict(init_params["device"])
+            if init_params["device"] is not None:
+                init_params["device"] = ComponentDevice.from_dict(init_params["device"])
+            init_params["backend"] = NamedEntityExtractorBackend[init_params["backend"]]
             return default_from_dict(cls, data)
         except Exception as e:
             raise DeserializationError(f"Couldn't deserialize {cls.__name__} instance") from e
 
     @property
     def initialized(self) -> bool:
         """
```

### Comparing `haystack_ai-2.1.1rc1/haystack/components/fetchers/link_content.py` & `haystack_ai-2.1.2rc1/haystack/components/fetchers/link_content.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/__init__.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/azure.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 from typing import Any, Callable, Dict, Optional
 
 # pylint: disable=import-error
 from openai.lib.azure import AzureOpenAI
 
-from haystack import default_from_dict, default_to_dict, logging
+from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.components.generators import OpenAIGenerator
 from haystack.dataclasses import StreamingChunk
 from haystack.utils import Secret, deserialize_callable, deserialize_secrets_inplace, serialize_callable
 
 logger = logging.getLogger(__name__)
 
 
+@component
 class AzureOpenAIGenerator(OpenAIGenerator):
     """
     A Generator component that uses OpenAI's large language models (LLMs) on Azure to generate text.
 
     It supports gpt-4 and gpt-3.5-turbo family of models.
 
     Users can pass any text generation parameters valid for the `openai.ChatCompletion.create` method
```

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_api.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_api.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_local.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_tgi.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_tgi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/openai.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/openai.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/utils.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/chat/__init__.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/chat/azure.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/chat/azure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 from typing import Any, Callable, Dict, Optional
 
 # pylint: disable=import-error
 from openai.lib.azure import AzureOpenAI
 
-from haystack import default_from_dict, default_to_dict, logging
+from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.components.generators.chat import OpenAIChatGenerator
 from haystack.dataclasses import StreamingChunk
 from haystack.utils import Secret, deserialize_callable, deserialize_secrets_inplace, serialize_callable
 
 logger = logging.getLogger(__name__)
 
 
+@component
 class AzureOpenAIChatGenerator(OpenAIChatGenerator):
     """
     A Chat Generator component that uses the Azure OpenAI API to generate text.
 
     Enables text generation using OpenAI's large language models (LLMs) on Azure. It supports `gpt-4` and `gpt-3.5-turbo`
     family of models accessed through the chat completions API endpoint.
```

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_api.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_api.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_local.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_tgi.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_tgi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/generators/chat/openai.py` & `haystack_ai-2.1.2rc1/haystack/components/generators/chat/openai.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/joiners/document_joiner.py` & `haystack_ai-2.1.2rc1/haystack/components/joiners/document_joiner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/others/multiplexer.py` & `haystack_ai-2.1.2rc1/haystack/components/others/multiplexer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/preprocessors/document_cleaner.py` & `haystack_ai-2.1.2rc1/haystack/components/preprocessors/document_cleaner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/preprocessors/document_splitter.py` & `haystack_ai-2.1.2rc1/haystack/components/preprocessors/document_splitter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/preprocessors/text_cleaner.py` & `haystack_ai-2.1.2rc1/haystack/components/preprocessors/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/rankers/lost_in_the_middle.py` & `haystack_ai-2.1.2rc1/haystack/components/rankers/lost_in_the_middle.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/rankers/meta_field.py` & `haystack_ai-2.1.2rc1/haystack/components/rankers/meta_field.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/rankers/sentence_transformers_diversity.py` & `haystack_ai-2.1.2rc1/haystack/components/rankers/sentence_transformers_diversity.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,17 +133,17 @@
         Deserializes the component from a dictionary.
 
         :param data:
             The dictionary to deserialize from.
         :returns:
             The deserialized component.
         """
-        serialized_device = data["init_parameters"]["device"]
-        data["init_parameters"]["device"] = ComponentDevice.from_dict(serialized_device)
-
+        init_params = data["init_parameters"]
+        if init_params["device"] is not None:
+            init_params["device"] = ComponentDevice.from_dict(init_params["device"])
         deserialize_secrets_inplace(data["init_parameters"], keys=["token"])
         return default_from_dict(cls, data)
 
     def _prepare_texts_to_embed(self, documents: List[Document]) -> List[str]:
         """
         Prepare the texts to embed by concatenating the Document text with the metadata fields to embed.
         """
```

### Comparing `haystack_ai-2.1.1rc1/haystack/components/rankers/transformers_similarity.py` & `haystack_ai-2.1.2rc1/haystack/components/rankers/transformers_similarity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/readers/extractive.py` & `haystack_ai-2.1.2rc1/haystack/components/readers/extractive.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/retrievers/filter_retriever.py` & `haystack_ai-2.1.2rc1/haystack/components/retrievers/filter_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/retrievers/in_memory/bm25_retriever.py` & `haystack_ai-2.1.2rc1/haystack/components/retrievers/in_memory/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/retrievers/in_memory/embedding_retriever.py` & `haystack_ai-2.1.2rc1/haystack/components/retrievers/in_memory/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/routers/__init__.py` & `haystack_ai-2.1.2rc1/haystack/components/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/routers/conditional_router.py` & `haystack_ai-2.1.2rc1/haystack/components/routers/conditional_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/routers/file_type_router.py` & `haystack_ai-2.1.2rc1/haystack/components/routers/file_type_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/routers/metadata_router.py` & `haystack_ai-2.1.2rc1/haystack/components/routers/metadata_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/routers/text_language_router.py` & `haystack_ai-2.1.2rc1/haystack/components/routers/text_language_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/routers/zero_shot_text_router.py` & `haystack_ai-2.1.2rc1/haystack/components/routers/zero_shot_text_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/samplers/top_p.py` & `haystack_ai-2.1.2rc1/haystack/components/samplers/top_p.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/validators/json_schema.py` & `haystack_ai-2.1.2rc1/haystack/components/validators/json_schema.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/websearch/searchapi.py` & `haystack_ai-2.1.2rc1/haystack/components/websearch/searchapi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/websearch/serper_dev.py` & `haystack_ai-2.1.2rc1/haystack/components/websearch/serper_dev.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/components/writers/document_writer.py` & `haystack_ai-2.1.2rc1/haystack/components/writers/document_writer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/errors.py` & `haystack_ai-2.1.2rc1/haystack/core/errors.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/serialization.py` & `haystack_ai-2.1.2rc1/haystack/core/serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/type_utils.py` & `haystack_ai-2.1.2rc1/haystack/core/type_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/component/component.py` & `haystack_ai-2.1.2rc1/haystack/core/component/component.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/component/sockets.py` & `haystack_ai-2.1.2rc1/haystack/core/component/sockets.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/component/types.py` & `haystack_ai-2.1.2rc1/haystack/core/component/types.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/pipeline/descriptions.py` & `haystack_ai-2.1.2rc1/haystack/core/pipeline/descriptions.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/pipeline/draw.py` & `haystack_ai-2.1.2rc1/haystack/core/pipeline/draw.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/pipeline/pipeline.py` & `haystack_ai-2.1.2rc1/haystack/core/pipeline/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -638,15 +638,15 @@
                     raise ValueError(f"Missing input for component {component_name}: {socket_name}")
                 if socket.senders and socket_name in component_inputs and not socket.is_variadic:
                     raise ValueError(
                         f"Input {socket_name} for component {component_name} is already sent by {socket.senders}."
                     )
 
     # TODO: We're ignoring these linting rules for the time being, after we properly optimize this function we'll remove the noqa
-    def run(  # noqa: C901, PLR0912, PLR0915 pylint: disable=too-many-branches
+    def run(  # noqa: C901, PLR0912, PLR0915 pylint: disable=too-many-branches,too-many-locals
         self, data: Dict[str, Any], debug: bool = False, include_outputs_from: Optional[Set[str]] = None
     ) -> Dict[str, Any]:
         """
         Runs the pipeline with given input data.
 
         :param data:
             A dictionary of inputs for the pipeline's components. Each key is a component name
@@ -855,15 +855,14 @@
                                     "senders": value.receivers,
                                 }
                                 for key, value in comp.__haystack_output__._sockets_dict.items()  # type: ignore
                             },
                         },
                     ) as span:
                         span.set_content_tag("haystack.component.input", last_inputs[name])
-                        logger.info("Running component {name}", name=name)
                         logger.info("Running component {component_name}", component_name=name)
                         res = comp.run(**last_inputs[name])
                         self.graph.nodes[name]["visits"] += 1
 
                         if not isinstance(res, Mapping):
                             raise PipelineRuntimeError(
                                 f"Component '{name}' didn't return a dictionary. "
@@ -1047,16 +1046,25 @@
                             break
 
                     waiting_for_input.remove((name, comp))
                     to_run.append((name, comp))
 
             if len(include_outputs_from) > 0:
                 for name, output in extra_outputs.items():
-                    if name not in final_outputs:
+                    inner = final_outputs.get(name)
+                    if inner is None:
                         final_outputs[name] = output
+                    else:
+                        # Let's not override any keys that are already
+                        # in the final_outputs as they might be different
+                        # from what we cached in extra_outputs, e.g. when loops
+                        # are involved.
+                        for k, v in output.items():
+                            if k not in inner:
+                                inner[k] = v
 
             return final_outputs
 
     def _prepare_component_input_data(self, data: Dict[str, Any]) -> Tuple[Dict[str, Dict[str, Any]], Dict[str, Any]]:
         """
         Prepares input data for pipeline components.
```

### Comparing `haystack_ai-2.1.1rc1/haystack/core/pipeline/template.py` & `haystack_ai-2.1.2rc1/haystack/core/pipeline/template.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2` & `haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2` & `haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2` & `haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2` & `haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/dataclasses/__init__.py` & `haystack_ai-2.1.2rc1/haystack/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/dataclasses/answer.py` & `haystack_ai-2.1.2rc1/haystack/dataclasses/answer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/dataclasses/byte_stream.py` & `haystack_ai-2.1.2rc1/haystack/dataclasses/byte_stream.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/dataclasses/chat_message.py` & `haystack_ai-2.1.2rc1/haystack/dataclasses/chat_message.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/dataclasses/document.py` & `haystack_ai-2.1.2rc1/haystack/dataclasses/document.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/dataclasses/sparse_embedding.py` & `haystack_ai-2.1.2rc1/haystack/dataclasses/sparse_embedding.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/dataclasses/streaming_chunk.py` & `haystack_ai-2.1.2rc1/haystack/dataclasses/streaming_chunk.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/document_stores/in_memory/document_store.py` & `haystack_ai-2.1.2rc1/haystack/document_stores/in_memory/document_store.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/document_stores/types/protocol.py` & `haystack_ai-2.1.2rc1/haystack/document_stores/types/protocol.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/evaluation/eval_run_result.py` & `haystack_ai-2.1.2rc1/haystack/evaluation/eval_run_result.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/telemetry/_environment.py` & `haystack_ai-2.1.2rc1/haystack/telemetry/_environment.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/telemetry/_telemetry.py` & `haystack_ai-2.1.2rc1/haystack/telemetry/_telemetry.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/document_store.py` & `haystack_ai-2.1.2rc1/haystack/testing/document_store.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/factory.py` & `haystack_ai-2.1.2rc1/haystack/testing/factory.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/test_utils.py` & `haystack_ai-2.1.2rc1/haystack/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/__init__.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/accumulate.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/accumulate.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/add_value.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/add_value.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/concatenate.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/concatenate.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/fstring.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/fstring.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/greet.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/greet.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/joiner.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/joiner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/parity.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/parity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/remainder.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/remainder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/self_loop.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/self_loop.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/subtract.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/subtract.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/testing/sample_components/threshold.py` & `haystack_ai-2.1.2rc1/haystack/testing/sample_components/threshold.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/tracing/datadog.py` & `haystack_ai-2.1.2rc1/haystack/tracing/datadog.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/tracing/opentelemetry.py` & `haystack_ai-2.1.2rc1/haystack/tracing/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/tracing/tracer.py` & `haystack_ai-2.1.2rc1/haystack/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/tracing/utils.py` & `haystack_ai-2.1.2rc1/haystack/tracing/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/utils/__init__.py` & `haystack_ai-2.1.2rc1/haystack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/utils/auth.py` & `haystack_ai-2.1.2rc1/haystack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/utils/callable_serialization.py` & `haystack_ai-2.1.2rc1/haystack/utils/callable_serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/utils/device.py` & `haystack_ai-2.1.2rc1/haystack/utils/device.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/utils/filters.py` & `haystack_ai-2.1.2rc1/haystack/utils/filters.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/utils/hf.py` & `haystack_ai-2.1.2rc1/haystack/utils/hf.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/utils/jupyter.py` & `haystack_ai-2.1.2rc1/haystack/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/utils/requests_utils.py` & `haystack_ai-2.1.2rc1/haystack/utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/haystack/utils/type_serialization.py` & `haystack_ai-2.1.2rc1/haystack/utils/type_serialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import importlib
 import inspect
 import sys
-from typing import Any, get_origin
+import typing
+from typing import Any, get_args, get_origin
 
 from haystack import DeserializationError
 
 
 def serialize_type(target: Any) -> str:
     """
     Serializes a type or an instance to its string representation, including the module name.
@@ -24,27 +25,31 @@
     # If the target is a string and contains a dot, treat it as an already serialized type
     if isinstance(target, str) and "." in target:
         return target
 
     # Determine if the target is a type or an instance of a typing object
     is_type_or_typing = isinstance(target, type) or bool(get_origin(target))
     type_obj = target if is_type_or_typing else type(target)
-    module = inspect.getmodule(type_obj)
     type_obj_repr = repr(type_obj)
 
     if type_obj_repr.startswith("typing."):
         # e.g., typing.List[int] -> List[int], we'll add the module below
         type_name = type_obj_repr.split(".", 1)[1]
+    elif origin := get_origin(type_obj):  # get the origin (base type of the parameterized generic type)
+        # get the arguments of the generic type
+        args = get_args(type_obj)
+        args_repr = ", ".join(serialize_type(arg) for arg in args)
+        type_name = f"{origin.__name__}[{args_repr}]"
     elif hasattr(type_obj, "__name__"):
         type_name = type_obj.__name__
     else:
         # If type cannot be serialized, raise an error
         raise ValueError(f"Could not serialize type: {type_obj_repr}")
 
-    # Construct the full path with module name if available
+    module = inspect.getmodule(type_obj)
     if module and hasattr(module, "__name__"):
         if module.__name__ == "builtins":
             # omit the module name for builtins, it just clutters the output
             # e.g. instead of 'builtins.str', we'll just return 'str'
             full_path = type_name
         else:
             full_path = f"{module.__name__}.{type_name}"
@@ -65,14 +70,22 @@
         The string representation of the type's full import path.
     :returns:
         The deserialized type object.
     :raises DeserializationError:
         If the type cannot be deserialized due to missing module or type.
     """
 
+    type_mapping = {
+        list: typing.List,
+        dict: typing.Dict,
+        set: typing.Set,
+        tuple: typing.Tuple,
+        frozenset: typing.FrozenSet,
+    }
+
     def parse_generic_args(args_str):
         args = []
         bracket_count = 0
         current_arg = ""
 
         for char in args_str:
             if char == "[":
@@ -96,15 +109,18 @@
         main_type_str, generics_str = type_str.split("[", 1)
         generics_str = generics_str[:-1]
 
         main_type = deserialize_type(main_type_str)
         generic_args = tuple(deserialize_type(arg) for arg in parse_generic_args(generics_str))
 
         # Reconstruct
-        return main_type[generic_args]
+        if sys.version_info >= (3, 9) or repr(main_type).startswith("typing."):
+            return main_type[generic_args]
+        else:
+            return type_mapping[main_type][generic_args]  # type: ignore
 
     else:
         # Handle non-generics
         parts = type_str.split(".")
         module_name = ".".join(parts[:-1]) or "builtins"
         type_name = parts[-1]
```

### Comparing `haystack_ai-2.1.1rc1/.gitignore` & `haystack_ai-2.1.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/LICENSE` & `haystack_ai-2.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/README.md` & `haystack_ai-2.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/pyproject.toml` & `haystack_ai-2.1.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.1rc1/PKG-INFO` & `haystack_ai-2.1.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: haystack-ai
-Version: 2.1.1rc1
+Version: 2.1.2rc1
 Summary: LLM framework to build customizable, production-ready LLM applications. Connect components (models, vector DBs, file converters) to pipelines or agents that can interact with your data.
 Project-URL: CI: GitHub, https://github.com/deepset-ai/haystack/actions
 Project-URL: Docs: RTD, https://haystack.deepset.ai/overview/intro
 Project-URL: GitHub: issues, https://github.com/deepset-ai/haystack/issues
 Project-URL: GitHub: repo, https://github.com/deepset-ai/haystack
 Project-URL: Homepage, https://github.com/deepset-ai/haystack
 Author-email: "deepset.ai" <malte.pietsch@deepset.ai>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: haystack-ai Version: 2.1.1rc1 Summary: LLM
+Metadata-Version: 2.3 Name: haystack-ai Version: 2.1.2rc1 Summary: LLM
 framework to build customizable, production-ready LLM applications. Connect
 components (models, vector DBs, file converters) to pipelines or agents that
 can interact with your data. Project-URL: CI: GitHub, https://github.com/
 deepset-ai/haystack/actions Project-URL: Docs: RTD, https://
 haystack.deepset.ai/overview/intro Project-URL: GitHub: issues, https://
 github.com/deepset-ai/haystack/issues Project-URL: GitHub: repo, https://
 github.com/deepset-ai/haystack Project-URL: Homepage, https://github.com/
```

