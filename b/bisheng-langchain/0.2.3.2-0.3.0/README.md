# Comparing `tmp/bisheng_langchain-0.2.3.2-py3-none-any.whl.zip` & `tmp/bisheng_langchain-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,83 +1,116 @@
-Zip file size: 127834 bytes, number of entries: 81
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 18:33 bisheng_langchain/__init__.py
--rw-r--r--  2.0 unx     7909 b- defN 24-Mar-21 18:33 bisheng_langchain/text_splitter.py
--rw-r--r--  2.0 unx      226 b- defN 24-Mar-21 18:33 bisheng_langchain/agents/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 18:33 bisheng_langchain/agents/chatglm_functions_agent/__init__.py
--rw-r--r--  2.0 unx    13674 b- defN 24-Mar-21 18:33 bisheng_langchain/agents/chatglm_functions_agent/base.py
--rw-r--r--  2.0 unx     3497 b- defN 24-Mar-21 18:33 bisheng_langchain/agents/chatglm_functions_agent/output_parser.py
--rw-r--r--  2.0 unx      992 b- defN 24-Mar-21 18:33 bisheng_langchain/agents/chatglm_functions_agent/prompt.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 18:33 bisheng_langchain/agents/llm_functions_agent/__init__.py
--rw-r--r--  2.0 unx    12308 b- defN 24-Mar-21 18:33 bisheng_langchain/agents/llm_functions_agent/base.py
--rw-r--r--  2.0 unx      430 b- defN 24-Mar-21 18:33 bisheng_langchain/autogen_role/__init__.py
--rw-r--r--  2.0 unx     4736 b- defN 24-Mar-21 18:33 bisheng_langchain/autogen_role/assistant.py
--rw-r--r--  2.0 unx     2499 b- defN 24-Mar-21 18:33 bisheng_langchain/autogen_role/custom.py
--rw-r--r--  2.0 unx     2314 b- defN 24-Mar-21 18:33 bisheng_langchain/autogen_role/groupchat_manager.py
--rw-r--r--  2.0 unx     5885 b- defN 24-Mar-21 18:33 bisheng_langchain/autogen_role/user.py
--rw-r--r--  2.0 unx      679 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/__init__.py
--rw-r--r--  2.0 unx     1903 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/loader_output.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/autogen/__init__.py
--rw-r--r--  2.0 unx     3270 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/autogen/auto_gen.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/combine_documents/__init__.py
--rw-r--r--  2.0 unx     2369 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/combine_documents/stuff.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/conversational_retrieval/__init__.py
--rw-r--r--  2.0 unx     5313 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/conversational_retrieval/base.py
--rw-r--r--  2.0 unx     8795 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/question_answering/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/retrieval/__init__.py
--rw-r--r--  2.0 unx     3050 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/retrieval/retrieval_chain.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/router/__init__.py
--rw-r--r--  2.0 unx      375 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/router/multi_rule.py
--rw-r--r--  2.0 unx     1835 b- defN 24-Mar-21 18:33 bisheng_langchain/chains/router/rule_router.py
--rw-r--r--  2.0 unx      635 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/__init__.py
--rw-r--r--  2.0 unx    22774 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/host_llm.py
--rw-r--r--  2.0 unx    13901 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/minimax.py
--rw-r--r--  2.0 unx    17082 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/proxy_llm.py
--rw-r--r--  2.0 unx    19172 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/qwen.py
--rw-r--r--  2.0 unx    17056 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/sensetime.py
--rw-r--r--  2.0 unx    13671 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/wenxin.py
--rw-r--r--  2.0 unx    14037 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/xunfeiai.py
--rw-r--r--  2.0 unx    15342 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/zhipuai.py
--rw-r--r--  2.0 unx      443 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/interface/__init__.py
--rw-r--r--  2.0 unx     4423 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/interface/minimax.py
--rw-r--r--  2.0 unx     2081 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/interface/openai.py
--rw-r--r--  2.0 unx     1141 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/interface/types.py
--rw-r--r--  2.0 unx       65 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/interface/utils.py
--rw-r--r--  2.0 unx     4246 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/interface/wenxin.py
--rw-r--r--  2.0 unx     7514 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/interface/xunfei.py
--rw-r--r--  2.0 unx     2636 b- defN 24-Mar-21 18:33 bisheng_langchain/chat_models/interface/zhipuai.py
--rw-r--r--  2.0 unx      366 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/__init__.py
--rw-r--r--  2.0 unx     6656 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/custom_kv.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/elem_html.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/elem_image.py
--rw-r--r--  2.0 unx    22243 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/elem_pdf.py
--rw-r--r--  2.0 unx     5169 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/elem_unstrcutured_loader.py
--rw-r--r--  2.0 unx     4063 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/universal_kv.py
--rw-r--r--  2.0 unx      171 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/parsers/__init__.py
--rw-r--r--  2.0 unx     1760 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/parsers/ellm_client.py
--rw-r--r--  2.0 unx      938 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/parsers/image.py
--rw-r--r--  2.0 unx     1612 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/parsers/ocr_client.py
--rw-r--r--  2.0 unx     8685 b- defN 24-Mar-21 18:33 bisheng_langchain/document_loaders/parsers/test_image.py
--rw-r--r--  2.0 unx      534 b- defN 24-Mar-21 18:33 bisheng_langchain/embeddings/__init__.py
--rw-r--r--  2.0 unx     6321 b- defN 24-Mar-21 18:33 bisheng_langchain/embeddings/host_embedding.py
--rw-r--r--  2.0 unx     3192 b- defN 24-Mar-21 18:33 bisheng_langchain/embeddings/huggingfacegte.py
--rw-r--r--  2.0 unx     3415 b- defN 24-Mar-21 18:33 bisheng_langchain/embeddings/huggingfacemultilingual.py
--rw-r--r--  2.0 unx     4737 b- defN 24-Mar-21 18:33 bisheng_langchain/embeddings/wenxin.py
--rw-r--r--  2.0 unx       98 b- defN 24-Mar-21 18:33 bisheng_langchain/embeddings/interface/__init__.py
--rw-r--r--  2.0 unx      461 b- defN 24-Mar-21 18:33 bisheng_langchain/embeddings/interface/types.py
--rw-r--r--  2.0 unx     3104 b- defN 24-Mar-21 18:33 bisheng_langchain/embeddings/interface/wenxin.py
--rw-r--r--  2.0 unx      153 b- defN 24-Mar-21 18:33 bisheng_langchain/input_output/__init__.py
--rw-r--r--  2.0 unx     1094 b- defN 24-Mar-21 18:33 bisheng_langchain/input_output/input.py
--rw-r--r--  2.0 unx    11585 b- defN 24-Mar-21 18:33 bisheng_langchain/input_output/output.py
--rw-r--r--  2.0 unx      210 b- defN 24-Mar-21 18:33 bisheng_langchain/retrievers/__init__.py
--rw-r--r--  2.0 unx     5942 b- defN 24-Mar-21 18:33 bisheng_langchain/retrievers/ensemble.py
--rw-r--r--  2.0 unx     4465 b- defN 24-Mar-21 18:33 bisheng_langchain/retrievers/mix_es_vector.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 18:33 bisheng_langchain/utils/__init__.py
--rw-r--r--  2.0 unx     8517 b- defN 24-Mar-21 18:33 bisheng_langchain/utils/requests.py
--rw-r--r--  2.0 unx      213 b- defN 24-Mar-21 18:33 bisheng_langchain/vectorstores/__init__.py
--rw-r--r--  2.0 unx    12929 b- defN 24-Mar-21 18:33 bisheng_langchain/vectorstores/elastic_keywords_search.py
--rw-r--r--  2.0 unx    35856 b- defN 24-Mar-21 18:33 bisheng_langchain/vectorstores/milvus.py
--rw-r--r--  2.0 unx     4353 b- defN 24-Mar-21 18:33 bisheng_langchain/vectorstores/retriever.py
--rw-r--r--  2.0 unx     2299 b- defN 24-Mar-21 18:33 bisheng_langchain-0.2.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-21 18:33 bisheng_langchain-0.2.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Mar-21 18:33 bisheng_langchain-0.2.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8278 b- defN 24-Mar-21 18:33 bisheng_langchain-0.2.3.2.dist-info/RECORD
-81 files, 407807 bytes uncompressed, 114142 bytes compressed:  72.0%
+Zip file size: 169423 bytes, number of entries: 114
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/__init__.py
+-rw-r--r--  2.0 unx     7909 b- defN 24-Apr-10 15:14 bisheng_langchain/text_splitter.py
+-rw-r--r--  2.0 unx      226 b- defN 24-Apr-10 15:14 bisheng_langchain/agents/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/agents/chatglm_functions_agent/__init__.py
+-rw-r--r--  2.0 unx    13674 b- defN 24-Apr-10 15:14 bisheng_langchain/agents/chatglm_functions_agent/base.py
+-rw-r--r--  2.0 unx     3497 b- defN 24-Apr-10 15:14 bisheng_langchain/agents/chatglm_functions_agent/output_parser.py
+-rw-r--r--  2.0 unx      992 b- defN 24-Apr-10 15:14 bisheng_langchain/agents/chatglm_functions_agent/prompt.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/agents/llm_functions_agent/__init__.py
+-rw-r--r--  2.0 unx    12296 b- defN 24-Apr-10 15:14 bisheng_langchain/agents/llm_functions_agent/base.py
+-rw-r--r--  2.0 unx      430 b- defN 24-Apr-10 15:14 bisheng_langchain/autogen_role/__init__.py
+-rw-r--r--  2.0 unx     4736 b- defN 24-Apr-10 15:14 bisheng_langchain/autogen_role/assistant.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-Apr-10 15:14 bisheng_langchain/autogen_role/custom.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-Apr-10 15:14 bisheng_langchain/autogen_role/groupchat_manager.py
+-rw-r--r--  2.0 unx     5885 b- defN 24-Apr-10 15:14 bisheng_langchain/autogen_role/user.py
+-rw-r--r--  2.0 unx      759 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/__init__.py
+-rw-r--r--  2.0 unx     1903 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/loader_output.py
+-rw-r--r--  2.0 unx     2805 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/transform.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/autogen/__init__.py
+-rw-r--r--  2.0 unx     3270 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/autogen/auto_gen.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/combine_documents/__init__.py
+-rw-r--r--  2.0 unx     2369 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/combine_documents/stuff.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/conversational_retrieval/__init__.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/conversational_retrieval/base.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/question_answering/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/retrieval/__init__.py
+-rw-r--r--  2.0 unx     3050 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/retrieval/retrieval_chain.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/router/__init__.py
+-rw-r--r--  2.0 unx      375 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/router/multi_rule.py
+-rw-r--r--  2.0 unx     1835 b- defN 24-Apr-10 15:14 bisheng_langchain/chains/router/rule_router.py
+-rw-r--r--  2.0 unx      635 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/__init__.py
+-rw-r--r--  2.0 unx    23152 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/host_llm.py
+-rw-r--r--  2.0 unx    13901 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/minimax.py
+-rw-r--r--  2.0 unx    17082 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/proxy_llm.py
+-rw-r--r--  2.0 unx    19971 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/qwen.py
+-rw-r--r--  2.0 unx    17056 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/sensetime.py
+-rw-r--r--  2.0 unx    13671 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/wenxin.py
+-rw-r--r--  2.0 unx    14037 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/xunfeiai.py
+-rw-r--r--  2.0 unx    15342 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/zhipuai.py
+-rw-r--r--  2.0 unx      443 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/interface/__init__.py
+-rw-r--r--  2.0 unx     4423 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/interface/minimax.py
+-rw-r--r--  2.0 unx     2081 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/interface/openai.py
+-rw-r--r--  2.0 unx     1141 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/interface/types.py
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/interface/utils.py
+-rw-r--r--  2.0 unx     4246 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/interface/wenxin.py
+-rw-r--r--  2.0 unx     7514 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/interface/xunfei.py
+-rw-r--r--  2.0 unx     2636 b- defN 24-Apr-10 15:14 bisheng_langchain/chat_models/interface/zhipuai.py
+-rw-r--r--  2.0 unx      366 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/__init__.py
+-rw-r--r--  2.0 unx     6656 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/custom_kv.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/elem_html.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/elem_image.py
+-rw-r--r--  2.0 unx    22243 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/elem_pdf.py
+-rw-r--r--  2.0 unx     5169 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/elem_unstrcutured_loader.py
+-rw-r--r--  2.0 unx     4063 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/universal_kv.py
+-rw-r--r--  2.0 unx      171 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/parsers/__init__.py
+-rw-r--r--  2.0 unx     1760 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/parsers/ellm_client.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/parsers/image.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/parsers/ocr_client.py
+-rw-r--r--  2.0 unx     8685 b- defN 24-Apr-10 15:14 bisheng_langchain/document_loaders/parsers/test_image.py
+-rw-r--r--  2.0 unx      534 b- defN 24-Apr-10 15:14 bisheng_langchain/embeddings/__init__.py
+-rw-r--r--  2.0 unx     6295 b- defN 24-Apr-10 15:14 bisheng_langchain/embeddings/host_embedding.py
+-rw-r--r--  2.0 unx     3192 b- defN 24-Apr-10 15:14 bisheng_langchain/embeddings/huggingfacegte.py
+-rw-r--r--  2.0 unx     3415 b- defN 24-Apr-10 15:14 bisheng_langchain/embeddings/huggingfacemultilingual.py
+-rw-r--r--  2.0 unx     4737 b- defN 24-Apr-10 15:14 bisheng_langchain/embeddings/wenxin.py
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-10 15:14 bisheng_langchain/embeddings/interface/__init__.py
+-rw-r--r--  2.0 unx      461 b- defN 24-Apr-10 15:14 bisheng_langchain/embeddings/interface/types.py
+-rw-r--r--  2.0 unx     3104 b- defN 24-Apr-10 15:14 bisheng_langchain/embeddings/interface/wenxin.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/__init__.py
+-rw-r--r--  2.0 unx     5083 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/assistant.py
+-rw-r--r--  2.0 unx     3786 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/auto_optimization.py
+-rw-r--r--  2.0 unx     1777 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/auto_tool_selected.py
+-rw-r--r--  2.0 unx     6345 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/load_tools.py
+-rw-r--r--  2.0 unx      213 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/message_types.py
+-rw-r--r--  2.0 unx     6671 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/utils.py
+-rw-r--r--  2.0 unx      261 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/agent_types/__init__.py
+-rw-r--r--  2.0 unx     8419 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/agent_types/llm_functions_agent.py
+-rw-r--r--  2.0 unx      568 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/prompts/__init__.py
+-rw-r--r--  2.0 unx     4151 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/prompts/assistant_prompt_opt.py
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/prompts/base_prompt.py
+-rw-r--r--  2.0 unx     5336 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/prompts/breif_description_prompt.py
+-rw-r--r--  2.0 unx     5962 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/prompts/opening_dialog_prompt.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/prompts/select_tools_prompt.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/__init__.py
+-rw-r--r--  2.0 unx     1593 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/api_tools/__init__.py
+-rw-r--r--  2.0 unx     3458 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/api_tools/base.py
+-rw-r--r--  2.0 unx     1814 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/api_tools/flow.py
+-rw-r--r--  2.0 unx    19270 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/api_tools/macro_data.py
+-rw-r--r--  2.0 unx     9277 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/api_tools/sina.py
+-rw-r--r--  2.0 unx     7461 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/api_tools/tianyancha.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/bing_search/__init__.py
+-rw-r--r--  2.0 unx     1710 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/bing_search/tool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/calculator/__init__.py
+-rw-r--r--  2.0 unx      705 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/calculator/tool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/code_interpreter/__init__.py
+-rw-r--r--  2.0 unx     8717 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/code_interpreter/tool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/dalle_image_generator/__init__.py
+-rw-r--r--  2.0 unx     7528 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/dalle_image_generator/tool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/get_current_time/__init__.py
+-rw-r--r--  2.0 unx      801 b- defN 24-Apr-10 15:14 bisheng_langchain/gpts/tools/get_current_time/tool.py
+-rw-r--r--  2.0 unx      153 b- defN 24-Apr-10 15:14 bisheng_langchain/input_output/__init__.py
+-rw-r--r--  2.0 unx     1094 b- defN 24-Apr-10 15:14 bisheng_langchain/input_output/input.py
+-rw-r--r--  2.0 unx    11585 b- defN 24-Apr-10 15:14 bisheng_langchain/input_output/output.py
+-rw-r--r--  2.0 unx      210 b- defN 24-Apr-10 15:14 bisheng_langchain/retrievers/__init__.py
+-rw-r--r--  2.0 unx     5942 b- defN 24-Apr-10 15:14 bisheng_langchain/retrievers/ensemble.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-Apr-10 15:14 bisheng_langchain/retrievers/mix_es_vector.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 15:14 bisheng_langchain/utils/__init__.py
+-rw-r--r--  2.0 unx     8688 b- defN 24-Apr-10 15:14 bisheng_langchain/utils/requests.py
+-rw-r--r--  2.0 unx      213 b- defN 24-Apr-10 15:14 bisheng_langchain/vectorstores/__init__.py
+-rw-r--r--  2.0 unx    12929 b- defN 24-Apr-10 15:14 bisheng_langchain/vectorstores/elastic_keywords_search.py
+-rw-r--r--  2.0 unx    35857 b- defN 24-Apr-10 15:14 bisheng_langchain/vectorstores/milvus.py
+-rw-r--r--  2.0 unx     4353 b- defN 24-Apr-10 15:14 bisheng_langchain/vectorstores/retriever.py
+-rw-r--r--  2.0 unx     2411 b- defN 24-Apr-10 15:15 bisheng_langchain-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 15:15 bisheng_langchain-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-10 15:15 bisheng_langchain-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    11703 b- defN 24-Apr-10 15:15 bisheng_langchain-0.3.0.dist-info/RECORD
+114 files, 527901 bytes uncompressed, 150081 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -42,14 +42,17 @@
 
 Filename: bisheng_langchain/chains/__init__.py
 Comment: 
 
 Filename: bisheng_langchain/chains/loader_output.py
 Comment: 
 
