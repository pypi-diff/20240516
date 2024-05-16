# Comparing `tmp/bisheng_langchain-0.3.0rc1-py3-none-any.whl.zip` & `tmp/bisheng_langchain-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,116 +1,151 @@
-Zip file size: 172642 bytes, number of entries: 114
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/__init__.py
--rw-r--r--  2.0 unx     7909 b- defN 24-Apr-17 11:13 bisheng_langchain/text_splitter.py
--rw-r--r--  2.0 unx      226 b- defN 24-Apr-17 11:13 bisheng_langchain/agents/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/agents/chatglm_functions_agent/__init__.py
--rw-r--r--  2.0 unx    13674 b- defN 24-Apr-17 11:13 bisheng_langchain/agents/chatglm_functions_agent/base.py
--rw-r--r--  2.0 unx     3497 b- defN 24-Apr-17 11:13 bisheng_langchain/agents/chatglm_functions_agent/output_parser.py
--rw-r--r--  2.0 unx      992 b- defN 24-Apr-17 11:13 bisheng_langchain/agents/chatglm_functions_agent/prompt.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/agents/llm_functions_agent/__init__.py
--rw-r--r--  2.0 unx    12296 b- defN 24-Apr-17 11:13 bisheng_langchain/agents/llm_functions_agent/base.py
--rw-r--r--  2.0 unx      430 b- defN 24-Apr-17 11:13 bisheng_langchain/autogen_role/__init__.py
--rw-r--r--  2.0 unx     4657 b- defN 24-Apr-17 11:13 bisheng_langchain/autogen_role/assistant.py
--rw-r--r--  2.0 unx     2464 b- defN 24-Apr-17 11:13 bisheng_langchain/autogen_role/custom.py
--rw-r--r--  2.0 unx     2234 b- defN 24-Apr-17 11:13 bisheng_langchain/autogen_role/groupchat_manager.py
--rw-r--r--  2.0 unx     5715 b- defN 24-Apr-17 11:13 bisheng_langchain/autogen_role/user.py
--rw-r--r--  2.0 unx      759 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/__init__.py
--rw-r--r--  2.0 unx     1903 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/loader_output.py
--rw-r--r--  2.0 unx     2805 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/transform.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/autogen/__init__.py
--rw-r--r--  2.0 unx     3270 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/autogen/auto_gen.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/combine_documents/__init__.py
--rw-r--r--  2.0 unx     2369 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/combine_documents/stuff.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/conversational_retrieval/__init__.py
--rw-r--r--  2.0 unx     5313 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/conversational_retrieval/base.py
--rw-r--r--  2.0 unx     8795 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/question_answering/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/retrieval/__init__.py
--rw-r--r--  2.0 unx     3050 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/retrieval/retrieval_chain.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/router/__init__.py
--rw-r--r--  2.0 unx      375 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/router/multi_rule.py
--rw-r--r--  2.0 unx     1835 b- defN 24-Apr-17 11:13 bisheng_langchain/chains/router/rule_router.py
--rw-r--r--  2.0 unx      635 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/__init__.py
--rw-r--r--  2.0 unx    23153 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/host_llm.py
--rw-r--r--  2.0 unx    13901 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/minimax.py
--rw-r--r--  2.0 unx    17082 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/proxy_llm.py
--rw-r--r--  2.0 unx    19971 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/qwen.py
--rw-r--r--  2.0 unx    17056 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/sensetime.py
--rw-r--r--  2.0 unx    13671 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/wenxin.py
--rw-r--r--  2.0 unx    14037 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/xunfeiai.py
--rw-r--r--  2.0 unx    15342 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/zhipuai.py
--rw-r--r--  2.0 unx      443 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/interface/__init__.py
--rw-r--r--  2.0 unx     4423 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/interface/minimax.py
--rw-r--r--  2.0 unx     2081 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/interface/openai.py
--rw-r--r--  2.0 unx     1141 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/interface/types.py
--rw-r--r--  2.0 unx       65 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/interface/utils.py
--rw-r--r--  2.0 unx     4246 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/interface/wenxin.py
--rw-r--r--  2.0 unx     7514 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/interface/xunfei.py
--rw-r--r--  2.0 unx     2636 b- defN 24-Apr-17 11:13 bisheng_langchain/chat_models/interface/zhipuai.py
--rw-r--r--  2.0 unx      366 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/__init__.py
--rw-r--r--  2.0 unx     6656 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/custom_kv.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/elem_html.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/elem_image.py
--rw-r--r--  2.0 unx    22243 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/elem_pdf.py
--rw-r--r--  2.0 unx     5169 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/elem_unstrcutured_loader.py
--rw-r--r--  2.0 unx     4063 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/universal_kv.py
--rw-r--r--  2.0 unx      171 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/parsers/__init__.py
--rw-r--r--  2.0 unx     1760 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/parsers/ellm_client.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/parsers/image.py
--rw-r--r--  2.0 unx     1612 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/parsers/ocr_client.py
--rw-r--r--  2.0 unx     8685 b- defN 24-Apr-17 11:13 bisheng_langchain/document_loaders/parsers/test_image.py
--rw-r--r--  2.0 unx      534 b- defN 24-Apr-17 11:13 bisheng_langchain/embeddings/__init__.py
--rw-r--r--  2.0 unx     6295 b- defN 24-Apr-17 11:13 bisheng_langchain/embeddings/host_embedding.py
--rw-r--r--  2.0 unx     3192 b- defN 24-Apr-17 11:13 bisheng_langchain/embeddings/huggingfacegte.py
--rw-r--r--  2.0 unx     3415 b- defN 24-Apr-17 11:13 bisheng_langchain/embeddings/huggingfacemultilingual.py
--rw-r--r--  2.0 unx     4737 b- defN 24-Apr-17 11:13 bisheng_langchain/embeddings/wenxin.py
--rw-r--r--  2.0 unx       98 b- defN 24-Apr-17 11:13 bisheng_langchain/embeddings/interface/__init__.py
--rw-r--r--  2.0 unx      461 b- defN 24-Apr-17 11:13 bisheng_langchain/embeddings/interface/types.py
--rw-r--r--  2.0 unx     3104 b- defN 24-Apr-17 11:13 bisheng_langchain/embeddings/interface/wenxin.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/__init__.py
--rw-r--r--  2.0 unx     5083 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/assistant.py
--rw-r--r--  2.0 unx     3626 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/auto_optimization.py
--rw-r--r--  2.0 unx     1582 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/auto_tool_selected.py
--rw-r--r--  2.0 unx     7871 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/load_tools.py
--rw-r--r--  2.0 unx      213 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/message_types.py
--rw-r--r--  2.0 unx     6671 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/utils.py
--rw-r--r--  2.0 unx      261 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/agent_types/__init__.py
--rw-r--r--  2.0 unx     8419 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/agent_types/llm_functions_agent.py
--rw-r--r--  2.0 unx      568 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/prompts/__init__.py
--rw-r--r--  2.0 unx     4151 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/prompts/assistant_prompt_opt.py
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/prompts/base_prompt.py
--rw-r--r--  2.0 unx     5336 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/prompts/breif_description_prompt.py
--rw-r--r--  2.0 unx     5965 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/prompts/opening_dialog_prompt.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/prompts/select_tools_prompt.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/__init__.py
--rw-r--r--  2.0 unx     1608 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/api_tools/__init__.py
--rw-r--r--  2.0 unx     3618 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/api_tools/base.py
--rw-r--r--  2.0 unx     2486 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/api_tools/flow.py
--rw-r--r--  2.0 unx    27429 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/api_tools/macro_data.py
--rw-r--r--  2.0 unx     9542 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/api_tools/sina.py
--rw-r--r--  2.0 unx     6684 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/api_tools/tianyancha.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/bing_search/__init__.py
--rw-r--r--  2.0 unx     1710 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/bing_search/tool.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/calculator/__init__.py
--rw-r--r--  2.0 unx      705 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/calculator/tool.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/code_interpreter/__init__.py
--rw-r--r--  2.0 unx    11443 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/code_interpreter/tool.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/dalle_image_generator/__init__.py
--rw-r--r--  2.0 unx     7528 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/dalle_image_generator/tool.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/get_current_time/__init__.py
--rw-r--r--  2.0 unx      801 b- defN 24-Apr-17 11:13 bisheng_langchain/gpts/tools/get_current_time/tool.py
--rw-r--r--  2.0 unx      153 b- defN 24-Apr-17 11:13 bisheng_langchain/input_output/__init__.py
--rw-r--r--  2.0 unx     1094 b- defN 24-Apr-17 11:13 bisheng_langchain/input_output/input.py
--rw-r--r--  2.0 unx    11585 b- defN 24-Apr-17 11:13 bisheng_langchain/input_output/output.py
--rw-r--r--  2.0 unx      210 b- defN 24-Apr-17 11:13 bisheng_langchain/retrievers/__init__.py
--rw-r--r--  2.0 unx     5942 b- defN 24-Apr-17 11:13 bisheng_langchain/retrievers/ensemble.py
--rw-r--r--  2.0 unx     4465 b- defN 24-Apr-17 11:13 bisheng_langchain/retrievers/mix_es_vector.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 11:13 bisheng_langchain/utils/__init__.py
--rw-r--r--  2.0 unx     8688 b- defN 24-Apr-17 11:13 bisheng_langchain/utils/requests.py
--rw-r--r--  2.0 unx      213 b- defN 24-Apr-17 11:13 bisheng_langchain/vectorstores/__init__.py
--rw-r--r--  2.0 unx    13286 b- defN 24-Apr-17 11:13 bisheng_langchain/vectorstores/elastic_keywords_search.py
--rw-r--r--  2.0 unx    36297 b- defN 24-Apr-17 11:13 bisheng_langchain/vectorstores/milvus.py
--rw-r--r--  2.0 unx     4353 b- defN 24-Apr-17 11:13 bisheng_langchain/vectorstores/retriever.py
--rw-r--r--  2.0 unx     2414 b- defN 24-Apr-17 11:13 bisheng_langchain-0.3.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 11:13 bisheng_langchain-0.3.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Apr-17 11:13 bisheng_langchain-0.3.0rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    11716 b- defN 24-Apr-17 11:13 bisheng_langchain-0.3.0rc1.dist-info/RECORD
-114 files, 540745 bytes uncompressed, 153276 bytes compressed:  71.7%
+Zip file size: 224447 bytes, number of entries: 149
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/__init__.py
+-rw-r--r--  2.0 unx     7909 b- defN 24-May-16 12:29 bisheng_langchain/text_splitter.py
+-rw-r--r--  2.0 unx      226 b- defN 24-May-16 12:29 bisheng_langchain/agents/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/agents/chatglm_functions_agent/__init__.py
+-rw-r--r--  2.0 unx    13674 b- defN 24-May-16 12:29 bisheng_langchain/agents/chatglm_functions_agent/base.py
+-rw-r--r--  2.0 unx     3497 b- defN 24-May-16 12:29 bisheng_langchain/agents/chatglm_functions_agent/output_parser.py
+-rw-r--r--  2.0 unx      992 b- defN 24-May-16 12:29 bisheng_langchain/agents/chatglm_functions_agent/prompt.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/agents/llm_functions_agent/__init__.py
+-rw-r--r--  2.0 unx    12296 b- defN 24-May-16 12:29 bisheng_langchain/agents/llm_functions_agent/base.py
+-rw-r--r--  2.0 unx      430 b- defN 24-May-16 12:29 bisheng_langchain/autogen_role/__init__.py
+-rw-r--r--  2.0 unx     4657 b- defN 24-May-16 12:29 bisheng_langchain/autogen_role/assistant.py
+-rw-r--r--  2.0 unx     2464 b- defN 24-May-16 12:29 bisheng_langchain/autogen_role/custom.py
+-rw-r--r--  2.0 unx     2234 b- defN 24-May-16 12:29 bisheng_langchain/autogen_role/groupchat_manager.py
+-rw-r--r--  2.0 unx     5715 b- defN 24-May-16 12:29 bisheng_langchain/autogen_role/user.py
+-rw-r--r--  2.0 unx      759 b- defN 24-May-16 12:29 bisheng_langchain/chains/__init__.py
+-rw-r--r--  2.0 unx     1903 b- defN 24-May-16 12:29 bisheng_langchain/chains/loader_output.py
+-rw-r--r--  2.0 unx     2805 b- defN 24-May-16 12:29 bisheng_langchain/chains/transform.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/chains/autogen/__init__.py
+-rw-r--r--  2.0 unx     3270 b- defN 24-May-16 12:29 bisheng_langchain/chains/autogen/auto_gen.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/chains/combine_documents/__init__.py
+-rw-r--r--  2.0 unx     2369 b- defN 24-May-16 12:29 bisheng_langchain/chains/combine_documents/stuff.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/chains/conversational_retrieval/__init__.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-May-16 12:29 bisheng_langchain/chains/conversational_retrieval/base.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-May-16 12:29 bisheng_langchain/chains/question_answering/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/chains/retrieval/__init__.py
+-rw-r--r--  2.0 unx     3050 b- defN 24-May-16 12:29 bisheng_langchain/chains/retrieval/retrieval_chain.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/chains/router/__init__.py
+-rw-r--r--  2.0 unx      375 b- defN 24-May-16 12:29 bisheng_langchain/chains/router/multi_rule.py
+-rw-r--r--  2.0 unx     1835 b- defN 24-May-16 12:29 bisheng_langchain/chains/router/rule_router.py
+-rw-r--r--  2.0 unx      635 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/__init__.py
+-rw-r--r--  2.0 unx    23153 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/host_llm.py
+-rw-r--r--  2.0 unx    13901 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/minimax.py
+-rw-r--r--  2.0 unx    17082 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/proxy_llm.py
+-rw-r--r--  2.0 unx    19971 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/qwen.py
+-rw-r--r--  2.0 unx    17056 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/sensetime.py
+-rw-r--r--  2.0 unx    13671 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/wenxin.py
+-rw-r--r--  2.0 unx    14037 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/xunfeiai.py
+-rw-r--r--  2.0 unx    15342 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/zhipuai.py
+-rw-r--r--  2.0 unx      443 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/interface/__init__.py
+-rw-r--r--  2.0 unx     4423 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/interface/minimax.py
+-rw-r--r--  2.0 unx     2081 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/interface/openai.py
+-rw-r--r--  2.0 unx     1141 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/interface/types.py
+-rw-r--r--  2.0 unx       65 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/interface/utils.py
+-rw-r--r--  2.0 unx     4246 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/interface/wenxin.py
+-rw-r--r--  2.0 unx     7514 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/interface/xunfei.py
+-rw-r--r--  2.0 unx     2636 b- defN 24-May-16 12:29 bisheng_langchain/chat_models/interface/zhipuai.py
+-rw-r--r--  2.0 unx      366 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/__init__.py
+-rw-r--r--  2.0 unx     6656 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/custom_kv.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/elem_html.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/elem_image.py
+-rw-r--r--  2.0 unx    22243 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/elem_pdf.py
+-rw-r--r--  2.0 unx     5336 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/elem_unstrcutured_loader.py
+-rw-r--r--  2.0 unx     4063 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/universal_kv.py
+-rw-r--r--  2.0 unx      171 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/parsers/__init__.py
+-rw-r--r--  2.0 unx     1760 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/parsers/ellm_client.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/parsers/image.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/parsers/ocr_client.py
+-rw-r--r--  2.0 unx     8685 b- defN 24-May-16 12:29 bisheng_langchain/document_loaders/parsers/test_image.py
+-rw-r--r--  2.0 unx      534 b- defN 24-May-16 12:29 bisheng_langchain/embeddings/__init__.py
+-rw-r--r--  2.0 unx     6295 b- defN 24-May-16 12:29 bisheng_langchain/embeddings/host_embedding.py
+-rw-r--r--  2.0 unx     3192 b- defN 24-May-16 12:29 bisheng_langchain/embeddings/huggingfacegte.py
+-rw-r--r--  2.0 unx     3415 b- defN 24-May-16 12:29 bisheng_langchain/embeddings/huggingfacemultilingual.py
+-rw-r--r--  2.0 unx     4737 b- defN 24-May-16 12:29 bisheng_langchain/embeddings/wenxin.py
+-rw-r--r--  2.0 unx       98 b- defN 24-May-16 12:29 bisheng_langchain/embeddings/interface/__init__.py
+-rw-r--r--  2.0 unx      461 b- defN 24-May-16 12:29 bisheng_langchain/embeddings/interface/types.py
+-rw-r--r--  2.0 unx     3104 b- defN 24-May-16 12:29 bisheng_langchain/embeddings/interface/wenxin.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/gpts/__init__.py
+-rw-r--r--  2.0 unx     5344 b- defN 24-May-16 12:29 bisheng_langchain/gpts/assistant.py
+-rw-r--r--  2.0 unx     3626 b- defN 24-May-16 12:29 bisheng_langchain/gpts/auto_optimization.py
+-rw-r--r--  2.0 unx     1582 b- defN 24-May-16 12:29 bisheng_langchain/gpts/auto_tool_selected.py
+-rw-r--r--  2.0 unx     8099 b- defN 24-May-16 12:29 bisheng_langchain/gpts/load_tools.py
+-rw-r--r--  2.0 unx      213 b- defN 24-May-16 12:29 bisheng_langchain/gpts/message_types.py
+-rw-r--r--  2.0 unx     6671 b- defN 24-May-16 12:29 bisheng_langchain/gpts/utils.py
+-rw-r--r--  2.0 unx      261 b- defN 24-May-16 12:29 bisheng_langchain/gpts/agent_types/__init__.py
+-rw-r--r--  2.0 unx     8715 b- defN 24-May-16 12:29 bisheng_langchain/gpts/agent_types/llm_functions_agent.py
+-rw-r--r--  2.0 unx      704 b- defN 24-May-16 12:29 bisheng_langchain/gpts/prompts/__init__.py
+-rw-r--r--  2.0 unx       57 b- defN 24-May-16 12:29 bisheng_langchain/gpts/prompts/assistant_prompt_base.py
+-rw-r--r--  2.0 unx     2421 b- defN 24-May-16 12:29 bisheng_langchain/gpts/prompts/assistant_prompt_cohere.py
+-rw-r--r--  2.0 unx     4151 b- defN 24-May-16 12:29 bisheng_langchain/gpts/prompts/assistant_prompt_opt.py
+-rw-r--r--  2.0 unx     5336 b- defN 24-May-16 12:29 bisheng_langchain/gpts/prompts/breif_description_prompt.py
+-rw-r--r--  2.0 unx     5965 b- defN 24-May-16 12:29 bisheng_langchain/gpts/prompts/opening_dialog_prompt.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-16 12:29 bisheng_langchain/gpts/prompts/select_tools_prompt.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/__init__.py
+-rw-r--r--  2.0 unx     1608 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/api_tools/__init__.py
+-rw-r--r--  2.0 unx     3618 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/api_tools/base.py
+-rw-r--r--  2.0 unx     2461 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/api_tools/flow.py
+-rw-r--r--  2.0 unx    27429 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/api_tools/macro_data.py
+-rw-r--r--  2.0 unx     3907 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/api_tools/openapi.py
+-rw-r--r--  2.0 unx     9542 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/api_tools/sina.py
+-rw-r--r--  2.0 unx     6684 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/api_tools/tianyancha.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/bing_search/__init__.py
+-rw-r--r--  2.0 unx     1710 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/bing_search/tool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/calculator/__init__.py
+-rw-r--r--  2.0 unx      705 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/calculator/tool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/code_interpreter/__init__.py
+-rw-r--r--  2.0 unx    11443 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/code_interpreter/tool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/dalle_image_generator/__init__.py
+-rw-r--r--  2.0 unx     7528 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/dalle_image_generator/tool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/get_current_time/__init__.py
+-rw-r--r--  2.0 unx      801 b- defN 24-May-16 12:29 bisheng_langchain/gpts/tools/get_current_time/tool.py
+-rw-r--r--  2.0 unx      153 b- defN 24-May-16 12:29 bisheng_langchain/input_output/__init__.py
+-rw-r--r--  2.0 unx     1094 b- defN 24-May-16 12:29 bisheng_langchain/input_output/input.py
+-rw-r--r--  2.0 unx    11585 b- defN 24-May-16 12:29 bisheng_langchain/input_output/output.py
+-rw-r--r--  2.0 unx      102 b- defN 24-May-16 12:29 bisheng_langchain/rag/__init__.py
+-rw-r--r--  2.0 unx    13749 b- defN 24-May-16 12:29 bisheng_langchain/rag/bisheng_rag_pipeline.py
+-rw-r--r--  2.0 unx    15898 b- defN 24-May-16 12:29 bisheng_langchain/rag/bisheng_rag_pipeline_v2.py
+-rw-r--r--  2.0 unx    16816 b- defN 24-May-16 12:29 bisheng_langchain/rag/bisheng_rag_pipeline_v2_cohere_raw_prompting.py
+-rw-r--r--  2.0 unx    11971 b- defN 24-May-16 12:29 bisheng_langchain/rag/bisheng_rag_tool.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-16 12:29 bisheng_langchain/rag/extract_info.py
+-rw-r--r--  2.0 unx     1840 b- defN 24-May-16 12:29 bisheng_langchain/rag/run_qa_gen_web.py
+-rw-r--r--  2.0 unx     2224 b- defN 24-May-16 12:29 bisheng_langchain/rag/run_rag_evaluate_web.py
+-rw-r--r--  2.0 unx     6361 b- defN 24-May-16 12:29 bisheng_langchain/rag/utils.py
+-rw-r--r--  2.0 unx     2266 b- defN 24-May-16 12:29 bisheng_langchain/rag/config/baseline.yaml
+-rw-r--r--  2.0 unx     2174 b- defN 24-May-16 12:29 bisheng_langchain/rag/config/baseline_caibao.yaml
+-rw-r--r--  2.0 unx     2812 b- defN 24-May-16 12:29 bisheng_langchain/rag/config/baseline_caibao_knowledge_v2.yaml
+-rw-r--r--  2.0 unx     2846 b- defN 24-May-16 12:29 bisheng_langchain/rag/config/baseline_caibao_v2.yaml
+-rw-r--r--  2.0 unx     2382 b- defN 24-May-16 12:29 bisheng_langchain/rag/config/baseline_demo_v2.yaml
+-rw-r--r--  2.0 unx     2398 b- defN 24-May-16 12:29 bisheng_langchain/rag/config/baseline_s2b_mix.yaml
+-rw-r--r--  2.0 unx     2350 b- defN 24-May-16 12:29 bisheng_langchain/rag/config/baseline_v2.yaml
+-rw-r--r--  2.0 unx      218 b- defN 24-May-16 12:29 bisheng_langchain/rag/init_retrievers/__init__.py
+-rw-r--r--  2.0 unx     2362 b- defN 24-May-16 12:29 bisheng_langchain/rag/init_retrievers/baseline_vector_retriever.py
+-rw-r--r--  2.0 unx     2523 b- defN 24-May-16 12:29 bisheng_langchain/rag/init_retrievers/keyword_retriever.py
+-rw-r--r--  2.0 unx     4653 b- defN 24-May-16 12:29 bisheng_langchain/rag/init_retrievers/mix_retriever.py
+-rw-r--r--  2.0 unx     3805 b- defN 24-May-16 12:29 bisheng_langchain/rag/init_retrievers/smaller_chunks_retriever.py
+-rw-r--r--  2.0 unx      223 b- defN 24-May-16 12:29 bisheng_langchain/rag/prompts/__init__.py
+-rw-r--r--  2.0 unx     1456 b- defN 24-May-16 12:29 bisheng_langchain/rag/prompts/extract_key_prompt.py
+-rw-r--r--  2.0 unx     1925 b- defN 24-May-16 12:29 bisheng_langchain/rag/prompts/prompt.py
+-rw-r--r--  2.0 unx     8151 b- defN 24-May-16 12:29 bisheng_langchain/rag/prompts/prompt_cohere.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/rag/qa_corpus/__init__.py
+-rw-r--r--  2.0 unx     6092 b- defN 24-May-16 12:29 bisheng_langchain/rag/qa_corpus/qa_generator.py
+-rw-r--r--  2.0 unx       72 b- defN 24-May-16 12:29 bisheng_langchain/rag/rerank/__init__.py
+-rw-r--r--  2.0 unx     1836 b- defN 24-May-16 12:29 bisheng_langchain/rag/rerank/rerank.py
+-rw-r--r--  2.0 unx     4490 b- defN 24-May-16 12:29 bisheng_langchain/rag/rerank/rerank_benchmark.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/rag/scoring/__init__.py
+-rw-r--r--  2.0 unx     3001 b- defN 24-May-16 12:29 bisheng_langchain/rag/scoring/llama_index_score.py
+-rw-r--r--  2.0 unx     7110 b- defN 24-May-16 12:29 bisheng_langchain/rag/scoring/ragas_score.py
+-rw-r--r--  2.0 unx      210 b- defN 24-May-16 12:29 bisheng_langchain/retrievers/__init__.py
+-rw-r--r--  2.0 unx     5975 b- defN 24-May-16 12:29 bisheng_langchain/retrievers/ensemble.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-May-16 12:29 bisheng_langchain/retrievers/mix_es_vector.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 12:29 bisheng_langchain/utils/__init__.py
+-rw-r--r--  2.0 unx     8688 b- defN 24-May-16 12:29 bisheng_langchain/utils/requests.py
+-rw-r--r--  2.0 unx      213 b- defN 24-May-16 12:29 bisheng_langchain/vectorstores/__init__.py
+-rw-r--r--  2.0 unx    13347 b- defN 24-May-16 12:29 bisheng_langchain/vectorstores/elastic_keywords_search.py
+-rw-r--r--  2.0 unx    36297 b- defN 24-May-16 12:29 bisheng_langchain/vectorstores/milvus.py
+-rw-r--r--  2.0 unx     4353 b- defN 24-May-16 12:29 bisheng_langchain/vectorstores/retriever.py
+-rw-r--r--  2.0 unx     2411 b- defN 24-May-16 12:29 bisheng_langchain-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 12:29 bisheng_langchain-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-May-16 12:29 bisheng_langchain-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    15365 b- defN 24-May-16 12:29 bisheng_langchain-0.3.1.dist-info/RECORD
+149 files, 687737 bytes uncompressed, 199099 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -222,18 +222,21 @@
 
 Filename: bisheng_langchain/gpts/agent_types/llm_functions_agent.py
 Comment: 
 
 Filename: bisheng_langchain/gpts/prompts/__init__.py
 Comment: 
 
