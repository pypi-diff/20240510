# Comparing `tmp/semantic_kernel-0.9.7b1.tar.gz` & `tmp/semantic_kernel-0.9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.9.7b1.tar", max compression
+gzip compressed data, was "semantic_kernel-0.9.8b1.tar", max compression
```

## Comparing `semantic_kernel-0.9.7b1.tar` & `semantic_kernel-0.9.8b1.tar`

### file list

```diff
@@ -1,222 +1,217 @@
--rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-0.9.7b1/pip/README.md
--rw-r--r--   0        0        0     5404 2024-05-06 13:16:31.745032 semantic_kernel-0.9.7b1/pyproject.toml
--rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/__init__.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     3223 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0      437 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/__init__.py
--rw-r--r--   0        0        0     1795 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
--rw-r--r--   0        0        0     9646 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
--rw-r--r--   0        0        0     3821 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
--rw-r--r--   0        0        0     2191 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
--rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     1169 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
--rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
--rw-r--r--   0        0        0     6662 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2119 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/__init__.py
--rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
--rw-r--r--   0        0        0     8403 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
--rw-r--r--   0        0        0     3962 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
--rw-r--r--   0        0        0     1805 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
--rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/utils.py
--rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0      246 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/const.py
--rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
--rw-r--r--   0        0        0     3817 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
--rw-r--r--   0        0        0     4031 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
--rw-r--r--   0        0        0    16094 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     5364 2024-03-20 18:24:28.763758 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
--rw-r--r--   0        0        0     8276 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     4815 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     4731 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0    18726 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
--rw-r--r--   0        0        0     3719 2024-03-20 18:24:28.763758 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
--rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
--rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
--rw-r--r--   0        0        0     4797 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     6342 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
--rw-r--r--   0        0        0     3016 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
--rw-r--r--   0        0        0      820 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/tool_call_behavior.py
--rw-r--r--   0        0        0     6935 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/utils.py
--rw-r--r--   0        0        0     3908 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/prompt_execution_settings.py
--rw-r--r--   0        0        0     1720 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/__init__.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/__init__.py
--rw-r--r--   0        0        0     6718 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/astra_client.py
--rw-r--r--   0        0        0    11819 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
--rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/utils.py
--rw-r--r--   0        0        0      242 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0    15787 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      213 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
--rw-r--r--   0        0        0    10299 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
--rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
--rw-r--r--   0        0        0     1592 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
--rw-r--r--   0        0        0    13020 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
--rw-r--r--   0        0        0      159 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0    12786 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
--rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
--rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    14863 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    20518 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
--rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/README.md
--rw-r--r--   0        0        0      178 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/__init__.py
--rw-r--r--   0        0        0    15281 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
--rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/utils.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/usearch/__init__.py
--rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
--rw-r--r--   0        0        0      188 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/weaviate/__init__.py
--rw-r--r--   0        0        0    11001 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/__init__.py
--rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
--rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
--rw-r--r--   0        0        0     1011 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/openai_utils.py
--rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openapi_plugin/__init__.py
--rw-r--r--   0        0        0     1241 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
--rw-r--r--   0        0        0    13518 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
--rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     2648 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-0.9.7b1/semantic_kernel/connectors/telemetry.py
--rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/connectors/utils/__init__.py
--rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/connectors/utils/document_loader.py
--rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/__init__.py
--rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/author_role.py
--rw-r--r--   0        0        0    13781 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/chat_history.py
--rw-r--r--   0        0        0    12276 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/chat_message_content.py
--rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/const.py
--rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/contents/finish_reason.py
--rw-r--r--   0        0        0     3729 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/function_call_content.py
--rw-r--r--   0        0        0     3913 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/function_result_content.py
--rw-r--r--   0        0        0      772 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/kernel_content.py
--rw-r--r--   0        0        0    11084 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/streaming_chat_message_content.py
--rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/streaming_content_mixin.py
--rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/streaming_text_content.py
--rw-r--r--   0        0        0     1957 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/text_content.py
--rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/contents/types.py
--rw-r--r--   0        0        0      747 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/__init__.py
--rw-r--r--   0        0        0     3452 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/conversation_summary_plugin.py
--rw-r--r--   0        0        0     4069 2024-05-06 13:16:31.755032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/http_plugin.py
--rw-r--r--   0        0        0     2474 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/math_plugin.py
--rw-r--r--   0        0        0     3783 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/text_memory_plugin.py
--rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/text_plugin.py
--rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/time_plugin.py
--rw-r--r--   0        0        0     1163 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/wait_plugin.py
--rw-r--r--   0        0        0     1789 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/web_search_engine_plugin.py
--rw-r--r--   0        0        0      316 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/events/__init__.py
--rw-r--r--   0        0        0     2068 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/events/function_invoked_event_args.py
--rw-r--r--   0        0        0     1420 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/events/function_invoking_event_args.py
--rw-r--r--   0        0        0     1725 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/events/kernel_events_args.py
--rw-r--r--   0        0        0      537 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/__init__.py
--rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/content_exceptions.py
--rw-r--r--   0        0        0     1176 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/function_exceptions.py
--rw-r--r--   0        0        0     1319 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/kernel_exceptions.py
--rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/planner_exceptions.py
--rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/service_exceptions.py
--rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/exceptions/template_engine_exceptions.py
--rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/functions/__init__.py
--rw-r--r--   0        0        0     2455 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/function_result.py
--rw-r--r--   0        0        0     1601 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_arguments.py
--rw-r--r--   0        0        0     9539 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function.py
--rw-r--r--   0        0        0     5517 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_decorator.py
--rw-r--r--   0        0        0     7585 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_from_method.py
--rw-r--r--   0        0        0    17580 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_from_prompt.py
--rw-r--r--   0        0        0     1912 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_metadata.py
--rw-r--r--   0        0        0      559 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_parameter_metadata.py
--rw-r--r--   0        0        0    23557 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_plugin.py
--rw-r--r--   0        0        0      791 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/prompt_rendering_result.py
--rw-r--r--   0        0        0      260 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/functions/types.py
--rw-r--r--   0        0        0    38918 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/kernel.py
--rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/kernel_pydantic.py
--rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6521 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     3619 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     1310 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/__init__.py
--rw-r--r--   0        0        0      126 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/action_planner/__init__.py
--rw-r--r--   0        0        0    11352 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/action_planner/action_planner.py
--rw-r--r--   0        0        0      392 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/action_planner/action_planner_config.py
--rw-r--r--   0        0        0      409 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/action_planner/skprompt.txt
--rw-r--r--   0        0        0     8152 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/basic_planner.py
--rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
--rw-r--r--   0        0        0    11240 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
--rw-r--r--   0        0        0     1676 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
--rw-r--r--   0        0        0      886 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
--rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
--rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
--rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/planners/plan.py
--rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/planner_extensions.py
--rw-r--r--   0        0        0      622 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/planner_options.py
--rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
--rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
--rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/__init__.py
--rw-r--r--   0        0        0     5924 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner.py
--rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
--rw-r--r--   0        0        0     4729 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0        0        0     4987 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
--rw-r--r--   0        0        0      881 2024-03-13 15:37:17.055380 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/config.json
--rw-r--r--   0        0        0     2847 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/skprompt.txt
--rw-r--r--   0        0        0      243 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/__init__.py
--rw-r--r--   0        0        0    16330 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/stepwise_planner.py
--rw-r--r--   0        0        0      982 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/stepwise_planner_config.py
--rw-r--r--   0        0        0      371 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/planners/stepwise_planner/system_step.py
--rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/__init__.py
--rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/const.py
--rw-r--r--   0        0        0     4128 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/handlebars_prompt_template.py
--rw-r--r--   0        0        0      340 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/input_variable.py
--rw-r--r--   0        0        0     4670 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/jinja2_prompt_template.py
--rw-r--r--   0        0        0     7935 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/kernel_prompt_template.py
--rw-r--r--   0        0        0      623 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/prompt_template_base.py
--rw-r--r--   0        0        0     4762 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/prompt_template_config.py
--rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/__init__.py
--rw-r--r--   0        0        0     4585 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
--rw-r--r--   0        0        0     2476 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
--rw-r--r--   0        0        0     1701 2024-03-15 14:30:59.091994 semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/template_function_helpers.py
--rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-0.9.7b1/semantic_kernel/py.typed
--rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/services/__init__.py
--rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/services/ai_service_client_base.py
--rw-r--r--   0        0        0     2555 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/services/ai_service_selector.py
--rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     7402 2024-04-16 13:30:52.656626 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/named_arg_block.py
--rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/utils/chat.py
--rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/utils/logging.py
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/utils/naming.py
--rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0    12327 2024-05-06 13:16:31.765032 semantic_kernel-0.9.7b1/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-0.9.7b1/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     5107 1970-01-01 00:00:00.000000 semantic_kernel-0.9.7b1/PKG-INFO
+-rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-0.9.8b1/pip/README.md
+-rw-r--r--   0        0        0     5406 2024-05-09 23:07:37.255180 semantic_kernel-0.9.8b1/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     3223 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0      437 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0     7538 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/function_call_behavior.py
+-rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/__init__.py
+-rw-r--r--   0        0        0     1795 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
+-rw-r--r--   0        0        0     9646 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
+-rw-r--r--   0        0        0     3821 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
+-rw-r--r--   0        0        0     2191 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
+-rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     1169 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
+-rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
+-rw-r--r--   0        0        0     6662 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2119 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/__init__.py
+-rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
+-rw-r--r--   0        0        0     8403 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
+-rw-r--r--   0        0        0     3962 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
+-rw-r--r--   0        0        0     1805 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
+-rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/utils.py
+-rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0      246 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/const.py
+-rw-r--r--   0        0        0     2464 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/contents/function_call.py
+-rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
+-rw-r--r--   0        0        0     3817 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
+-rw-r--r--   0        0        0     4147 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
+-rw-r--r--   0        0        0    16094 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     5364 2024-03-20 18:24:28.763758 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
+-rw-r--r--   0        0        0     8276 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     4815 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     4731 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0    19477 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
+-rw-r--r--   0        0        0     3719 2024-03-20 18:24:28.763758 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
+-rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
+-rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
+-rw-r--r--   0        0        0     4797 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     6342 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
+-rw-r--r--   0        0        0     3016 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
+-rw-r--r--   0        0        0     2908 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/utils.py
+-rw-r--r--   0        0        0     3908 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/prompt_execution_settings.py
+-rw-r--r--   0        0        0     1720 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/__init__.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/__init__.py
+-rw-r--r--   0        0        0     6718 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/astra_client.py
+-rw-r--r--   0        0        0    11819 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
+-rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/utils.py
+-rw-r--r--   0        0        0      242 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0    15787 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      213 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
+-rw-r--r--   0        0        0    10299 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
+-rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
+-rw-r--r--   0        0        0     1592 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
+-rw-r--r--   0        0        0    13020 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
+-rw-r--r--   0        0        0      159 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0    12786 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
+-rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
+-rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    14991 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    20518 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/README.md
+-rw-r--r--   0        0        0      178 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/__init__.py
+-rw-r--r--   0        0        0    15281 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
+-rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/utils.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/usearch/__init__.py
+-rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
+-rw-r--r--   0        0        0      188 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/weaviate/__init__.py
+-rw-r--r--   0        0        0    11001 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
+-rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
+-rw-r--r--   0        0        0     1011 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/openai_utils.py
+-rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openapi_plugin/__init__.py
+-rw-r--r--   0        0        0     1241 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
+-rw-r--r--   0        0        0    13518 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
+-rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     2648 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-0.9.8b1/semantic_kernel/connectors/telemetry.py
+-rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/connectors/utils/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/connectors/utils/document_loader.py
+-rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/__init__.py
+-rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/author_role.py
+-rw-r--r--   0        0        0    13781 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/chat_history.py
+-rw-r--r--   0        0        0    12276 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/chat_message_content.py
+-rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/const.py
+-rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/contents/finish_reason.py
+-rw-r--r--   0        0        0     3729 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/function_call_content.py
+-rw-r--r--   0        0        0     3913 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/function_result_content.py
+-rw-r--r--   0        0        0      772 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/kernel_content.py
+-rw-r--r--   0        0        0    11084 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_chat_message_content.py
+-rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_content_mixin.py
+-rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_text_content.py
+-rw-r--r--   0        0        0     1957 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/text_content.py
+-rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/contents/types.py
+-rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3452 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/conversation_summary_plugin.py
+-rw-r--r--   0        0        0     4069 2024-05-06 13:16:31.755032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/http_plugin.py
+-rw-r--r--   0        0        0     2474 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/math_plugin.py
+-rw-r--r--   0        0        0     5868 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/README.md
+-rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
+-rw-r--r--   0        0        0     9409 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
+-rw-r--r--   0        0        0     1106 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
+-rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
+-rw-r--r--   0        0        0     3783 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/text_memory_plugin.py
+-rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/text_plugin.py
+-rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/time_plugin.py
+-rw-r--r--   0        0        0     1163 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/wait_plugin.py
+-rw-r--r--   0        0        0     1789 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/web_search_engine_plugin.py
+-rw-r--r--   0        0        0      316 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/events/__init__.py
+-rw-r--r--   0        0        0     2068 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/events/function_invoked_event_args.py
+-rw-r--r--   0        0        0     1420 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/events/function_invoking_event_args.py
+-rw-r--r--   0        0        0     1725 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/events/kernel_events_args.py
+-rw-r--r--   0        0        0      537 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/__init__.py
+-rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/content_exceptions.py
+-rw-r--r--   0        0        0     1176 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/function_exceptions.py
+-rw-r--r--   0        0        0     1319 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/kernel_exceptions.py
+-rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/planner_exceptions.py
+-rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/service_exceptions.py
+-rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/exceptions/template_engine_exceptions.py
+-rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/functions/__init__.py
+-rw-r--r--   0        0        0     2455 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/function_result.py
+-rw-r--r--   0        0        0     1601 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_arguments.py
+-rw-r--r--   0        0        0     9539 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function.py
+-rw-r--r--   0        0        0     5517 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_decorator.py
+-rw-r--r--   0        0        0     7585 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_from_method.py
+-rw-r--r--   0        0        0    17568 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_from_prompt.py
+-rw-r--r--   0        0        0     1912 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_metadata.py
+-rw-r--r--   0        0        0      559 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_parameter_metadata.py
+-rw-r--r--   0        0        0    23557 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_plugin.py
+-rw-r--r--   0        0        0      791 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/prompt_rendering_result.py
+-rw-r--r--   0        0        0      260 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/functions/types.py
+-rw-r--r--   0        0        0    41973 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/kernel_pydantic.py
+-rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6521 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3619 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/planners/__init__.py
+-rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
+-rw-r--r--   0        0        0    11592 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
+-rw-r--r--   0        0        0     1675 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
+-rw-r--r--   0        0        0      928 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
+-rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
+-rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
+-rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/planners/plan.py
+-rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/planners/planner_extensions.py
+-rw-r--r--   0        0        0      592 2024-05-09 23:07:37.265180 semantic_kernel-0.9.8b1/semantic_kernel/planners/planner_options.py
+-rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     5899 2024-05-09 23:07:37.275180 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     4720 2024-05-09 23:07:37.275180 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     4987 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/const.py
+-rw-r--r--   0        0        0     4128 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/handlebars_prompt_template.py
+-rw-r--r--   0        0        0      340 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/input_variable.py
+-rw-r--r--   0        0        0     4750 2024-05-09 23:07:37.275180 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/jinja2_prompt_template.py
+-rw-r--r--   0        0        0     7935 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/kernel_prompt_template.py
+-rw-r--r--   0        0        0      623 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/prompt_template_base.py
+-rw-r--r--   0        0        0     4762 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/prompt_template_config.py
+-rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/__init__.py
+-rw-r--r--   0        0        0     4585 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
+-rw-r--r--   0        0        0     2476 2024-05-06 13:16:31.765032 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
+-rw-r--r--   0        0        0     1701 2024-03-15 14:30:59.091994 semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/template_function_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-0.9.8b1/semantic_kernel/py.typed
+-rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/services/__init__.py
+-rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/services/ai_service_client_base.py
+-rw-r--r--   0        0        0     2648 2024-05-09 23:07:37.275180 semantic_kernel-0.9.8b1/semantic_kernel/services/ai_service_selector.py
+-rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     7402 2024-04-16 13:30:52.656626 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/named_arg_block.py
+-rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/utils/chat.py
+-rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/utils/logging.py
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/utils/naming.py
+-rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0    12623 2024-05-09 23:07:37.275180 semantic_kernel-0.9.8b1/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-0.9.8b1/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 semantic_kernel-0.9.8b1/PKG-INFO
```

### Comparing `semantic_kernel-0.9.7b1/pip/README.md` & `semantic_kernel-0.9.8b1/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/pyproject.toml` & `semantic_kernel-0.9.8b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.9.7b1"
+version = "0.9.8b1"
 description = "Semantic Kernel Python SDK"
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.13"
@@ -53,15 +53,15 @@
     { version = ">=2.3,<2.3.8", markers = 'python_version > "3.8"', optional = true}
 ]
 milvus = [
     { version = "^2.2,<2.3", markers = 'python_version == "3.8" and sys_platform != "win32"', optional = true},
     { version = ">=2.3,<2.3.8", markers = 'python_version > "3.8" and sys_platform != "win32"', optional = true}
 ]
 weaviate-client = { version = ">=3.18,<5.0", optional = true}