+Filename: bisheng_langchain/chains/transform.py
+Comment: 
+
 Filename: bisheng_langchain/chains/autogen/__init__.py
 Comment: 
 
 Filename: bisheng_langchain/chains/autogen/auto_gen.py
 Comment: 
 
 Filename: bisheng_langchain/chains/combine_documents/__init__.py
@@ -189,14 +192,110 @@
 
 Filename: bisheng_langchain/embeddings/interface/types.py
 Comment: 
 
 Filename: bisheng_langchain/embeddings/interface/wenxin.py
 Comment: 
 
+Filename: bisheng_langchain/gpts/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/assistant.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/auto_optimization.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/auto_tool_selected.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/load_tools.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/message_types.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/utils.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/agent_types/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/agent_types/llm_functions_agent.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/prompts/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/prompts/assistant_prompt_opt.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/prompts/base_prompt.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/prompts/breif_description_prompt.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/prompts/opening_dialog_prompt.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/prompts/select_tools_prompt.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/api_tools/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/api_tools/base.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/api_tools/flow.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/api_tools/macro_data.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/api_tools/sina.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/api_tools/tianyancha.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/bing_search/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/bing_search/tool.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/calculator/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/calculator/tool.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/code_interpreter/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/code_interpreter/tool.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/dalle_image_generator/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/dalle_image_generator/tool.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/get_current_time/__init__.py
+Comment: 
+
+Filename: bisheng_langchain/gpts/tools/get_current_time/tool.py
+Comment: 
+
 Filename: bisheng_langchain/input_output/__init__.py
 Comment: 
 
 Filename: bisheng_langchain/input_output/input.py
 Comment: 
 
 Filename: bisheng_langchain/input_output/output.py