-Filename: bisheng_langchain/gpts/prompts/assistant_prompt_opt.py
+Filename: bisheng_langchain/gpts/prompts/assistant_prompt_base.py
 Comment: 
 
-Filename: bisheng_langchain/gpts/prompts/base_prompt.py
+Filename: bisheng_langchain/gpts/prompts/assistant_prompt_cohere.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/prompts/assistant_prompt_opt.py
 Comment: 
 
 Filename: bisheng_langchain/gpts/prompts/breif_description_prompt.py
 Comment: 
 
 Filename: bisheng_langchain/gpts/prompts/opening_dialog_prompt.py
 Comment: 
@@ -252,14 +255,17 @@
 
 Filename: bisheng_langchain/gpts/tools/api_tools/flow.py
 Comment: 
 
 Filename: bisheng_langchain/gpts/tools/api_tools/macro_data.py
 Comment: 
 
+Filename: bisheng_langchain/gpts/tools/api_tools/openapi.py
+Comment: 
+
 Filename: bisheng_langchain/gpts/tools/api_tools/sina.py
 Comment: 
 
 Filename: bisheng_langchain/gpts/tools/api_tools/tianyancha.py
 Comment: 
 
 Filename: bisheng_langchain/gpts/tools/bing_search/__init__.py
@@ -297,14 +303,113 @@
 
 Filename: bisheng_langchain/input_output/input.py
 Comment: 
 
 Filename: bisheng_langchain/input_output/output.py
 Comment: 
 