-pinecone-client = { version = "^2.2.2", optional = true}
+pinecone-client = { version = ">=3.0.0", optional = true}
 psycopg = { version="^3.1.9", extras=["binary","pool"], optional = true}
 redis = { version = "^4.6.0", optional = true}
 azure-search-documents = {version = "11.6.0b1", allow-prereleases = true, optional = true}
 azure-core = { version = "^1.28.0", optional = true}
 azure-identity = { version = "^1.13.0", optional = true}
 usearch = { version = "^2.9", optional = true}
 pyarrow = { version = ">=12.0.1,<16.0.0", optional = true}
@@ -106,15 +106,15 @@
     { version = ">=2.3,<2.3.8", markers = 'python_version > "3.8"'}
 ]
 milvus = [
     { version = "^2.2,<2.3", markers = 'python_version == "3.8" and sys_platform != "win32"'},
     { version = ">=2.3,<2.3.8", markers = 'python_version > "3.8" and sys_platform != "win32"'}
 ]
 weaviate-client = ">=3.18,<5.0"
-pinecone-client = "^2.2.2"
+pinecone-client = ">=3.0.0"
 psycopg = { version="^3.1.9", extras=["binary","pool"]}
 redis = "^4.6.0"
 azure-search-documents = {version = "11.6.0b1", allow-prereleases = true}
 azure-core = "^1.28.0"
 azure-identity = "^1.13.0"
 usearch = "^2.9"
 pyarrow = ">=12.0.1,<16.0.0"
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+# Copyright (c) Microsoft. All rights reserved.
+from __future__ import annotations
+
 import logging
 from typing import Any, Dict, List, Literal, Optional, Union
 
 from pydantic import Field, field_validator, model_validator
 