@@ -225,20 +324,20 @@
 
 Filename: bisheng_langchain/vectorstores/milvus.py
 Comment: 
 
 Filename: bisheng_langchain/vectorstores/retriever.py
 Comment: 
 
-Filename: bisheng_langchain-0.2.3.2.dist-info/METADATA
+Filename: bisheng_langchain-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: bisheng_langchain-0.2.3.2.dist-info/WHEEL
+Filename: bisheng_langchain-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: bisheng_langchain-0.2.3.2.dist-info/top_level.txt
+Filename: bisheng_langchain-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bisheng_langchain-0.2.3.2.dist-info/RECORD
+Filename: bisheng_langchain-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bisheng_langchain/agents/llm_functions_agent/base.py

```diff
@@ -4,24 +4,24 @@
 from typing import Any, List, Optional, Sequence, Tuple, Union
 
 from bisheng_langchain.chat_models.host_llm import HostQwenChat
 from bisheng_langchain.chat_models.proxy_llm import ProxyChatLLM
 from langchain.agents import BaseSingleActionAgent
 from langchain.callbacks.base import BaseCallbackManager
 from langchain.callbacks.manager import Callbacks
-from langchain.chat_models.openai import ChatOpenAI
 from langchain.prompts.chat import (BaseMessagePromptTemplate, ChatPromptTemplate,
                                     HumanMessagePromptTemplate, MessagesPlaceholder)
 from langchain.schema import AgentAction, AgentFinish, BasePromptTemplate, OutputParserException
 from langchain.schema.language_model import BaseLanguageModel
 from langchain.schema.messages import AIMessage, BaseMessage, FunctionMessage, SystemMessage
 from langchain.tools import BaseTool
 from langchain.tools.convert_to_openai import format_tool_to_openai_function
 from langchain_core.agents import AgentActionMessageLog
 from langchain_core.pydantic_v1 import root_validator
+from langchain_openai import ChatOpenAI
 
 
 def _convert_agent_action_to_messages(agent_action: AgentAction,
                                       observation: str) -> List[BaseMessage]:
     """Convert an agent action to a message.
 
     This code is used to reconstruct the original AI message from the agent action.
```

