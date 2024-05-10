# Comparing `tmp/swarmauri-0.1.97.tar.gz` & `tmp/swarmauri-0.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarmauri-0.1.97.tar", last modified: Mon Apr 29 22:27:24 2024, max compression
+gzip compressed data, was "swarmauri-0.1.98.tar", last modified: Tue Apr 30 00:13:55 2024, max compression
```

## Comparing `swarmauri-0.1.97.tar` & `swarmauri-0.1.98.tar`

### file list

```diff
@@ -1,502 +1,502 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.462099 swarmauri-0.1.97/
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-29 22:27:24.458099 swarmauri-0.1.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 22:27:10.000000 swarmauri-0.1.97/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 22:27:24.462099 swarmauri-0.1.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-29 22:27:10.000000 swarmauri-0.1.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.378098 swarmauri-0.1.97/swarmauri/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.382098 swarmauri-0.1.97/swarmauri/community/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.382098 swarmauri-0.1.97/swarmauri/community/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.382098 swarmauri-0.1.97/swarmauri/community/document_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/document_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.382098 swarmauri-0.1.97/swarmauri/community/document_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/document_stores/concrete/RedisDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/document_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.382098 swarmauri-0.1.97/swarmauri/community/retrievers/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.382098 swarmauri-0.1.97/swarmauri/community/retrievers/base/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/retrievers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.382098 swarmauri-0.1.97/swarmauri/community/retrievers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/retrievers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.382098 swarmauri-0.1.97/swarmauri/community/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.382098 swarmauri-0.1.97/swarmauri/community/tools/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/tools/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.386098 swarmauri-0.1.97/swarmauri/community/tools/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/tools/concrete/DownloadPdfTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/tools/concrete/EntityRecognitionTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/tools/concrete/GmailReadTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/tools/concrete/GmailSendTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/tools/concrete/PaCMAP.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/tools/concrete/SentimentAnalysisTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/tools/concrete/WebScrapingTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/tools/concrete/ZapierHookTool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/community/tools/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.386098 swarmauri-0.1.97/swarmauri/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.386098 swarmauri-0.1.97/swarmauri/core/agent_apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agent_apis/IAgentCommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agent_apis/IAgentRouterCRUD.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agent_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.386098 swarmauri-0.1.97/swarmauri/core/agent_factories/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agent_factories/IAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agent_factories/IExportConf.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agent_factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.386098 swarmauri-0.1.97/swarmauri/core/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agents/IAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agents/IAgentConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agents/IAgentName.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agents/IAgentParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agents/IAgentRetriever.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agents/IAgentToolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agents/IAgentVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.390098 swarmauri-0.1.97/swarmauri/core/chains/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/chains/ICallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/chains/IChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/chains/IChainFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/chains/IChainStep.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.390098 swarmauri-0.1.97/swarmauri/core/chunkers/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/chunkers/IChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/chunkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.390098 swarmauri-0.1.97/swarmauri/core/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/conversations/IConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/conversations/IMaxSize.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/conversations/ISystemContext.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.390098 swarmauri-0.1.97/swarmauri/core/distances/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/distances/IDistanceSimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.390098 swarmauri-0.1.97/swarmauri/core/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/document_stores/IDocumentRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/document_stores/IDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.390098 swarmauri-0.1.97/swarmauri/core/documents/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/documents/IDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/documents/IEmbed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/documents/IExperimentDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.390098 swarmauri-0.1.97/swarmauri/core/experiment_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/experiment_stores/IExperimentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/experiment_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.390098 swarmauri-0.1.97/swarmauri/core/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/messages/IMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.394098 swarmauri-0.1.97/swarmauri/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/metrics/IAggMeasurements.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/metrics/ICalculateMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/metrics/IMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/metrics/IThreshold.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.394098 swarmauri-0.1.97/swarmauri/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/models/IFit.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/models/IModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/models/IPredict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.394098 swarmauri-0.1.97/swarmauri/core/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/parsers/IParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.394098 swarmauri-0.1.97/swarmauri/core/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/prompts/IPrompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/prompts/ITemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.394098 swarmauri-0.1.97/swarmauri/core/swarm_apis/
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/swarm_apis/ISwarmAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/swarm_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.398098 swarmauri-0.1.97/swarmauri/core/swarms/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/swarms/ISwarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/swarms/ISwarmAgentRegistration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/swarms/ISwarmChainCRUD.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/swarms/ISwarmComponent.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/swarms/ISwarmConfigurationExporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/swarms/ISwarmFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.398098 swarmauri-0.1.97/swarmauri/core/toolkits/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/toolkits/IToolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/toolkits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.398098 swarmauri-0.1.97/swarmauri/core/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/tools/IParameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/tools/ITool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.398098 swarmauri-0.1.97/swarmauri/core/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/tracing/IChainTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/tracing/ITraceContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/tracing/ITracer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.398098 swarmauri-0.1.97/swarmauri/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/utils/ITransactional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.402098 swarmauri-0.1.97/swarmauri/core/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IAngleBetweenVectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IDecompose.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IDivergence.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IGradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IOrthogonalProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IReflect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/ISaveLoadStore.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/ISimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/ISimiliarityQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorArithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorBasisCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorLinearCombination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorNorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorRotate.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorSpan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.402098 swarmauri-0.1.97/swarmauri/core/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vectorizers/IFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vectorizers/ISaveModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vectorizers/IVectorize.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.402098 swarmauri-0.1.97/swarmauri/core/vectors/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vectors/IVector.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vectors/IVectorMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vectors/IVectorProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vectors/IVectorTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/core/vectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.402098 swarmauri-0.1.97/swarmauri/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.406098 swarmauri-0.1.97/swarmauri/experimental/chains/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/chains/ChainOrderStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/chains/ChainOrderStrategyBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/chains/ChainProcessingStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/chains/ChainProcessingStrategyBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/chains/IChainOrderStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/chains/IChainProcessingStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/chains/MatrixOrderStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/chains/MatrixProcessingStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/chains/TypeAgnosticCallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.406098 swarmauri-0.1.97/swarmauri/experimental/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/conversations/ConsensusBuildingConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/conversations/SemanticConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.410098 swarmauri-0.1.97/swarmauri/experimental/distances/
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/distances/CanberraDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/distances/ChebyshevDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/distances/HaversineDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/distances/ManhattanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/distances/MinkowskiDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/distances/SSASimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/distances/SSIVSimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/distances/ScannVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/distances/SorensenDiceDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/distances/SquaredEuclideanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.410098 swarmauri-0.1.97/swarmauri/experimental/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/document_stores/TriplesDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/document_stores/Word2VecDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.410098 swarmauri-0.1.97/swarmauri/experimental/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/models/HierarchicalAttentionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/models/SageMaker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.410098 swarmauri-0.1.97/swarmauri/experimental/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/parsers/PDFToTextParser.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.410098 swarmauri-0.1.97/swarmauri/experimental/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/tools/CypherQueryTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/tools/FileDownloaderTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/tools/LinkedInArticleTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/tools/OutlookSendMailTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/tools/SQLite3QueryTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/tools/TwitterPostTool.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.410098 swarmauri-0.1.97/swarmauri/experimental/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/tracing/RemoteTrace.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.414099 swarmauri-0.1.97/swarmauri/experimental/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/utils/ISerializable.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/utils/get_last_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/utils/log_prompt_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/utils/save_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.414099 swarmauri-0.1.97/swarmauri/experimental/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/vector_stores/TriplesDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.414099 swarmauri-0.1.97/swarmauri/experimental/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/vectorizers/DGLVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/experimental/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.414099 swarmauri-0.1.97/swarmauri/standard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.414099 swarmauri-0.1.97/swarmauri/standard/agent_factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agent_factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.414099 swarmauri-0.1.97/swarmauri/standard/agent_factories/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agent_factories/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.414099 swarmauri-0.1.97/swarmauri/standard/agent_factories/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agent_factories/concrete/AgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agent_factories/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.414099 swarmauri-0.1.97/swarmauri/standard/agents/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.418099 swarmauri-0.1.97/swarmauri/standard/agents/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/base/AgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/base/ConversationAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/base/NamedAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/base/ToolAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/base/VectorStoreAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.418099 swarmauri-0.1.97/swarmauri/standard/agents/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/concrete/ChatSwarmAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/concrete/GenerativeRagAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/concrete/RagAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/concrete/SingleCommandAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/concrete/ToolAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/agents/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.418099 swarmauri-0.1.97/swarmauri/standard/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.418099 swarmauri-0.1.97/swarmauri/standard/apis/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/apis/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.418099 swarmauri-0.1.97/swarmauri/standard/apis/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/apis/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.418099 swarmauri-0.1.97/swarmauri/standard/chains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.418099 swarmauri-0.1.97/swarmauri/standard/chains/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chains/base/ChainBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chains/base/ChainStepBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chains/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.418099 swarmauri-0.1.97/swarmauri/standard/chains/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chains/concrete/CallableChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chains/concrete/ChainStep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chains/concrete/StateChain.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chains/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.422098 swarmauri-0.1.97/swarmauri/standard/chunkers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chunkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.422098 swarmauri-0.1.97/swarmauri/standard/chunkers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chunkers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.422098 swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.422098 swarmauri-0.1.97/swarmauri/standard/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.422098 swarmauri-0.1.97/swarmauri/standard/conversations/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/base/ConversationBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/base/SystemContextBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.422098 swarmauri-0.1.97/swarmauri/standard/conversations/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/concrete/MaxSizeConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/concrete/SessionCacheConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/concrete/SharedConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/concrete/SimpleConversation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/conversations/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.422098 swarmauri-0.1.97/swarmauri/standard/distances/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/distances/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.426099 swarmauri-0.1.97/swarmauri/standard/distances/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/distances/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.426099 swarmauri-0.1.97/swarmauri/standard/distances/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/distances/concrete/ChiSquaredDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/distances/concrete/CosineDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/distances/concrete/EuclideanDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/distances/concrete/JaccardIndexDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/distances/concrete/LevenshteinDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/distances/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.426099 swarmauri-0.1.97/swarmauri/standard/document_stores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/document_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.426099 swarmauri-0.1.97/swarmauri/standard/document_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/document_stores/base/DocumentStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/document_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.426099 swarmauri-0.1.97/swarmauri/standard/document_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/document_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.426099 swarmauri-0.1.97/swarmauri/standard/documents/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.426099 swarmauri-0.1.97/swarmauri/standard/documents/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/documents/base/DocumentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/documents/base/EmbeddedBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/documents/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.426099 swarmauri-0.1.97/swarmauri/standard/documents/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/documents/concrete/Document.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/documents/concrete/EmbeddedDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/documents/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.426099 swarmauri-0.1.97/swarmauri/standard/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.426099 swarmauri-0.1.97/swarmauri/standard/exceptions/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/exceptions/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.430099 swarmauri-0.1.97/swarmauri/standard/exceptions/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/exceptions/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.430099 swarmauri-0.1.97/swarmauri/standard/messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.430099 swarmauri-0.1.97/swarmauri/standard/messages/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/messages/base/MessageBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/messages/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.430099 swarmauri-0.1.97/swarmauri/standard/messages/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/messages/concrete/AgentMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/messages/concrete/FunctionMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/messages/concrete/HumanMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/messages/concrete/SystemMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/messages/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.430099 swarmauri-0.1.97/swarmauri/standard/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.430099 swarmauri-0.1.97/swarmauri/standard/metrics/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/base/AggregateMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/base/CalculateMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/base/MetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/base/ThresholdMetricBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.434099 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/HitRateAtK.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/ImpressionAtK.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/MeanMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/StaticValueMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/ZeroMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/metrics/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.434099 swarmauri-0.1.97/swarmauri/standard/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.434099 swarmauri-0.1.97/swarmauri/standard/models/base/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/base/ModelBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.434099 swarmauri-0.1.97/swarmauri/standard/models/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/concrete/AzureGPT.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/concrete/CohereModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/concrete/GroqModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/concrete/GroqToolModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/concrete/MistralModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/concrete/MistralToolModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/concrete/OpenAIImageGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/concrete/OpenAIModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/concrete/OpenAIToolModel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/models/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.434099 swarmauri-0.1.97/swarmauri/standard/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.434099 swarmauri-0.1.97/swarmauri/standard/parsers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.438099 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/CSVParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/MarkdownParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/PythonParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/RegExParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/TFIDFParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/TextBlobNounParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/URLExtractorParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/XMLParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/parsers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.438099 swarmauri-0.1.97/swarmauri/standard/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.438099 swarmauri-0.1.97/swarmauri/standard/prompts/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/prompts/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.438099 swarmauri-0.1.97/swarmauri/standard/prompts/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/prompts/concrete/Prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/prompts/concrete/PromptGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/prompts/concrete/PromptTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/prompts/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.438099 swarmauri-0.1.97/swarmauri/standard/states/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/states/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/states/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/states/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/states/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/swarms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/swarms/base/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/swarms/base/SwarmComponentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/swarms/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/swarms/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/swarms/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/toolkits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/toolkits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/toolkits/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/toolkits/base/ToolkitBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/toolkits/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/toolkits/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/toolkits/concrete/Toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/toolkits/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/tools/base/
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tools/base/ToolBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tools/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/tools/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tools/concrete/AdditionTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tools/concrete/Parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tools/concrete/TestTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tools/concrete/WeatherTool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tools/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.442099 swarmauri-0.1.97/swarmauri/standard/tracing/base/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tracing/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.446099 swarmauri-0.1.97/swarmauri/standard/tracing/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tracing/concrete/CallableTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tracing/concrete/ChainTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tracing/concrete/SimpleTraceContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tracing/concrete/SimpleTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tracing/concrete/TracedVariable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tracing/concrete/VariableTracer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/tracing/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.446099 swarmauri-0.1.97/swarmauri/standard/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/utils/get_class_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/utils/load_documents_from_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.446099 swarmauri-0.1.97/swarmauri/standard/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vector_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.446099 swarmauri-0.1.97/swarmauri/standard/vector_stores/base/
--rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vector_stores/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.446099 swarmauri-0.1.97/swarmauri/standard/vector_stores/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vector_stores/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.446099 swarmauri-0.1.97/swarmauri/standard/vectorizers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectorizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.446099 swarmauri-0.1.97/swarmauri/standard/vectorizers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectorizers/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.450099 swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.450099 swarmauri-0.1.97/swarmauri/standard/vectors/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.450099 swarmauri-0.1.97/swarmauri/standard/vectors/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectors/base/VectorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectors/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.450099 swarmauri-0.1.97/swarmauri/standard/vectors/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectors/concrete/SimpleVector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectors/concrete/VectorProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 22:27:10.000000 swarmauri-0.1.97/swarmauri/standard/vectors/concrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:27:24.450099 swarmauri-0.1.97/swarmauri.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-29 22:27:24.000000 swarmauri-0.1.97/swarmauri.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18264 2024-04-29 22:27:24.000000 swarmauri-0.1.97/swarmauri.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:27:24.000000 swarmauri-0.1.97/swarmauri.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-29 22:27:24.000000 swarmauri-0.1.97/swarmauri.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 22:27:24.000000 swarmauri-0.1.97/swarmauri.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.240254 swarmauri-0.1.98/
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-30 00:13:55.240254 swarmauri-0.1.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-30 00:13:41.000000 swarmauri-0.1.98/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 00:13:55.240254 swarmauri-0.1.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-30 00:13:41.000000 swarmauri-0.1.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.164255 swarmauri-0.1.98/swarmauri/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.164255 swarmauri-0.1.98/swarmauri/community/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.164255 swarmauri-0.1.98/swarmauri/community/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.164255 swarmauri-0.1.98/swarmauri/community/document_stores/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/document_stores/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.164255 swarmauri-0.1.98/swarmauri/community/document_stores/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/document_stores/concrete/RedisDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/document_stores/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.164255 swarmauri-0.1.98/swarmauri/community/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.164255 swarmauri-0.1.98/swarmauri/community/retrievers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/retrievers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.168255 swarmauri-0.1.98/swarmauri/community/retrievers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/retrievers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.168255 swarmauri-0.1.98/swarmauri/community/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.168255 swarmauri-0.1.98/swarmauri/community/tools/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/tools/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.168255 swarmauri-0.1.98/swarmauri/community/tools/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/tools/concrete/DownloadPdfTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/tools/concrete/EntityRecognitionTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/tools/concrete/GmailReadTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/tools/concrete/GmailSendTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/tools/concrete/PaCMAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/tools/concrete/SentimentAnalysisTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/tools/concrete/WebScrapingTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/tools/concrete/ZapierHookTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/community/tools/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.168255 swarmauri-0.1.98/swarmauri/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.168255 swarmauri-0.1.98/swarmauri/core/agent_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agent_apis/IAgentCommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agent_apis/IAgentRouterCRUD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agent_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.168255 swarmauri-0.1.98/swarmauri/core/agent_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agent_factories/IAgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agent_factories/IExportConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agent_factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.172255 swarmauri-0.1.98/swarmauri/core/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agents/IAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agents/IAgentConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agents/IAgentName.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agents/IAgentParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agents/IAgentRetriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agents/IAgentToolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agents/IAgentVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.172255 swarmauri-0.1.98/swarmauri/core/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/chains/ICallableChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/chains/IChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/chains/IChainFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/chains/IChainStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.172255 swarmauri-0.1.98/swarmauri/core/chunkers/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/chunkers/IChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/chunkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.172255 swarmauri-0.1.98/swarmauri/core/conversations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/conversations/IConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/conversations/IMaxSize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/conversations/ISystemContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.172255 swarmauri-0.1.98/swarmauri/core/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/distances/IDistanceSimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/distances/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.172255 swarmauri-0.1.98/swarmauri/core/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/document_stores/IDocumentRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/document_stores/IDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.176255 swarmauri-0.1.98/swarmauri/core/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/documents/IDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/documents/IEmbed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/documents/IExperimentDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.176255 swarmauri-0.1.98/swarmauri/core/experiment_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/experiment_stores/IExperimentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/experiment_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.176255 swarmauri-0.1.98/swarmauri/core/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/messages/IMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.176255 swarmauri-0.1.98/swarmauri/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/metrics/IAggMeasurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/metrics/ICalculateMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/metrics/IMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/metrics/IThreshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.176255 swarmauri-0.1.98/swarmauri/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/models/IFit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/models/IModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/models/IPredict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.176255 swarmauri-0.1.98/swarmauri/core/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/parsers/IParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.176255 swarmauri-0.1.98/swarmauri/core/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/prompts/IPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/prompts/ITemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/prompts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.176255 swarmauri-0.1.98/swarmauri/core/swarm_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/swarm_apis/ISwarmAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/swarm_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.180255 swarmauri-0.1.98/swarmauri/core/swarms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/swarms/ISwarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/swarms/ISwarmAgentRegistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/swarms/ISwarmChainCRUD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/swarms/ISwarmComponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/swarms/ISwarmConfigurationExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/swarms/ISwarmFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.180255 swarmauri-0.1.98/swarmauri/core/toolkits/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/toolkits/IToolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/toolkits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.180255 swarmauri-0.1.98/swarmauri/core/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/tools/IParameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/tools/ITool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.180255 swarmauri-0.1.98/swarmauri/core/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/tracing/IChainTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/tracing/ITraceContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/tracing/ITracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.180255 swarmauri-0.1.98/swarmauri/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/utils/ITransactional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.184255 swarmauri-0.1.98/swarmauri/core/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IAngleBetweenVectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IDecompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IDivergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IGradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IOrthogonalProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IReflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/ISaveLoadStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/ISimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/ISimiliarityQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorArithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorBasisCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorLinearCombination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorNorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorRotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorSpan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vector_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.184255 swarmauri-0.1.98/swarmauri/core/vectorizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vectorizers/IFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vectorizers/ISaveModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vectorizers/IVectorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vectorizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.188255 swarmauri-0.1.98/swarmauri/core/vectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vectors/IVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vectors/IVectorMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vectors/IVectorProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vectors/IVectorTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/core/vectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.188255 swarmauri-0.1.98/swarmauri/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.188255 swarmauri-0.1.98/swarmauri/experimental/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/chains/ChainOrderStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/chains/ChainOrderStrategyBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/chains/ChainProcessingStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/chains/ChainProcessingStrategyBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/chains/IChainOrderStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/chains/IChainProcessingStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/chains/MatrixOrderStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/chains/MatrixProcessingStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/chains/TypeAgnosticCallableChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.188255 swarmauri-0.1.98/swarmauri/experimental/conversations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/conversations/ConsensusBuildingConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/conversations/SemanticConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.192255 swarmauri-0.1.98/swarmauri/experimental/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/distances/CanberraDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/distances/ChebyshevDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/distances/HaversineDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/distances/ManhattanDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/distances/MinkowskiDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/distances/SSASimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/distances/SSIVSimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/distances/ScannVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/distances/SorensenDiceDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/distances/SquaredEuclideanDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/distances/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.192255 swarmauri-0.1.98/swarmauri/experimental/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/document_stores/TriplesDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/document_stores/Word2VecDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.192255 swarmauri-0.1.98/swarmauri/experimental/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/models/HierarchicalAttentionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/models/SageMaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.192255 swarmauri-0.1.98/swarmauri/experimental/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/parsers/PDFToTextParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.192255 swarmauri-0.1.98/swarmauri/experimental/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/tools/CypherQueryTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/tools/FileDownloaderTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/tools/LinkedInArticleTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/tools/OutlookSendMailTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/tools/SQLite3QueryTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/tools/TwitterPostTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.192255 swarmauri-0.1.98/swarmauri/experimental/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/tracing/RemoteTrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.196255 swarmauri-0.1.98/swarmauri/experimental/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/utils/ISerializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/utils/get_last_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/utils/log_prompt_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/utils/save_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.196255 swarmauri-0.1.98/swarmauri/experimental/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/vector_stores/TriplesDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/vector_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.196255 swarmauri-0.1.98/swarmauri/experimental/vectorizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/vectorizers/DGLVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/experimental/vectorizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.196255 swarmauri-0.1.98/swarmauri/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.196255 swarmauri-0.1.98/swarmauri/standard/agent_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agent_factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.196255 swarmauri-0.1.98/swarmauri/standard/agent_factories/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agent_factories/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.196255 swarmauri-0.1.98/swarmauri/standard/agent_factories/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agent_factories/concrete/AgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agent_factories/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.196255 swarmauri-0.1.98/swarmauri/standard/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.196255 swarmauri-0.1.98/swarmauri/standard/agents/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/base/AgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/base/ConversationAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/base/NamedAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/base/ToolAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/base/VectorStoreAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.200255 swarmauri-0.1.98/swarmauri/standard/agents/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/concrete/ChatSwarmAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/concrete/GenerativeRagAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/concrete/RagAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/concrete/SingleCommandAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/concrete/ToolAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/agents/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.200255 swarmauri-0.1.98/swarmauri/standard/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.200255 swarmauri-0.1.98/swarmauri/standard/apis/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/apis/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.200255 swarmauri-0.1.98/swarmauri/standard/apis/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/apis/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.200255 swarmauri-0.1.98/swarmauri/standard/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.200255 swarmauri-0.1.98/swarmauri/standard/chains/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chains/base/ChainBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chains/base/ChainStepBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chains/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.200255 swarmauri-0.1.98/swarmauri/standard/chains/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chains/concrete/CallableChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chains/concrete/ChainStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chains/concrete/StateChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chains/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.200255 swarmauri-0.1.98/swarmauri/standard/chunkers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chunkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.200255 swarmauri-0.1.98/swarmauri/standard/chunkers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chunkers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.204254 swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.204254 swarmauri-0.1.98/swarmauri/standard/conversations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.204254 swarmauri-0.1.98/swarmauri/standard/conversations/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/base/ConversationBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/base/SystemContextBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.204254 swarmauri-0.1.98/swarmauri/standard/conversations/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/concrete/MaxSizeConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/concrete/SessionCacheConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/concrete/SharedConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/concrete/SimpleConversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/conversations/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.204254 swarmauri-0.1.98/swarmauri/standard/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/distances/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.204254 swarmauri-0.1.98/swarmauri/standard/distances/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/distances/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/distances/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/distances/concrete/ChiSquaredDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/distances/concrete/CosineDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/distances/concrete/EuclideanDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/distances/concrete/JaccardIndexDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/distances/concrete/LevenshteinDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/distances/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/document_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/document_stores/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/document_stores/base/DocumentStoreBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/document_stores/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/document_stores/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/document_stores/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/documents/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/documents/base/DocumentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/documents/base/EmbeddedBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/documents/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/documents/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/documents/concrete/Document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/documents/concrete/EmbeddedDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/documents/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/exceptions/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/exceptions/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/exceptions/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/exceptions/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.208255 swarmauri-0.1.98/swarmauri/standard/messages/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/messages/base/MessageBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/messages/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.212255 swarmauri-0.1.98/swarmauri/standard/messages/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/messages/concrete/AgentMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/messages/concrete/FunctionMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/messages/concrete/HumanMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/messages/concrete/SystemMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/messages/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.212255 swarmauri-0.1.98/swarmauri/standard/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.212255 swarmauri-0.1.98/swarmauri/standard/metrics/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/base/AggregateMetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/base/CalculateMetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/base/MetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/base/ThresholdMetricBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.212255 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/HitRateAtK.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/ImpressionAtK.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/MeanMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/StaticValueMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/ZeroMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/metrics/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.212255 swarmauri-0.1.98/swarmauri/standard/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.212255 swarmauri-0.1.98/swarmauri/standard/models/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/base/ModelBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.216255 swarmauri-0.1.98/swarmauri/standard/models/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/concrete/AzureGPT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/concrete/CohereModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/concrete/GroqModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/concrete/GroqToolModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/concrete/MistralModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/concrete/MistralToolModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/concrete/OpenAIImageGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/concrete/OpenAIModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/concrete/OpenAIToolModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/models/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.216255 swarmauri-0.1.98/swarmauri/standard/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.216255 swarmauri-0.1.98/swarmauri/standard/parsers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/CSVParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/MarkdownParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/PythonParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/RegExParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/TFIDFParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/TextBlobNounParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/URLExtractorParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/XMLParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/parsers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/prompts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/prompts/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/prompts/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/prompts/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/prompts/concrete/Prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/prompts/concrete/PromptGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/prompts/concrete/PromptTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/prompts/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/states/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/states/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/states/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/states/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/states/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/swarms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/swarms/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/swarms/base/SwarmComponentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/swarms/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/swarms/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/swarms/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/toolkits/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/toolkits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/toolkits/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/toolkits/base/ToolkitBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/toolkits/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/toolkits/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/toolkits/concrete/Toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/toolkits/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.220255 swarmauri-0.1.98/swarmauri/standard/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.224254 swarmauri-0.1.98/swarmauri/standard/tools/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tools/base/ToolBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tools/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.224254 swarmauri-0.1.98/swarmauri/standard/tools/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tools/concrete/AdditionTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tools/concrete/Parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tools/concrete/TestTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tools/concrete/WeatherTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tools/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.224254 swarmauri-0.1.98/swarmauri/standard/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.224254 swarmauri-0.1.98/swarmauri/standard/tracing/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tracing/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.224254 swarmauri-0.1.98/swarmauri/standard/tracing/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tracing/concrete/CallableTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tracing/concrete/ChainTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tracing/concrete/SimpleTraceContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tracing/concrete/SimpleTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tracing/concrete/TracedVariable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tracing/concrete/VariableTracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/tracing/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.224254 swarmauri-0.1.98/swarmauri/standard/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/utils/get_class_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/utils/load_documents_from_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.224254 swarmauri-0.1.98/swarmauri/standard/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vector_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.224254 swarmauri-0.1.98/swarmauri/standard/vector_stores/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vector_stores/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.228255 swarmauri-0.1.98/swarmauri/standard/vector_stores/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vector_stores/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.228255 swarmauri-0.1.98/swarmauri/standard/vectorizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectorizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.228255 swarmauri-0.1.98/swarmauri/standard/vectorizers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectorizers/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.228255 swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.228255 swarmauri-0.1.98/swarmauri/standard/vectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.228255 swarmauri-0.1.98/swarmauri/standard/vectors/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectors/base/VectorBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectors/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.228255 swarmauri-0.1.98/swarmauri/standard/vectors/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectors/concrete/SimpleVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectors/concrete/VectorProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:13:41.000000 swarmauri-0.1.98/swarmauri/standard/vectors/concrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:13:55.228255 swarmauri-0.1.98/swarmauri.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-30 00:13:55.000000 swarmauri-0.1.98/swarmauri.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18264 2024-04-30 00:13:55.000000 swarmauri-0.1.98/swarmauri.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:13:55.000000 swarmauri-0.1.98/swarmauri.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-30 00:13:55.000000 swarmauri-0.1.98/swarmauri.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 00:13:55.000000 swarmauri-0.1.98/swarmauri.egg-info/top_level.txt
```

### Comparing `swarmauri-0.1.97/PKG-INFO` & `swarmauri-0.1.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri
-Version: 0.1.97
+Version: 0.1.98
 Summary: This repository includes core interfaces, standard ABCs and concrete references, third party plugins, and experimental modules for the swarmaURI framework.
 Home-page: http://github.com/swarmauri/swarmauri-sdk
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `swarmauri-0.1.97/README.md` & `swarmauri-0.1.98/README.md`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/setup.py` & `swarmauri-0.1.98/setup.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/community/document_stores/concrete/RedisDocumentStore.py` & `swarmauri-0.1.98/swarmauri/community/document_stores/concrete/RedisDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py` & `swarmauri-0.1.98/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/community/tools/concrete/DownloadPdfTool.py` & `swarmauri-0.1.98/swarmauri/community/tools/concrete/DownloadPdfTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/community/tools/concrete/EntityRecognitionTool.py` & `swarmauri-0.1.98/swarmauri/community/tools/concrete/EntityRecognitionTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/community/tools/concrete/GmailReadTool.py` & `swarmauri-0.1.98/swarmauri/community/tools/concrete/GmailReadTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/community/tools/concrete/GmailSendTool.py` & `swarmauri-0.1.98/swarmauri/community/tools/concrete/GmailSendTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/community/tools/concrete/PaCMAP.py` & `swarmauri-0.1.98/swarmauri/community/tools/concrete/PaCMAP.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/community/tools/concrete/SentimentAnalysisTool.py` & `swarmauri-0.1.98/swarmauri/community/tools/concrete/SentimentAnalysisTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/community/tools/concrete/WebScrapingTool.py` & `swarmauri-0.1.98/swarmauri/community/tools/concrete/WebScrapingTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/community/tools/concrete/ZapierHookTool.py` & `swarmauri-0.1.98/swarmauri/community/tools/concrete/ZapierHookTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/agent_apis/IAgentCommands.py` & `swarmauri-0.1.98/swarmauri/core/agent_apis/IAgentCommands.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/agent_apis/IAgentRouterCRUD.py` & `swarmauri-0.1.98/swarmauri/core/agent_apis/IAgentRouterCRUD.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/agent_factories/IAgentFactory.py` & `swarmauri-0.1.98/swarmauri/core/agent_factories/IAgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/agent_factories/IExportConf.py` & `swarmauri-0.1.98/swarmauri/core/agent_factories/IExportConf.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/agents/IAgent.py` & `swarmauri-0.1.98/swarmauri/core/agents/IAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/chains/IChain.py` & `swarmauri-0.1.98/swarmauri/core/chains/IChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/chains/IChainFactory.py` & `swarmauri-0.1.98/swarmauri/core/chains/IChainFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/chains/IChainStep.py` & `swarmauri-0.1.98/swarmauri/core/chains/IChainStep.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/conversations/IConversation.py` & `swarmauri-0.1.98/swarmauri/core/conversations/IConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/conversations/ISystemContext.py` & `swarmauri-0.1.98/swarmauri/core/conversations/ISystemContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/distances/IDistanceSimilarity.py` & `swarmauri-0.1.98/swarmauri/core/distances/IDistanceSimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/document_stores/IDocumentRetrieve.py` & `swarmauri-0.1.98/swarmauri/core/document_stores/IDocumentRetrieve.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/document_stores/IDocumentStore.py` & `swarmauri-0.1.98/swarmauri/core/document_stores/IDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/documents/IDocument.py` & `swarmauri-0.1.98/swarmauri/core/documents/IDocument.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/documents/IExperimentDocument.py` & `swarmauri-0.1.98/swarmauri/core/documents/IExperimentDocument.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/experiment_stores/IExperimentStore.py` & `swarmauri-0.1.98/swarmauri/core/experiment_stores/IExperimentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/experiment_stores/__init__.py` & `swarmauri-0.1.98/swarmauri/core/experiment_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/messages/IMessage.py` & `swarmauri-0.1.98/swarmauri/core/messages/IMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/metrics/IAggMeasurements.py` & `swarmauri-0.1.98/swarmauri/core/metrics/IAggMeasurements.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/metrics/ICalculateMetric.py` & `swarmauri-0.1.98/swarmauri/core/metrics/ICalculateMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/metrics/IMetric.py` & `swarmauri-0.1.98/swarmauri/core/metrics/IMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/parsers/IParser.py` & `swarmauri-0.1.98/swarmauri/core/parsers/IParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/prompts/ITemplate.py` & `swarmauri-0.1.98/swarmauri/core/prompts/ITemplate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py` & `swarmauri-0.1.98/swarmauri/core/swarm_apis/IAgentRegistrationAPI.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/swarm_apis/ISwarmAPI.py` & `swarmauri-0.1.98/swarmauri/core/swarm_apis/ISwarmAPI.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/swarms/ISwarm.py` & `swarmauri-0.1.98/swarmauri/core/swarms/ISwarm.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/swarms/ISwarmAgentRegistration.py` & `swarmauri-0.1.98/swarmauri/core/swarms/ISwarmAgentRegistration.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/swarms/ISwarmChainCRUD.py` & `swarmauri-0.1.98/swarmauri/core/swarms/ISwarmChainCRUD.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/swarms/ISwarmConfigurationExporter.py` & `swarmauri-0.1.98/swarmauri/core/swarms/ISwarmConfigurationExporter.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/swarms/ISwarmFactory.py` & `swarmauri-0.1.98/swarmauri/core/swarms/ISwarmFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/toolkits/IToolkit.py` & `swarmauri-0.1.98/swarmauri/core/toolkits/IToolkit.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/tools/IParameter.py` & `swarmauri-0.1.98/swarmauri/core/tools/IParameter.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/tracing/IChainTracer.py` & `swarmauri-0.1.98/swarmauri/core/tracing/IChainTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/tracing/ITraceContext.py` & `swarmauri-0.1.98/swarmauri/core/tracing/ITraceContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/tracing/ITracer.py` & `swarmauri-0.1.98/swarmauri/core/tracing/ITracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/utils/ITransactional.py` & `swarmauri-0.1.98/swarmauri/core/utils/ITransactional.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IAngleBetweenVectors.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IAngleBetweenVectors.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IDecompose.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IDecompose.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IDivergence.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IDivergence.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IGradient.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IGradient.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IOrthogonalProject.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IOrthogonalProject.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IProject.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IProject.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IReflect.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IReflect.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/ISaveLoadStore.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/ISaveLoadStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/ISimilarity.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/ISimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/ISimiliarityQuery.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/ISimiliarityQuery.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorArithmetic.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorArithmetic.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorBasisCheck.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorBasisCheck.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorLinearCombination.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorLinearCombination.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorNorm.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorNorm.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorRetrieve.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorRetrieve.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorRotate.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorRotate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorSpan.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorSpan.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vector_stores/IVectorStore.py` & `swarmauri-0.1.98/swarmauri/core/vector_stores/IVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vectorizers/ISaveModel.py` & `swarmauri-0.1.98/swarmauri/core/vectorizers/ISaveModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vectorizers/IVectorize.py` & `swarmauri-0.1.98/swarmauri/core/vectorizers/IVectorize.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vectors/IVector.py` & `swarmauri-0.1.98/swarmauri/core/vectors/IVector.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vectors/IVectorMeta.py` & `swarmauri-0.1.98/swarmauri/core/vectors/IVectorMeta.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vectors/IVectorProduct.py` & `swarmauri-0.1.98/swarmauri/core/vectors/IVectorProduct.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/core/vectors/IVectorTransform.py` & `swarmauri-0.1.98/swarmauri/core/vectors/IVectorTransform.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/chains/ChainOrderStrategy.py` & `swarmauri-0.1.98/swarmauri/experimental/chains/ChainOrderStrategy.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/chains/ChainProcessingStrategy.py` & `swarmauri-0.1.98/swarmauri/experimental/chains/ChainProcessingStrategy.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/chains/ChainProcessingStrategyBase.py` & `swarmauri-0.1.98/swarmauri/experimental/chains/ChainProcessingStrategyBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/chains/IChainProcessingStrategy.py` & `swarmauri-0.1.98/swarmauri/experimental/chains/IChainProcessingStrategy.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/chains/MatrixOrderStrategy.py` & `swarmauri-0.1.98/swarmauri/experimental/chains/MatrixOrderStrategy.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/chains/MatrixProcessingStrategy.py` & `swarmauri-0.1.98/swarmauri/experimental/chains/MatrixProcessingStrategy.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/chains/TypeAgnosticCallableChain.py` & `swarmauri-0.1.98/swarmauri/experimental/chains/TypeAgnosticCallableChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/conversations/ConsensusBuildingConversation.py` & `swarmauri-0.1.98/swarmauri/experimental/conversations/ConsensusBuildingConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/conversations/SemanticConversation.py` & `swarmauri-0.1.98/swarmauri/experimental/conversations/SemanticConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/distances/CanberraDistance.py` & `swarmauri-0.1.98/swarmauri/experimental/distances/CanberraDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/distances/ChebyshevDistance.py` & `swarmauri-0.1.98/swarmauri/experimental/distances/ChebyshevDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/distances/HaversineDistance.py` & `swarmauri-0.1.98/swarmauri/experimental/distances/HaversineDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/distances/ManhattanDistance.py` & `swarmauri-0.1.98/swarmauri/experimental/distances/ManhattanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/distances/MinkowskiDistance.py` & `swarmauri-0.1.98/swarmauri/experimental/distances/MinkowskiDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/distances/SSASimilarity.py` & `swarmauri-0.1.98/swarmauri/experimental/distances/SSASimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/distances/SSIVSimilarity.py` & `swarmauri-0.1.98/swarmauri/experimental/distances/SSIVSimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/distances/ScannVectorStore.py` & `swarmauri-0.1.98/swarmauri/experimental/distances/ScannVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/distances/SorensenDiceDistance.py` & `swarmauri-0.1.98/swarmauri/experimental/distances/SorensenDiceDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/distances/SquaredEuclideanDistance.py` & `swarmauri-0.1.98/swarmauri/experimental/distances/SquaredEuclideanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/document_stores/TriplesDocumentStore.py` & `swarmauri-0.1.98/swarmauri/experimental/document_stores/TriplesDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/document_stores/Word2VecDocumentStore.py` & `swarmauri-0.1.98/swarmauri/experimental/document_stores/Word2VecDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/models/HierarchicalAttentionModel.py` & `swarmauri-0.1.98/swarmauri/experimental/models/HierarchicalAttentionModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/models/SageMaker.py` & `swarmauri-0.1.98/swarmauri/experimental/models/SageMaker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/parsers/PDFToTextParser.py` & `swarmauri-0.1.98/swarmauri/experimental/parsers/PDFToTextParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/tools/CypherQueryTool.py` & `swarmauri-0.1.98/swarmauri/experimental/tools/CypherQueryTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/tools/FileDownloaderTool.py` & `swarmauri-0.1.98/swarmauri/experimental/tools/FileDownloaderTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/tools/LinkedInArticleTool.py` & `swarmauri-0.1.98/swarmauri/experimental/tools/LinkedInArticleTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/tools/OutlookSendMailTool.py` & `swarmauri-0.1.98/swarmauri/experimental/tools/OutlookSendMailTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/tools/SQLite3QueryTool.py` & `swarmauri-0.1.98/swarmauri/experimental/tools/SQLite3QueryTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/tools/TwitterPostTool.py` & `swarmauri-0.1.98/swarmauri/experimental/tools/TwitterPostTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/tracing/RemoteTrace.py` & `swarmauri-0.1.98/swarmauri/experimental/tracing/RemoteTrace.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/utils/ISerializable.py` & `swarmauri-0.1.98/swarmauri/experimental/utils/ISerializable.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/utils/get_last_frame.py` & `swarmauri-0.1.98/swarmauri/experimental/utils/get_last_frame.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/utils/log_prompt_response.py` & `swarmauri-0.1.98/swarmauri/experimental/utils/log_prompt_response.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/utils/save_schema.py` & `swarmauri-0.1.98/swarmauri/experimental/utils/save_schema.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/vector_stores/TriplesDocumentStore.py` & `swarmauri-0.1.98/swarmauri/experimental/vector_stores/TriplesDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py` & `swarmauri-0.1.98/swarmauri/experimental/vector_stores/Word2VecDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/experimental/vectorizers/DGLVectorizer.py` & `swarmauri-0.1.98/swarmauri/experimental/vectorizers/DGLVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agent_factories/concrete/AgentFactory.py` & `swarmauri-0.1.98/swarmauri/standard/agent_factories/concrete/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py` & `swarmauri-0.1.98/swarmauri/standard/agent_factories/concrete/ConfDrivenAgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py` & `swarmauri-0.1.98/swarmauri/standard/agent_factories/concrete/ReflectiveAgentFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/base/AgentBase.py` & `swarmauri-0.1.98/swarmauri/standard/agents/base/AgentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/base/ConversationAgentBase.py` & `swarmauri-0.1.98/swarmauri/standard/agents/base/ConversationAgentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/base/NamedAgentBase.py` & `swarmauri-0.1.98/swarmauri/standard/agents/base/NamedAgentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/base/ToolAgentBase.py` & `swarmauri-0.1.98/swarmauri/standard/agents/base/ToolAgentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/base/VectorStoreAgentBase.py` & `swarmauri-0.1.98/swarmauri/standard/agents/base/VectorStoreAgentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/concrete/ChatSwarmAgent.py` & `swarmauri-0.1.98/swarmauri/standard/agents/concrete/ChatSwarmAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/concrete/GenerativeRagAgent.py` & `swarmauri-0.1.98/swarmauri/standard/agents/concrete/GenerativeRagAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py` & `swarmauri-0.1.98/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py` & `swarmauri-0.1.98/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/concrete/RagAgent.py` & `swarmauri-0.1.98/swarmauri/standard/agents/concrete/RagAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py` & `swarmauri-0.1.98/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/concrete/SingleCommandAgent.py` & `swarmauri-0.1.98/swarmauri/standard/agents/concrete/SingleCommandAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/agents/concrete/ToolAgent.py` & `swarmauri-0.1.98/swarmauri/standard/agents/concrete/ToolAgent.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/chains/base/ChainBase.py` & `swarmauri-0.1.98/swarmauri/standard/chains/base/ChainBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/chains/base/ChainStepBase.py` & `swarmauri-0.1.98/swarmauri/standard/chains/base/ChainStepBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/chains/concrete/CallableChain.py` & `swarmauri-0.1.98/swarmauri/standard/chains/concrete/CallableChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/chains/concrete/ChainStep.py` & `swarmauri-0.1.98/swarmauri/standard/chains/concrete/ChainStep.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/chains/concrete/StateChain.py` & `swarmauri-0.1.98/swarmauri/standard/chains/concrete/StateChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py` & `swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py` & `swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py` & `swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py` & `swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py` & `swarmauri-0.1.98/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/conversations/base/ConversationBase.py` & `swarmauri-0.1.98/swarmauri/standard/conversations/base/ConversationBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/conversations/base/SystemContextBase.py` & `swarmauri-0.1.98/swarmauri/standard/conversations/base/SystemContextBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py` & `swarmauri-0.1.98/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py` & `swarmauri-0.1.98/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/conversations/concrete/MaxSizeConversation.py` & `swarmauri-0.1.98/swarmauri/standard/conversations/concrete/MaxSizeConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py` & `swarmauri-0.1.98/swarmauri/standard/conversations/concrete/MaxSystemContextConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/conversations/concrete/SessionCacheConversation.py` & `swarmauri-0.1.98/swarmauri/standard/conversations/concrete/SessionCacheConversation.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         res.extend(self._history[-self._max_size:])
         return res
 
     def session_to_dict(self) -> List[dict]:
         """
         Converts session messages to a list of dictionaries.
         """