+Filename: bisheng_langchain/rag/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/rag/bisheng_rag_pipeline.py
+Comment: 
+
+Filename: bisheng_langchain/rag/bisheng_rag_pipeline_v2.py
+Comment: 
+
+Filename: bisheng_langchain/rag/bisheng_rag_pipeline_v2_cohere_raw_prompting.py
+Comment: 
+
+Filename: bisheng_langchain/rag/bisheng_rag_tool.py
+Comment: 
+
+Filename: bisheng_langchain/rag/extract_info.py
+Comment: 
+
+Filename: bisheng_langchain/rag/run_qa_gen_web.py
+Comment: 
+
+Filename: bisheng_langchain/rag/run_rag_evaluate_web.py
+Comment: 
+
+Filename: bisheng_langchain/rag/utils.py
+Comment: 
+
+Filename: bisheng_langchain/rag/config/baseline.yaml
+Comment: 
+
+Filename: bisheng_langchain/rag/config/baseline_caibao.yaml
+Comment: 
+
+Filename: bisheng_langchain/rag/config/baseline_caibao_knowledge_v2.yaml
+Comment: 
+
+Filename: bisheng_langchain/rag/config/baseline_caibao_v2.yaml
+Comment: 
+
+Filename: bisheng_langchain/rag/config/baseline_demo_v2.yaml
+Comment: 
+
+Filename: bisheng_langchain/rag/config/baseline_s2b_mix.yaml
+Comment: 
+
+Filename: bisheng_langchain/rag/config/baseline_v2.yaml
+Comment: 
+
+Filename: bisheng_langchain/rag/init_retrievers/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/rag/init_retrievers/baseline_vector_retriever.py
+Comment: 
+
+Filename: bisheng_langchain/rag/init_retrievers/keyword_retriever.py
+Comment: 
+
+Filename: bisheng_langchain/rag/init_retrievers/mix_retriever.py
+Comment: 
+
+Filename: bisheng_langchain/rag/init_retrievers/smaller_chunks_retriever.py
+Comment: 
+
+Filename: bisheng_langchain/rag/prompts/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/rag/prompts/extract_key_prompt.py
+Comment: 
+
+Filename: bisheng_langchain/rag/prompts/prompt.py
+Comment: 
+
+Filename: bisheng_langchain/rag/prompts/prompt_cohere.py
+Comment: 
+
+Filename: bisheng_langchain/rag/qa_corpus/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/rag/qa_corpus/qa_generator.py
+Comment: 
+
+Filename: bisheng_langchain/rag/rerank/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/rag/rerank/rerank.py
+Comment: 
+
+Filename: bisheng_langchain/rag/rerank/rerank_benchmark.py
+Comment: 
+
+Filename: bisheng_langchain/rag/scoring/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/rag/scoring/llama_index_score.py
+Comment: 
+
+Filename: bisheng_langchain/rag/scoring/ragas_score.py
+Comment: 
+
 Filename: bisheng_langchain/retrievers/__init__.py
 Comment: 
 
 Filename: bisheng_langchain/retrievers/ensemble.py
 Comment: 
 
 Filename: bisheng_langchain/retrievers/mix_es_vector.py