## bisheng_langchain/chains/__init__.py

```diff
@@ -1,13 +1,14 @@
 from bisheng_langchain.chains.autogen.auto_gen import AutoGenChain
 from bisheng_langchain.chains.combine_documents.stuff import StuffDocumentsChain
 from bisheng_langchain.chains.conversational_retrieval.base import ConversationalRetrievalChain
 from bisheng_langchain.chains.retrieval.retrieval_chain import RetrievalChain
 from bisheng_langchain.chains.router.multi_rule import MultiRuleChain
 from bisheng_langchain.chains.router.rule_router import RuleBasedRouter
+from bisheng_langchain.chains.transform import TransformChain
 
 from .loader_output import LoaderOutputChain
 
 __all__ = [
     'StuffDocumentsChain', 'LoaderOutputChain', 'AutoGenChain', 'RuleBasedRouter',
-    'MultiRuleChain', 'RetrievalChain', 'ConversationalRetrievalChain'
+    'MultiRuleChain', 'RetrievalChain', 'ConversationalRetrievalChain', 'TransformChain'
 ]
```

## bisheng_langchain/chat_models/host_llm.py

```diff
@@ -196,14 +196,15 @@
             self.client.headers = self.headers
             messages = kwargs.get('messages')
             temperature = kwargs.get('temperature')
             top_p = kwargs.get('top_p')
             max_tokens = kwargs.get('max_tokens')
             do_sample = kwargs.get('do_sample')
             params = {
+                'stream': False,
                 'messages': messages,
                 'model': self.model_name,
                 'top_p': top_p,
                 'temperature': temperature,
                 'max_tokens': max_tokens,
                 'do_sample': do_sample,
                 'function_call': kwargs.get('function_call', None),
@@ -281,25 +282,35 @@
                         else:
                             yield txt.decode('utf-8').strip()
             except requests.exceptions.Timeout as exc:
                 raise ValueError(f'timeout in host llm infer, url=[{self.host_base_url}]') from exc
             except Exception as e:
                 raise ValueError(f'exception in host llm infer: [{e}]') from e
 
+        text_haf = ''
         async for response in _acompletion_with_retry(**kwargs):
             is_error = False
             if response:
                 if response.startswith('event:error'):
                     is_error = True
                 elif response.startswith('data:'):
                     text = response[len('data:'):].strip()
-                    if text.startswith('{'):
-                        yield (is_error, response[len('data:'):])
-                    else:
-                        logger.info('agenerate_no_json text=%s', text)
+                    if text == '[DONE]':
+                        break
+                    try:
+                        json.loads(text_haf + text)
+                        yield (is_error, text_haf + text)
+                        text_haf = ''
+                    except Exception:
+                        # 拆包了
+                        if text_haf.startswith('{'):
+                            text_haf = text
+                            continue
+                        logger.error(f'response_not_json response={response}')
+
                     if is_error:
                         break
                 elif response.startswith('{'):
                     yield (is_error, response)
                 else:
                     continue
 
@@ -517,14 +528,15 @@
     max_tokens: int = 4096
 
     @property
     def _llm_type(self) -> str:
         """Return type of chat model."""
         return 'qwen1.5_chat'
 
+
 class HostLlama2Chat(BaseHostChatLLM):
     # Llama-2-7b-chat-hf, Llama-2-13b-chat-hf, Llama-2-70b-chat-hf
     model_name: str = Field('Llama-2-7b-chat-hf', alias='model')
 
     temperature: float = 0.9
     top_p: float = 0.6
     max_tokens: int = 4096
@@ -545,28 +557,30 @@
     host_base_url: str
 
     @property
     def _llm_type(self) -> str:
         """Return type of chat model."""
         return 'custom_llm_chat'
 
+
 class HostYuanChat(BaseHostChatLLM):
     # use custom llm chat api, api should compatiable with openai definition
     model_name: str = Field('Yuan2-2B-Janus-hf', alias='model')
 
     temperature: float = 1
     top_p: float = 0.9
     max_tokens: int = 4096
     host_base_url: str
 
     @property
     def _llm_type(self) -> str:
         """Return type of chat model."""
         return 'yuan2'
-    
+
+
 class HostYiChat(BaseHostChatLLM):
     # use custom llm chat api, api should compatiable with openai definition
     model_name: str = Field('Yi-34B-Chat', alias='model')
 
     temperature: float = 0.6
     top_p: float = 0.8
     max_tokens: int = 4096
```

## bisheng_langchain/chat_models/qwen.py