+from semantic_kernel.connectors.ai.function_call_behavior import FunctionCallBehavior
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.exceptions import ServiceInvalidExecutionSettingsError
 
 logger = logging.getLogger(__name__)
 
 
 class OpenAIPromptExecutionSettings(PromptExecutionSettings):
@@ -51,21 +55,20 @@
         return self
 
 
 class OpenAIChatPromptExecutionSettings(OpenAIPromptExecutionSettings):
     """Specific settings for the Chat Completion endpoint."""
 
     response_format: Optional[Dict[Literal["type"], Literal["text", "json_object"]]] = None
-    tools: Optional[List[Dict[str, Any]]] = None
+    tools: Optional[List[Dict[str, Any]]] = Field(None, max_length=64)
     tool_choice: Optional[str] = None
     function_call: Optional[str] = None
     functions: Optional[List[Dict[str, Any]]] = None
     messages: Optional[List[Dict[str, Any]]] = None
-    auto_invoke_kernel_functions: Optional[bool] = Field(default=False, exclude=True)
-    max_auto_invoke_attempts: Optional[int] = Field(default=5, exclude=True)
+    function_call_behavior: Optional[FunctionCallBehavior] = Field(None, exclude=True)
 
     @field_validator("functions", "function_call", mode="after")
     @classmethod
     def validate_function_call(cls, v: Optional[Union[str, List[Dict[str, Any]]]] = None):
         if v is not None:
             logger.warning(
                 "The function_call and functions parameters are deprecated. Please use the tool_choice and tools parameters instead."  # noqa: E501
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # Copyright (c) Microsoft. All rights reserved.
 
+import asyncio
 import logging
 from copy import copy
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Optional, Tuple, Union
 
 from openai import AsyncStream
 from openai.types.chat.chat_completion import ChatCompletion, Choice
 from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 from openai.types.chat.chat_completion_chunk import Choice as ChunkChoice
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
+from semantic_kernel.connectors.ai.function_call_behavior import FunctionCallBehavior
+from semantic_kernel.connectors.ai.open_ai.contents.function_call import FunctionCall
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIChatPromptExecutionSettings,
-    OpenAIPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIHandler
-from semantic_kernel.connectors.ai.open_ai.services.tool_call_behavior import ToolCallBehavior
+from semantic_kernel.connectors.ai.open_ai.services.utils import update_settings_from_function_call_configuration
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.contents.author_role import AuthorRole
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
 from semantic_kernel.contents.finish_reason import FinishReason
 from semantic_kernel.contents.function_call_content import FunctionCallContent
 from semantic_kernel.contents.function_result_content import FunctionResultContent
@@ -50,88 +52,120 @@
     def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
         """Create a request settings object."""
         return OpenAIChatPromptExecutionSettings
 
     async def complete_chat(
         self,
         chat_history: ChatHistory,
-        settings: OpenAIPromptExecutionSettings,
+        settings: OpenAIChatPromptExecutionSettings,
         **kwargs: Any,
     ) -> List["ChatMessageContent"]:
         """Executes a chat completion request and returns the result.
 
         Arguments:
             chat_history {ChatHistory} -- The chat history to use for the chat completion.
             settings {OpenAIChatPromptExecutionSettings | AzureChatPromptExecutionSettings} -- The settings to use
                 for the chat completion request.
             kwargs {Dict[str, Any]} -- The optional arguments.
 
         Returns:
             List[ChatMessageContent] -- The completion result(s).
         """
-        tool_call_behavior = self._get_tool_call_behavior(settings)
+
         kernel = kwargs.get("kernel", None)
         arguments = kwargs.get("arguments", None)
-        if tool_call_behavior.auto_invoke_kernel_functions and (kernel is None or arguments is None):
+        if (
+            settings.function_call_behavior is not None
+            and settings.function_call_behavior.auto_invoke_kernel_functions
+            and (kernel is None or arguments is None)
+        ):
             raise ServiceInvalidExecutionSettingsError(
-                "The kernel argument and arguments are required for OpenAI tool calling."
+                "The kernel argument and arguments are required for auto invoking OpenAI tool calls."
             )
+        # behavior for non-function calling or for enable, but not auto-invoke.
+        settings = self._prepare_settings(settings, chat_history, stream_request=False, kernel=kernel)
+        if settings.function_call_behavior is None or (
+            settings.function_call_behavior and not settings.function_call_behavior.auto_invoke_kernel_functions
+        ):
+            return await self._send_chat_request(settings)
 
-        for _ in range(tool_call_behavior.max_auto_invoke_attempts):
-            settings = self._prepare_settings(settings, chat_history, stream_request=False)
+        # loop for auto-invoke function calls
+        for _ in range(settings.function_call_behavior.max_auto_invoke_attempts):
             completions = await self._send_chat_request(settings)
-            if not tool_call_behavior.auto_invoke_kernel_functions or all(
+            if all(
                 not isinstance(item, FunctionCallContent) for completion in completions for item in completion.items
             ):
                 return completions
             await self._process_chat_response_with_tool_call(
                 completions=completions, chat_history=chat_history, kernel=kernel, arguments=arguments
             )
+            settings = self._prepare_settings(settings, chat_history, stream_request=False, kernel=kernel)
 
     async def complete_chat_stream(
         self,
         chat_history: ChatHistory,
-        settings: OpenAIPromptExecutionSettings,
+        settings: OpenAIChatPromptExecutionSettings,
         **kwargs: Any,
     ) -> AsyncGenerator[List[StreamingChatMessageContent], Any]:
         """Executes a streaming chat completion request and returns the result.
 
         Arguments:
             chat_history {ChatHistory} -- The chat history to use for the chat completion.
             settings {OpenAIChatPromptExecutionSettings | AzureChatPromptExecutionSettings} -- The settings to use
                 for the chat completion request.
             kwargs {Dict[str, Any]} -- The optional arguments.
 
         Yields:
             List[StreamingChatMessageContent] -- A stream of
                 StreamingChatMessageContent when using Azure.
         """
-        tool_call_behavior = self._get_tool_call_behavior(settings)
         kernel = kwargs.get("kernel", None)
         arguments = kwargs.get("arguments", None)
-        if tool_call_behavior.auto_invoke_kernel_functions and (kernel is None or arguments is None):
+        if (
+            settings.function_call_behavior is not None
+            and settings.function_call_behavior.auto_invoke_kernel_functions
+            and (kernel is None or arguments is None)
+        ):
             raise ServiceInvalidExecutionSettingsError(
                 "The kernel argument and arguments are required for OpenAI tool calling."
             )
 
-        for _ in range(tool_call_behavior.max_auto_invoke_attempts):
-            settings = self._prepare_settings(settings, chat_history, stream_request=True)
+        # Prepare settings for streaming requests
+        settings = self._prepare_settings(settings, chat_history, stream_request=True, kernel=kernel)
+
+        # Behavior for non-function calling or for enable, but not auto-invoke
+        if settings.function_call_behavior is None or (
+            settings.function_call_behavior and not settings.function_call_behavior.auto_invoke_kernel_functions
+        ):
+            async for content, _ in self._process_chat_stream_response(
+                response=await self._send_chat_stream_request(settings),
+                chat_history=chat_history,
+                kernel=kernel,
+                tool_call_behavior=None,  # type: ignore
+                arguments=arguments,
+            ):
+                yield content
+            return
+
+        # Loop for auto-invoke function calls
+        for _ in range(settings.function_call_behavior.max_auto_invoke_attempts):
             response = await self._send_chat_stream_request(settings)
             finish_reason = None
             async for content, finish_reason in self._process_chat_stream_response(
                 response=response,
                 chat_history=chat_history,
                 kernel=kernel,
-                tool_call_behavior=tool_call_behavior,
+                tool_call_behavior=settings.function_call_behavior,  # type: ignore
                 arguments=arguments,
             ):
                 if content:
                     yield content
             if finish_reason != FinishReason.TOOL_CALLS:
                 break
+            settings = self._prepare_settings(settings, chat_history, stream_request=True, kernel=kernel)
 
     def _chat_message_content_to_dict(self, message: "ChatMessageContent") -> Dict[str, Optional[str]]:
         msg = super()._chat_message_content_to_dict(message)
         if message.role == "assistant":
             if tool_calls := getattr(message, "tool_calls", None):
                 msg["tool_calls"] = [tool_call.model_dump() for tool_call in tool_calls]
             if function_call := getattr(message, "function_call", None):
@@ -169,21 +203,21 @@
         kernel: "Kernel",
         arguments: "KernelArguments",
     ) -> None:
         """Process the completions in the chat response"""
         for result in completions:
             # An assistant message needs to be followed be a tool call response
             chat_history = store_results(chat_history=chat_history, results=[result])
-            await self._process_tool_calls(result, kernel, chat_history, arguments)
+            await self._process_tool_calls(result=result, kernel=kernel, chat_history=chat_history, arguments=arguments)
 
     async def _process_chat_stream_response(
         self,
         response: AsyncStream,
         chat_history: ChatHistory,
-        tool_call_behavior: ToolCallBehavior,
+        tool_call_behavior: FunctionCallBehavior,
         kernel: Optional["Kernel"] = None,
         arguments: Optional["KernelArguments"] = None,
     ) -> AsyncGenerator[Tuple[List["StreamingChatMessageContent"], Optional["FinishReason"]], Any]:
         """Process the chat stream response and handle tool calls if applicable."""
         full_content = None
         async for chunk in response:
             if len(chunk.choices) == 0:
@@ -191,15 +225,15 @@
 
             chunk_metadata = self._get_metadata_from_streaming_chat_response(chunk)
             contents = [
                 self._create_streaming_chat_message_content(chunk, choice, chunk_metadata) for choice in chunk.choices
             ]
             if not contents:
                 continue
-            if not tool_call_behavior.auto_invoke_kernel_functions:
+            if not tool_call_behavior or not tool_call_behavior.auto_invoke_kernel_functions:
                 yield contents, None
                 continue
 
             full_content = contents[0] if full_content is None else full_content + contents[0]
             finish_reason = getattr(full_content, "finish_reason", None)
             if not any(isinstance(item, FunctionCallContent) for item in full_content.items) or finish_reason not in (
                 FinishReason.STOP,
@@ -315,95 +349,87 @@
             return []
         return [
             FunctionCallContent(
                 id="legacy_function_call", name=content.function_call.name, arguments=content.function_call.arguments
             )
         ]
 
-    def _get_tool_call_behavior(self, execution_settings: OpenAIPromptExecutionSettings) -> ToolCallBehavior:
-        """Gets the auto invoke and max iterations settings through ToolCallBehavior."""
-        auto_invoke_kernel_functions = False
-        max_auto_invoke_attempts = 1
-        if isinstance(execution_settings, OpenAIChatPromptExecutionSettings):
-            if execution_settings.auto_invoke_kernel_functions is not None:
-                auto_invoke_kernel_functions = execution_settings.auto_invoke_kernel_functions
-            if auto_invoke_kernel_functions and execution_settings.max_auto_invoke_attempts is not None:
-                max_auto_invoke_attempts = (
-                    execution_settings.max_auto_invoke_attempts if auto_invoke_kernel_functions else 1
-                )
-
-        return ToolCallBehavior(
-            auto_invoke_kernel_functions=auto_invoke_kernel_functions, max_auto_invoke_attempts=max_auto_invoke_attempts
-        )
-
     # endregion
     # region request preparation
 
     def _prepare_settings(
         self,
         settings: OpenAIChatPromptExecutionSettings,
         chat_history: ChatHistory,
         stream_request: bool = False,
+        kernel: "Kernel | None" = None,
     ) -> OpenAIChatPromptExecutionSettings:
-        """Prepare the promp execution settings for the chat request."""
+        """Prepare the prompt execution settings for the chat request."""
         settings.messages = self._prepare_chat_history_for_request(chat_history)
         settings.stream = stream_request
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
 
-        # If auto_invoke_kernel_functions is True and num_of_responses > 1 provide a warning
-        # that the num_of_responses will be configured to one.
-        if settings.auto_invoke_kernel_functions and settings.number_of_responses > 1:
-            logger.warning(
-                (
-                    "Auto invoking functions does not support more than one num_of_response. "
-                    "The num_of_responses setting is configured as 1."
-                )
+        if settings.function_call_behavior and kernel:
+            settings.function_call_behavior.configure(
+                kernel=kernel,
+                update_settings_callback=update_settings_from_function_call_configuration,
+                settings=settings,
             )
-            settings.number_of_responses = 1
         return settings
 
     # endregion
     # region tool calling
 
     async def _process_tool_calls(
         self,
         result: ChatMessageContent,
         kernel: "Kernel",
         chat_history: ChatHistory,
         arguments: "KernelArguments",
     ) -> None:
+        """Processes the tool calls in parallel in the result and return it as part of the chat history."""
+        logger.info(f"processing {len(result.items)} tool calls in parallel.")
+        await asyncio.gather(
+            *[
+                self._process_tool_call(result=tc, kernel=kernel, chat_history=chat_history, arguments=arguments)
+                for tc in result.items
+            ]
+        )
+
+    async def _process_tool_call(
+        self,
+        result: ChatMessageContent,
+        kernel: "Kernel",
+        chat_history: ChatHistory,
+        arguments: "KernelArguments",
+    ) -> None:
         """Processes the tool calls in the result and return it as part of the chat history."""
-        logger.info(f"processing {len(result.items)} tool calls")
         args_cloned = copy(arguments)
-        for function_call in result.items:
-            if not isinstance(function_call, FunctionCallContent):
-                continue
-            try:
-                func_args = function_call.parse_arguments()
-                if func_args:
-                    args_cloned.update(func_args)
-            except FunctionCallInvalidArgumentsException as exc:
-                logger.exception(
-                    f"Received invalid arguments for function {function_call.name}: {exc}. Trying tool call again."
-                )
-                frc = FunctionResultContent.from_function_call_content_and_result(
-                    function_call_content=function_call,
-                    result="The tool call arguments are malformed, please try again.",
-                )
-                chat_history.add_message(message=frc.to_chat_message_content())
-                continue
-            logger.info(f"Calling {function_call.name} function with args: {function_call.arguments}")
-            try:
-                func_result = await kernel.invoke(**function_call.split_name_dict(), arguments=args_cloned)
-            except Exception as exc:
-                logger.exception(f"Error occurred while invoking function {function_call.name}")
-                raise ServiceInvalidResponseError(
-                    f"Error occurred while invoking function {function_call.name}"
-                ) from exc
+        func: FunctionCall | None = result
+        if not func:
+            return
+        try:
+            parsed_args = func.parse_arguments()
+            if parsed_args:
+                args_cloned.update(parsed_args)
+        except FunctionCallInvalidArgumentsException as exc:
+            logger.exception(f"Received invalid arguments for function {func.name}: {exc}. Trying tool call again.")
             frc = FunctionResultContent.from_function_call_content_and_result(
-                function_call_content=function_call, result=func_result
+                function_call_content=result,
+                result="The tool call arguments are malformed, please try again.",
             )
             chat_history.add_message(message=frc.to_chat_message_content())
+            return
+        logger.info(f"Calling {func.name} function with args: {func.arguments}")
+        try:
+            func_result = await kernel.invoke(**func.split_name_dict(), arguments=args_cloned)
+        except Exception as exc:
+            logger.exception(f"Error occurred while invoking function {func.name}")
+            raise ServiceInvalidResponseError(f"Error occurred while invoking function {func.name}") from exc
+        frc = FunctionResultContent.from_function_call_content_and_result(
+            function_call_content=result, result=func_result
+        )
+        chat_history.add_message(message=frc.to_chat_message_content())
 
 
 # endregion
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/prompt_execution_settings.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/astra_client.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/astra_client.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/astradb/utils.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/astradb/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,88 +1,85 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import List, Optional, Tuple
+from typing import List, NamedTuple, Optional, Tuple
 
-import pinecone
 from numpy import ndarray
-from pinecone import FetchResponse, IndexDescription
+from pinecone import FetchResponse, IndexDescription, IndexList, Pinecone, ServerlessSpec
 
 from semantic_kernel.connectors.memory.pinecone.utils import (
     build_payload,
     parse_payload,
 )
 from semantic_kernel.exceptions import (
     ServiceInitializationError,
     ServiceInvalidRequestError,
     ServiceResourceNotFoundError,
     ServiceResponseException,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 
-# Limitations set by Pinecone at https://docs.pinecone.io/docs/limits
+# Limitations set by Pinecone at https://docs.pinecone.io/reference/known-limitations
 MAX_DIMENSIONALITY = 20000
 MAX_UPSERT_BATCH_SIZE = 100
 MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE = 10000
 MAX_QUERY_WITH_METADATA_BATCH_SIZE = 1000
 MAX_FETCH_BATCH_SIZE = 1000
 MAX_DELETE_BATCH_SIZE = 1000
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class PineconeMemoryStore(MemoryStoreBase):
     """A memory store that uses Pinecone as the backend."""
 
     _pinecone_api_key: str
-    _pinecone_environment: str
     _default_dimensionality: int
 
+    DEFAULT_INDEX_SPEC: ServerlessSpec = ServerlessSpec(
+        cloud="aws",
+        region="us-east-1",
+    )
+
     def __init__(
         self,
         api_key: str,
-        environment: str,
         default_dimensionality: int,
         **kwargs,
     ) -> None:
         """Initializes a new instance of the PineconeMemoryStore class.
 
         Arguments:
             pinecone_api_key {str} -- The Pinecone API key.
-            pinecone_environment {str} -- The Pinecone environment.
             default_dimensionality {int} -- The default dimensionality to use for new collections.
         """
         if kwargs.get("logger"):
             logger.warning("The `logger` parameter is deprecated. Please use the `logging` module instead.")
         if default_dimensionality > MAX_DIMENSIONALITY:
             raise ServiceInitializationError(
                 f"Dimensionality of {default_dimensionality} exceeds "
                 + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
             )
         self._pinecone_api_key = api_key
-        self._pinecone_environment = environment
         self._default_dimensionality = default_dimensionality
 
-        pinecone.init(api_key=self._pinecone_api_key, environment=self._pinecone_environment)
+        self.pinecone = Pinecone(api_key=self._pinecone_api_key)
+        self.collection_names_cache = set()
 
     async def create_collection(
         self,
         collection_name: str,
         dimension_num: Optional[int] = None,
         distance_type: Optional[str] = "cosine",
-        num_of_pods: Optional[int] = 1,
-        replica_num: Optional[int] = 0,
-        type_of_pod: Optional[str] = "p1.x1",
-        metadata_config: Optional[dict] = None,
+        index_spec: NamedTuple = DEFAULT_INDEX_SPEC,
     ) -> None:
         """Creates a new collection in Pinecone if it does not exist.
             This function creates an index, by default the following index
-            settings are used: metric = cosine, pods = 1, replicas = 0,
-            pod_type = p1.x1, metadata_config = None.
+            settings are used: metric = cosine, cloud = aws, region = us-east-1.
 
         Arguments:
             collection_name {str} -- The name of the collection to create.
             In Pinecone, a collection is represented as an index. The concept
             of "collection" in Pinecone is just a static copy of an index.
 
         Returns:
@@ -91,83 +88,85 @@
         if dimension_num is None:
             dimension_num = self._default_dimensionality
         if dimension_num > MAX_DIMENSIONALITY:
             raise ServiceInitializationError(
                 f"Dimensionality of {dimension_num} exceeds " + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
             )
 
-        if collection_name not in pinecone.list_indexes():
-            pinecone.create_index(
-                name=collection_name,
-                dimension=dimension_num,
-                metric=distance_type,
-                pods=num_of_pods,
-                replicas=replica_num,
-                pod_type=type_of_pod,
-                metadata_config=metadata_config,
+        if not await self.does_collection_exist(collection_name):
+            self.pinecone.create_index(
+                name=collection_name, dimension=dimension_num, metric=distance_type, spec=index_spec
             )
+            self.collection_names_cache.add(collection_name)
 
     async def describe_collection(self, collection_name: str) -> Optional[IndexDescription]:
         """Gets the description of the index.
         Arguments:
             collection_name {str} -- The name of the index to get.
         Returns:
             Optional[dict] -- The index.
         """
-        if collection_name in pinecone.list_indexes():
-            return pinecone.describe_index(collection_name)
+        if await self.does_collection_exist(collection_name):
+            return self.pinecone.describe_index(collection_name)
         return None
 
     async def get_collections(
         self,
-    ) -> List[str]:
+    ) -> IndexList:
         """Gets the list of collections.
 
         Returns:
-            List[str] -- The list of collections.
+            IndexList -- The list of collections.
         """
-        return list(pinecone.list_indexes())
+        return self.pinecone.list_indexes()
 
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection.
 
         Arguments:
             collection_name {str} -- The name of the collection to delete.
 
         Returns:
             None
         """
-        if collection_name in pinecone.list_indexes():
-            pinecone.delete_index(collection_name)
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
-        return collection_name in pinecone.list_indexes()
+        if collection_name in self.collection_names_cache:
+            return True
+
+        index_collection_names = self.pinecone.list_indexes().names()
+        self.collection_names_cache |= set(index_collection_names)
+
+        return collection_name in index_collection_names
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
         """Upserts a record.
 
         Arguments:
             collection_name {str} -- The name of the collection to upsert the record into.
             record {MemoryRecord} -- The record to upsert.
 
         Returns:
             str -- The unique database key of the record. In Pinecone, this is the record ID.
         """
-        if collection_name not in pinecone.list_indexes():
+        if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        collection = pinecone.Index(collection_name)
+        collection = self.pinecone.Index(collection_name)
 
         upsert_response = collection.upsert(
             vectors=[(record._id, record.embedding.tolist(), build_payload(record))],
             namespace="",
         )
 
         if upsert_response.upserted_count is None:
@@ -181,18 +180,18 @@
         Arguments:
             collection_name {str} -- The name of the collection to upsert the records into.
             records {List[MemoryRecord]} -- The records to upsert.
 
         Returns:
             List[str] -- The unique database keys of the records.
         """
-        if collection_name not in pinecone.list_indexes():
+        if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        collection = pinecone.Index(collection_name)
+        collection = self.pinecone.Index(collection_name)
 
         vectors = [
             (
                 record._id,
                 record.embedding.tolist(),
                 build_payload(record),
             )
@@ -213,18 +212,18 @@
             collection_name {str} -- The name of the collection to get the record from.
             key {str} -- The unique database key of the record.
             with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
 
         Returns:
             MemoryRecord -- The record.
         """
-        if collection_name not in pinecone.list_indexes():
+        if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        collection = pinecone.Index(collection_name)
+        collection = self.pinecone.Index(collection_name)
         fetch_response = collection.fetch([key])
 
         if len(fetch_response.vectors) == 0:
             raise ServiceResourceNotFoundError(f"Record with key '{key}' does not exist")
 
         return parse_payload(fetch_response.vectors[key], with_embedding)
 
@@ -237,15 +236,15 @@
             collection_name {str} -- The name of the collection to get the records from.
             keys {List[str]} -- The unique database keys of the records.
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
         Returns:
             List[MemoryRecord] -- The records.
         """
-        if collection_name not in pinecone.list_indexes():
+        if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
         fetch_response = await self.__get_batch(collection_name, keys, with_embeddings)
         return [parse_payload(fetch_response.vectors[key], with_embeddings) for key in fetch_response.vectors.keys()]
 
     async def remove(self, collection_name: str, key: str) -> None:
         """Removes a record.
@@ -253,34 +252,34 @@
         Arguments:
             collection_name {str} -- The name of the collection to remove the record from.
             key {str} -- The unique database key of the record to remove.
 
         Returns:
             None
         """
-        if collection_name not in pinecone.list_indexes():
+        if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        collection = pinecone.Index(collection_name)
+        collection = self.pinecone.Index(collection_name)
         collection.delete([key])
 
     async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
         """Removes a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the records from.
             keys {List[str]} -- The unique database keys of the records to remove.
 
         Returns:
             None
         """
-        if collection_name not in pinecone.list_indexes():
+        if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        collection = pinecone.Index(collection_name)
+        collection = self.pinecone.Index(collection_name)
         for i in range(0, len(keys), MAX_DELETE_BATCH_SIZE):
             collection.delete(keys[i : i + MAX_DELETE_BATCH_SIZE])
         collection.delete(keys)
 
     async def get_nearest_match(
         self,
         collection_name: str,
@@ -324,18 +323,18 @@
             limit {int} -- The maximum number of matches to return.
             min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
         Returns:
             List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
         """
-        if collection_name not in pinecone.list_indexes():
+        if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        collection = pinecone.Index(collection_name)
+        collection = self.pinecone.Index(collection_name)
 
         if limit > MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE:
             raise ServiceInvalidRequestError(
                 "Limit must be less than or equal to " + f"{MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE}"
             )
         elif limit > MAX_QUERY_WITH_METADATA_BATCH_SIZE:
             query_response = collection.query(
@@ -371,15 +370,15 @@
             if len(matches) > 0
             else []
         )
 
     async def __get_batch(
         self, collection_name: str, keys: List[str], with_embeddings: bool = False
     ) -> "FetchResponse":
-        index = pinecone.Index(collection_name)
+        index = self.pinecone.Index(collection_name)
         if len(keys) > MAX_FETCH_BATCH_SIZE:
             fetch_response = index.fetch(keys[0:MAX_FETCH_BATCH_SIZE])
             for i in range(MAX_FETCH_BATCH_SIZE, len(keys), MAX_FETCH_BATCH_SIZE):
                 fetch_response.vectors.update(index.fetch(keys[i : i + MAX_FETCH_BATCH_SIZE]).vectors)
         else:
             fetch_response = index.fetch(keys)
         return fetch_response
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/README.md` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/redis/utils.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/redis/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/openai_plugin/openai_utils.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/openai_plugin/openai_utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/search_engine/google_connector.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/telemetry.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/telemetry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/connectors/utils/document_loader.py` & `semantic_kernel-0.9.8b1/semantic_kernel/connectors/utils/document_loader.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/contents/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/contents/chat_history.py` & `semantic_kernel-0.9.8b1/semantic_kernel/contents/chat_history.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/contents/chat_message_content.py` & `semantic_kernel-0.9.8b1/semantic_kernel/contents/chat_message_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/contents/function_call_content.py` & `semantic_kernel-0.9.8b1/semantic_kernel/contents/function_call_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/contents/function_result_content.py` & `semantic_kernel-0.9.8b1/semantic_kernel/contents/function_result_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/contents/kernel_content.py` & `semantic_kernel-0.9.8b1/semantic_kernel/contents/kernel_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/contents/streaming_chat_message_content.py` & `semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/contents/streaming_content_mixin.py` & `semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_content_mixin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/contents/streaming_text_content.py` & `semantic_kernel-0.9.8b1/semantic_kernel/contents/streaming_text_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/contents/text_content.py` & `semantic_kernel-0.9.8b1/semantic_kernel/contents/text_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/contents/types.py` & `semantic_kernel-0.9.8b1/semantic_kernel/contents/types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from semantic_kernel.core_plugins.conversation_summary_plugin import (
     ConversationSummaryPlugin,
 )
 from semantic_kernel.core_plugins.http_plugin import HttpPlugin
 from semantic_kernel.core_plugins.math_plugin import MathPlugin
+from semantic_kernel.core_plugins.sessions_python_tool.sessions_python_plugin import (
+    SessionsPythonTool,
+)
 from semantic_kernel.core_plugins.text_memory_plugin import TextMemoryPlugin
 from semantic_kernel.core_plugins.text_plugin import TextPlugin
 from semantic_kernel.core_plugins.time_plugin import TimePlugin
 from semantic_kernel.core_plugins.web_search_engine_plugin import WebSearchEnginePlugin
 
 __all__ = [
     "TextMemoryPlugin",
     "TextPlugin",
     "TimePlugin",
     "HttpPlugin",
     "ConversationSummaryPlugin",
     "MathPlugin",
+    "SessionsPythonTool",
     "WebSearchEnginePlugin",
 ]
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/conversation_summary_plugin.py` & `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/conversation_summary_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/http_plugin.py` & `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/http_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/math_plugin.py` & `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/math_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/text_memory_plugin.py` & `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/text_memory_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/text_plugin.py` & `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/text_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/time_plugin.py` & `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/time_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/wait_plugin.py` & `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/wait_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/core_plugins/web_search_engine_plugin.py` & `semantic_kernel-0.9.8b1/semantic_kernel/core_plugins/web_search_engine_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/events/function_invoked_event_args.py` & `semantic_kernel-0.9.8b1/semantic_kernel/events/function_invoked_event_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/events/function_invoking_event_args.py` & `semantic_kernel-0.9.8b1/semantic_kernel/events/function_invoking_event_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/events/kernel_events_args.py` & `semantic_kernel-0.9.8b1/semantic_kernel/events/kernel_events_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/content_exceptions.py` & `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/content_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/function_exceptions.py` & `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/function_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/kernel_exceptions.py` & `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/kernel_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/planner_exceptions.py` & `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/planner_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/service_exceptions.py` & `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/service_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/exceptions/template_engine_exceptions.py` & `semantic_kernel-0.9.8b1/semantic_kernel/exceptions/template_engine_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/functions/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/functions/function_result.py` & `semantic_kernel-0.9.8b1/semantic_kernel/functions/function_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_arguments.py` & `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_arguments.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function.py` & `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_decorator.py` & `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_from_method.py` & `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_from_method.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_from_prompt.py` & `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_from_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         arguments: KernelArguments,
     ) -> FunctionResult:
         """Handles the chat service call."""
         chat_history = ChatHistory.from_rendered_prompt(prompt)
 
         # pass the kernel in for auto function calling
         kwargs: dict[str, Any] = {}
-        if hasattr(execution_settings, "auto_invoke_kernel_functions"):
+        if hasattr(execution_settings, "function_call_behavior"):
             kwargs["kernel"] = kernel
             kwargs["arguments"] = arguments
 
         try:
             completions = await service.complete_chat(
                 chat_history=chat_history,
                 settings=execution_settings,
@@ -276,15 +276,15 @@
         prompt: str,
         arguments: KernelArguments,
     ) -> AsyncGenerator[FunctionResult | list[StreamingChatMessageContent], Any]:
         """Handles the chat service call."""
 
         # pass the kernel in for auto function calling
         kwargs: dict[str, Any] = {}
-        if hasattr(execution_settings, "auto_invoke_kernel_functions"):
+        if hasattr(execution_settings, "function_call_behavior"):
             kwargs["kernel"] = kernel
             kwargs["arguments"] = arguments
 
         chat_history = ChatHistory.from_rendered_prompt(prompt)
         try:
             async for partial_content in service.complete_chat_stream(
                 chat_history=chat_history,
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_function_metadata.py` & `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_function_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_parameter_metadata.py` & `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_parameter_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/functions/kernel_plugin.py` & `semantic_kernel-0.9.8b1/semantic_kernel/functions/kernel_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/functions/prompt_rendering_result.py` & `semantic_kernel-0.9.8b1/semantic_kernel/functions/prompt_rendering_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/kernel.py` & `semantic_kernel-0.9.8b1/semantic_kernel/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 from copy import copy
+from functools import singledispatchmethod
 from typing import TYPE_CHECKING, Any, AsyncGenerator, AsyncIterable, Callable, Literal, Type, TypeVar, Union
 
 from pydantic import Field, field_validator
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
 from semantic_kernel.events import FunctionInvokedEventArgs, FunctionInvokingEventArgs
@@ -241,14 +242,16 @@
 
         Returns:
             FunctionResult | list[FunctionResult] | None: The result of the function(s)
 
         """
         if arguments is None:
             arguments = KernelArguments(**kwargs)
+        else:
+            arguments.update(kwargs)
         if not function:
             if not function_name or not plugin_name:
                 raise KernelFunctionNotFoundError("No function or plugin name provided")
             function = self.get_function(plugin_name, function_name)
         function_invoking_args = self.on_function_invoking(function.metadata, arguments)
         if function_invoking_args.is_cancel_requested:
             logger.info(
@@ -462,15 +465,15 @@
             del self.function_invoked_handlers[id(handler)]
 
     # endregion
     # region Plugins & Functions
 
     def add_plugin(
         self,
-        plugin: KernelPlugin | Any | dict[str, Any] | None = None,
+        plugin: KernelPlugin | object | dict[str, Any] | None = None,
         plugin_name: str | None = None,
         parent_directory: str | None = None,
         description: str | None = None,
         class_init_arguments: dict[str, dict[str, Any]] | None = None,
     ) -> "KernelPlugin":
         """
         Adds a plugin to the kernel's collection of plugins. If a plugin is provided,
@@ -514,24 +517,24 @@
                 parent_directory=parent_directory,
                 description=description,
                 class_init_arguments=class_init_arguments,
             )
             return self.plugins[plugin_name]
         raise ValueError("plugin or parent_directory must be provided.")
 
-    def add_plugins(self, plugins: list[KernelPlugin | object] | dict[str, KernelPlugin | object]) -> None:
+    def add_plugins(self, plugins: list[KernelPlugin] | dict[str, KernelPlugin | object]) -> None:
         """
         Adds a list of plugins to the kernel's collection of plugins.
 
         Args:
             plugins (list[KernelPlugin] | dict[str, KernelPlugin]): The plugins to add to the kernel
         """
         if isinstance(plugins, list):
-            for plugin in plugins:
-                self.add_plugin(plugin)
+            for plug in plugins:
+                self.add_plugin(plug)
             return
         for name, plugin in plugins.items():
             self.add_plugin(plugin, plugin_name=name)
 
     def add_function(
         self,
         plugin_name: str,
@@ -749,17 +752,29 @@
             plugin_name = None
             function_name = names[0]
         else:
             plugin_name = names[0]
             function_name = names[1]
         return self.get_function(plugin_name, function_name)
 
-    def get_list_of_function_metadata(
+    def get_full_list_of_function_metadata(self) -> list["KernelFunctionMetadata"]:
+        """Get a list of all function metadata in the plugins."""
+        if not self.plugins:
+            return []
+        return [func.metadata for plugin in self.plugins.values() for func in plugin]
+
+    @singledispatchmethod
+    def get_list_of_function_metadata(self, *args: Any, **kwargs: Any) -> list["KernelFunctionMetadata"]:
+        """Get a list of all function metadata in the plugin collection."""
+        raise NotImplementedError("This method is not implemented for the provided arguments.")
+
+    @get_list_of_function_metadata.register(bool)
+    def get_list_of_function_metadata_bool(
         self, include_prompt: bool = True, include_native: bool = True
-    ) -> list[KernelFunctionMetadata]:
+    ) -> list["KernelFunctionMetadata"]:
         """
         Get a list of the function metadata in the plugin collection
 
         Args:
             include_prompt (bool): Whether to include semantic functions in the list.
             include_native (bool): Whether to include native functions in the list.
 
@@ -771,14 +786,59 @@
         return [
             func.metadata
             for plugin in self.plugins.values()
             for func in plugin.functions.values()
             if (include_prompt and func.is_prompt) or (include_native and not func.is_prompt)
         ]
 
+    @get_list_of_function_metadata.register(dict)
+    def get_list_of_function_metadata_filters(
+        self,
+        filters: dict[
+            Literal["excluded_plugins", "included_plugins", "excluded_functions", "included_functions"], list[str]
+        ],
+    ) -> list["KernelFunctionMetadata"]:
+        """Get a list of Kernel Function Metadata based on filters.
+
+        Args:
+            filters (dict[str, list[str]]): The filters to apply to the function list.
+                The keys are:
+                    - included_plugins: A list of plugin names to include.
+                    - excluded_plugins: A list of plugin names to exclude.
+                    - included_functions: A list of function names to include.
+                    - excluded_functions: A list of function names to exclude.
+                The included and excluded parameters are mutually exclusive.
+                The function names are checked against the fully qualified name of a function.
+
+        Returns:
+            list[KernelFunctionMetadata]: The list of Kernel Function Metadata that match the filters.
+        """
+        if not self.plugins:
+            return []
+        included_plugins = filters.get("included_plugins", None)
+        excluded_plugins = filters.get("excluded_plugins", [])
+        included_functions = filters.get("included_functions", None)
+        excluded_functions = filters.get("excluded_functions", [])
+        if included_plugins and excluded_plugins:
+            raise ValueError("Cannot use both included_plugins and excluded_plugins at the same time.")
+        if included_functions and excluded_functions:
+            raise ValueError("Cannot use both included_functions and excluded_functions at the same time.")
+
+        result: list["KernelFunctionMetadata"] = []
+        for plugin_name, plugin in self.plugins.items():
+            if plugin_name in excluded_plugins or (included_plugins and plugin_name not in included_plugins):
+                continue
+            for function in plugin:
+                if function.fully_qualified_name in excluded_functions or (
+                    included_functions and function.fully_qualified_name not in included_functions
+                ):
+                    continue
+                result.append(function.metadata)
+        return result
+
     # endregion
     # region Services
 
     def select_ai_service(
         self, function: "KernelFunction", arguments: KernelArguments
     ) -> tuple[ALL_SERVICE_TYPES, PromptExecutionSettings]:
         """Uses the AI service selector to select a service for the function."""
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/kernel_pydantic.py` & `semantic_kernel-0.9.8b1/semantic_kernel/kernel_pydantic.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.9.8b1/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.9.8b1/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.9.8b1/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from semantic_kernel.planners.action_planner.action_planner import ActionPlanner
-from semantic_kernel.planners.basic_planner import BasicPlanner
+
 from semantic_kernel.planners.function_calling_stepwise_planner.function_calling_stepwise_planner import (
     FunctionCallingStepwisePlanner,
 )
 from semantic_kernel.planners.function_calling_stepwise_planner.function_calling_stepwise_planner_options import (
     FunctionCallingStepwisePlannerOptions,
 )
 from semantic_kernel.planners.function_calling_stepwise_planner.function_calling_stepwise_planner_result import (
     FunctionCallingStepwisePlannerResult,
 )
 from semantic_kernel.planners.plan import Plan
 from semantic_kernel.planners.planner_options import PlannerOptions
 from semantic_kernel.planners.sequential_planner import SequentialPlanner
-from semantic_kernel.planners.stepwise_planner import StepwisePlanner
-from semantic_kernel.planners.stepwise_planner.stepwise_planner_config import StepwisePlannerConfig
 
 __all__ = [
-    "BasicPlanner",
     "Plan",
     "SequentialPlanner",
-    "StepwisePlanner",
-    "StepwisePlannerConfig",
-    "ActionPlanner",
     "PlannerOptions",
     "FunctionCallingStepwisePlannerOptions",
     "FunctionCallingStepwisePlanner",
     "FunctionCallingStepwisePlannerResult",
 ]
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 import logging
 import os
 from copy import copy
 from typing import Any, Optional
 
 import yaml
 
+from semantic_kernel.connectors.ai.function_call_behavior import FunctionCallBehavior
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIChatPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.open_ai.services.azure_chat_completion import AzureChatCompletion
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_chat_completion import OpenAIChatCompletion
-from semantic_kernel.connectors.ai.open_ai.utils import get_function_calling_object, get_tool_call_object
+from semantic_kernel.connectors.ai.open_ai.services.utils import kernel_function_metadata_to_openai_tool_format
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.contents.function_call_content import FunctionCallContent
 from semantic_kernel.exceptions.planner_exceptions import PlannerInvalidConfigurationError
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.kernel import Kernel
 from semantic_kernel.kernel_pydantic import KernelBaseModel
@@ -121,35 +122,34 @@
             ) from exc
 
         if not isinstance(chat_completion, (OpenAIChatCompletion, AzureChatCompletion)):
             raise PlannerInvalidConfigurationError(
                 f"The service with id `{self.service_id}` is not an OpenAI based service."
             )
 
-        prompt_execution_settings: (
-            OpenAIChatPromptExecutionSettings
-        ) = self.options.execution_settings or chat_completion.get_prompt_execution_settings_class()(
-            service_id=self.service_id
+        prompt_execution_settings: OpenAIChatPromptExecutionSettings = (
+            self.options.execution_settings
+            or chat_completion.instantiate_prompt_execution_settings(service_id=self.service_id)
         )
         if self.options.max_completion_tokens:
             prompt_execution_settings.max_tokens = self.options.max_completion_tokens
-        prompt_execution_settings.max_auto_invoke_attempts = self.options.max_iterations
 
         # Clone the kernel so that we can add planner-specific plugins without affecting the original kernel instance
         cloned_kernel = copy(kernel)
         cloned_kernel.add_plugin(UserInteraction(), "UserInteraction")
 
         # Create and invoke a kernel function to generate the initial plan
         initial_plan = await self._generate_plan(question=question, kernel=cloned_kernel, arguments=arguments)
 
         chat_history_for_steps = await self._build_chat_history_for_step(
             goal=question, initial_plan=initial_plan, kernel=cloned_kernel, arguments=arguments, service=chat_completion
         )
-        prompt_execution_settings.tool_choice = "auto"
-        prompt_execution_settings.tools = get_tool_call_object(kernel, {"exclude_plugin": [self.service_id]})
+        prompt_execution_settings.function_call_behavior = FunctionCallBehavior.EnableFunctions(
+            auto_invoke=False, filters={"excluded_plugins": list(self.options.excluded_plugins)}
+        )
         for i in range(self.options.max_iterations):
             # sleep for a bit to avoid rate limiting
             if i > 0:
                 await asyncio.sleep(self.options.min_iteration_time_ms / 1000.0)  # convert ms to sec
             # For each step, request another completion to select a function for that step
             chat_history_for_steps.add_user_message(STEPWISE_USER_MESSAGE)
             chat_result = await chat_completion.complete_chat(
@@ -161,23 +161,27 @@
             chat_history_for_steps.add_message(chat_result)
 
             if not any(isinstance(item, FunctionCallContent) for item in chat_result.items):
                 chat_history_for_steps.add_user_message("That function call is invalid. Try something else!")
                 continue
 
             # Try to get the final answer out
-            if (
-                chat_result.items[0]
-                and isinstance(chat_result.items[0], FunctionCallContent)
-                and chat_result.items[0].name == USER_INTERACTION_SEND_FINAL_ANSWER
-            ):
-                args = chat_result.items[0].parse_arguments()
-                answer = args["answer"]
+            function_call_content = next(
+                (
+                    item
+                    for item in chat_result.items
+                    if isinstance(item, FunctionCallContent) and item.name == USER_INTERACTION_SEND_FINAL_ANSWER
+                ),
+                None,
+            )
+
+            if function_call_content is not None:
+                args = function_call_content.parse_arguments()
                 return FunctionCallingStepwisePlannerResult(
-                    final_answer=answer,
+                    final_answer=args.get("answer", ""),
                     chat_history=chat_history_for_steps,
                     iterations=i + 1,
                 )
 
             try:
                 await chat_completion._process_tool_calls(
                     result=chat_result, kernel=cloned_kernel, chat_history=chat_history_for_steps, arguments=arguments
@@ -237,17 +241,21 @@
         self,
         question: str,
         kernel: Kernel,
         arguments: KernelArguments,
     ) -> str:
         """Generate the plan for the given question using the kernel"""
         generate_plan_function = self._create_config_from_yaml(kernel)
-        functions_manual = get_function_calling_object(
-            kernel, {"exclude_function": [f"{self.service_id}", "sequential_planner-create_plan"]}
-        )
+        # TODO: revisit when function call behavior is finalized, and other function calling models are added
+        functions_manual = [
+            kernel_function_metadata_to_openai_tool_format(f)
+            for f in kernel.get_list_of_function_metadata(
+                {"excluded_functions": [f"{self.service_id}", "sequential_planner-create_plan"]}
+            )
+        ]
         generated_plan_args = KernelArguments(
             name_delimiter="-",
             available_functions=functions_manual,
             goal=question,
         )
         generated_plan_args.update(arguments)
         generate_plan_result = await kernel.invoke(generate_plan_function, generated_plan_args)
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) Microsoft. All rights reserved.
-
 from __future__ import annotations
 
 from typing import Any, Callable
 
 from pydantic import model_validator
 
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
+from __future__ import annotations
 
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
@@ -12,15 +13,15 @@
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class FunctionCallingStepwisePlannerResult(KernelBaseModel):
     """The result of the function calling stepwise planner"""
 
     final_answer: str = ""
-    chat_history: ChatHistory = None
+    chat_history: ChatHistory | None = None
     iterations: int = 0
 
 
 class UserInteraction:
     """The Kernel Function used to interact with the user"""
 
     @kernel_function(description="The final answer to return to the user", name="SendFinalAnswer")
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/plan.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/plan.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/planner_extensions.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/planner_options.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/planner_options.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Copyright (c) Microsoft. All rights reserved.
-
 from __future__ import annotations
 
-from typing import Callable, List, Optional, Set
+from typing import Callable
 
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class PlannerOptions(KernelBaseModel):
     """The default planner options that planners inherit from"""
 
-    excluded_plugins: Set[str] = set()
-    excluded_functions: Set[str] = set()
-    get_available_functions: Optional[Callable[["PlannerOptions", Optional[str]], List[KernelFunctionMetadata]]] = None
+    excluded_plugins: set[str] = set()
+    excluded_functions: set[str] = set()
+    get_available_functions: Callable[[PlannerOptions, str | None], list[KernelFunctionMetadata]] | None = None
     # TODO semantic_memory_config
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 from semantic_kernel.exceptions import PlannerCreatePlanError, PlannerException, PlannerInvalidGoalError
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.kernel import Kernel
 from semantic_kernel.planners.plan import Plan
 from semantic_kernel.planners.sequential_planner.sequential_planner_config import SequentialPlannerConfig
-from semantic_kernel.planners.sequential_planner.sequential_planner_extensions import (
-    SequentialPlannerKernelExtension as KernelContextExtension,
-)
+from semantic_kernel.planners.sequential_planner.sequential_planner_extensions import SequentialPlannerKernelExtension
 from semantic_kernel.planners.sequential_planner.sequential_planner_parser import SequentialPlanParser
 from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
 
 SEQUENTIAL_PLANNER_DEFAULT_DESCRIPTION = (
     "Given a request or command or goal generate a step by step plan to "
     + "fulfill the request using functions. This ability is also known as decision making and function flow"
 )
@@ -90,15 +88,15 @@
             prompt_template_config=prompt_config,
         )
 
     async def create_plan(self, goal: str) -> Plan:
         if len(goal) == 0:
             raise PlannerInvalidGoalError("The goal specified is empty")
 
-        relevant_function_manual = await KernelContextExtension.get_functions_manual(
+        relevant_function_manual = await SequentialPlannerKernelExtension.get_functions_manual(
             self._kernel, self._arguments, goal, self.config
         )
         self._arguments["available_functions"] = relevant_function_manual
         self._arguments["input"] = goal
 
         plan_result = await self._function_flow_function.invoke(self._kernel, self._arguments)
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,16 @@
     ):
         excluded_plugins = config.excluded_plugins or []
         excluded_functions = config.excluded_functions or []
         included_functions = config.included_functions or []
 
         available_functions = [
             func
-            for func in kernel.get_list_of_function_metadata()
-            if (func.plugin_name not in excluded_plugins and func.name not in excluded_functions)
+            for func in kernel.get_list_of_function_metadata({"excluded_plugins": excluded_plugins})
+            if func.name not in excluded_functions
         ]
 
         if semantic_query is None or config.relevancy_threshold is None:
             # If no semantic query is provided, return all available functions.
             # If a Memory provider has not been registered, return all available functions.
             return available_functions
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py` & `semantic_kernel-0.9.8b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/__init__.py` & `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/const.py` & `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/const.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/handlebars_prompt_template.py` & `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/handlebars_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/jinja2_prompt_template.py` & `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/jinja2_prompt_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from typing import TYPE_CHECKING, Any, Optional
 
-from jinja2 import BaseLoader, Environment, TemplateError
+from jinja2 import BaseLoader, TemplateError
+from jinja2.sandbox import ImmutableSandboxedEnvironment
 from pydantic import PrivateAttr, field_validator
 
 from semantic_kernel.exceptions import Jinja2TemplateRenderException, Jinja2TemplateSyntaxError
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.prompt_template.const import JINJA2_TEMPLATE_FORMAT_NAME
 from semantic_kernel.prompt_template.prompt_template_base import PromptTemplateBase
 from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
@@ -39,29 +40,29 @@
             configuration details required for rendering the template.
 
     Raises:
         ValueError: If the template format specified in the configuration is not 'jinja2'.
         Jinja2TemplateSyntaxError: If there is a syntax error in the Jinja2 template.
     """
 
-    _env: Environment = PrivateAttr()
+    _env: ImmutableSandboxedEnvironment = PrivateAttr()
 
     @field_validator("prompt_template_config")
     @classmethod
     def validate_template_format(cls, v: "PromptTemplateConfig") -> "PromptTemplateConfig":
         if v.template_format != JINJA2_TEMPLATE_FORMAT_NAME:
             raise ValueError(f"Invalid prompt template format: {v.template_format}. Expected: jinja2")
         return v
 
     def model_post_init(self, __context: Any) -> None:
         if not self.prompt_template_config.template:
             self._env = None
             return
         try:
-            self._env = Environment(loader=BaseLoader())
+            self._env = ImmutableSandboxedEnvironment(loader=BaseLoader())
         except TemplateError as e:
             logger.error(f"Invalid jinja2 template: {self.prompt_template_config.template}")
             raise Jinja2TemplateSyntaxError(f"Invalid jinja2 template: {self.prompt_template_config.template}") from e
 
     async def render(self, kernel: "Kernel", arguments: Optional["KernelArguments"] = None) -> str:
         """
         Using the prompt template, replace the variables with their values
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/kernel_prompt_template.py` & `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/kernel_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/prompt_template_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/prompt_template_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/prompt_template_config.py` & `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py` & `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py` & `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/prompt_template/utils/template_function_helpers.py` & `semantic_kernel-0.9.8b1/semantic_kernel/prompt_template/utils/template_function_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.9.8b1/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/services/ai_service_client_base.py` & `semantic_kernel-0.9.8b1/semantic_kernel/services/ai_service_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/services/ai_service_selector.py` & `semantic_kernel-0.9.8b1/semantic_kernel/services/ai_service_selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,12 +37,15 @@
         if func_exec_settings := getattr(function, "prompt_execution_settings", None):
             for id, settings in func_exec_settings.items():
                 if id not in execution_settings_dict:
                     execution_settings_dict[id] = settings
         if not execution_settings_dict:
             execution_settings_dict = {"default": PromptExecutionSettings()}
         for service_id, settings in execution_settings_dict.items():
-            service = kernel.get_service(service_id, type=(TextCompletionClientBase, ChatCompletionClientBase))
+            try:
+                service = kernel.get_service(service_id, type=(TextCompletionClientBase, ChatCompletionClientBase))
+            except KernelServiceNotFoundError:
+                continue
             if service:
                 service_settings = service.get_prompt_execution_settings_from_settings(settings)
                 return service, service_settings
         raise KernelServiceNotFoundError("No service found.")
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/named_arg_block.py` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/named_arg_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.9.8b1/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.9.8b1/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.9.8b1/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/utils/naming.py` & `semantic_kernel-0.9.8b1/semantic_kernel/utils/naming.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/utils/null_logger.py` & `semantic_kernel-0.9.8b1/semantic_kernel/utils/null_logger.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/utils/settings.py` & `semantic_kernel-0.9.8b1/semantic_kernel/utils/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,40 +100,27 @@
     connection_string = config.get("POSTGRES_CONNECTION_STRING", None)
 
     assert connection_string, "Postgres connection string not found in .env file"
 
     return connection_string
 
 
-def pinecone_settings_from_dot_env() -> Tuple[str, Optional[str]]:
+def pinecone_settings_from_dot_env() -> str:
     """
-    Reads the Pinecone API key and Environment from the .env file.
+    Reads the Pinecone API key from the .env file.
     Returns:
-        Tuple[str, str]: The Pinecone API key, the Pinecone Environment
+        str: The Pinecone API key
     """
 
-    api_key, environment = None, None
-    with open(".env", "r") as f:
-        lines = f.readlines()
-
-        for line in lines:
-            if line.startswith("PINECONE_API_KEY"):
-                parts = line.split("=")[1:]
-                api_key = "=".join(parts).strip().strip('"')
-                continue
-
-            if line.startswith("PINECONE_ENVIRONMENT"):
-                parts = line.split("=")[1:]
-                environment = "=".join(parts).strip().strip('"')
-                continue
+    config = dotenv_values(".env")
+    api_key = config.get("PINECONE_API_KEY", None)
 
     assert api_key, "Pinecone API key not found in .env file"
-    assert environment, "Pinecone environment not found in .env file"
 
-    return api_key, environment
+    return api_key
 
 
 def astradb_settings_from_dot_env() -> Tuple[str, Optional[str]]:
     """
     Reads the Astradb API key and Environment from the .env file.
     Returns:
         Tuple[str, str]: The Astradb API key, the Astradb Environment
@@ -360,7 +347,31 @@
     Reads the Booking Sample environment variables for the .env file.
 
     Returns:
         dict[str, str]: Booking Sample environment variables
     """
     client_id, tenant_id, client_secret = booking_sample_settings_from_dot_env()
     return {"client_id": client_id, "tenant_id": tenant_id, "client_secret": client_secret}
+
+
+def azure_container_apps_settings_from_dot_env() -> str:
+    """
+    Reads the Azure Container Apps environment variables from the .env file.
+    Returns:
+        str: Azure Container Apps pool management connection string
+    """
+    config = dotenv_values(".env")
+    connection_string = config.get("ACA_POOL_MANAGEMENT_ENDPOINT", None)
+
+    assert connection_string is not None, "Azure Container Apps connection string not found in .env file"
+
+    return connection_string
+
+
+def azure_container_apps_settings_from_dot_env_as_dict() -> dict[str, str]:
+    """
+    Reads the Azure Container Apps environment variables from the .env file.
+    Returns:
+        Dict[str, str]: Azure Container Apps environment variables
+    """
+    pool_management_endpoint = azure_container_apps_settings_from_dot_env()
+    return {"pool_management_endpoint": pool_management_endpoint}
```

### Comparing `semantic_kernel-0.9.7b1/semantic_kernel/utils/validation.py` & `semantic_kernel-0.9.8b1/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.7b1/PKG-INFO` & `semantic_kernel-0.9.8b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.9.7b1
+Version: 0.9.8b1
 Summary: Semantic Kernel Python SDK
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -41,15 +41,15 @@
 Requires-Dist: motor (>=3.3.2,<4.0.0)
 Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: numpy (>=1.24,<2.0) ; python_version == "3.8"
 Requires-Dist: numpy (>=1.25) ; python_version >= "3.9" and python_version < "3.12"
 Requires-Dist: numpy (>=1.26) ; python_version >= "3.12"
 Requires-Dist: openai (>=1.0)
 Requires-Dist: openapi_core (>=0.18,<0.20)
-Requires-Dist: pinecone-client (>=2.2.2,<3.0.0) ; extra == "pinecone" or extra == "all"
+Requires-Dist: pinecone-client (>=3.0.0) ; extra == "pinecone" or extra == "all"
 Requires-Dist: prance (>=23.6.21.0,<24.0.0.0)
 Requires-Dist: psycopg[binary,pool] (>=3.1.9,<4.0.0) ; extra == "postgres" or extra == "all"
 Requires-Dist: pyarrow (>=12.0.1,<16.0.0) ; extra == "usearch" or extra == "all"
 Requires-Dist: pybars4 (>=0.9.13,<0.10.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: pymilvus (>=2.2,<2.3) ; (python_version == "3.8") and (extra == "milvus" or extra == "all")
 Requires-Dist: pymilvus (>=2.3,<2.3.8) ; (python_version > "3.8") and (extra == "milvus" or extra == "all")
```