@@ -324,20 +429,20 @@
 
 Filename: bisheng_langchain/vectorstores/milvus.py
 Comment: 
 
 Filename: bisheng_langchain/vectorstores/retriever.py
 Comment: 
 
-Filename: bisheng_langchain-0.3.0rc1.dist-info/METADATA
+Filename: bisheng_langchain-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: bisheng_langchain-0.3.0rc1.dist-info/WHEEL
+Filename: bisheng_langchain-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: bisheng_langchain-0.3.0rc1.dist-info/top_level.txt
+Filename: bisheng_langchain-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bisheng_langchain-0.3.0rc1.dist-info/RECORD
+Filename: bisheng_langchain-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bisheng_langchain/document_loaders/elem_unstrcutured_loader.py

```diff
@@ -81,24 +81,26 @@
         parameters = {'start': self.start, 'n': self.n}
         parameters.update(self.extra_kwargs)
         payload = dict(filename=os.path.basename(self.file_name),
                        b64_data=[b64_data],
                        mode='partition',
                        parameters=parameters)
 
-        resp = requests.post(self.unstructured_api_url, headers=self.headers, json=payload).json()
+        resp = requests.post(self.unstructured_api_url, headers=self.headers, json=payload)
+        if resp.status_code != 200:
+            raise Exception(f'file partition {os.path.basename(self.file_name)} failed resp={resp.text}')
 
+        resp = resp.json()
         if 200 != resp.get('status_code'):
-            logger.info(f'not return resp={resp}')
+            logger.info(f'file partition {os.path.basename(self.file_name)} error resp={resp}')
         partitions = resp['partitions']
         if not partitions:
             logger.info(f'partition_error resp={resp}')
         logger.info(f'unstruct_return code={resp.get("status_code")}')
 
-        partitions = resp['partitions']
         content, metadata = merge_partitions(partitions)
         metadata['source'] = self.file_name
 
         doc = Document(page_content=content, metadata=metadata)
         return [doc]
```