```diff
@@ -9,15 +9,15 @@
 
 from bisheng_langchain.utils.requests import Requests
 # import requests
 from langchain.callbacks.manager import AsyncCallbackManagerForLLMRun, CallbackManagerForLLMRun
 from langchain.chat_models.base import BaseChatModel
 from langchain.schema import ChatGeneration, ChatResult
 from langchain.schema.messages import (AIMessage, BaseMessage, ChatMessage, FunctionMessage,
-                                       HumanMessage, SystemMessage)
+                                       HumanMessage, SystemMessage, ToolMessage)
 from langchain.utils import get_from_dict_or_env
 from langchain_core.pydantic_v1 import Field, root_validator
 from tenacity import (before_sleep_log, retry, retry_if_exception_type, stop_after_attempt,
                       wait_exponential)
 
 if TYPE_CHECKING:
     import tiktoken
@@ -56,40 +56,61 @@
         return HumanMessage(content=_dict['content'])
     elif role == 'assistant':
         content = _dict['content'] or ''  # OpenAI returns None for tool invocations
         if _dict.get('function_call'):
             additional_kwargs = {'function_call': dict(_dict['function_call'])}
         else:
             additional_kwargs = {}
+        if _dict.get("tool_calls"):
+            additional_kwargs = {'tool_calls': _dict['tool_calls']}
+        else:
+            additional_kwargs = {}
         return AIMessage(content=content, additional_kwargs=additional_kwargs)
     elif role == 'system':
         return SystemMessage(content=_dict['content'])
     elif role == 'function':
         return FunctionMessage(content=_dict['content'], name=_dict['name'])
+    elif role == "tool":
+        additional_kwargs = {}
+        if "name" in _dict:
+            additional_kwargs["name"] = _dict["name"]
+        return ToolMessage(
+            content=_dict.get("content", ""),
+            tool_call_id=_dict.get("tool_call_id"),
+            additional_kwargs=additional_kwargs,
+        )
     else:
         return ChatMessage(content=_dict['content'], role=role)
 
 
 def _convert_message_to_dict(message: BaseMessage) -> dict:
     if isinstance(message, ChatMessage):
         message_dict = {'role': message.role, 'content': message.content}
     elif isinstance(message, HumanMessage):
         message_dict = {'role': 'user', 'content': message.content}
     elif isinstance(message, AIMessage):
         message_dict = {'role': 'assistant', 'content': message.content}
         if 'function_call' in message.additional_kwargs:
             message_dict['function_call'] = message.additional_kwargs['function_call']
+        if "tool_calls" in message.additional_kwargs:
+            message_dict["tool_calls"] = message.additional_kwargs["tool_calls"]
     elif isinstance(message, SystemMessage):
         message_dict = {'role': 'system', 'content': message.content}
     elif isinstance(message, FunctionMessage):
         message_dict = {
             'role': 'function',
             'content': message.content,
             'name': message.name,
         }
+    elif isinstance(message, ToolMessage):
+        message_dict = {
+            "role": "tool",
+            "content": message.content,
+            "tool_call_id": message.tool_call_id,
+        }
     else:
         raise ValueError(f'Got unknown type {message}')
     if 'name' in message.additional_kwargs:
         message_dict['name'] = message.additional_kwargs['name']
     return message_dict
 
 
@@ -277,15 +298,15 @@
     ) -> ChatResult:
         message_dicts, params = self._create_message_dicts(messages, stop)
         params = {**params, **kwargs}
         if self.streaming:
             inner_completion = ''
             role = 'assistant'
             params['stream'] = True
-            function_call: Optional[dict] = None
+            tool_calls: Optional[list[dict]] = None
             async for is_error, stream_resp in self.acompletion_with_retry(messages=message_dicts,
                                                                            **params):
                 output = None
                 msg = json.loads(stream_resp)
                 if is_error:
                     logger.error(stream_resp)
                     raise ValueError(stream_resp)
@@ -293,26 +314,26 @@
                     output = msg['output']
                 choices = output.get('choices')
                 if choices:
                     for choice in choices:
                         role = choice['message'].get('role', role)
                         token = choice['message'].get('content', '')
                         inner_completion += token or ''
-                        _function_call = choice['message'].get('function_call')
+                        _tool_calls = choice['message'].get('tool_calls')
                         if run_manager:
                             await run_manager.on_llm_new_token(token)
-                        if _function_call:
-                            if function_call is None:
-                                function_call = _function_call
+                        if _tool_calls:
+                            if tool_calls is None:
+                                tool_calls = _tool_calls
                             else:
-                                function_call['arguments'] += _function_call['arguments']
+                                tool_calls[0]['arguments'] += _tool_calls[0]['arguments']
             message = _convert_dict_to_message({
                 'content': inner_completion,
                 'role': role,
-                'function_call': function_call,
+                'tool_calls': tool_calls,
             })
             return ChatResult(generations=[ChatGeneration(message=message)])
         else:
             response = [
                 response
                 async for _, response in self.acompletion_with_retry(messages=message_dicts,
                                                                      **params)
```

## bisheng_langchain/document_loaders/custom_kv.py

```diff
@@ -160,11 +160,11 @@
             except Exception as e:
                 logger.error(
                     f'task_result_error scene_id={self.elem_server_id} res={result} except={str(e)}'
                 )
                 raise Exception('custom_kv parse_error')
         else:
             logger.error(f'custom_kv=create_task resp={resp.text}')
-            raise Exception('custom_kv create task file')
+            raise Exception('custom_kv create task fail')
         content = json.dumps(document_result)
         doc = Document(page_content=content)
         return [doc]
```

## bisheng_langchain/embeddings/host_embedding.py

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import requests
 from langchain.embeddings.base import Embeddings
 from langchain.utils import get_from_dict_or_env
-from langchain_core.pydantic_v1 import BaseModel, Extra, Field, root_validator
+from langchain_core.pydantic_v1 import BaseModel, Field, root_validator
 from tenacity import (before_sleep_log, retry, retry_if_exception_type, stop_after_attempt,
                       wait_exponential)
 
 logger = logging.getLogger(__name__)
 
 
 def _create_retry_decorator(embeddings: HostEmbeddings) -> Callable[[Any], Any]:
@@ -60,19 +60,14 @@
     model_kwargs: Optional[Dict[str, Any]] = Field(default_factory=dict)
     """Holds any model parameters valid for `create` call not explicitly specified."""
 
     verbose: Optional[bool] = False
 
     url_ep: Optional[str] = None
 
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         values['host_base_url'] = get_from_dict_or_env(values, 'host_base_url', 'HostBaseUrl')
         model = values['model']
         try:
             url = values['host_base_url']
@@ -104,20 +99,22 @@
         max_text_to_split = 200
         outp = None
 
         start_index = 0
         len_text = len(texts)
         while start_index < len_text:
             inp_local = {
-                'texts':texts[start_index:min(start_index + max_text_to_split, len_text)],
-                'model':self.model,
-                'type':emb_type
-                }
+                'texts': texts[start_index:min(start_index + max_text_to_split, len_text)],
+                'model': self.model,
+                'type': emb_type
+            }
             try:
-                outp_single = self.client(url=self.url_ep, json=inp_local, timeout=self.request_timeout).json()
+                outp_single = self.client(url=self.url_ep,
+                                          json=inp_local,
+                                          timeout=self.request_timeout).json()
                 if outp is None:
                     outp = outp_single
                 else:
                     outp['embeddings'] += outp_single['embeddings']
             except requests.exceptions.Timeout:
                 raise Exception(f'timeout in host embedding infer, url=[{self.url_ep}]')
             except Exception as e:
@@ -158,14 +155,15 @@
     embedding_ctx_length: int = 512
 
 
 class JINAEmbedding(HostEmbeddings):
     model: str = 'jina'
     embedding_ctx_length: int = 512
 