-        return [message.to_dict() for message in self.session]
+        return [message.as_dict() for message in self.session]
 
     @property
     def session(self) -> List[IMessage]:
         return self._history[-self._session_cache_max_size:]
 
     @property
     def system_context(self) -> Union[SystemMessage, None]:
```

### Comparing `swarmauri-0.1.97/swarmauri/standard/conversations/concrete/SharedConversation.py` & `swarmauri-0.1.98/swarmauri/standard/conversations/concrete/SharedConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/distances/concrete/ChiSquaredDistance.py` & `swarmauri-0.1.98/swarmauri/standard/distances/concrete/ChiSquaredDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/distances/concrete/CosineDistance.py` & `swarmauri-0.1.98/swarmauri/standard/distances/concrete/CosineDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/distances/concrete/EuclideanDistance.py` & `swarmauri-0.1.98/swarmauri/standard/distances/concrete/EuclideanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/distances/concrete/JaccardIndexDistance.py` & `swarmauri-0.1.98/swarmauri/standard/distances/concrete/JaccardIndexDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/distances/concrete/LevenshteinDistance.py` & `swarmauri-0.1.98/swarmauri/standard/distances/concrete/LevenshteinDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/document_stores/base/DocumentStoreBase.py` & `swarmauri-0.1.98/swarmauri/standard/document_stores/base/DocumentStoreBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py` & `swarmauri-0.1.98/swarmauri/standard/document_stores/base/DocumentStoreRetrieveBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/documents/base/DocumentBase.py` & `swarmauri-0.1.98/swarmauri/standard/documents/base/DocumentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/documents/base/EmbeddedBase.py` & `swarmauri-0.1.98/swarmauri/standard/documents/base/EmbeddedBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py` & `swarmauri-0.1.98/swarmauri/standard/exceptions/concrete/IndexErrorWithContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/messages/base/MessageBase.py` & `swarmauri-0.1.98/swarmauri/standard/messages/base/MessageBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/messages/concrete/FunctionMessage.py` & `swarmauri-0.1.98/swarmauri/standard/messages/concrete/FunctionMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/messages/concrete/HumanMessage.py` & `swarmauri-0.1.98/swarmauri/standard/messages/concrete/HumanMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/messages/concrete/SystemMessage.py` & `swarmauri-0.1.98/swarmauri/standard/messages/concrete/SystemMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/base/AggregateMetricBase.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/base/AggregateMetricBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/base/CalculateMetricBase.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/base/CalculateMetricBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/base/MetricBase.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/base/MetricBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/base/ThresholdMetricBase.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/base/ThresholdMetricBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/concrete/FirstImpressionMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/concrete/HitRateAtK.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/concrete/HitRateAtK.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/concrete/ImpressionAtK.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/concrete/ImpressionAtK.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/concrete/MeanMetric.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/concrete/MeanMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/concrete/StaticValueMetric.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/concrete/StaticValueMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/concrete/SystemUsabilityScaleMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/concrete/TaskSuccessRateMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/concrete/ThresholdMeanMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/concrete/TimeOnTaskMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/metrics/concrete/ZeroMetric.py` & `swarmauri-0.1.98/swarmauri/standard/metrics/concrete/ZeroMetric.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/models/base/ModelBase.py` & `swarmauri-0.1.98/swarmauri/standard/models/base/ModelBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/models/concrete/AzureGPT.py` & `swarmauri-0.1.98/swarmauri/standard/models/concrete/AzureGPT.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/models/concrete/CohereModel.py` & `swarmauri-0.1.98/swarmauri/standard/models/concrete/CohereModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/models/concrete/GroqModel.py` & `swarmauri-0.1.98/swarmauri/standard/models/concrete/GroqModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/models/concrete/GroqToolModel.py` & `swarmauri-0.1.98/swarmauri/standard/models/concrete/GroqToolModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/models/concrete/MistralModel.py` & `swarmauri-0.1.98/swarmauri/standard/models/concrete/MistralModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/models/concrete/MistralToolModel.py` & `swarmauri-0.1.98/swarmauri/standard/models/concrete/MistralToolModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/models/concrete/OpenAIImageGenerator.py` & `swarmauri-0.1.98/swarmauri/standard/models/concrete/OpenAIImageGenerator.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/models/concrete/OpenAIModel.py` & `swarmauri-0.1.98/swarmauri/standard/models/concrete/OpenAIModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/models/concrete/OpenAIToolModel.py` & `swarmauri-0.1.98/swarmauri/standard/models/concrete/OpenAIToolModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/CSVParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/CSVParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/MarkdownParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/MarkdownParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/PythonParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/PythonParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/RegExParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/RegExParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/TFIDFParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/TFIDFParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/TextBlobNounParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/TextBlobNounParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/URLExtractorParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/URLExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/parsers/concrete/XMLParser.py` & `swarmauri-0.1.98/swarmauri/standard/parsers/concrete/XMLParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/prompts/concrete/Prompt.py` & `swarmauri-0.1.98/swarmauri/standard/prompts/concrete/Prompt.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/prompts/concrete/PromptGenerator.py` & `swarmauri-0.1.98/swarmauri/standard/prompts/concrete/PromptGenerator.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/prompts/concrete/PromptTemplate.py` & `swarmauri-0.1.98/swarmauri/standard/prompts/concrete/PromptTemplate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/swarms/base/SwarmComponentBase.py` & `swarmauri-0.1.98/swarmauri/standard/swarms/base/SwarmComponentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py` & `swarmauri-0.1.98/swarmauri/standard/swarms/concrete/SimpleSwarmFactory.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/toolkits/base/ToolkitBase.py` & `swarmauri-0.1.98/swarmauri/standard/toolkits/base/ToolkitBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/tools/base/ToolBase.py` & `swarmauri-0.1.98/swarmauri/standard/tools/base/ToolBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/tools/concrete/AdditionTool.py` & `swarmauri-0.1.98/swarmauri/standard/tools/concrete/AdditionTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/tools/concrete/Parameter.py` & `swarmauri-0.1.98/swarmauri/standard/tools/concrete/Parameter.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/tools/concrete/TestTool.py` & `swarmauri-0.1.98/swarmauri/standard/tools/concrete/TestTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/tools/concrete/WeatherTool.py` & `swarmauri-0.1.98/swarmauri/standard/tools/concrete/WeatherTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/tracing/concrete/CallableTracer.py` & `swarmauri-0.1.98/swarmauri/standard/tracing/concrete/CallableTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/tracing/concrete/ChainTracer.py` & `swarmauri-0.1.98/swarmauri/standard/tracing/concrete/ChainTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/tracing/concrete/SimpleTraceContext.py` & `swarmauri-0.1.98/swarmauri/standard/tracing/concrete/SimpleTraceContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/tracing/concrete/SimpleTracer.py` & `swarmauri-0.1.98/swarmauri/standard/tracing/concrete/SimpleTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/tracing/concrete/TracedVariable.py` & `swarmauri-0.1.98/swarmauri/standard/tracing/concrete/TracedVariable.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/tracing/concrete/VariableTracer.py` & `swarmauri-0.1.98/swarmauri/standard/tracing/concrete/VariableTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/utils/get_class_hash.py` & `swarmauri-0.1.98/swarmauri/standard/utils/get_class_hash.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/utils/load_documents_from_json.py` & `swarmauri-0.1.98/swarmauri/standard/utils/load_documents_from_json.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py` & `swarmauri-0.1.98/swarmauri/standard/vector_stores/base/SaveLoadStoreBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py` & `swarmauri-0.1.98/swarmauri/standard/vector_stores/base/VectorDocumentStoreBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py` & `swarmauri-0.1.98/swarmauri/standard/vector_stores/base/VectorDocumentStoreRetrieveBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py` & `swarmauri-0.1.98/swarmauri/standard/vector_stores/concrete/Doc2VecVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py` & `swarmauri-0.1.98/swarmauri/standard/vector_stores/concrete/MLMVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py` & `swarmauri-0.1.98/swarmauri/standard/vector_stores/concrete/SpatialDocVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py` & `swarmauri-0.1.98/swarmauri/standard/vector_stores/concrete/TFIDFVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py` & `swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/Doc2VecVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py` & `swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/MLMVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py` & `swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/NMFVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py` & `swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/SpatialDocVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py` & `swarmauri-0.1.98/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vectors/base/VectorBase.py` & `swarmauri-0.1.98/swarmauri/standard/vectors/base/VectorBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri/standard/vectors/concrete/VectorProduct.py` & `swarmauri-0.1.98/swarmauri/standard/vectors/concrete/VectorProduct.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri.egg-info/PKG-INFO` & `swarmauri-0.1.98/swarmauri.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri
-Version: 0.1.97
+Version: 0.1.98
 Summary: This repository includes core interfaces, standard ABCs and concrete references, third party plugins, and experimental modules for the swarmaURI framework.
 Home-page: http://github.com/swarmauri/swarmauri-sdk
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `swarmauri-0.1.97/swarmauri.egg-info/SOURCES.txt` & `swarmauri-0.1.98/swarmauri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.97/swarmauri.egg-info/requires.txt` & `swarmauri-0.1.98/swarmauri.egg-info/requires.txt`

 * *Files identical despite different names*

