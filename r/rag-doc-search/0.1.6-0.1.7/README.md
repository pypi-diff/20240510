# Comparing `tmp/rag_doc_search-0.1.6.tar.gz` & `tmp/rag_doc_search-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_doc_search-0.1.6.tar", max compression
+gzip compressed data, was "rag_doc_search-0.1.7.tar", max compression
```

## Comparing `rag_doc_search-0.1.6.tar` & `rag_doc_search-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3303 2024-04-24 12:39:35.747312 rag_doc_search-0.1.6/README.md
--rw-r--r--   0        0        0      675 2024-04-24 12:40:06.521215 rag_doc_search-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1692 2024-04-09 09:50:20.319082 rag_doc_search-0.1.6/rag_doc_search/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.064794 rag_doc_search-0.1.6/rag_doc_search/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.066001 rag_doc_search-0.1.6/rag_doc_search/src/bot_models/__init__.py
--rw-r--r--   0        0        0     2991 2024-04-15 11:57:02.681552 rag_doc_search-0.1.6/rag_doc_search/src/bot_models/azure_chatbot_model.py
--rw-r--r--   0        0        0     3265 2024-03-07 06:31:57.292277 rag_doc_search-0.1.6/rag_doc_search/src/bot_models/bedrock_chatbot_model.py
--rw-r--r--   0        0        0     4691 2024-04-24 12:39:35.748041 rag_doc_search-0.1.6/rag_doc_search/src/bot_models/chatbot_model.py
--rw-r--r--   0        0        0     2463 2024-04-09 09:50:20.320028 rag_doc_search-0.1.6/rag_doc_search/src/bot_models/openai_chatbot_model.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.069930 rag_doc_search-0.1.6/rag_doc_search/src/enums/__init__.py
--rw-r--r--   0        0        0      657 2024-04-09 09:50:20.320782 rag_doc_search-0.1.6/rag_doc_search/src/enums/provider.py
--rw-r--r--   0        0        0      530 2024-03-05 06:19:39.072113 rag_doc_search-0.1.6/rag_doc_search/src/enums/search_type.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.072542 rag_doc_search-0.1.6/rag_doc_search/src/models/__init__.py
--rw-r--r--   0        0        0      583 2024-03-05 06:19:39.074318 rag_doc_search-0.1.6/rag_doc_search/src/models/chat_response.py
--rw-r--r--   0        0        0      215 2024-03-05 06:19:39.074627 rag_doc_search-0.1.6/rag_doc_search/src/models/user_prompt.py
--rw-r--r--   0        0        0      578 2024-03-05 06:19:39.075688 rag_doc_search-0.1.6/rag_doc_search/src/prompt_templates/default_prompt_templates.py
--rw-r--r--   0        0        0        0 2024-03-05 06:19:39.047879 rag_doc_search-0.1.6/rag_doc_search/utils/__init__.py
--rw-r--r--   0        0        0      945 2024-03-07 06:31:57.296465 rag_doc_search-0.1.6/rag_doc_search/utils/callback.py
--rw-r--r--   0        0        0    13546 2024-04-24 12:39:53.863413 rag_doc_search-0.1.6/rag_doc_search/utils/config.py
--rw-r--r--   0        0        0     2318 2024-03-05 06:19:39.052900 rag_doc_search-0.1.6/rag_doc_search/utils/miscellaneous.py
--rw-r--r--   0        0        0     4292 1970-01-01 00:00:00.000000 rag_doc_search-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3303 2024-04-24 12:39:35.747312 rag_doc_search-0.1.7/README.md
+-rw-r--r--   0        0        0      675 2024-05-01 07:43:02.682900 rag_doc_search-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1692 2024-04-09 09:50:20.319082 rag_doc_search-0.1.7/rag_doc_search/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.064794 rag_doc_search-0.1.7/rag_doc_search/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.066001 rag_doc_search-0.1.7/rag_doc_search/src/bot_models/__init__.py
+-rw-r--r--   0        0        0     5362 2024-05-09 15:07:41.091294 rag_doc_search-0.1.7/rag_doc_search/src/bot_models/azure_chatbot_model.py
+-rw-r--r--   0        0        0     5551 2024-05-09 15:06:18.129697 rag_doc_search-0.1.7/rag_doc_search/src/bot_models/bedrock_chatbot_model.py
+-rw-r--r--   0        0        0     5818 2024-05-09 14:50:16.763209 rag_doc_search-0.1.7/rag_doc_search/src/bot_models/chatbot_model.py
+-rw-r--r--   0        0        0     4889 2024-05-09 15:06:27.437127 rag_doc_search-0.1.7/rag_doc_search/src/bot_models/openai_chatbot_model.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.069930 rag_doc_search-0.1.7/rag_doc_search/src/enums/__init__.py
+-rw-r--r--   0        0        0      657 2024-04-09 09:50:20.320782 rag_doc_search-0.1.7/rag_doc_search/src/enums/provider.py
+-rw-r--r--   0        0        0      530 2024-03-05 06:19:39.072113 rag_doc_search-0.1.7/rag_doc_search/src/enums/search_type.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.072542 rag_doc_search-0.1.7/rag_doc_search/src/models/__init__.py
+-rw-r--r--   0        0        0      583 2024-03-05 06:19:39.074318 rag_doc_search-0.1.7/rag_doc_search/src/models/chat_response.py
+-rw-r--r--   0        0        0      215 2024-03-05 06:19:39.074627 rag_doc_search-0.1.7/rag_doc_search/src/models/user_prompt.py
+-rw-r--r--   0        0        0      578 2024-03-05 06:19:39.075688 rag_doc_search-0.1.7/rag_doc_search/src/prompt_templates/default_prompt_templates.py
+-rw-r--r--   0        0        0        0 2024-03-05 06:19:39.047879 rag_doc_search-0.1.7/rag_doc_search/utils/__init__.py
+-rw-r--r--   0        0        0      945 2024-03-07 06:31:57.296465 rag_doc_search-0.1.7/rag_doc_search/utils/callback.py
+-rw-r--r--   0        0        0    13465 2024-05-09 14:53:30.848540 rag_doc_search-0.1.7/rag_doc_search/utils/config.py
+-rw-r--r--   0        0        0     2318 2024-03-05 06:19:39.052900 rag_doc_search-0.1.7/rag_doc_search/utils/miscellaneous.py
+-rw-r--r--   0        0        0     4292 1970-01-01 00:00:00.000000 rag_doc_search-0.1.7/PKG-INFO
```

### Comparing `rag_doc_search-0.1.6/README.md` & `rag_doc_search-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.6/pyproject.toml` & `rag_doc_search-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rag-doc-search"
-version = "0.1.6"
+version = "0.1.7"
 description = "This package offers a lightweight and straightforward solution for implementing Retrieval-augmented generation (RAG) functionality with large language models (LLMs)."
 authors = ["Harshad Kadam <harshad.kadam@sourcefuse.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 boto3 = "^1.34.55"
```

### Comparing `rag_doc_search-0.1.6/rag_doc_search/__init__.py` & `rag_doc_search-0.1.7/rag_doc_search/__init__.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.6/rag_doc_search/src/bot_models/chatbot_model.py` & `rag_doc_search-0.1.7/rag_doc_search/src/bot_models/bedrock_chatbot_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,147 @@
-from langchain.prompts import PromptTemplate
-from langchain.chains import ConversationalRetrievalChain
-from langchain.memory import ConversationBufferWindowMemory
-from langchain.callbacks.manager import AsyncCallbackManager
-from langchain.callbacks.tracers import LangChainTracer
-from langchain.schema.vectorstore import VectorStore
-from langchain.schema.embeddings import Embeddings
-from langchain.chains import RetrievalQA
+import boto3
+import os
+
+from langchain_community.embeddings.bedrock import BedrockEmbeddings
+from langchain.llms.bedrock import Bedrock
 from langchain.schema.language_model import BaseLanguageModel
+from langchain.chains import RetrievalQA
+from langchain.chains import ConversationalRetrievalChain
+from langchain.prompts import PromptTemplate
 
-from rag_doc_search.src.prompt_templates.default_prompt_templates import (
-    DEFAULT_PROMPT_TEMPLATE,
-    DEFAULT_CHAT_HISTORY_PROMPT,
-)
-from rag_doc_search.utils.miscellaneous import get_chat_history
-from rag_doc_search.utils.miscellaneous import get_logger
+from rag_doc_search.src.bot_models.chatbot_model import ChatBotModel
+from rag_doc_search import config
+from rag_doc_search.utils.callback import StreamingLLMCallbackHandler
 
 
-class ChatBotModel:
+class BedrockChatBot(ChatBotModel):
     """
-    A class representing the Base ChatBot.
+    A class representing the Bedrock ChatBot.
 
-    This class serves as an implementation of a base chatbot for diff LLM's.
+    This class serves as an implementation of a chatbot using the Bedrock.
     """
 
-    def __init__(
-        self, embeddings: Embeddings, vector_store: VectorStore, retriever_args: dict
-    ):
-        self.prompt_template = DEFAULT_PROMPT_TEMPLATE
-        self.embeddings = (embeddings,)
-        self.vector_store = vector_store
-        self.logger = get_logger()
-        self.retriever_args = retriever_args
-        self.logger.info(
-            f"search_type: {self.retriever_args.get('search_type')} \n search_args: {self.retriever_args.get('search_args')}"
-        )
-
-    def create_stream_manager(self, stream_handler, tracing) -> AsyncCallbackManager:
-        """
-        Creates and returns an instance of AsyncCallbackManager for handling asynchronous callbacks.
-
-        Parameters:
-        - `stream_handler`: The handler for managing the stream.
-        - `tracing`: A boolean indicating whether tracing is enabled.
-
-        Returns:
-        An instance of AsyncCallbackManager.
-        """
-        manager = AsyncCallbackManager([])
-        stream_manager = AsyncCallbackManager([stream_handler])
-        if tracing:
-            tracer = LangChainTracer()
-            tracer.load_default_session()
-            manager.add_handler(tracer)
-            stream_manager.add_handler(tracer)
-
-        return stream_manager
-
-    def create_qa_chain(self, cl_llm: BaseLanguageModel) -> RetrievalQA:
-        """
-        Creates and returns an instance of RetrievalQA for question-answering using a provided language model.
-
-        Parameters:
-        - `cl_llm`: An instance of LanguageModel such as OpenAI or Bedrock Model.
-
+    def __init__(self):
+        self.config = config
+        session = boto3.Session(
+            aws_access_key_id=os.environ.get("AWS_ACCESS_KEY"),
+            aws_secret_access_key=os.environ.get("AWS_SECRET_ACCESS_KEY"),
+        )
+
+        boto3_bedrock = session.client(
+            service_name="bedrock-runtime", region_name=os.environ.get("AWS_REGION")
+        )
+        self.embeddings = BedrockEmbeddings(
+            model_id=self.config.embeddings_model, client=boto3_bedrock
+        )
+        self.boto3_bedrock = boto3_bedrock
+        super().__init__(
+            embeddings=self.embeddings,
+        )
+
+    def create_qa_instance(
+        self,
+        index_or_collection_name: str = None,
+        prompt_template: PromptTemplate = None,
+        retriever_args: dict = None,
+    ) -> RetrievalQA:
+        """
+        Creates and returns an instance of RetrivalQA using Bedrock Language Model.
+
+        Args:
+        - index_or_collection_name (str, optional): Collection or index name for which vector store
+        needs to be initialized.
+        - prompt_template (PromptTemplate, optional): Custom prompt template.
+        - retriever_args (dict, optional): A dictionary containing configuration settings for retrievers.
+
+        Example:
+            retriever_args = {
+                "search_type": "similarity" | "mmr" | "similarity_score_threshold"
+                "search_args": {
+                    "k": 10,
+                    "fetch_k": 500,
+                    "lambda_mult": 0.1,
+                    "score_threshold": 0.1
+                }
+            }
         Returns:
         An instance of RetrievalQA.
         """
-        PROMPT = PromptTemplate(
-            template=self.prompt_template, input_variables=["context", "question"]
+        cl_llm: BaseLanguageModel = Bedrock(
+            model_id=self.config.llm,
+            client=self.boto3_bedrock,
+            model_kwargs={
+                "max_tokens_to_sample": self.config.llm_max_output_tokens,
+                "temperature": self.config.llm_temperature,
+            },
+        )
+        vector_store = self.config.get_vector_store(
+            embeddings=self.embeddings,
+            index_or_collection_name=index_or_collection_name,
+        )
+        retriever_args: dict = (
+            self.config.validate_and_get_retriever_arguments(retriever_args)
+            if retriever_args
+            else self.config.retriever_args
         )
 
-        qa = RetrievalQA.from_chain_type(
-            llm=cl_llm,
-            chain_type="stuff",
-            retriever=self.vector_store.as_retriever(
-                search_type=self.retriever_args.get("search_type"),
-                search_kwargs=self.retriever_args.get("search_args"),
-            ),
-            return_source_documents=True,
-            chain_type_kwargs={"prompt": PROMPT},
-        )
+        qa = self.create_qa_chain(cl_llm, vector_store, prompt_template, retriever_args)
         return qa
 
-    def create_conversational_qa_chain(
-        self, cl_llm: BaseLanguageModel
+    def create_conversational_qa_instance(
+        self,
+        stream_handler: StreamingLLMCallbackHandler,
+        index_or_collection_name: str = None,
+        prompt_template: PromptTemplate = None,
+        retriever_args: dict = None,
+        tracing: bool = False,
     ) -> ConversationalRetrievalChain:
         """
-        Creates and returns an instance of ConversationalRetrievalChain for handling conversational question-answering
-        using a provided language model.
+        Creates and returns an instance of ConversationalRetrievalChain for conversational question-answering using Bedrock Language Model.
 
         Parameters:
-        - `cl_llm`: An instance of LanguageModel such as OpenAI or Bedrock Model.
+        - `stream_handler`: An instance of StreamingLLMCallbackHandler used for handling streaming callbacks.
+        - index_or_collection_name (str, optional): Collection or index name for which vector store
+        needs to be initialized.
+        - prompt_template (PromptTemplate, optional): Custom prompt template.
+        - retriever_args (dict, optional): A dictionary containing configuration settings for retrievers.
+        - `tracing`: A boolean indicating whether tracing is enabled. Default is False.
+
+        Example:
+            retriever_args = {
+                "search_type": "similarity" | "mmr" | "similarity_score_threshold"
+                "search_args": {
+                    "k": 10,
+                    "fetch_k": 500,
+                    "lambda_mult": 0.1,
+                    "score_threshold": 0.1
+                }
+            }
 
         Returns:
-        An instance of ConversationalRetrievalChain.
+        An instance of ConversationalRetrievalChain for conversational question-answering.
         """
-        memory_chain = ConversationBufferWindowMemory(
-            memory_key="chat_history",
-            ai_prefix="Assistant",
-            return_messages=True,
-            k=0,
-            output_key="answer",
-        )
-
-        # the condense prompt for Claude
-        condense_prompt = PromptTemplate.from_template(DEFAULT_CHAT_HISTORY_PROMPT)
-
-        qa = ConversationalRetrievalChain.from_llm(
-            llm=cl_llm,
-            retriever=self.vector_store.as_retriever(
-                search_type=self.retriever_args.get("search_type"),
-                search_kwargs=self.retriever_args.get("search_args"),
-            ),
-            # return_source_documents=True,
-            memory=memory_chain,
-            get_chat_history=get_chat_history,
-            condense_question_prompt=condense_prompt,
-            chain_type="stuff",  # 'refine',
-        )
-
-        # the LLMChain prompt to get the answer. the ConversationalRetrievalChange does not expose this parameter in the constructor
-        qa.combine_docs_chain.llm_chain.prompt = PromptTemplate.from_template(
-            self.prompt_template
+        stream_manager = self.create_stream_manager(stream_handler, tracing)
+        cl_llm: BaseLanguageModel = Bedrock(
+            model_id=self.config.llm,
+            client=self.boto3_bedrock,
+            model_kwargs={
+                "max_tokens_to_sample": self.config.llm_max_output_tokens,
+                "temperature": self.config.llm_temperature,
+            },
+            streaming=True,
+            callback_manager=stream_manager,
+        )
+        vector_store = self.config.get_vector_store(
+            embeddings=self.embeddings,
+            index_or_collection_name=index_or_collection_name,
+        )
+        retriever_args: dict = (
+            self.config.validate_and_get_retriever_arguments(retriever_args)
+            if retriever_args
+            else self.config.retriever_args
+        )
+
+        qa = self.create_conversational_qa_chain(
+            cl_llm, vector_store, prompt_template, retriever_args
         )
         return qa
```

### Comparing `rag_doc_search-0.1.6/rag_doc_search/src/enums/provider.py` & `rag_doc_search-0.1.7/rag_doc_search/src/enums/provider.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.6/rag_doc_search/src/enums/search_type.py` & `rag_doc_search-0.1.7/rag_doc_search/src/enums/search_type.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.6/rag_doc_search/src/models/chat_response.py` & `rag_doc_search-0.1.7/rag_doc_search/src/models/chat_response.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.6/rag_doc_search/src/prompt_templates/default_prompt_templates.py` & `rag_doc_search-0.1.7/rag_doc_search/src/prompt_templates/default_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.6/rag_doc_search/utils/callback.py` & `rag_doc_search-0.1.7/rag_doc_search/utils/callback.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.6/rag_doc_search/utils/config.py` & `rag_doc_search-0.1.7/rag_doc_search/utils/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         match self.ai_provider:
             case AIProvider.OPENAI:
                 if not os.environ.get("OPENAI_API_KEY"):
                     raise ValueError(
                         "OPENAI_API_KEY environment variable is required for OpenAI"
                     )
-            
+
             case AIProvider.AZURE_OPENAI:
                 if not os.environ.get("AZURE_OPENAI_API_KEY"):
                     raise ValueError(
                         "AZURE_OPENAI_API_KEY environment variable is required for Azure OpenAI"
                     )
                 if not os.environ.get("AZURE_OPENAI_ENDPOINT"):
                     raise ValueError(
@@ -145,51 +145,61 @@
                 ):
                     raise ValueError(
                         "PGVECTOR_HOST, PGVECTOR_PORT, PGVECTOR_DATABASE, PGVECTOR_USER and PGVECTOR_PASSWORD environment variables are required for PgVector"
                     )
             case _:
                 self.logger.warning("Default case VectorStoreProvider")
 
-    def _validate_and_initialize_retriever_arguments(self, config_json: dict):
+    def validate_and_get_retriever_arguments(self, retriever_args: dict):
         """
         Validates and initializes the retriever arguments based on the configuration JSON.
         Also validates and initializes retriever config properties.
 
         Parameters:
-        - `config_json`: A dictionary containing configuration settings.
+        - `retriever_args`: A dictionary containing configuration settings for retrievers.
+
+        Returns:
+        A dictionary containing retriever configuration properties which can be used in vector store retriever.
 
         Raises:
         - `ValueError`: If the configuration is invalid or missing required properties.
         """
 
-        retriever_args = config_json.get("retriever", {})
         search_type_str = retriever_args.get("search_type", "")
         try:
-            self.retriever_search_type = RetrieverSearchType(search_type_str)
+            retriever_search_type = RetrieverSearchType(search_type_str)
         except ValueError:
             raise ValueError(
                 f"Invalid value for 'search_type'. Expected values: {', '.join(member.value for member in RetrieverSearchType)}"
             )
 
         search_args = retriever_args.get("search_args", {})
 
-        self.retriever_search_args_k = int(search_args.get("k", 4))
-        self.retriever_search_args_fetch_k = int(search_args.get("fetch_k", 20))
-
-        self.retriever_search_args_lambda_mult = float(
-            search_args.get("lambda_mult", 0.5)
-        )
-        if not (0 <= self.retriever_search_args_lambda_mult <= 1):
+        retriever_search_args_lambda_mult = float(search_args.get("lambda_mult", 0.5))
+        if not (0 <= retriever_search_args_lambda_mult <= 1):
             raise ValueError(
                 "Invalid lambda_mult value in config -> retriever -> search args"
             )
+        retriever_args = {
+            "k": int(search_args.get("k", 4)),
+            "fetch_k": int(search_args.get("fetch_k", 20)),
+        }
+        match retriever_search_type:
+            case RetrieverSearchType.mmr:
+                if retriever_search_args_lambda_mult > 0:
+                    retriever_args["lambda_mult"] = retriever_search_args_lambda_mult
+            case RetrieverSearchType.similarity_score_threshold:
+                retriever_args["score_threshold"] = float(
+                    search_args.get("score_threshold", 0)
+                )
 
-        self.retriever_search_args_score_threshold = float(
-            search_args.get("score_threshold", 0)
-        )
+        return {
+            "search_type": retriever_search_type.value,
+            "search_args": retriever_args,
+        }
 
     def _validate_and_initialize(self, config_json: dict):
         """
         Validates and initializes various configuration properties based on the provided JSON.
 
         Parameters:
         - `config_json`: A dictionary containing configuration settings.
@@ -198,15 +208,16 @@
         - `ValueError`: If the configuration is invalid or missing required properties.
         """
         self.logger = get_logger()
         self.logger.info("Vaidating the config")
 
         self._validate_and_initialize_ai_provider(config_json)
         self._validate_and_initialize_vector_store_provider(config_json)
-        self._validate_and_initialize_retriever_arguments(config_json)
+        # self._validate_and_initialize_retriever_arguments(config_json)
+        self.retriever_args = self.validate_and_get_retriever_arguments(config_json.get("retriever", {}))
 
         # Validate Embeddings model, llm, llm_temperature, and llm_max_output_tokens
         self.embeddings_model = config_json.get("embeddings_model", "")
         if not self.embeddings_model:
             raise ValueError("No value provided for the key 'embeddings_model'")
 
         self.llm = config_json.get("llm", "")
@@ -222,76 +233,60 @@
             raise ValueError("Invalid llm_max_output_tokens value in config")
 
         # Set the name property
         self.name = config_json.get("name", "")
 
         self.vector_store = None
 
-    def get_vector_store(self, embeddings: Embeddings) -> VectorStore:
+    def get_vector_store(
+        self, embeddings: Embeddings, index_or_collection_name: str = None
+    ) -> VectorStore:
         """
         Uses the vector store provider to create a requested provider using the required information for that vector store such as FAISS and PgVector.
 
         Parameters:
         - `embeddings`: An instance of the Embeddings class.
-
+        - index_or_collection_name (str, optional): Collection or index name for which vector store
+        needs to be initialized. If not provided, it will be used from the one which is provided in config.
         Returns:
         A VectorStore instance based on the specified provider.
 
         Raises:
         - `ValueError`: If the specified vector store provider is not supported.
         """
-        if self.vector_store is None:
-            match self.vector_store_provider:
-                case VectorStoreProvider.FAISS:
-                    self.vector_store = FAISS.load_local(
-                        folder_path=self.faiss_vector_embeddings_location,
-                        embeddings=embeddings,
-                        index_name=self.faiss_index_name,
-                        allow_dangerous_deserialization=True,
-                    )
-
-                case VectorStoreProvider.PGVector:
-                    CONNECTION_STRING = PGVector.connection_string_from_db_params(
-                        driver="psycopg2",
-                        host=os.environ.get("PGVECTOR_HOST", "localhost"),
-                        port=int(os.environ.get("PGVECTOR_PORT", "5432")),
-                        database=os.environ.get("PGVECTOR_DATABASE", "postgres"),
-                        user=os.environ.get("PGVECTOR_USER", "postgres"),
-                        password=os.environ.get("PGVECTOR_PASSWORD", "postgres"),
-                    )
-                    self.vector_store = PGVector(
-                        collection_name="city_bot",
-                        connection_string=CONNECTION_STRING,
-                        embedding_function=embeddings,
-                    )
-                    self.vector_store.as_retriever
-                case _:
-                    self.logger.warning("Default case VectorStoreProvider")
-        return self.vector_store
-
-    def get_retriever_args(self) -> dict:
-        """
-        Retrieves retriever information from the configuration.
-
-        Returns:
-        A dictionary containing retriever configuration properties which can be used in vector store retriever.
+        match self.vector_store_provider:
+            case VectorStoreProvider.FAISS:
+                index_name = (
+                    index_or_collection_name
+                    if index_or_collection_name
+                    else self.faiss_index_name
+                )
+                vector_store = FAISS.load_local(
+                    folder_path=self.faiss_vector_embeddings_location,
+                    embeddings=embeddings,
+                    index_name=index_name,
+                    allow_dangerous_deserialization=True,
+                )
 
-        Raises:
-        - `ValueError`: If the retriever configuration is invalid or missing required properties.
-        """
-        retriever_args = {
-            "k": self.retriever_search_args_k,
-            "fetch_k": self.retriever_search_args_fetch_k,
-        }
-        match self.retriever_search_type:
-            case RetrieverSearchType.mmr:
-                if self.retriever_search_args_lambda_mult <= 0:
-                    retriever_args["lambda_mult"] = self.retriever_search_args_fetch_k
-            case RetrieverSearchType.similarity_score_threshold:
-                retriever_args[
-                    "score_threshold"
-                ] = self.retriever_search_args_score_threshold
+            case VectorStoreProvider.PGVector:
+                collection_name = (
+                    index_or_collection_name
+                    if index_or_collection_name
+                    else self.collection_name
+                )
+                CONNECTION_STRING = PGVector.connection_string_from_db_params(
+                    driver="psycopg2",
+                    host=os.environ.get("PGVECTOR_HOST", "localhost"),
+                    port=int(os.environ.get("PGVECTOR_PORT", "5432")),
+                    database=os.environ.get("PGVECTOR_DATABASE", "postgres"),
+                    user=os.environ.get("PGVECTOR_USER", "postgres"),
+                    password=os.environ.get("PGVECTOR_PASSWORD", "postgres"),
+                )
+                vector_store = PGVector(
+                    collection_name=collection_name,
+                    connection_string=CONNECTION_STRING,
+                    embedding_function=embeddings,
+                )
+            case _:
+                self.logger.warning("Default case VectorStoreProvider")
+        return vector_store
 
-        return {
-            "search_type": self.retriever_search_type.value,
-            "search_args": retriever_args,
-        }
```

### Comparing `rag_doc_search-0.1.6/rag_doc_search/utils/miscellaneous.py` & `rag_doc_search-0.1.7/rag_doc_search/utils/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `rag_doc_search-0.1.6/PKG-INFO` & `rag_doc_search-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag-doc-search
-Version: 0.1.6
+Version: 0.1.7
 Summary: This package offers a lightweight and straightforward solution for implementing Retrieval-augmented generation (RAG) functionality with large language models (LLMs).
 Author: Harshad Kadam
 Author-email: harshad.kadam@sourcefuse.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