+
 class CustomHostEmbedding(HostEmbeddings):
     model: str = Field('custom-embedding', alias='model')
     embedding_ctx_length: int = 512
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
```

## bisheng_langchain/utils/requests.py

```diff
@@ -134,24 +134,28 @@
 
     The main purpose of this wrapper is to always return a text output.
     """
 
     headers: Optional[Dict[str, str]] = None
     aiosession: Optional[aiohttp.ClientSession] = None
     auth: Optional[Any] = None
+    request_timeout: Union[float, Tuple[float, float]] = 120
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
         arbitrary_types_allowed = True
 
     @property
     def requests(self) -> Requests:
-        return Requests(headers=self.headers, aiosession=self.aiosession, auth=self.auth)
+        return Requests(headers=self.headers,
+                        aiosession=self.aiosession,
+                        auth=self.auth,
+                        request_timeout=self.request_timeout)
 
     def get(self, url: str, **kwargs: Any) -> str:
         """GET the URL and return the text."""
         return self.requests.get(url, **kwargs).text
 
     def post(self, url: str, json: Dict[str, Any], **kwargs: Any) -> str:
         """POST to the URL and return the text."""
```

## bisheng_langchain/vectorstores/milvus.py

```diff
@@ -136,15 +136,15 @@
                 'params': {
                     'nprobe': 10
                 }
             },
             'HNSW': {
                 'metric_type': 'L2',
                 'params': {
-                    'ef': 10
+                    'ef': 100
                 }
             },
             'RHNSW_FLAT': {
                 'metric_type': 'L2',
                 'params': {
                     'ef': 10
                 }
```

## Comparing `bisheng_langchain-0.2.3.2.dist-info/METADATA` & `bisheng_langchain-0.3.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisheng-langchain
-Version: 0.2.3.2
+Version: 0.3.0
 Summary: bisheng langchain modules
 Home-page: https://github.com/dataelement/bisheng
 Author: DataElem
 Author-email: contact@dataelem.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,26 +12,29 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: langchain
+Requires-Dist: langchain ==0.1.12
 Requires-Dist: zhipuai
 Requires-Dist: websocket-client
 Requires-Dist: elasticsearch
 Requires-Dist: opencv-python ==4.5.5.64
 Requires-Dist: Pillow ==9.5.0
 Requires-Dist: bisheng-pyautogen
 Requires-Dist: jieba ==0.42.1
 Requires-Dist: pydantic ==1.10.13
 Requires-Dist: pymupdf ==1.23.8
 Requires-Dist: shapely ==2.0.2
 Requires-Dist: filetype ==1.2.0
+Requires-Dist: langgraph ==0.0.30
+Requires-Dist: openai ==1.14.3
+Requires-Dist: langchain-openai ==0.1.0
 
 ## What is bisheng-langchain?
 
 bisheng-langchain is an open-source langchain extending library built to power building LLM application.
 bisheng-langchain provides more components to support Chinese LLMs and and Chinese based token environments for prompt engineering and ICL template.
```

## Comparing `bisheng_langchain-0.2.3.2.dist-info/RECORD` & `bisheng_langchain-0.3.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -2,80 +2,113 @@
 bisheng_langchain/text_splitter.py,sha256=OAD57cAxPfZoVeBTzicLycel4RehxMULi6Ebi2Wc0Rg,7909
 bisheng_langchain/agents/__init__.py,sha256=ctsKj77fS8qlkhz_9sS_AhCjFvFNxEpJ9KBYVrApLRg,226
 bisheng_langchain/agents/chatglm_functions_agent/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/agents/chatglm_functions_agent/base.py,sha256=tyytq0XIFXpfxDP0s5QKeprKOunMqi1fHMfQ0-kOmDE,13674
 bisheng_langchain/agents/chatglm_functions_agent/output_parser.py,sha256=M7vDzQFqFUMmL250FHeNKXMwatkCdD0x1D0hyqGYRAA,3497
 bisheng_langchain/agents/chatglm_functions_agent/prompt.py,sha256=OiBTRUOhvhSyO2jO2ByUUiaCrkK_tIUH9pMWWKs-aF4,992
 bisheng_langchain/agents/llm_functions_agent/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bisheng_langchain/agents/llm_functions_agent/base.py,sha256=4mzDOGheLGcP55xrGcYkLiH4kIII2IJjtYLAJAu41es,12308
+bisheng_langchain/agents/llm_functions_agent/base.py,sha256=DbykNAk3vU2sfTPTSM2KotHygXgzAJSUmo4tA0h9ezc,12296
 bisheng_langchain/autogen_role/__init__.py,sha256=MnTGbAOK770JM9l95Qcxu93s2gNAmhlil7K9HdFG81o,430
 bisheng_langchain/autogen_role/assistant.py,sha256=VGCoxJaRxRG6ZIJa2TsxcLZbMbF4KC8PRB76DOuznNU,4736
 bisheng_langchain/autogen_role/custom.py,sha256=8xxtAzNF_N1fysyChynVD19t659Qvtcyj_LNiOrE7ew,2499
 bisheng_langchain/autogen_role/groupchat_manager.py,sha256=O9XIove5yzyF_g3K5DnF-Fasdx0sUrRWMogYgEDYJAI,2314
 bisheng_langchain/autogen_role/user.py,sha256=lISbJN5yFsUXHnDCUwr5t6R8O8K3dOMspH4l4_kITnE,5885
-bisheng_langchain/chains/__init__.py,sha256=bZXTCzBbsaU9ks90SU5T2u2py006sArwKZJgCc8BNn8,679
+bisheng_langchain/chains/__init__.py,sha256=oxN2tUMt_kNxKd_FzCQ7x8xIwojtdCNNKo-DI7q0unM,759
 bisheng_langchain/chains/loader_output.py,sha256=02ZercAFaudStTZ4t7mcVkGRj5pD78HZ6NO8HbmbDH8,1903
+bisheng_langchain/chains/transform.py,sha256=G2fMqoMB62e03ES--aoVjEo06FzYWb87jCt3EOsiwwg,2805
 bisheng_langchain/chains/autogen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/chains/autogen/auto_gen.py,sha256=QIkfCO9-VN2wRkl3_TWVj-JkdL2dqMQNy93j3uB401s,3270
 bisheng_langchain/chains/combine_documents/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/chains/combine_documents/stuff.py,sha256=z_E_wfhJrAYWcNVRPomPm5fGRDI3hqoC52wcMzgzxVA,2369
 bisheng_langchain/chains/conversational_retrieval/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/chains/conversational_retrieval/base.py,sha256=XiqBqov6No-wTVCou6qyMT5p2JQgoQI7OLQOYH8XUos,5313
 bisheng_langchain/chains/question_answering/__init__.py,sha256=_gOZMc-SWprK6xc-Jj64jcr9nc-G4YkZbEYwfJNq_bY,8795
 bisheng_langchain/chains/retrieval/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/chains/retrieval/retrieval_chain.py,sha256=7VLJ-IPVjKfmAVgVET4cvKCO9DCMxwsGgVhW-wz5RZM,3050
 bisheng_langchain/chains/router/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/chains/router/multi_rule.py,sha256=BiFryj3-7rOxfttD-MyOkKWLCSGB9LVYd2rjOsIfQC8,375
 bisheng_langchain/chains/router/rule_router.py,sha256=R2YRUnwn7s_7DbsSn27uPn4cIV0D-5iXEORXir0tNGM,1835
 bisheng_langchain/chat_models/__init__.py,sha256=4-HTLE_SXO4hmNJu6yQxiQKBt2IFca_ezllVBLmvbEE,635
-bisheng_langchain/chat_models/host_llm.py,sha256=HY2HtMwiW-0TeyVlDZ85Vr0ldRhr3M7ICMdrWqll1OM,22774
+bisheng_langchain/chat_models/host_llm.py,sha256=sBu_Vg-r7z6IJUV8Etwll4JTG5OvET-IXH7PZw8Ijrc,23152
 bisheng_langchain/chat_models/minimax.py,sha256=JLs_f6vWD9beZYUtjD4FG28G8tZHrGUAWOwdLIuJomw,13901
 bisheng_langchain/chat_models/proxy_llm.py,sha256=wzVBZik9WC3-f7kyQ1eu3Ooibqpcocln08knf5lV1Nw,17082
-bisheng_langchain/chat_models/qwen.py,sha256=3_ncSsTJLaHH4FpWnfhU1ZJt0YlyhK4Utg_HSxepSiM,19172
+bisheng_langchain/chat_models/qwen.py,sha256=W73KxDRQBUZEzttEM4K7ZzPqbN-82O6YQmpX-HB_wZU,19971
 bisheng_langchain/chat_models/sensetime.py,sha256=fuQ5yYGO5F7o7iQ7us17MlL4TAWRRFCCpNN9bAF-ydc,17056
 bisheng_langchain/chat_models/wenxin.py,sha256=OBXmFWkUWZMu1lUz6hPAEawsbAcdgMWcm9WkJJLZyng,13671
 bisheng_langchain/chat_models/xunfeiai.py,sha256=Yz09-I8u6XhGVnT5mdel15Z3CCQZqApJkgnaxyiZNFk,14037
 bisheng_langchain/chat_models/zhipuai.py,sha256=MgN8pFInUB6q5agZSnAOipYxTIxAAGhh-Zq6NXs9Hxc,15342
 bisheng_langchain/chat_models/interface/__init__.py,sha256=KwcZMPSxFiXu6joXoZEgq6THxZeDXA8neZcOuLKBpUk,443
 bisheng_langchain/chat_models/interface/minimax.py,sha256=tF3S7ryFtYVXwh7jHHH9z1eY8nMCy0iLiFocsPSJ3pA,4423
 bisheng_langchain/chat_models/interface/openai.py,sha256=v4kxxglJoVMJ9kxaRDIJnWHBSvjl9vRhzQb5Fr-keg0,2081
 bisheng_langchain/chat_models/interface/types.py,sha256=FZwQJPDnStQ3oJx5ubyGJlvrhnGCgqhhnZDYSLmqFOs,1141
 bisheng_langchain/chat_models/interface/utils.py,sha256=qww_uYsWDqK7cLuv-KzZmmlg9SZAHOi4R_6I6S4XLIk,65
 bisheng_langchain/chat_models/interface/wenxin.py,sha256=z_K1Nj78dDYYgiVIzc5sGkOiGr8OAoRwaKwmpWXssH0,4246
 bisheng_langchain/chat_models/interface/xunfei.py,sha256=DPHAZM_uHg0A8GnebgkRbLENhBW7bBtRHzKC0gFKZgc,7514
 bisheng_langchain/chat_models/interface/zhipuai.py,sha256=67Ej6DRk-IlXUfEZPg-pjcYPyqZb32ClrBP-9k-3EEs,2636
 bisheng_langchain/document_loaders/__init__.py,sha256=LuQ-zMYxde2FeiEcvVtjQqnHozki5pF_pDDa88_fBdg,366
-bisheng_langchain/document_loaders/custom_kv.py,sha256=sUKeK0e8-cCmKyj1FsR7SzBNWjo5zRwHWVS5tKVxuPs,6656
+bisheng_langchain/document_loaders/custom_kv.py,sha256=xWUPhcr1hjbdya4zgEHG4Fl0sI4RNQ6D2vqFo0c24G8,6656
 bisheng_langchain/document_loaders/elem_html.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/document_loaders/elem_image.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bisheng_langchain/document_loaders/elem_pdf.py,sha256=K-TXILGNFLFjavhun_MFbUF4t2_WGA3Z-kbnr75lmW8,22243
 bisheng_langchain/document_loaders/elem_unstrcutured_loader.py,sha256=bJQObxHnk8FaF8RUBkqODzgeikrZ8wdl_TQPa2oEoQo,5169
 bisheng_langchain/document_loaders/universal_kv.py,sha256=dJF_GQGKBMUjB_kX9CSp7xZRhXgwVuGPbMIzJwPh-C0,4063
 bisheng_langchain/document_loaders/parsers/__init__.py,sha256=OOM_FJkwaU-zNS58fASw0TH8FNT6VXKb0VrvisgdrII,171
 bisheng_langchain/document_loaders/parsers/ellm_client.py,sha256=B4Dea8xXXnGvB9j2OXv53HILNUmnWeNJz9ssNM-2fLM,1760
 bisheng_langchain/document_loaders/parsers/image.py,sha256=7Vx4dD_WiSTojS4TMIJFxfE8nvze0kwNnwTd6f1cLds,938
 bisheng_langchain/document_loaders/parsers/ocr_client.py,sha256=rRh1coJYn24n7FaINBZH5yO6Edm9TRywY6UOXpcerVo,1612
 bisheng_langchain/document_loaders/parsers/test_image.py,sha256=EJHozq5oFfLBlLL5Lr6XFkrkvSttPpohprs9OjDzAKM,8685
 bisheng_langchain/embeddings/__init__.py,sha256=_zLLb9cH4Ct4UpKQhtXr7V2IQ7LUnlCKkKTroTE_Enk,534
-bisheng_langchain/embeddings/host_embedding.py,sha256=CK_hZgOd3VJrkyh4Zyb3SrpkxlRRfy7ffanWfhkjIcE,6321
+bisheng_langchain/embeddings/host_embedding.py,sha256=eWhV6JZCclSr6jZXWbjhHURiWaUB8sC8CbgGCEa-AKk,6295
 bisheng_langchain/embeddings/huggingfacegte.py,sha256=RPfSXu7oMv6vgIjLqrPZ1Qz3K0yEuYn7VO0u7m7PzK8,3192
 bisheng_langchain/embeddings/huggingfacemultilingual.py,sha256=g7-yKJ-qIPUZQaRnGz312S-f3aJCGcdHemAR3znE-uo,3415
 bisheng_langchain/embeddings/wenxin.py,sha256=6zx53tSUguvny4gGe5CTmfwV-QtGqKmcT-Jlgf2xVUs,4737
 bisheng_langchain/embeddings/interface/__init__.py,sha256=GNY3tibpRxpAdAfSvQmXBKo0xKSLke_9y4clofi_WOE,98
 bisheng_langchain/embeddings/interface/types.py,sha256=VdurbtsnjCPdlOjPFcK2Mg6r9bJYYHb3tepvkk-y3nM,461
 bisheng_langchain/embeddings/interface/wenxin.py,sha256=5d9gI4enmfkD80s0FHKiDt33O0mwM8Xc5WTubnMUy8c,3104
+bisheng_langchain/gpts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bisheng_langchain/gpts/assistant.py,sha256=KCYPU1Bs4GtWcLk9Ya2NuQyXE0Twn7-92eSBTIzpq7I,5083
+bisheng_langchain/gpts/auto_optimization.py,sha256=Vf3zzYEpVf916dYt4RV9E1uw4vTXjE7ZXogUIdxjHYU,3786
+bisheng_langchain/gpts/auto_tool_selected.py,sha256=25lFLadqQ36t63EKMEF3zJOG_jkoRB9IfP5eRkY1JZo,1777
+bisheng_langchain/gpts/load_tools.py,sha256=C7tlRLy4wAArr9qtkRl9dW6QXdspLLbcv0UvulW9A9U,6345
+bisheng_langchain/gpts/message_types.py,sha256=7EJOx62j9E1U67jxWgxE_I7a8IjAvvKANknXkD2gFm0,213
+bisheng_langchain/gpts/utils.py,sha256=t3YDxaJ0OYd6EKsek7PJFRYnsezwzEFK5oVU-PRbu5g,6671
+bisheng_langchain/gpts/agent_types/__init__.py,sha256=bg0zlTYGfNXoSBqcICHlzNpVQbejMYeyji_dzvP5qQ0,261
+bisheng_langchain/gpts/agent_types/llm_functions_agent.py,sha256=ynFHXuaqABeiKvhcetOFQPyQMlNtEAdtTccoIwiJbGQ,8419
+bisheng_langchain/gpts/prompts/__init__.py,sha256=IfuoxVpsSLKJtDx0aJbRgnSZYZr_kDPsL92CvefzF-s,568
+bisheng_langchain/gpts/prompts/assistant_prompt_opt.py,sha256=TZsRK4XPMrUhGg0PoMyiE3wE-aG34UmlVflkCl_c0QI,4151
+bisheng_langchain/gpts/prompts/base_prompt.py,sha256=v2eO0c6RF8e6MtGdleHs5B4YTkikg6IZUuBvL2zvyOI,55
+bisheng_langchain/gpts/prompts/breif_description_prompt.py,sha256=w4A5et0jB-GkxEMQBp4i6GKX3RkVeu7NzWEjOZZAicM,5336
+bisheng_langchain/gpts/prompts/opening_dialog_prompt.py,sha256=U6SDslWuXAB1ZamLZVujpEjAY8L244IZfD2qFVRTzPM,5962
+bisheng_langchain/gpts/prompts/select_tools_prompt.py,sha256=AyvVnrLEsQy7RHuGTPkcrMUxgA98Q0TzF-xweoc7GyY,1400
+bisheng_langchain/gpts/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bisheng_langchain/gpts/tools/api_tools/__init__.py,sha256=mrmTV5bT5R1mEx9hbMAWKzNAAC4EL6biNn53dx5lYsc,1593
+bisheng_langchain/gpts/tools/api_tools/base.py,sha256=TF5MW0e62YvcfABp_-U32ESMKvN9CXPFKqiCeaZ3xFk,3458
+bisheng_langchain/gpts/tools/api_tools/flow.py,sha256=u1_ASWlCcZarKR-293kACB_qQ1RzJuzPC3YZSl2JR-E,1814
+bisheng_langchain/gpts/tools/api_tools/macro_data.py,sha256=rlFNhjJ3HEHfWeW9Wqb27eeF1Q1Qmd2SA8VfgUK4ACs,19270
+bisheng_langchain/gpts/tools/api_tools/sina.py,sha256=DCDuG-gxyFO2LCPdT-oy358iyfTMyMTP0-6awXYEfpg,9277
+bisheng_langchain/gpts/tools/api_tools/tianyancha.py,sha256=sQbjPt8K0dLupFprWwc_z938DBB8nB7ydyIV5frWSJ0,7461
+bisheng_langchain/gpts/tools/bing_search/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bisheng_langchain/gpts/tools/bing_search/tool.py,sha256=v_VlqcMplITA5go5qWA4qZ5p43E1-1s0bzmyY7H0hqY,1710
+bisheng_langchain/gpts/tools/calculator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bisheng_langchain/gpts/tools/calculator/tool.py,sha256=iwGPE7jvxZg_jUL2Aq9HHwnRJrF9-ongwrsBX6uk1U0,705
+bisheng_langchain/gpts/tools/code_interpreter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bisheng_langchain/gpts/tools/code_interpreter/tool.py,sha256=PGipxd-qtW31GonRGfGow7nylI-osSnmBsvEJDlMUCE,8717
+bisheng_langchain/gpts/tools/dalle_image_generator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bisheng_langchain/gpts/tools/dalle_image_generator/tool.py,sha256=mhxdNNhBESjbOy30Rnp6hQhnrV4evQpv-B1fFXcU-68,7528
+bisheng_langchain/gpts/tools/get_current_time/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bisheng_langchain/gpts/tools/get_current_time/tool.py,sha256=3uvk7Yu07qhZy1sBrFMhGEwyxEGMB8vubizs9x-6DG8,801
 bisheng_langchain/input_output/__init__.py,sha256=sW_GB7MlrHYsqY1Meb_LeimQqNsMz1gH-00Tqb2BUyM,153
 bisheng_langchain/input_output/input.py,sha256=I5YDmgbvvj1o2lO9wi8LE37wM0wP5jkhUREU32YrZMQ,1094
 bisheng_langchain/input_output/output.py,sha256=6U-az6-Cwz665C2YmcH3SYctWVjPFjmW8s70CA_qphk,11585
 bisheng_langchain/retrievers/__init__.py,sha256=XqBeNyPyNCJf-SzNBiFlkxtjrtHUFTTi5pe2yPyOKrA,210
 bisheng_langchain/retrievers/ensemble.py,sha256=nLsTKpJmaigrECCWzrvDUwhE-qs9Mg7gPRXfPo5qFMI,5942
 bisheng_langchain/retrievers/mix_es_vector.py,sha256=dSrrsuMPSgGiu181EOzACyIKiDXR0qNBQz_914USD3E,4465
 bisheng_langchain/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bisheng_langchain/utils/requests.py,sha256=20ooDlMDMkXig--rSyRqbnAlbGLscBvvkHzFk2AmyGM,8517
+bisheng_langchain/utils/requests.py,sha256=vWGKyNTxApVeaVdKxqACfIT1Q8wMy-jC3kUv2Ce9Mzc,8688
 bisheng_langchain/vectorstores/__init__.py,sha256=zCZgDe7LyQ0iDkfcm5UJ5NxwKQSRHnqrsjx700Fy11M,213
 bisheng_langchain/vectorstores/elastic_keywords_search.py,sha256=ACUzgeTwzVOVrm0EqBXF_VhzwrWZJbKYQgqNSW5VhbQ,12929
-bisheng_langchain/vectorstores/milvus.py,sha256=-gXIQzzmoPggLS2KEGUtp6kHg9peoawBlSVuOwQndHQ,35856
+bisheng_langchain/vectorstores/milvus.py,sha256=hk1XqmWoz04lltubzRcZHEcXXFMkxMeK84hH0GZoo1c,35857
 bisheng_langchain/vectorstores/retriever.py,sha256=hj4nAAl352EV_ANnU2OHJn7omCH3nBK82ydo14KqMH4,4353
-bisheng_langchain-0.2.3.2.dist-info/METADATA,sha256=bBbyzXtoG8QPpc1m68dlwZBKBZffry7sCq_BY68h7fU,2299
-bisheng_langchain-0.2.3.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-bisheng_langchain-0.2.3.2.dist-info/top_level.txt,sha256=Z6pPNyCo4ihyr9iqGQbH8sJiC4dAUwA_mAyGRQB5_Fs,18
-bisheng_langchain-0.2.3.2.dist-info/RECORD,,
+bisheng_langchain-0.3.0.dist-info/METADATA,sha256=lMi-o-cJ2A6Knag8E11kUld2Tv_WLpD_f0pjXPqBQ7s,2411
+bisheng_langchain-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+bisheng_langchain-0.3.0.dist-info/top_level.txt,sha256=Z6pPNyCo4ihyr9iqGQbH8sJiC4dAUwA_mAyGRQB5_Fs,18
+bisheng_langchain-0.3.0.dist-info/RECORD,,
```