## bisheng_langchain/gpts/assistant.py

```diff
@@ -122,16 +122,19 @@
         result = asyncio.run(self.assistant.ainvoke(inputs))
         return result
 
 
 if __name__ == "__main__":
     from langchain.globals import set_debug
 
-    set_debug(True)
-    # chat_history = []
-    chat_history = ['你好', '你好，有什么可以帮助你吗？', '福蓉科技股价多少?', '福蓉科技（股票代码：300049）的当前股价为48.67元。']
-    query = "去年这个时候的股价是多少？"
-    bisheng_assistant = BishengAssistant("config/base_scene.yaml")
+    # set_debug(True)
+    chat_history = []
+    query = "请简要分析中科创达软件股份有限公司2019年聘任、解聘会计师事务的情况。"
+    # chat_history = ['你好', '你好，有什么可以帮助你吗？', '福蓉科技股价多少?', '福蓉科技（股票代码：300049）的当前股价为48.67元。']
+    # query = '去年这个时候的股价是多少？'
+    # bisheng_assistant = BishengAssistant("config/base_scene.yaml")
+    # bisheng_assistant = BishengAssistant("config/knowledge_scene.yaml")
+    bisheng_assistant = BishengAssistant("config/rag_scene.yaml")
     result = bisheng_assistant.run(query, chat_history=chat_history)
     for r in result:
         print(f'------------------')
         print(type(r), r)
```

## bisheng_langchain/gpts/load_tools.py

```diff
@@ -22,14 +22,15 @@
 from langchain_community.tools.bearly.tool import BearlyInterpreterTool
 from langchain_community.utilities.arxiv import ArxivAPIWrapper
 from langchain_community.utilities.bing_search import BingSearchAPIWrapper
 from langchain_core.callbacks import BaseCallbackManager, Callbacks
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.tools import BaseTool, Tool
 from mypy_extensions import Arg, KwArg
+from bisheng_langchain.rag import BishengRAGTool
 
 
 def _get_current_time() -> BaseTool:
     return get_current_time
 
 
 def _get_calculator() -> BaseTool:
@@ -82,14 +83,15 @@
 
 
 # 第二个list内填必填参数，第三个list内填可选参数
 _EXTRA_PARAM_TOOLS: Dict[str, Tuple[Callable[[KwArg(Any)], BaseTool], List[Optional[str]], List[Optional[str]]]] = {  # type: ignore
     'dalle_image_generator': (_get_dalle_image_generator, ['openai_api_key', 'openai_proxy'], []),
     'bing_search': (_get_bing_search, ['bing_subscription_key', 'bing_search_url'], []),
     'bisheng_code_interpreter': (_get_native_code_interpreter, ["minio"], ['files']),
+    'bisheng_rag': (BishengRAGTool.get_rag_tool, ['name', 'description'], ['vector_store', 'keyword_store', 'llm', 'collection_name', 'max_content', 'sort_by_source_and_index']),
 }
 
 _API_TOOLS: Dict[str, Tuple[Callable[[KwArg(Any)], BaseTool], List[str]]] = {**ALL_API_TOOLS}  # type: ignore
 
 _ALL_TOOLS = {
     **_BASE_TOOLS,
     **_LLM_TOOLS,
```

## bisheng_langchain/gpts/agent_types/llm_functions_agent.py

```diff
@@ -1,9 +1,9 @@
 import json
-
+import re
 from bisheng_langchain.gpts.message_types import LiberalFunctionMessage, LiberalToolMessage
 from langchain.tools import BaseTool
 from langchain.tools.render import format_tool_to_openai_tool
 from langchain_core.language_models.base import LanguageModelLike
 from langchain_core.messages import FunctionMessage, SystemMessage, ToolMessage
 from langgraph.graph import END
 from langgraph.graph.message import MessageGraph
@@ -35,14 +35,20 @@
     tool_executor = ToolExecutor(tools)
 
     # Define the function that determines whether to continue or not
     def should_continue(messages):
         last_message = messages[-1]
         # If there is no function call, then we finish
         if 'tool_calls' not in last_message.additional_kwargs:
+            if '|<instruct>|' in system_message:
+                # cohere model
+                pattern = r"Answer:(.+)\nGrounded answer"
+                match = re.search(pattern, last_message.content)
+                if match:
+                    last_message.content = match.group(1)
             return 'end'
         # Otherwise if there is, we continue
         else:
             return 'continue'
 
     # Define the function to execute tools
     async def call_tool(messages):
```

## bisheng_langchain/gpts/prompts/__init__.py

```diff
@@ -1,15 +1,17 @@
 from bisheng_langchain.gpts.prompts.assistant_prompt_opt import ASSISTANT_PROMPT_OPT
-from bisheng_langchain.gpts.prompts.base_prompt import DEFAULT_SYSTEM_MESSAGE
+from bisheng_langchain.gpts.prompts.assistant_prompt_base import ASSISTANT_PROMPT_DEFAULT
+from bisheng_langchain.gpts.prompts.assistant_prompt_cohere import ASSISTANT_PROMPT_COHERE
 from bisheng_langchain.gpts.prompts.breif_description_prompt import BREIF_DES_PROMPT
 from bisheng_langchain.gpts.prompts.opening_dialog_prompt import OPENDIALOG_PROMPT
 from bisheng_langchain.gpts.prompts.select_tools_prompt import HUMAN_MSG, SYS_MSG
 
 
 __all__ = [
-    "DEFAULT_SYSTEM_MESSAGE",
+    "ASSISTANT_PROMPT_DEFAULT",
+    "ASSISTANT_PROMPT_COHERE",
     "ASSISTANT_PROMPT_OPT",
     "OPENDIALOG_PROMPT",
     "BREIF_DES_PROMPT",
     "SYS_MSG",
     "HUMAN_MSG",
 ]
```

## bisheng_langchain/gpts/tools/api_tools/flow.py

```diff
@@ -1,14 +1,15 @@
 from loguru import logger
-from pydantic import BaseModel, Field
+from langchain_core.pydantic_v1 import BaseModel, Field
 from typing import Any
 from .base import APIToolBase
 from .base import MultArgsSchemaTool
 from langchain_core.tools import BaseTool
 
+
 class FlowTools(APIToolBase):
 
     def run(self, query: str) -> str:
         """Run query through api and parse result."""
         if query:
             self.params[self.input_key] = {
                 'question': query
@@ -48,17 +49,16 @@
                 'Milvus-9KIR6': {
                     'collection_id': collection_id
                 }
             }
         }
 
         class InputArgs(BaseModel):
-            """args_schema"""
             query: str = Field(description='questions to ask')
-              
+
         return cls(url=url, params=params, input_key=input_key, args_schema=InputArgs)
     
     @classmethod
     def get_api_tool(cls, name, **kwargs: Any) -> BaseTool:
         attr_name = name.split('_', 1)[-1]
         class_method = getattr(cls, attr_name)
         function_description = kwargs.get('description','')
```

## bisheng_langchain/retrievers/ensemble.py

```diff
@@ -63,27 +63,28 @@
         return fused_documents
 
     async def _aget_relevant_documents(
         self,
         query: str,
         *,
         run_manager: AsyncCallbackManagerForRetrieverRun,
+        **kwagrs: Any,
     ) -> List[Document]:
         """
         Asynchronously get the relevant documents for a given query.
 
         Args:
             query: The query to search for.
 
         Returns:
             A list of reranked documents.
         """
 
         # Get fused result of the retrievers.
-        fused_documents = await self.arank_fusion(query, run_manager)
+        fused_documents = await self.arank_fusion(query, run_manager, **kwagrs)
 
         return fused_documents
 
     def rank_fusion(
         self,
         query: str,
         run_manager: CallbackManagerForRetrieverRun,
```

## bisheng_langchain/vectorstores/elastic_keywords_search.py

```diff
@@ -224,24 +224,25 @@
         if k == 0:
             # pm need to control
             return []
         assert must_or_should in ['must', 'should'], 'only support must and should.'
         # llm or jiaba extract keywords
         if self.llm_chain:
             keywords_str = self.llm_chain.run(query)
-            print('keywords_str:', keywords_str)
+            print('llm search keywords:', keywords_str)
             try:
                 keywords = eval(keywords_str)
                 if not isinstance(keywords, list):
                     raise ValueError('Keywords extracted by llm is not list.')
             except Exception as e:
                 print(str(e))
                 keywords = jieba.analyse.extract_tags(query, topK=10, withWeight=False)
         else:
             keywords = jieba.analyse.extract_tags(query, topK=10, withWeight=False)
+            print('jieba search keywords:', keywords)
         match_query = {'bool': {must_or_should: []}}
         for key in keywords:
             match_query['bool'][must_or_should].append({query_strategy: {'text': key}})
         response = self.client_search(self.client, self.index_name, match_query, size=k)
         hits = [hit for hit in response['hits']['hits']]
         docs_and_scores = [(
             Document(
```

## Comparing `bisheng_langchain-0.3.0rc1.dist-info/METADATA` & `bisheng_langchain-0.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisheng-langchain
-Version: 0.3.0rc1
+Version: 0.3.1
 Summary: bisheng langchain modules
 Home-page: https://github.com/dataelement/bisheng
 Author: DataElem
 Author-email: contact@dataelem.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `bisheng_langchain-0.3.0rc1.dist-info/RECORD` & `bisheng_langchain-0.3.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 bisheng_langchain/chat_models/interface/xunfei.py,sha256=DPHAZM_uHg0A8GnebgkRbLENhBW7bBtRHzKC0gFKZgc,7514
 bisheng_langchain/chat_models/interface/zhipuai.py,sha256=67Ej6DRk-IlXUfEZPg-pjcYPyqZb32ClrBP-9k-3EEs,2636
 bisheng_langchain/document_loaders/__init__.py,sha256=LuQ-zMYxde2FeiEcvVtjQqnHozki5pF_pDDa88_fBdg,366
 bisheng_langchain/document_loaders/custom_kv.py,sha256=xWUPhcr1hjbdya4zgEHG4Fl0sI4RNQ6D2vqFo0c24G8,6656
 bisheng_langchain/document_loaders/elem_html.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/document_loaders/elem_image.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/document_loaders/elem_pdf.py,sha256=K-TXILGNFLFjavhun_MFbUF4t2_WGA3Z-kbnr75lmW8,22243
-bisheng_langchain/document_loaders/elem_unstrcutured_loader.py,sha256=bJQObxHnk8FaF8RUBkqODzgeikrZ8wdl_TQPa2oEoQo,5169
+bisheng_langchain/document_loaders/elem_unstrcutured_loader.py,sha256=Dcu70Wz4vdUpq9y2vWPWroRdq6JrlOJNERoFTnZO0oU,5336
 bisheng_langchain/document_loaders/universal_kv.py,sha256=dJF_GQGKBMUjB_kX9CSp7xZRhXgwVuGPbMIzJwPh-C0,4063
 bisheng_langchain/document_loaders/parsers/__init__.py,sha256=OOM_FJkwaU-zNS58fASw0TH8FNT6VXKb0VrvisgdrII,171
 bisheng_langchain/document_loaders/parsers/ellm_client.py,sha256=B4Dea8xXXnGvB9j2OXv53HILNUmnWeNJz9ssNM-2fLM,1760
 bisheng_langchain/document_loaders/parsers/image.py,sha256=7Vx4dD_WiSTojS4TMIJFxfE8nvze0kwNnwTd6f1cLds,938
 bisheng_langchain/document_loaders/parsers/ocr_client.py,sha256=rRh1coJYn24n7FaINBZH5yO6Edm9TRywY6UOXpcerVo,1612
 bisheng_langchain/document_loaders/parsers/test_image.py,sha256=EJHozq5oFfLBlLL5Lr6XFkrkvSttPpohprs9OjDzAKM,8685
 bisheng_langchain/embeddings/__init__.py,sha256=_zLLb9cH4Ct4UpKQhtXr7V2IQ7LUnlCKkKTroTE_Enk,534
@@ -61,33 +61,35 @@
 bisheng_langchain/embeddings/huggingfacegte.py,sha256=RPfSXu7oMv6vgIjLqrPZ1Qz3K0yEuYn7VO0u7m7PzK8,3192
 bisheng_langchain/embeddings/huggingfacemultilingual.py,sha256=g7-yKJ-qIPUZQaRnGz312S-f3aJCGcdHemAR3znE-uo,3415
 bisheng_langchain/embeddings/wenxin.py,sha256=6zx53tSUguvny4gGe5CTmfwV-QtGqKmcT-Jlgf2xVUs,4737
 bisheng_langchain/embeddings/interface/__init__.py,sha256=GNY3tibpRxpAdAfSvQmXBKo0xKSLke_9y4clofi_WOE,98
 bisheng_langchain/embeddings/interface/types.py,sha256=VdurbtsnjCPdlOjPFcK2Mg6r9bJYYHb3tepvkk-y3nM,461
 bisheng_langchain/embeddings/interface/wenxin.py,sha256=5d9gI4enmfkD80s0FHKiDt33O0mwM8Xc5WTubnMUy8c,3104
 bisheng_langchain/gpts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bisheng_langchain/gpts/assistant.py,sha256=KCYPU1Bs4GtWcLk9Ya2NuQyXE0Twn7-92eSBTIzpq7I,5083
+bisheng_langchain/gpts/assistant.py,sha256=OEB9HA-FpNKGOviVoafld4MHDIEQS5u9AU0QlMuJ-po,5344
 bisheng_langchain/gpts/auto_optimization.py,sha256=WNsC19rgvuDYQlSIaYThq5RqCbuobDbzCwAJW4Ksw0c,3626
 bisheng_langchain/gpts/auto_tool_selected.py,sha256=21WETf9o0YS-QEBwv3mmZRObKWszefQkXEqAA6KzoaM,1582
-bisheng_langchain/gpts/load_tools.py,sha256=JZpwTH5cvaLdab8-TbTxBGHug-llnCQR0wB4VsduSrs,7871
+bisheng_langchain/gpts/load_tools.py,sha256=LiiK1OqFu7Ki-F_Rhfi1rgp0wBQCSrTDdqsgwciTOIU,8099
 bisheng_langchain/gpts/message_types.py,sha256=7EJOx62j9E1U67jxWgxE_I7a8IjAvvKANknXkD2gFm0,213
 bisheng_langchain/gpts/utils.py,sha256=t3YDxaJ0OYd6EKsek7PJFRYnsezwzEFK5oVU-PRbu5g,6671
 bisheng_langchain/gpts/agent_types/__init__.py,sha256=bg0zlTYGfNXoSBqcICHlzNpVQbejMYeyji_dzvP5qQ0,261
-bisheng_langchain/gpts/agent_types/llm_functions_agent.py,sha256=ynFHXuaqABeiKvhcetOFQPyQMlNtEAdtTccoIwiJbGQ,8419
-bisheng_langchain/gpts/prompts/__init__.py,sha256=IfuoxVpsSLKJtDx0aJbRgnSZYZr_kDPsL92CvefzF-s,568
+bisheng_langchain/gpts/agent_types/llm_functions_agent.py,sha256=IXg5u8dSk-FcLvjrvvLcN5revGccXylXkD73ZWhaDWs,8715
+bisheng_langchain/gpts/prompts/__init__.py,sha256=pOnXvk6_PjqAoLrh68sI9o3o6znKGxoLMVFP-0XTCJo,704
+bisheng_langchain/gpts/prompts/assistant_prompt_base.py,sha256=Q69qWxtwaeGPPwMWXQ44OsQPg7wHB7nYT17wbqQe3kM,57
+bisheng_langchain/gpts/prompts/assistant_prompt_cohere.py,sha256=GLQ77oXqSlE7Xes2ObsFsNon5nOJOCRhQOKE5bUpgaI,2421
 bisheng_langchain/gpts/prompts/assistant_prompt_opt.py,sha256=TZsRK4XPMrUhGg0PoMyiE3wE-aG34UmlVflkCl_c0QI,4151
-bisheng_langchain/gpts/prompts/base_prompt.py,sha256=v2eO0c6RF8e6MtGdleHs5B4YTkikg6IZUuBvL2zvyOI,55
 bisheng_langchain/gpts/prompts/breif_description_prompt.py,sha256=w4A5et0jB-GkxEMQBp4i6GKX3RkVeu7NzWEjOZZAicM,5336
 bisheng_langchain/gpts/prompts/opening_dialog_prompt.py,sha256=VVF0JLHtetupVB0kabiFHWDHlQaa4nFLcbYXgIBA3nw,5965
 bisheng_langchain/gpts/prompts/select_tools_prompt.py,sha256=AyvVnrLEsQy7RHuGTPkcrMUxgA98Q0TzF-xweoc7GyY,1400
 bisheng_langchain/gpts/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/gpts/tools/api_tools/__init__.py,sha256=CkEjgIFM4GIv86V1B7SsFLaB6M86c54QuO8wIRizUZ8,1608
 bisheng_langchain/gpts/tools/api_tools/base.py,sha256=fWQSDIOVb4JZrtJ9ML9q2ycsAa-_61gXTD0MT19J1LM,3618
-bisheng_langchain/gpts/tools/api_tools/flow.py,sha256=rHCRpaafriQomMaOqSeKjPXwVUO_nAsFDNRIjOofbuI,2486
+bisheng_langchain/gpts/tools/api_tools/flow.py,sha256=ot2YAYgQGWgUpb2nCECAmpqHY6m0SgzwkupF9kDT3lU,2461
 bisheng_langchain/gpts/tools/api_tools/macro_data.py,sha256=FyG-qtl2ECS1CDKt6olN0eDTDM91d-UvDkMDBiVLgYQ,27429
+bisheng_langchain/gpts/tools/api_tools/openapi.py,sha256=3MlIpzR_NhZogaA-zbH6fnT_KUMm10NnbtDYcxKedS8,3907
 bisheng_langchain/gpts/tools/api_tools/sina.py,sha256=GGA4ZYvNEpqBZ_l8MUYqgkI8xZe9XcGa9-KlHZVqr6I,9542
 bisheng_langchain/gpts/tools/api_tools/tianyancha.py,sha256=abDAz-yAH1-2rKiSmZ6TgnrNUnpgAZpDY8oDiWfWapc,6684
 bisheng_langchain/gpts/tools/bing_search/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/gpts/tools/bing_search/tool.py,sha256=v_VlqcMplITA5go5qWA4qZ5p43E1-1s0bzmyY7H0hqY,1710
 bisheng_langchain/gpts/tools/calculator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/gpts/tools/calculator/tool.py,sha256=iwGPE7jvxZg_jUL2Aq9HHwnRJrF9-ongwrsBX6uk1U0,705
 bisheng_langchain/gpts/tools/code_interpreter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -95,20 +97,53 @@
 bisheng_langchain/gpts/tools/dalle_image_generator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/gpts/tools/dalle_image_generator/tool.py,sha256=mhxdNNhBESjbOy30Rnp6hQhnrV4evQpv-B1fFXcU-68,7528
 bisheng_langchain/gpts/tools/get_current_time/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/gpts/tools/get_current_time/tool.py,sha256=3uvk7Yu07qhZy1sBrFMhGEwyxEGMB8vubizs9x-6DG8,801
 bisheng_langchain/input_output/__init__.py,sha256=sW_GB7MlrHYsqY1Meb_LeimQqNsMz1gH-00Tqb2BUyM,153
 bisheng_langchain/input_output/input.py,sha256=I5YDmgbvvj1o2lO9wi8LE37wM0wP5jkhUREU32YrZMQ,1094
 bisheng_langchain/input_output/output.py,sha256=6U-az6-Cwz665C2YmcH3SYctWVjPFjmW8s70CA_qphk,11585
+bisheng_langchain/rag/__init__.py,sha256=gGa3hx0HjA_11FxbnR3P0C0y_OwcZM-sYTHdAajmylk,102
+bisheng_langchain/rag/bisheng_rag_pipeline.py,sha256=neoBK3TtuQ07_WeuJCzYlvtsDQNepUa_68NT8VCgytw,13749
+bisheng_langchain/rag/bisheng_rag_pipeline_v2.py,sha256=FWmhOSLAKWqqhdj55Y6WoFJ5GYwK8fJdN3o-mqPmabI,15898
+bisheng_langchain/rag/bisheng_rag_pipeline_v2_cohere_raw_prompting.py,sha256=Gql3IXaSTtW8WaC7wLLid0TURXoF0hRqAgl3GAYBBCo,16816
+bisheng_langchain/rag/bisheng_rag_tool.py,sha256=X7mhqYHapLlqfpu90BaW-C3aDeW_PENIci9lNyQv-tI,11971
+bisheng_langchain/rag/extract_info.py,sha256=emrdvzU9EfdTQU_IBF4RkwaTXmYLk1MOJgdfYhw6VtA,1753
+bisheng_langchain/rag/run_qa_gen_web.py,sha256=-fIvHNnD3lD0iNU5m0Me1GDwRjlcsB8tE5RnPtFRG2s,1840
+bisheng_langchain/rag/run_rag_evaluate_web.py,sha256=a9vMhq-ZhEiHHr43uKUzKtjdk280uAP_UHQW_eOaQMw,2224
+bisheng_langchain/rag/utils.py,sha256=ZR3BwjjLX4XT49aRDv-pf8Z4Mqcbmt2_qbDSwXfDfso,6361
+bisheng_langchain/rag/config/baseline.yaml,sha256=cFkfVpuNtmexYkQxXbqbcqQ4eDhx81kmIXf8T_rc_Oo,2266
+bisheng_langchain/rag/config/baseline_caibao.yaml,sha256=uU2HSlPXB8uLq9Fh03wENs06STdMA9CS6ry3X-Wkn-E,2174
+bisheng_langchain/rag/config/baseline_caibao_knowledge_v2.yaml,sha256=KrkMmHu-myQ8u4FlydXLwsppD4ucQGAYYtGGA0HCJzE,2812
+bisheng_langchain/rag/config/baseline_caibao_v2.yaml,sha256=WY9wek70eeBhhyiNmkfyrffxhTfBntqPyLMRmoqM_vE,2846
+bisheng_langchain/rag/config/baseline_demo_v2.yaml,sha256=hCa7bZMCcOWpu6bsAFX4DU1b7MV4eN2phyzvZzFZKkU,2382
+bisheng_langchain/rag/config/baseline_s2b_mix.yaml,sha256=rkPfzU2-mvjRrZ0zMHaQsncPhq8DrdvVFsw4Sg_jeKc,2398
+bisheng_langchain/rag/config/baseline_v2.yaml,sha256=yUMlK9CbeIqIrb4iJj14BaqH7JJ15QdUIf1EHd7T_R8,2350
+bisheng_langchain/rag/init_retrievers/__init__.py,sha256=qpLLAuqZPtumTlJj17Ie5AbDDmiUiDxYefg_pumqu-c,218
+bisheng_langchain/rag/init_retrievers/baseline_vector_retriever.py,sha256=oRKZZpxlLQAtsubIcAXeXpf1a9h6Pt6uOtNTLeD2jps,2362
+bisheng_langchain/rag/init_retrievers/keyword_retriever.py,sha256=NRT0fBx6HFR7j9IbRl_NBuqF7hnL-9v5GCqHpgnrfPQ,2523
+bisheng_langchain/rag/init_retrievers/mix_retriever.py,sha256=Whxq4kjNPLsxnHcVo60usdFFwLTCD-1jO38q08LXkVQ,4653
+bisheng_langchain/rag/init_retrievers/smaller_chunks_retriever.py,sha256=RQ7QLEOOhBrkw-EimXVJqIGa96D-KkNDik2h9hzg9fU,3805
+bisheng_langchain/rag/prompts/__init__.py,sha256=IUCq9gzqGQN_6IDk0D_F5t3mOUI_KbmSzYnnXoX4VKE,223
+bisheng_langchain/rag/prompts/extract_key_prompt.py,sha256=THdcwolRzaKkddgEhabUDytn-caHs9UwECPkPxijWAs,1456
+bisheng_langchain/rag/prompts/prompt.py,sha256=HPQ4mnMXDL9YsgBqK4S1M2sE6icq2uDL17KKgvEkovI,1925
+bisheng_langchain/rag/prompts/prompt_cohere.py,sha256=FhW-RCIVnIfKtEqV_-7aQav1riIJmA0jV2hGxCSoysk,8151
+bisheng_langchain/rag/qa_corpus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bisheng_langchain/rag/qa_corpus/qa_generator.py,sha256=ZdipOLBd16XfKXygq1JeUx4iv3tfUsprk1HNuC5hcIk,6092
+bisheng_langchain/rag/rerank/__init__.py,sha256=lcMRa_o5HGNnN9Hn6zHCimYq02OuD9pRAg6eFPZNgR8,72
+bisheng_langchain/rag/rerank/rerank.py,sha256=RoEwFFb4t4l0aZQmE2-HHHfWIzNLKe9NuFDIoYoWz5g,1836
+bisheng_langchain/rag/rerank/rerank_benchmark.py,sha256=OU9bh7dQ0-faw4hpz6BPEtmbQEhISTekvRiWpksOfCc,4490
+bisheng_langchain/rag/scoring/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bisheng_langchain/rag/scoring/llama_index_score.py,sha256=Xh8YFT14JGxE3OL2x4JSRa8nGlOK5DlWlsrzbmA2gu8,3001
+bisheng_langchain/rag/scoring/ragas_score.py,sha256=ClVoRg1O7s5OMcsB2E5UbVHj_ErQ3WKr9hao8BcK6NA,7110
 bisheng_langchain/retrievers/__init__.py,sha256=XqBeNyPyNCJf-SzNBiFlkxtjrtHUFTTi5pe2yPyOKrA,210
-bisheng_langchain/retrievers/ensemble.py,sha256=nLsTKpJmaigrECCWzrvDUwhE-qs9Mg7gPRXfPo5qFMI,5942
+bisheng_langchain/retrievers/ensemble.py,sha256=umjBaZYBEdhJ2F7GlzQgXVLYjSfpybTptiJJbUgryZE,5975
 bisheng_langchain/retrievers/mix_es_vector.py,sha256=dSrrsuMPSgGiu181EOzACyIKiDXR0qNBQz_914USD3E,4465
 bisheng_langchain/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/utils/requests.py,sha256=vWGKyNTxApVeaVdKxqACfIT1Q8wMy-jC3kUv2Ce9Mzc,8688
 bisheng_langchain/vectorstores/__init__.py,sha256=zCZgDe7LyQ0iDkfcm5UJ5NxwKQSRHnqrsjx700Fy11M,213
-bisheng_langchain/vectorstores/elastic_keywords_search.py,sha256=JV_GM40cYx0PtPPvH2JYxtsMV0psSW2CDKagpR4M_0o,13286
+bisheng_langchain/vectorstores/elastic_keywords_search.py,sha256=Pm1rS50GJ0HWbjBsFDgs28SVuVbjGSRPOor6yJlnE7w,13347
 bisheng_langchain/vectorstores/milvus.py,sha256=lrnezKnYXhyH5M1g3a-Mcwpj9mwzAj44TKmzyUXlQYY,36297
 bisheng_langchain/vectorstores/retriever.py,sha256=hj4nAAl352EV_ANnU2OHJn7omCH3nBK82ydo14KqMH4,4353
-bisheng_langchain-0.3.0rc1.dist-info/METADATA,sha256=vHWUJcrt2hO4QpW5o0Al8bn23d6c3zpm9yf_2NWGEmE,2414
-bisheng_langchain-0.3.0rc1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-bisheng_langchain-0.3.0rc1.dist-info/top_level.txt,sha256=Z6pPNyCo4ihyr9iqGQbH8sJiC4dAUwA_mAyGRQB5_Fs,18
-bisheng_langchain-0.3.0rc1.dist-info/RECORD,,
+bisheng_langchain-0.3.1.dist-info/METADATA,sha256=uorWxDbAnQkGAmbh0c-ZmAnTf5MgzyhcY8hLKNDIp-Q,2411
+bisheng_langchain-0.3.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+bisheng_langchain-0.3.1.dist-info/top_level.txt,sha256=Z6pPNyCo4ihyr9iqGQbH8sJiC4dAUwA_mAyGRQB5_Fs,18
+bisheng_langchain-0.3.1.dist-info/RECORD,,
```

