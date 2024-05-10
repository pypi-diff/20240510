# Comparing `tmp/beyondllm-0.0.1.tar.gz` & `tmp/beyondllm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beyondllm-0.0.1.tar", max compression
+gzip compressed data, was "beyondllm-0.2.0.tar", max compression
```

## Comparing `beyondllm-0.0.1.tar` & `beyondllm-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,46 @@
--rw-r--r--   0        0        0    11357 2024-04-19 11:46:46.289524 beyondllm-0.0.1/LICENSE
--rw-r--r--   0        0        0     6139 2024-04-19 11:46:46.289524 beyondllm-0.0.1/README.md
--rw-r--r--   0        0        0      618 2024-04-19 14:15:25.204671 beyondllm-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 11:46:46.292524 beyondllm-0.0.1/src/beyondllm/__init__.py
--rw-r--r--   0        0        0      263 2024-04-19 11:46:46.292524 beyondllm-0.0.1/src/beyondllm/embeddings/__init__.py
--rw-r--r--   0        0        0     1822 2024-04-19 11:46:46.292524 beyondllm-0.0.1/src/beyondllm/embeddings/azure.py
--rw-r--r--   0        0        0      857 2024-04-19 11:46:46.292524 beyondllm-0.0.1/src/beyondllm/embeddings/base.py
--rw-r--r--   0        0        0     1862 2024-04-19 11:46:46.292524 beyondllm-0.0.1/src/beyondllm/embeddings/gemini_embed.py
--rw-r--r--   0        0        0     1568 2024-04-19 11:46:46.292524 beyondllm-0.0.1/src/beyondllm/embeddings/hf.py
--rw-r--r--   0        0        0     1906 2024-04-19 11:46:46.292524 beyondllm-0.0.1/src/beyondllm/embeddings/hf_inference.py
--rw-r--r--   0        0        0     1864 2024-04-19 11:46:46.292524 beyondllm-0.0.1/src/beyondllm/embeddings/openaiembed.py
--rw-r--r--   0        0        0     1576 2024-04-19 11:46:46.292524 beyondllm-0.0.1/src/beyondllm/embeddings/qdrantfast.py
--rw-r--r--   0        0        0       30 2024-04-19 11:46:46.292524 beyondllm-0.0.1/src/beyondllm/generator/__init__.py
--rw-r--r--   0        0        0      425 2024-04-19 11:46:46.292524 beyondllm-0.0.1/src/beyondllm/generator/base.py
--rw-r--r--   0        0        0     5849 2024-04-19 11:46:46.293524 beyondllm-0.0.1/src/beyondllm/generator/generate.py
--rw-r--r--   0        0        0        0 2024-04-19 11:46:46.293524 beyondllm-0.0.1/src/beyondllm/index/base.py
--rw-r--r--   0        0        0      210 2024-04-19 11:46:46.293524 beyondllm-0.0.1/src/beyondllm/llms/__init__.py
--rw-r--r--   0        0        0     2193 2024-04-19 11:46:46.293524 beyondllm-0.0.1/src/beyondllm/llms/azurechat.py
--rw-r--r--   0        0        0      807 2024-04-19 11:46:46.293524 beyondllm-0.0.1/src/beyondllm/llms/base.py
--rw-r--r--   0        0        0     2213 2024-04-19 11:46:46.293524 beyondllm-0.0.1/src/beyondllm/llms/chatopenai.py
--rw-r--r--   0        0        0     2447 2024-04-19 11:46:46.293524 beyondllm-0.0.1/src/beyondllm/llms/gemini.py
--rw-r--r--   0        0        0     2335 2024-04-19 11:46:46.293524 beyondllm-0.0.1/src/beyondllm/llms/hf.py
--rw-r--r--   0        0        0     1734 2024-04-19 11:46:46.293524 beyondllm-0.0.1/src/beyondllm/llms/ollama.py
--rw-r--r--   0        0        0     1441 2024-04-19 11:46:46.293524 beyondllm-0.0.1/src/beyondllm/loaders/base.py
--rw-r--r--   0        0        0     1390 2024-04-19 11:46:46.293524 beyondllm-0.0.1/src/beyondllm/loaders/llamaParseLoader.py
--rw-r--r--   0        0        0     1774 2024-04-19 11:46:46.294524 beyondllm-0.0.1/src/beyondllm/loaders/notionLoader.py
--rw-r--r--   0        0        0     1282 2024-04-19 11:46:46.294524 beyondllm-0.0.1/src/beyondllm/loaders/simpleLoader.py
--rw-r--r--   0        0        0     1730 2024-04-19 11:46:46.294524 beyondllm-0.0.1/src/beyondllm/loaders/urlLoader.py
--rw-r--r--   0        0        0     1903 2024-04-19 11:46:46.294524 beyondllm-0.0.1/src/beyondllm/loaders/youtubeLoader.py
--rw-r--r--   0        0        0     4478 2024-04-19 11:46:46.294524 beyondllm-0.0.1/src/beyondllm/retrieve.py
--rw-r--r--   0        0        0     2017 2024-04-19 11:46:46.294524 beyondllm-0.0.1/src/beyondllm/retrievers/base.py
--rw-r--r--   0        0        0     3347 2024-04-19 14:15:25.208672 beyondllm-0.0.1/src/beyondllm/retrievers/crossEncoderReranker.py
--rw-r--r--   0        0        0     3395 2024-04-19 11:46:46.294524 beyondllm-0.0.1/src/beyondllm/retrievers/flagReranker.py
--rw-r--r--   0        0        0     5568 2024-04-19 11:46:46.294524 beyondllm-0.0.1/src/beyondllm/retrievers/hybridRetriever.py
--rw-r--r--   0        0        0     1770 2024-04-19 11:46:46.294524 beyondllm-0.0.1/src/beyondllm/retrievers/normalRetriever.py
--rw-r--r--   0        0        0     3167 2024-04-19 11:46:46.295524 beyondllm-0.0.1/src/beyondllm/retrievers/utils.py
--rw-r--r--   0        0        0     1658 2024-04-19 11:46:46.295524 beyondllm-0.0.1/src/beyondllm/source.py
--rw-r--r--   0        0        0     4496 2024-04-19 11:46:46.295524 beyondllm-0.0.1/src/beyondllm/utils.py
--rw-r--r--   0        0        0        0 2024-04-19 11:46:46.295524 beyondllm-0.0.1/src/beyondllm/vectordb/base.py
--rw-r--r--   0        0        0     7057 1970-01-01 00:00:00.000000 beyondllm-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 05:03:30.256152 beyondllm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5593 2024-05-10 05:03:30.256405 beyondllm-0.2.0/README.md
+-rw-r--r--   0        0        0      624 2024-05-10 05:03:30.267094 beyondllm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 05:03:30.267498 beyondllm-0.2.0/src/beyondllm/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-10 05:03:30.267674 beyondllm-0.2.0/src/beyondllm/embeddings/__init__.py
+-rw-r--r--   0        0        0     2366 2024-05-10 05:03:30.267799 beyondllm-0.2.0/src/beyondllm/embeddings/azure.py
+-rw-r--r--   0        0        0      869 2024-05-10 05:03:30.267897 beyondllm-0.2.0/src/beyondllm/embeddings/base.py
+-rw-r--r--   0        0        0     3390 2024-05-10 05:03:30.268002 beyondllm-0.2.0/src/beyondllm/embeddings/finetune.py
+-rw-r--r--   0        0        0     1862 2024-05-10 05:03:30.268097 beyondllm-0.2.0/src/beyondllm/embeddings/gemini_embed.py
+-rw-r--r--   0        0        0     1568 2024-05-10 05:03:30.268193 beyondllm-0.2.0/src/beyondllm/embeddings/hf.py
+-rw-r--r--   0        0        0     1906 2024-05-10 05:03:30.268315 beyondllm-0.2.0/src/beyondllm/embeddings/hf_inference.py
+-rw-r--r--   0        0        0     1864 2024-05-10 05:03:30.268415 beyondllm-0.2.0/src/beyondllm/embeddings/openaiembed.py
+-rw-r--r--   0        0        0     1576 2024-05-10 05:03:30.268531 beyondllm-0.2.0/src/beyondllm/embeddings/qdrantfast.py
+-rw-r--r--   0        0        0     6664 2024-05-10 05:03:30.268671 beyondllm-0.2.0/src/beyondllm/embeddings/utils.py
+-rw-r--r--   0        0        0       30 2024-05-10 05:03:30.268828 beyondllm-0.2.0/src/beyondllm/generator/__init__.py
+-rw-r--r--   0        0        0      425 2024-05-10 05:03:30.269037 beyondllm-0.2.0/src/beyondllm/generator/base.py
+-rw-r--r--   0        0        0     5849 2024-05-10 05:03:30.269167 beyondllm-0.2.0/src/beyondllm/generator/generate.py
+-rw-r--r--   0        0        0        0 2024-05-10 05:03:30.269254 beyondllm-0.2.0/src/beyondllm/index/base.py
+-rw-r--r--   0        0        0      251 2024-05-10 05:03:30.269426 beyondllm-0.2.0/src/beyondllm/llms/__init__.py
+-rw-r--r--   0        0        0     2930 2024-05-10 05:03:30.269548 beyondllm-0.2.0/src/beyondllm/llms/azurechat.py
+-rw-r--r--   0        0        0      807 2024-05-10 05:03:30.269649 beyondllm-0.2.0/src/beyondllm/llms/base.py
+-rw-r--r--   0        0        0     2213 2024-05-10 05:03:30.269747 beyondllm-0.2.0/src/beyondllm/llms/chatopenai.py
+-rw-r--r--   0        0        0     2456 2024-05-10 05:03:30.269867 beyondllm-0.2.0/src/beyondllm/llms/gemini.py
+-rw-r--r--   0        0        0     2335 2024-05-10 05:03:30.269967 beyondllm-0.2.0/src/beyondllm/llms/hf.py
+-rw-r--r--   0        0        0     2654 2024-05-10 05:03:30.270074 beyondllm-0.2.0/src/beyondllm/llms/multimodal.py
+-rw-r--r--   0        0        0     1734 2024-05-10 05:03:30.270172 beyondllm-0.2.0/src/beyondllm/llms/ollama.py
+-rw-r--r--   0        0        0     1441 2024-05-10 05:03:30.270328 beyondllm-0.2.0/src/beyondllm/loaders/base.py
+-rw-r--r--   0        0        0     1390 2024-05-10 05:03:30.270456 beyondllm-0.2.0/src/beyondllm/loaders/llamaParseLoader.py
+-rw-r--r--   0        0        0     1774 2024-05-10 05:03:30.270552 beyondllm-0.2.0/src/beyondllm/loaders/notionLoader.py
+-rw-r--r--   0        0        0     1282 2024-05-10 05:03:30.270654 beyondllm-0.2.0/src/beyondllm/loaders/simpleLoader.py
+-rw-r--r--   0        0        0     1730 2024-05-10 05:03:30.270745 beyondllm-0.2.0/src/beyondllm/loaders/urlLoader.py
+-rw-r--r--   0        0        0     1903 2024-05-10 05:03:30.270840 beyondllm-0.2.0/src/beyondllm/loaders/youtubeLoader.py
+-rw-r--r--   0        0        0     4679 2024-05-10 05:03:30.270975 beyondllm-0.2.0/src/beyondllm/retrieve.py
+-rw-r--r--   0        0        0     2117 2024-05-10 05:03:30.271137 beyondllm-0.2.0/src/beyondllm/retrievers/base.py
+-rw-r--r--   0        0        0     4104 2024-05-10 05:03:30.271279 beyondllm-0.2.0/src/beyondllm/retrievers/crossEncoderReranker.py
+-rw-r--r--   0        0        0     4153 2024-05-10 05:03:30.271402 beyondllm-0.2.0/src/beyondllm/retrievers/flagReranker.py
+-rw-r--r--   0        0        0     6133 2024-05-10 05:03:30.271659 beyondllm-0.2.0/src/beyondllm/retrievers/hybridRetriever.py
+-rw-r--r--   0        0        0     2634 2024-05-10 05:03:30.271751 beyondllm-0.2.0/src/beyondllm/retrievers/normalRetriever.py
+-rw-r--r--   0        0        0     3167 2024-05-10 05:03:30.271853 beyondllm-0.2.0/src/beyondllm/retrievers/utils.py
+-rw-r--r--   0        0        0     1658 2024-05-10 05:03:30.271950 beyondllm-0.2.0/src/beyondllm/source.py
+-rw-r--r--   0        0        0     4496 2024-05-10 05:03:30.272071 beyondllm-0.2.0/src/beyondllm/utils.py
+-rw-r--r--   0        0        0       73 2024-05-10 05:03:30.272212 beyondllm-0.2.0/src/beyondllm/vectordb/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-10 05:03:30.272304 beyondllm-0.2.0/src/beyondllm/vectordb/base.py
+-rw-r--r--   0        0        0     2920 2024-05-10 05:03:30.272528 beyondllm-0.2.0/src/beyondllm/vectordb/chroma.py
+-rw-r--r--   0        0        0     4287 2024-05-10 05:03:30.272658 beyondllm-0.2.0/src/beyondllm/vectordb/pinecone.py
+-rw-r--r--   0        0        0     6515 1970-01-01 00:00:00.000000 beyondllm-0.2.0/PKG-INFO
```

### Comparing `beyondllm-0.0.1/LICENSE` & `beyondllm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/README.md` & `beyondllm-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,66 +3,31 @@
 <h2 align="center">Build - Rapid Experiment - Evaluate - Repeat</h2>
 
 ![Thumbnails](https://github.com/aiplanethub/beyondllm/assets/132284203/489bb644-f87e-4477-a639-a63552f84cd7)
 
 <a href="https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-3776AB.svg?style=flat&logo=python&logoColor=white"><img src="https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python Versions"></a>
 <a href="https://discord.gg/4aWV7He2QU"><img src="https://dcbadge.vercel.app/api/server/4aWV7He2QU?style=flat" alt="Discord" /></a>
 <a href="https://twitter.com/aiplanethub"><img src="https://img.shields.io/twitter/follow/aiplanethub" alt="Twitter" /></a>
-<a href="https://colab.research.google.com/drive/1dJZF5113e5XQsm6GxuW3ShYCBZcUs3-_?usp=sharing" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Try an example"/></a>
+<a href="https://colab.research.google.com/drive/1S1UL2uCahHkfJsurRA3f7dcR6IHjg-IM?usp=sharing" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Try an example"/></a>
 
-[![GitHub stars](https://img.shields.io/github/stars/aiplanethub/beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/)
-[![License](https://img.shields.io/github/license/aiplanethub/beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/blob/main/LICENSE)
-[![Contributors](https://img.shields.io/github/contributors/username/repo.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/graphs/contributors)
+[![Contributors](https://img.shields.io/github/contributors/aiplanethub/beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/graphs/contributors)
 [![Code of Conduct](https://img.shields.io/badge/code%20of%20conduct-contributor%20covenant-green.svg?style=flat-square)](CODE_OF_CONDUCT.md)
 
 <p>Beyond LLM offers an all-in-one toolkit for experimentation, evaluation, and deployment of Retrieval-Augmented Generation (RAG) systems, simplifying the process with automated integration, customizable evaluation metrics, and support for various Large Language Models (LLMs) tailored to specific needs, ultimately aiming to reduce LLM hallucination risks and enhance reliability.</p>
 <i><a href="https://discord.gg/4aWV7He2QU">👉 Join our Discord community!</a></i>
 </div>
 
 Try out a quick demo on Google Colab:
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1dJZF5113e5XQsm6GxuW3ShYCBZcUs3-_?usp=sharing)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1S1UL2uCahHkfJsurRA3f7dcR6IHjg-IM?usp=sharing)
 
 ## Quick install
 
-1. To install Beyond LLM i.e., a private repo, we can use Access Token of GitHub. 
-
-   ```bash
-   git clone https://<UPDATE-WITH-YOUR-TOKEN>@github.com/aiplanethub/beyondllm.git
-   ```
-
-3. Go to the project directory
-
-   ```bash
-   cd beyondllm
-   ```
-
-4. Install the package
-
-   ```bash
-   pip install .
-   ```
-
-   OR,
-
-   ```bash
-   pip install -e .
-   ```
-
-   When using the `-e` flag, the package is installed in editable mode. This means that if you make changes to the source code, you do not need to reinstall the package for the changes to take effect.
-
-Install on Google Colab
-
 ```bash
-!git clone https://<UPDATE-WITH-YOUR-TOKEN>@github.com/aiplanethub/beyondllm.git
-
-%cd /content/beyondllm/
-
-pip install .
-
+pip install beyondllm
 ```
 
 ## Quickstart Guide- Chat with YouTube Video
 
 In this quick start guide, we'll demonstrate how to create a Chat with YouTube video RAG application using Beyond LLM with less than 8 lines of code. This 8 lines of code includes:
 * Getting custom data source
 * Retrieving documents
@@ -116,23 +81,34 @@
 MRR:1.0
 
 Context relevancy Score: 8.0
 Answer relevancy Score: 7.0
 Groundness score: 7.666666666666667
 ```
 
-## Get in Touch
+## Documentation
+
+See the [beyondllm.aiplanet.com](https://beyondllm.aiplanet.com/) for complete documentation.
 
-You can schedule a 1:1 meeting with our Team to get started with GenAI Stack, OpenAGI, AI Planet Open Source LLMs(Buddhi, effi and Panda Coder) and Beyond LLM. Schedule the call here: [https://calendly.com/jaintarun](https://calendly.com/jaintarun)
 
 ## Contribution guidelines
 
 Beyond LLM thrives in the rapidly evolving landscape of open-source projects. We wholeheartedly welcome contributions in various capacities, be it through innovative features, enhanced infrastructure, or refined documentation.
 
+See [Contributing guide](https://github.com/aiplanethub/beyondllm/blob/main/CONTRIBUTING.md) for more information on contributing to the BeyondLLM library. 
+
 ## Acknowledgements
 
 * [HuggingFace](https://github.com/huggingface)
 * [LlamaIndex](https://github.com/jerryjliu/llama_index)
 * [OpenAI](https://github.com/openai)
 * [Google Gemini](https://ai.google.dev/)
   
 and the entire OpenSource community.
+
+## License
+
+The contents of this repository are licensed under the [Apache License, version 2.0](https://github.com/aiplanethub/beyondllm/blob/main/LICENSE).
+
+## Get in Touch
+
+You can schedule a 1:1 meeting with our Team to get started with GenAI Stack, OpenAGI, AI Planet Open Source LLMs(Buddhi, effi and Panda Coder) and Beyond LLM. Schedule the call here: [https://calendly.com/jaintarun](https://calendly.com/jaintarun)
```

#### html2text {}

```diff
@@ -1,46 +1,35 @@
                             ************ BBeeyyoonnddLLLLMM ************
            ********** BBuuiilldd -- RRaappiidd EExxppeerriimmeenntt -- EEvvaalluuaattee -- RReeppeeaatt **********
    ![Thumbnails](https://github.com/aiplanethub/beyondllm/assets/132284203/
  489bb644-f87e-4477-a639-a63552f84cd7) _[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_D_i_s_c_o_r_d_]_[_T_w_i_t_t_e_r_]_[_T_r_y
- _a_n_ _e_x_a_m_p_l_e_][![GitHub stars](https://img.shields.io/github/stars/aiplanethub/
-beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/) [!
-         [License](https://img.shields.io/github/license/aiplanethub/
-  beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/
-blob/main/LICENSE) [![Contributors](https://img.shields.io/github/contributors/
-username/repo.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/
-    graphs/contributors) [![Code of Conduct](https://img.shields.io/badge/
-   code%20of%20conduct-contributor%20covenant-green.svg?style=flat-square)]
+    _a_n_ _e_x_a_m_p_l_e_][![Contributors](https://img.shields.io/github/contributors/
+ aiplanethub/beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/
+  beyondllm/graphs/contributors) [![Code of Conduct](https://img.shields.io/
+badge/code%20of%20conduct-contributor%20covenant-green.svg?style=flat-square)]
                              (CODE_OF_CONDUCT.md)
  Beyond LLM offers an all-in-one toolkit for experimentation, evaluation, and
   deployment of Retrieval-Augmented Generation (RAG) systems, simplifying the
    process with automated integration, customizable evaluation metrics, and
  support for various Large Language Models (LLMs) tailored to specific needs,
  ultimately aiming to reduce LLM hallucination risks and enhance reliability.
                        _ð____ _J_o_i_n_ _o_u_r_ _D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_!
 Try out a quick demo on Google Colab: [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1dJZF5113e5XQsm6GxuW3ShYCBZcUs3-_?usp=sharing)
-## Quick install 1. To install Beyond LLM i.e., a private repo, we can use
-Access Token of GitHub. ```bash git clone https://@github.com/aiplanethub/
-beyondllm.git ``` 3. Go to the project directory ```bash cd beyondllm ``` 4.
-Install the package ```bash pip install . ``` OR, ```bash pip install -e . ```
-When using the `-e` flag, the package is installed in editable mode. This means
-that if you make changes to the source code, you do not need to reinstall the
-package for the changes to take effect. Install on Google Colab ```bash !git
-clone https://@github.com/aiplanethub/beyondllm.git %cd /content/beyondllm/ pip
-install . ``` ## Quickstart Guide- Chat with YouTube Video In this quick start
-guide, we'll demonstrate how to create a Chat with YouTube video RAG
-application using Beyond LLM with less than 8 lines of code. This 8 lines of
-code includes: * Getting custom data source * Retrieving documents * Generating
-LLM responses * Evaluating embeddings * Evaluating LLM responses ### Approach-
-1: Using Default LLM and Embeddings Build customised RAG in less than ``5 lines
-of code`` using Beyond LLM. ```python from beyondllm import
-source,retrieve,generator import os os.environ['GOOGLE_API_KEY'] = "Your Google
-API Key:" data = source.fit("https://www.youtube.com/
+colab.research.google.com/drive/1S1UL2uCahHkfJsurRA3f7dcR6IHjg-IM?usp=sharing)
+## Quick install ```bash pip install beyondllm ``` ## Quickstart Guide- Chat
+with YouTube Video In this quick start guide, we'll demonstrate how to create a
+Chat with YouTube video RAG application using Beyond LLM with less than 8 lines
+of code. This 8 lines of code includes: * Getting custom data source *
+Retrieving documents * Generating LLM responses * Evaluating embeddings *
+Evaluating LLM responses ### Approach-1: Using Default LLM and Embeddings Build
+customised RAG in less than ``5 lines of code`` using Beyond LLM. ```python
+from beyondllm import source,retrieve,generator import os os.environ
+['GOOGLE_API_KEY'] = "Your Google API Key:" data = source.fit("https://
+www.youtube.com/
 watch?v=oJJyTztI_6g",dtype="youtube",chunk_size=512,chunk_overlap=50) retriever
 = retrieve.auto_retriever(data,type="normal",top_k=3) pipeline =
 generator.Generate(question="what tool is video mentioning
 about?",retriever=retriever) print(pipeline.call()) ``` ### Approach-2: With
 Custom LLM and Embeddings Beyond LLM support various Embeddings and LLMs that
 are two very important components in Retrieval Augmented Generation. ```python
 from beyondllm import source,retrieve,embeddings,llms,generator import os from
@@ -56,17 +45,23 @@
 ```bash The tool mentioned in the context is called Jupiter, which is an AI
 Guru designed to simplify the learning of complex data science topics. Users
 can access Jupiter by logging into AI Planet, accessing any course for free,
 and then requesting explanations of topics from Jupiter in various styles, such
 as in the form of a movie plot. Jupiter aims to make AI education more
 accessible and interactive for everyone. Hit_rate:1.0 MRR:1.0 Context relevancy
 Score: 8.0 Answer relevancy Score: 7.0 Groundness score: 7.666666666666667 ```
-## Get in Touch You can schedule a 1:1 meeting with our Team to get started
-with GenAI Stack, OpenAGI, AI Planet Open Source LLMs(Buddhi, effi and Panda
-Coder) and Beyond LLM. Schedule the call here: [https://calendly.com/jaintarun]
-(https://calendly.com/jaintarun) ## Contribution guidelines Beyond LLM thrives
-in the rapidly evolving landscape of open-source projects. We wholeheartedly
-welcome contributions in various capacities, be it through innovative features,
-enhanced infrastructure, or refined documentation. ## Acknowledgements *
-[HuggingFace](https://github.com/huggingface) * [LlamaIndex](https://
-github.com/jerryjliu/llama_index) * [OpenAI](https://github.com/openai) *
-[Google Gemini](https://ai.google.dev/) and the entire OpenSource community.
+## Documentation See the [beyondllm.aiplanet.com](https://
+beyondllm.aiplanet.com/) for complete documentation. ## Contribution guidelines
+Beyond LLM thrives in the rapidly evolving landscape of open-source projects.
+We wholeheartedly welcome contributions in various capacities, be it through
+innovative features, enhanced infrastructure, or refined documentation. See
+[Contributing guide](https://github.com/aiplanethub/beyondllm/blob/main/
+CONTRIBUTING.md) for more information on contributing to the BeyondLLM library.
+## Acknowledgements * [HuggingFace](https://github.com/huggingface) *
+[LlamaIndex](https://github.com/jerryjliu/llama_index) * [OpenAI](https://
+github.com/openai) * [Google Gemini](https://ai.google.dev/) and the entire
+OpenSource community. ## License The contents of this repository are licensed
+under the [Apache License, version 2.0](https://github.com/aiplanethub/
+beyondllm/blob/main/LICENSE). ## Get in Touch You can schedule a 1:1 meeting
+with our Team to get started with GenAI Stack, OpenAGI, AI Planet Open Source
+LLMs(Buddhi, effi and Panda Coder) and Beyond LLM. Schedule the call here:
+[https://calendly.com/jaintarun](https://calendly.com/jaintarun)
```

### Comparing `beyondllm-0.0.1/pyproject.toml` & `beyondllm-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "beyondllm"
-version = "0.0.1"
+version = "0.2.0"
 description = "Beyond LLM is an toolkit to Build Experiment Evaluate and Observe RAG pipelines"
 authors = ["AI Planet <tech@aiplanet.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.9 | ~3.10 | ~3.11"
 llama-index = "0.10.27"
 llama-index-embeddings-gemini = "0.1.6"
 nltk = "3.8.1"
 numpy = "1.26.4"
 openai = "1.20.0"
-pydantic = "2.7.0"
+pydantic = ">=1.10.5,<2"
 sqlalchemy = "2.0.29"
 pysbd = "0.3.4"
 pypdf = "4.2.0"
 pyyaml = "6.0.1"
 regex = "2024.4.16"
 tiktoken = "0.6.0"
 pandas = "2.0.3"
```

### Comparing `beyondllm-0.0.1/src/beyondllm/embeddings/azure.py` & `beyondllm-0.2.0/src/beyondllm/embeddings/openaiembed.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-from beyondllm.embeddings.base import EmbeddingConfig
-from dataclasses import dataclass
+from beyondllm.embeddings.base import BaseEmbeddings,EmbeddingConfig
+from dataclasses import dataclass, field
 import warnings
 warnings.filterwarnings("ignore")
+import os
 
 @dataclass
-class AzureAIEmbeddings:
+class OpenAIEmbeddings:
     """
-    from beyondllm.embeddings import AzureAIEmbeddings
-    embed_model = AzureAIEmbeddings(endpoint_url="https:---",azure_key="",api_version="",deployment_name="")
+    from beyondllm.embeddings import OpenAIEmbeddings
+    embed_model = OpenAIEmbeddings(model_name="text-embedding-3-small",api_key="sk-")
     """
-    azure_key: str
-    endpoint_url: str
-    api_version: str
-    deployment_name: str
+    api_key: str = ""
+    model_name:  str = field(default='text-embedding-3-small')
 
     def __post_init__(self):
+        if not self.api_key:  
+            self.api_key = os.getenv('OPENAI_API_KEY') 
+            if not self.api_key: 
+                raise ValueError("OPENAI_API_KEY is not provided and not found in environment variables.")
         self.load()
 
     def load(self):
         try:
-            from llama_index.embeddings.azure_openai import AzureOpenAIEmbedding
+            from llama_index.embeddings.openai import OpenAIEmbedding
         except:
-            raise ImportError("Azure OpenAI Embeddings library is not installed. Please install it with ``pip install llama-index-embeddings-azure_openai``.")
+            raise ImportError("OpenAI Embeddings library is not installed. Please install it with ``pip install llama-index-embeddings-openai``.")
         
         try:
-            self.client = AzureOpenAIEmbedding(
-                api_key=self.azure_key,
-                azure_endpoint = self.endpoint_url,
-                api_version = self.api_version,
-                deployment_name = self.deployment_name
-            )
+            self.client = OpenAIEmbedding(model_name=self.model_name,api_key = self.api_key)
 
         except Exception as e:
-            raise Exception("Failed to load the embeddings from AzureOpenAI:", str(e))
+            raise Exception("Failed to load the embeddings from OpenAI:", str(e))
         
         return self.client
     
     def embed_text(self,text):
         embeds = self.client.get_text_embedding(text) 
         return embeds
     
@@ -48,8 +46,8 @@
         agg_embedding = self.client.get_agg_embedding_from_queries(*args, **kwargs)
         return agg_embedding
 
     @staticmethod
     def load_from_kwargs(self,kwargs): 
         embed_config = EmbeddingConfig(**kwargs)
         self.config = embed_config
-        self.load()
+        self.load()
```

### Comparing `beyondllm-0.0.1/src/beyondllm/embeddings/base.py` & `beyondllm-0.2.0/src/beyondllm/embeddings/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pydantic import BaseModel
 
 class EmbeddingConfig(BaseModel):
-    """Base configuration model for all LLMs.
+    """Base configuration model for all Embeddings.
 
-    This class can be extended to include more fields specific to certain LLMs.
+    This class can be extended to include more fields specific to certain Embeddings.
     """
     pass 
 
 class BaseEmbeddings(BaseModel):
     def load(self):
         raise NotImplementedError("This method should be implemented by subclasses.")
```

### Comparing `beyondllm-0.0.1/src/beyondllm/embeddings/gemini_embed.py` & `beyondllm-0.2.0/src/beyondllm/embeddings/gemini_embed.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/embeddings/hf.py` & `beyondllm-0.2.0/src/beyondllm/embeddings/hf.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/embeddings/hf_inference.py` & `beyondllm-0.2.0/src/beyondllm/embeddings/hf_inference.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/embeddings/qdrantfast.py` & `beyondllm-0.2.0/src/beyondllm/embeddings/qdrantfast.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/generator/generate.py` & `beyondllm-0.2.0/src/beyondllm/generator/generate.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/llms/azurechat.py` & `beyondllm-0.2.0/src/beyondllm/llms/chatopenai.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from beyondllm.llms.base import BaseLLMModel, ModelConfig
 from typing import Any, Dict, List, Optional
-from dataclasses import dataclass
+import os
+from dataclasses import dataclass,field
 
 @dataclass
-class AzureOpenAIModel:
+class ChatOpenAIModel:
     """
     Class representing a Chat Language Model (LLM) model using OpenAI
     Example:
-    >>> from beyondllm.llms import ChatOpenAIModel
-    >>> llm = AzureOpenAIModel(model="gpt4",api_key = "<your_api_key>",deployment_name="",endpoint_url="",model_kwargs={"max_tokens":512,"temperature":0.1})
+    from beyondllm.llms import ChatOpenAIModel
+    llm = ChatOpenAIModel(model="gpt-3.5-turbo",api_key = "",model_kwargs = {"max_tokens":512,"temperature":0.1})
     """
-    api_key: str
-    deployment_name: str
-    endpoint_url: str
-    model: str = "gpt4"
-    model_kwargs: Optional[Dict] = None
+    api_key: str = ""
+    model: str = field(default="gpt-3.5-turbo")
+    model_kwargs: Optional[Dict]  = None
 
     def __post_init__(self):
+        if not self.api_key:  
+            self.api_key = os.getenv('OPENAI_API_KEY') 
+            if not self.api_key: 
+                raise ValueError("OPENAI_API_KEY is not provided and not found in environment variables.")
         self.load_llm()
 
     def load_llm(self):
         try:
             import openai
         except ImportError:
-            raise ImportError("AzureChat Model is not installed. Please install it with ``pip install openai``.")
+            raise ImportError("OpenAI library is not installed. Please install it with ``pip install openai``.")
         
         try:
-            self.client = openai.AzureOpenAI(
-                api_version = "2023-05-15",
-                azure_endpoint = self.endpoint_url,
-                azure_deployment = self.deployment_name,  
-                api_key = self.api_key
-            )
-        except Exception as e:
-            raise Exception("Failed to load the model from Azure OpenAI:", str(e))
+            self.client = openai.OpenAI(api_key=self.api_key)
 
+        except Exception as e:
+            raise Exception("Failed to load the model from OpenAI:", str(e))
+        
+        return self.client
 
     def predict(self,prompt:Any):
         if self.model_kwargs is not None:
             response = self.client.chat.completions.create(
                 model = self.model,
                 messages=[
                     {"role": "system", "content": "You are a helpful assistant."},
                     {"role": "user", "content": prompt}
                 ],
-            **self.model_kwargs
+                **self.model_kwargs
             )
         else:
             response = self.client.chat.completions.create(
                 model = self.model,
                 messages=[
                     {"role": "system", "content": "You are a helpful assistant."},
                     {"role": "user", "content": prompt}
```

### Comparing `beyondllm-0.0.1/src/beyondllm/llms/base.py` & `beyondllm-0.2.0/src/beyondllm/llms/base.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/llms/chatopenai.py` & `beyondllm-0.2.0/src/beyondllm/llms/gemini.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 from beyondllm.llms.base import BaseLLMModel, ModelConfig
 from typing import Any, Dict, List, Optional
-import os
 from dataclasses import dataclass,field
+import os
 
 @dataclass
-class ChatOpenAIModel:
+class GeminiModel:
     """
-    Class representing a Chat Language Model (LLM) model using OpenAI
+    Class representing a Language Model (LLM) model using Google Generative AI
     Example:
-    from beyondllm.llms import ChatOpenAIModel
-    llm = ChatOpenAIModel(model="gpt-3.5-turbo",api_key = "",model_kwargs = {"max_tokens":512,"temperature":0.1})
+    ```
+    >>> from beyondllm.llms import GeminiModel
+    >>> llm = GeminiModel(model_name="gemini-pro",google_api_key = "<your_api_key>",model_kwargs={"temperature":0.2})
+    ```
+    or 
+    ```
+    >>> import os
+    >>> os.environ['GOOGLE_API_KEY'] = "***********" #replace with your key
+    >>> from beyondllm.llms import GeminiModel
+    >>> llm = GeminiModel(model_name="gemini-pro")
+    ```
     """
-    api_key: str = ""
-    model: str = field(default="gpt-3.5-turbo")
-    model_kwargs: Optional[Dict]  = None
+    google_api_key:str = ""
+    model_name:str = "gemini-pro"
+    model_kwargs: dict = field(default_factory=lambda: {
+                    "temperature": 0,
+                    "top_p": 1,
+                    "top_k": 1,
+                    "max_output_tokens": 2048,
+            })
 
     def __post_init__(self):
-        if not self.api_key:  
-            self.api_key = os.getenv('OPENAI_API_KEY') 
-            if not self.api_key: 
-                raise ValueError("OPENAI_API_KEY is not provided and not found in environment variables.")
+        if not self.google_api_key:  
+            self.google_api_key = os.getenv('GOOGLE_API_KEY') 
+            if not self.google_api_key: 
+                raise ValueError("GOOGLE_API_KEY is not provided and not found in environment variables.")
         self.load_llm()
 
     def load_llm(self):
         try:
-            import openai
+            import google.generativeai as genai
         except ImportError:
-            raise ImportError("OpenAI library is not installed. Please install it with ``pip install openai``.")
+            raise ImportError("Google Generative AI library is not installed. Please install it with ``pip install google-generativeai``.")
         
         try:
-            self.client = openai.OpenAI(api_key=self.api_key)
+            VALID_MODEL_SUPPORT = ["gemini-1.0-pro","gemini-pro",'gemini-1.5-pro-latest']
+            if self.model_name not in VALID_MODEL_SUPPORT:
+                raise f"Model not supported. Currently we only support: {','.join(VALID_MODEL_SUPPORT)}."
+            
+            genai.configure(api_key = self.google_api_key)
+            self.client = genai.GenerativeModel(model_name=self.model_name,
+                                                generation_config=self.model_kwargs)
 
         except Exception as e:
-            raise Exception("Failed to load the model from OpenAI:", str(e))
-        
-        return self.client
+            raise Exception("Failed to load the model from Gemini Google Generative AI:", str(e))
 
-    def predict(self,prompt:Any):
-        if self.model_kwargs is not None:
-            response = self.client.chat.completions.create(
-                model = self.model,
-                messages=[
-                    {"role": "system", "content": "You are a helpful assistant."},
-                    {"role": "user", "content": prompt}
-                ],
-                **self.model_kwargs
-            )
-        else:
-            response = self.client.chat.completions.create(
-                model = self.model,
-                messages=[
-                    {"role": "system", "content": "You are a helpful assistant."},
-                    {"role": "user", "content": prompt}
-                ]
-            )
-        
-        return response.choices[0].message.content
 
+    def predict(self,prompt:Any):
+        response = self.client.generate_content(prompt)
+        return response.text
+    
     @staticmethod
     def load_from_kwargs(self,kwargs): 
         model_config = ModelConfig(**kwargs)
         self.config = model_config
         self.load_llm()
```

### Comparing `beyondllm-0.0.1/src/beyondllm/llms/gemini.py` & `beyondllm-0.2.0/src/beyondllm/llms/multimodal.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from beyondllm.llms.base import BaseLLMModel, ModelConfig
 from typing import Any, Dict, List, Optional
 from dataclasses import dataclass,field
+from PIL import Image
 import os
 
 @dataclass
-class GeminiModel:
+class GeminiMultiModal:
     """
     Class representing a Language Model (LLM) model using Google Generative AI
     Example:
     ```
-    >>> from beyondllm.llms import GeminiModel
-    >>> llm = GeminiModel(model_name="gemini-pro",google_api_key = "<your_api_key>",model_kwargs={"temperature":0.2})
+    >>> from beyondllm.llms import GeminiMultiModal
+    >>> llm = GeminiMultiModal(model_name="gemini-pro-vision",google_api_key = "<your_api_key>",model_kwargs={"temperature":0.2})
     ```
     or 
     ```
     >>> import os
     >>> os.environ['GOOGLE_API_KEY'] = "***********" #replace with your key
-    >>> from beyondllm.llms import GeminiModel
-    >>> llm = GeminiModel(model_name="gemini-pro")
+    >>> from beyondllm.llms import GeminiMultiModal
+    >>> llm = GeminiMultiModal(model_name="gemini-pro-vision")
     ```
     """
     google_api_key:str = ""
-    model_name:str = "gemini-pro"
+    model_name:str = "gemini-pro-vision"
     model_kwargs: dict = field(default_factory=lambda: {
                     "temperature": 0,
                     "top_p": 1,
                     "top_k": 1,
                     "max_output_tokens": 2048,
             })
 
@@ -39,29 +40,30 @@
     def load_llm(self):
         try:
             import google.generativeai as genai
         except ImportError:
             raise ImportError("Google Generative AI library is not installed. Please install it with ``pip install google-generativeai``.")
         
         try:
-            VALID_MODEL_SUPPORT = ["gemini-1.0-pro","gemini-pro",""]
+            VALID_MODEL_SUPPORT = ["gemini-1.0-pro-vision-latest","gemini-pro-vision"]
             if self.model_name not in VALID_MODEL_SUPPORT:
-                raise "Model not supported. Currently we only support `gemini-pro` and `gemini-1.0-pro`"
-            
+                raise f"Model not supported. Currently we only support: {','.join(VALID_MODEL_SUPPORT)}."
             
             genai.configure(api_key = self.google_api_key)
             self.client = genai.GenerativeModel(model_name=self.model_name,
                                                 generation_config=self.model_kwargs)
 
         except Exception as e:
             raise Exception("Failed to load the model from Gemini Google Generative AI:", str(e))
 
-
-    def predict(self,prompt:Any):
-        response = self.client.generate_content(prompt)
+    def vision(self,image: Image ,prompt:Optional[str] = None):
+        if prompt:
+            response = self.client.generate_content([prompt,image])
+        else:
+            response = self.client.generate_content(image)
         return response.text
     
     @staticmethod
     def load_from_kwargs(self,kwargs): 
         model_config = ModelConfig(**kwargs)
         self.config = model_config
         self.load_llm()
```

### Comparing `beyondllm-0.0.1/src/beyondllm/llms/hf.py` & `beyondllm-0.2.0/src/beyondllm/llms/hf.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/llms/ollama.py` & `beyondllm-0.2.0/src/beyondllm/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/loaders/base.py` & `beyondllm-0.2.0/src/beyondllm/loaders/base.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/loaders/llamaParseLoader.py` & `beyondllm-0.2.0/src/beyondllm/loaders/llamaParseLoader.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/loaders/notionLoader.py` & `beyondllm-0.2.0/src/beyondllm/loaders/notionLoader.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/loaders/simpleLoader.py` & `beyondllm-0.2.0/src/beyondllm/loaders/simpleLoader.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/loaders/urlLoader.py` & `beyondllm-0.2.0/src/beyondllm/loaders/urlLoader.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/loaders/youtubeLoader.py` & `beyondllm-0.2.0/src/beyondllm/loaders/youtubeLoader.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/retrieve.py` & `beyondllm-0.2.0/src/beyondllm/retrieve.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,51 +2,53 @@
 os.environ['TOKENIZERS_PARALLELISM'] = 'true'
 
 from beyondllm.embeddings import GeminiEmbeddings
 from beyondllm.retrievers.normalRetriever import NormalRetriever
 from beyondllm.retrievers.utils import generate_qa_dataset, evaluate_from_dataset
 import pandas as pd
 
-def auto_retriever(data,embed_model=None,type="normal",top_k=4,**kwargs):
+def auto_retriever(data=None,embed_model=None,type="normal",top_k=4,vectordb=None,**kwargs):
     """
     Automatically selects and initializes a retriever based on the specified type.
     Parameters:
         data: The dataset to be used by the retriever for information retrieval.
         embed_model: The embedding model to be used for generating embeddings. 
            - Default Embedding: Fast Embeddings
         type (str): The type of retriever to use. Options include 'normal', 'flag-rerank', 
                     'cross-rerank', and 'hybrid'. Defaults to 'normal'.
         top_k (int): The number of top results to retrieve. Defaults to 4.
+        vectordb (VectorDb): The vectordb to use for retrieval
     Additional parameters:
         reranker: Name of the reranking model to be used. To be specified only for type = 'flag-rerank' and 'cross-rerank'
         mode: Possible options are 'AND' or 'OR'. To be specified only for type = 'hybrid. 'AND' mode will retrieve nodes in common between
                     keyword and vector retriever. top_k will be overridden in this case.
     Returns:
         A BaseRetriever instance.
     Example:
         from beyondllm.retrieve import auto_retriever
         
         data = <your dataset here>
         embed_model = <pass your embed model here>
+        vector_store = <pass your vector-store object here>
         
-        retriever = auto_retriever(data=data, embed_model=embed_model, type="normal", top_k=5)
+        retriever = auto_retriever(data=data, embed_model=embed_model, type="normal", top_k=5, vectordb=vector_store)
     """
     if embed_model is None:
         embed_model = GeminiEmbeddings()
     if type == 'normal':
-        retriever = NormalRetriever(data,embed_model,top_k,**kwargs)
+        retriever = NormalRetriever(data,embed_model,top_k,vectordb,**kwargs)
     elif type == 'flag-rerank':
         from .retrievers.flagReranker import FlagEmbeddingRerankRetriever
-        retriever = FlagEmbeddingRerankRetriever(data,embed_model,top_k,**kwargs)
+        retriever = FlagEmbeddingRerankRetriever(data,embed_model,top_k,vectordb,**kwargs)
     elif type == 'cross-rerank':
         from .retrievers.crossEncoderReranker import CrossEncoderRerankRetriever
-        retriever = CrossEncoderRerankRetriever(data,embed_model,top_k,**kwargs)
+        retriever = CrossEncoderRerankRetriever(data,embed_model,top_k,vectordb,**kwargs)
     elif type == 'hybrid':
         from .retrievers.hybridRetriever import HybridRetriever
-        retriever = HybridRetriever(data,embed_model,top_k,**kwargs)
+        retriever = HybridRetriever(data,embed_model,top_k,vectordb,**kwargs)
     else:
         raise NotImplementedError(f"Retriever for the type '{type}' is not implemented.")
 
     return retriever
 
 # def compare_retrievers(data,llm, retrievers_list):
 #     """
```

### Comparing `beyondllm-0.0.1/src/beyondllm/retrievers/base.py` & `beyondllm-0.2.0/src/beyondllm/retrievers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,20 @@
     """
     A base class for creating retrievers that can load indexes and perform retrieval operations.
     
     Attributes:
         data: The dataset to be indexed or retrieved from.
         embed_model: The embedding model used to generate embeddings for the data.
         top_k: The top k similarity search results to be retrieved
+        vectordb: The vectordb to be used for retrieval
     """
-    def __init__(self, data, embed_model,**kwargs):
+    def __init__(self, data, embed_model, vectordb, **kwargs):
         self.data = data
         self.embed_model = embed_model
+        self.vectordb = vectordb
 
     def load_index(self):
         raise NotImplementedError("This method should be implemented by subclasses.")
     
     def as_retriever(self):
         raise NotImplementedError("This method should be implemented by subclasses.")
```

### Comparing `beyondllm-0.0.1/src/beyondllm/retrievers/crossEncoderReranker.py` & `beyondllm-0.2.0/src/beyondllm/retrievers/crossEncoderReranker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from beyondllm.retrievers.base import BaseRetriever
-from llama_index.core import VectorStoreIndex, ServiceContext
+from llama_index.core import VectorStoreIndex, ServiceContext,StorageContext
 from llama_index.core.schema import QueryBundle
 import sys
 import subprocess
 try:
     from sentence_transformers import CrossEncoder
     from llama_index.core.postprocessor import SentenceTransformerRerank
 except ImportError:
@@ -41,18 +41,42 @@
         super().__init__(data, embed_model,*args, **kwargs)
         self.embed_model = embed_model
         self.data = data
         self.top_k = top_k
         self.reranker = kwargs.get('reranker',"cross-encoder/ms-marco-MiniLM-L-2-v2")
 
     def load_index(self):
-        service_context = ServiceContext.from_defaults(llm=None, embed_model=self.embed_model)
-        index = VectorStoreIndex(
-            self.data, service_context= service_context,
-        )
+        if self.data is None:
+            index = self.initialize_from_vector_store()
+        else:
+            index = self.initialize_from_data()
+
+        return index
+    
+    def initialize_from_vector_store(self):
+        if self.vectordb is None:
+            raise ValueError("Vector store must be provided if no data is passed")
+        else:
+            index = VectorStoreIndex.from_vector_store(
+                self.vectordb,
+                embed_model=self.embed_model,
+            )
+        return index
+
+
+    def initialize_from_data(self):
+        if self.vectordb==None:
+            index = VectorStoreIndex(
+                self.data, embed_model=self.embed_model
+            )
+        else:
+            storage_context = StorageContext.from_defaults(vector_store=self.vectordb)
+            index = VectorStoreIndex(
+                self.data, storage_context=storage_context, embed_model=self.embed_model
+            )
         return index
     
     def retrieve(self, query):
         retriever = self.as_retriever()
         unranked_nodes = retriever.retrieve(query)
 
         reranker = SentenceTransformerRerank(
```

### Comparing `beyondllm-0.0.1/src/beyondllm/retrievers/flagReranker.py` & `beyondllm-0.2.0/src/beyondllm/retrievers/flagReranker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from beyondllm.retrievers.base import BaseRetriever
-from llama_index.core import VectorStoreIndex, ServiceContext
+from llama_index.core import VectorStoreIndex, ServiceContext, StorageContext
 import sys
 import subprocess
 try:
     from llama_index.postprocessor.flag_embedding_reranker import FlagEmbeddingReranker
 except ImportError:
     user_agree = input("The feature you're trying to use requires a additional libraries:llama-index-postprocessor-flag-embedding-reranker, FlagEmbedding Would you like to install it now? [y/N]: ")
     if user_agree.lower() == 'y':
@@ -40,18 +40,42 @@
         super().__init__(data, embed_model,*args, **kwargs)
         self.embed_model = embed_model
         self.data = data
         self.top_k = top_k
         self.reranker = kwargs.get('reranker',"BAAI/bge-reranker-large")
 
     def load_index(self):
-        service_context = ServiceContext.from_defaults(llm=None, embed_model=self.embed_model)
-        index = VectorStoreIndex(
-            self.data, service_context= service_context,
-        )
+        if self.data is None:
+            index = self.initialize_from_vector_store()
+        else:
+            index = self.initialize_from_data()
+
+        return index
+    
+    def initialize_from_vector_store(self):
+        if self.vectordb is None:
+            raise ValueError("Vector store must be provided if no data is passed")
+        else:
+            index = VectorStoreIndex.from_vector_store(
+                self.vectordb,
+                embed_model=self.embed_model,
+            )
+        return index
+
+
+    def initialize_from_data(self):
+        if self.vectordb==None:
+            index = VectorStoreIndex(
+                self.data, embed_model=self.embed_model
+            )
+        else:
+            storage_context = StorageContext.from_defaults(vector_store=self.vectordb)
+            index = VectorStoreIndex(
+                self.data, storage_context=storage_context, embed_model=self.embed_model
+            )
         return index
     
     def retrieve(self, query):
         retriever = self.as_retriever()
         unranked_nodes = retriever.retrieve(query)
 
         reranker = FlagEmbeddingReranker(
```

### Comparing `beyondllm-0.0.1/src/beyondllm/retrievers/hybridRetriever.py` & `beyondllm-0.2.0/src/beyondllm/retrievers/hybridRetriever.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,22 +84,37 @@
         self.top_k = top_k
         self.mode = kwargs.get('mode', 'AND')  
 
         if self.mode not in ['AND', 'OR']:
             raise ValueError("Invalid mode. Mode must be 'AND' or 'OR'.")
 
     def load_index(self):
-        service_context = ServiceContext.from_defaults(llm=None, embed_model=self.embed_model)
-        storage_context = StorageContext.from_defaults()
-        vector_index = VectorStoreIndex(
-            self.data, service_context= service_context, storage_context=storage_context
-        )
-        keyword_index = SimpleKeywordTableIndex(
-            self.data,service_context=service_context,storage_context=storage_context
-        )
+        if self.data is None:
+            raise ValueError("Data needs to be passed for keyword retrieval.")
+        else:
+            vector_index, keyword_index = self.initialize_from_data()
+
+        return vector_index, keyword_index
+
+    def initialize_from_data(self):
+        if self.vectordb==None:
+            vector_index = VectorStoreIndex(
+                self.data, embed_model=self.embed_model
+            )
+            keyword_index = SimpleKeywordTableIndex(
+                self.data, service_context=ServiceContext.from_defaults(llm=None,embed_model=None)
+            )
+        else:
+            storage_context = StorageContext.from_defaults(vector_store=self.vectordb)
+            vector_index = VectorStoreIndex(
+                self.data, storage_context=storage_context, embed_model=self.embed_model
+            )
+            keyword_index = SimpleKeywordTableIndex(
+                self.data, service_context=ServiceContext.from_defaults(llm=None,embed_model=None)
+            )
         return vector_index, keyword_index
     
     def as_retriever(self):
         vector_index, keyword_index = self.load_index()
 
         vector_retriever = vector_index.as_retriever(similarity_top_k=self.top_k)
         keyword_retriever = keyword_index.as_retriever(similarity_top_k=self.top_k)
```

### Comparing `beyondllm-0.0.1/src/beyondllm/retrievers/normalRetriever.py` & `beyondllm-0.2.0/src/beyondllm/retrievers/normalRetriever.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,70 @@
 from beyondllm.retrievers.base import BaseRetriever
-from llama_index.core import VectorStoreIndex, ServiceContext
+from llama_index.core import VectorStoreIndex, ServiceContext, StorageContext
 
 class NormalRetriever(BaseRetriever):
     """
     A simple retriever that uses vector similarity search to retrieve relevant documents.
 
     Example:
         from beyondllm.retrieve import auto_retrievers
 
         data = ...  # Load your data
         embed_model = # Load your embed model
         retriever = auto_retriever(data=data, embed_model=embed_model, type="normal", top_k=5)
 
         results = retriever.retrieve("<your query>")
     """
-    def __init__(self, data, embed_model, top_k,*args, **kwargs):
+    def __init__(self, data, embed_model, top_k, vectordb,*args, **kwargs):
         """
         Initializes a NormalRetriever instance.
 
         Args:
             data: The dataset to be indexed.
             embed_model: The embedding model to use.
             top_k: The number of top results to retrieve.
+            vectordb: The vectordb to use for retrieval
         """
-        super().__init__(data, embed_model,*args, **kwargs)
+        super().__init__(data, embed_model, vectordb,*args, **kwargs)
         self.embed_model = embed_model
         self.data = data
         self.top_k = top_k
+        self.vectordb = vectordb
 
     def load_index(self):
-        service_context = ServiceContext.from_defaults(llm=None, embed_model=self.embed_model)
-        index = VectorStoreIndex(
-            self.data, service_context= service_context
-        )
+        if self.data is None:
+            index = self.initialize_from_vector_store()
+        else:
+            index = self.initialize_from_data()
+
         return index
     
+    def initialize_from_vector_store(self):
+        if self.vectordb is None:
+            raise ValueError("Vector store must be provided if no data is passed")
+        else:
+            index = VectorStoreIndex.from_vector_store(
+                self.vectordb,
+                embed_model=self.embed_model,
+            )
+        return index
+
+
+    def initialize_from_data(self):
+        if self.vectordb==None:
+            index = VectorStoreIndex(
+                self.data, embed_model=self.embed_model
+            )
+        else:
+            storage_context = StorageContext.from_defaults(vector_store=self.vectordb)
+            index = VectorStoreIndex(
+                self.data, storage_context=storage_context, embed_model=self.embed_model
+            )
+        return index
+
     def retrieve(self, query):
         retriever = self.as_retriever()
         return retriever.retrieve(query)
 
     def as_retriever(self):
         index = self.load_index()
```

### Comparing `beyondllm-0.0.1/src/beyondllm/retrievers/utils.py` & `beyondllm-0.2.0/src/beyondllm/retrievers/utils.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/source.py` & `beyondllm-0.2.0/src/beyondllm/source.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/src/beyondllm/utils.py` & `beyondllm-0.2.0/src/beyondllm/utils.py`

 * *Files identical despite different names*

### Comparing `beyondllm-0.0.1/PKG-INFO` & `beyondllm-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: beyondllm
-Version: 0.0.1
+Version: 0.2.0
 Summary: Beyond LLM is an toolkit to Build Experiment Evaluate and Observe RAG pipelines
 Author: AI Planet
 Author-email: tech@aiplanet.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llama-index (==0.10.27)
 Requires-Dist: llama-index-embeddings-gemini (==0.1.6)
 Requires-Dist: nltk (==3.8.1)
 Requires-Dist: numpy (==1.26.4)
 Requires-Dist: openai (==1.20.0)
 Requires-Dist: pandas (==2.0.3)
-Requires-Dist: pydantic (==2.7.0)
+Requires-Dist: pydantic (>=1.10.5,<2)
 Requires-Dist: pypdf (==4.2.0)
 Requires-Dist: pysbd (==0.3.4)
 Requires-Dist: pyyaml (==6.0.1)
 Requires-Dist: regex (==2024.4.16)
 Requires-Dist: sqlalchemy (==2.0.29)
 Requires-Dist: tiktoken (==0.6.0)
 Description-Content-Type: text/markdown
@@ -29,66 +29,31 @@
 <h2 align="center">Build - Rapid Experiment - Evaluate - Repeat</h2>
 
 ![Thumbnails](https://github.com/aiplanethub/beyondllm/assets/132284203/489bb644-f87e-4477-a639-a63552f84cd7)
 
 <a href="https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-3776AB.svg?style=flat&logo=python&logoColor=white"><img src="https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python Versions"></a>
 <a href="https://discord.gg/4aWV7He2QU"><img src="https://dcbadge.vercel.app/api/server/4aWV7He2QU?style=flat" alt="Discord" /></a>
 <a href="https://twitter.com/aiplanethub"><img src="https://img.shields.io/twitter/follow/aiplanethub" alt="Twitter" /></a>
-<a href="https://colab.research.google.com/drive/1dJZF5113e5XQsm6GxuW3ShYCBZcUs3-_?usp=sharing" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Try an example"/></a>
+<a href="https://colab.research.google.com/drive/1S1UL2uCahHkfJsurRA3f7dcR6IHjg-IM?usp=sharing" target="_blank"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Try an example"/></a>
 
-[![GitHub stars](https://img.shields.io/github/stars/aiplanethub/beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/)
-[![License](https://img.shields.io/github/license/aiplanethub/beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/blob/main/LICENSE)
-[![Contributors](https://img.shields.io/github/contributors/username/repo.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/graphs/contributors)
+[![Contributors](https://img.shields.io/github/contributors/aiplanethub/beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/graphs/contributors)
 [![Code of Conduct](https://img.shields.io/badge/code%20of%20conduct-contributor%20covenant-green.svg?style=flat-square)](CODE_OF_CONDUCT.md)
 
 <p>Beyond LLM offers an all-in-one toolkit for experimentation, evaluation, and deployment of Retrieval-Augmented Generation (RAG) systems, simplifying the process with automated integration, customizable evaluation metrics, and support for various Large Language Models (LLMs) tailored to specific needs, ultimately aiming to reduce LLM hallucination risks and enhance reliability.</p>
 <i><a href="https://discord.gg/4aWV7He2QU">👉 Join our Discord community!</a></i>
 </div>
 
 Try out a quick demo on Google Colab:
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1dJZF5113e5XQsm6GxuW3ShYCBZcUs3-_?usp=sharing)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1S1UL2uCahHkfJsurRA3f7dcR6IHjg-IM?usp=sharing)
 
 ## Quick install
 
-1. To install Beyond LLM i.e., a private repo, we can use Access Token of GitHub. 
-
-   ```bash
-   git clone https://<UPDATE-WITH-YOUR-TOKEN>@github.com/aiplanethub/beyondllm.git
-   ```
-
-3. Go to the project directory
-
-   ```bash
-   cd beyondllm
-   ```
-
-4. Install the package
-
-   ```bash
-   pip install .
-   ```
-
-   OR,
-
-   ```bash
-   pip install -e .
-   ```
-
-   When using the `-e` flag, the package is installed in editable mode. This means that if you make changes to the source code, you do not need to reinstall the package for the changes to take effect.
-
-Install on Google Colab
-
 ```bash
-!git clone https://<UPDATE-WITH-YOUR-TOKEN>@github.com/aiplanethub/beyondllm.git
-
-%cd /content/beyondllm/
-
-pip install .
-
+pip install beyondllm
 ```
 
 ## Quickstart Guide- Chat with YouTube Video
 
 In this quick start guide, we'll demonstrate how to create a Chat with YouTube video RAG application using Beyond LLM with less than 8 lines of code. This 8 lines of code includes:
 * Getting custom data source
 * Retrieving documents
@@ -142,24 +107,35 @@
 MRR:1.0
 
 Context relevancy Score: 8.0
 Answer relevancy Score: 7.0
 Groundness score: 7.666666666666667
 ```
 
-## Get in Touch
+## Documentation
+
+See the [beyondllm.aiplanet.com](https://beyondllm.aiplanet.com/) for complete documentation.
 
-You can schedule a 1:1 meeting with our Team to get started with GenAI Stack, OpenAGI, AI Planet Open Source LLMs(Buddhi, effi and Panda Coder) and Beyond LLM. Schedule the call here: [https://calendly.com/jaintarun](https://calendly.com/jaintarun)
 
 ## Contribution guidelines
 
 Beyond LLM thrives in the rapidly evolving landscape of open-source projects. We wholeheartedly welcome contributions in various capacities, be it through innovative features, enhanced infrastructure, or refined documentation.
 
+See [Contributing guide](https://github.com/aiplanethub/beyondllm/blob/main/CONTRIBUTING.md) for more information on contributing to the BeyondLLM library. 
+
 ## Acknowledgements
 
 * [HuggingFace](https://github.com/huggingface)
 * [LlamaIndex](https://github.com/jerryjliu/llama_index)
 * [OpenAI](https://github.com/openai)
 * [Google Gemini](https://ai.google.dev/)
   
 and the entire OpenSource community.
 
+## License
+
+The contents of this repository are licensed under the [Apache License, version 2.0](https://github.com/aiplanethub/beyondllm/blob/main/LICENSE).
+
+## Get in Touch
+
+You can schedule a 1:1 meeting with our Team to get started with GenAI Stack, OpenAGI, AI Planet Open Source LLMs(Buddhi, effi and Panda Coder) and Beyond LLM. Schedule the call here: [https://calendly.com/jaintarun](https://calendly.com/jaintarun)
+
```

#### html2text {}

```diff
@@ -1,59 +1,48 @@
-Metadata-Version: 2.1 Name: beyondllm Version: 0.0.1 Summary: Beyond LLM is an
+Metadata-Version: 2.1 Name: beyondllm Version: 0.2.0 Summary: Beyond LLM is an
 toolkit to Build Experiment Evaluate and Observe RAG pipelines Author: AI
 Planet Author-email: tech@aiplanet.com Requires-Python: >=3.9,<3.12 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: llama-index (==0.10.27)
 Requires-Dist: llama-index-embeddings-gemini (==0.1.6) Requires-Dist: nltk
 (==3.8.1) Requires-Dist: numpy (==1.26.4) Requires-Dist: openai (==1.20.0)
-Requires-Dist: pandas (==2.0.3) Requires-Dist: pydantic (==2.7.0) Requires-
+Requires-Dist: pandas (==2.0.3) Requires-Dist: pydantic (>=1.10.5,<2) Requires-
 Dist: pypdf (==4.2.0) Requires-Dist: pysbd (==0.3.4) Requires-Dist: pyyaml
 (==6.0.1) Requires-Dist: regex (==2024.4.16) Requires-Dist: sqlalchemy
 (==2.0.29) Requires-Dist: tiktoken (==0.6.0) Description-Content-Type: text/
 markdown
                             ************ BBeeyyoonnddLLLLMM ************
            ********** BBuuiilldd -- RRaappiidd EExxppeerriimmeenntt -- EEvvaalluuaattee -- RReeppeeaatt **********
    ![Thumbnails](https://github.com/aiplanethub/beyondllm/assets/132284203/
  489bb644-f87e-4477-a639-a63552f84cd7) _[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_D_i_s_c_o_r_d_]_[_T_w_i_t_t_e_r_]_[_T_r_y
- _a_n_ _e_x_a_m_p_l_e_][![GitHub stars](https://img.shields.io/github/stars/aiplanethub/
-beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/) [!
-         [License](https://img.shields.io/github/license/aiplanethub/
-  beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/
-blob/main/LICENSE) [![Contributors](https://img.shields.io/github/contributors/
-username/repo.svg?style=flat-square)](https://github.com/aiplanethub/beyondllm/
-    graphs/contributors) [![Code of Conduct](https://img.shields.io/badge/
-   code%20of%20conduct-contributor%20covenant-green.svg?style=flat-square)]
+    _a_n_ _e_x_a_m_p_l_e_][![Contributors](https://img.shields.io/github/contributors/
+ aiplanethub/beyondllm.svg?style=flat-square)](https://github.com/aiplanethub/
+  beyondllm/graphs/contributors) [![Code of Conduct](https://img.shields.io/
+badge/code%20of%20conduct-contributor%20covenant-green.svg?style=flat-square)]
                              (CODE_OF_CONDUCT.md)
  Beyond LLM offers an all-in-one toolkit for experimentation, evaluation, and
   deployment of Retrieval-Augmented Generation (RAG) systems, simplifying the
    process with automated integration, customizable evaluation metrics, and
  support for various Large Language Models (LLMs) tailored to specific needs,
  ultimately aiming to reduce LLM hallucination risks and enhance reliability.
                        _ð____ _J_o_i_n_ _o_u_r_ _D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_!
 Try out a quick demo on Google Colab: [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1dJZF5113e5XQsm6GxuW3ShYCBZcUs3-_?usp=sharing)
-## Quick install 1. To install Beyond LLM i.e., a private repo, we can use
-Access Token of GitHub. ```bash git clone https://@github.com/aiplanethub/
-beyondllm.git ``` 3. Go to the project directory ```bash cd beyondllm ``` 4.
-Install the package ```bash pip install . ``` OR, ```bash pip install -e . ```
-When using the `-e` flag, the package is installed in editable mode. This means
-that if you make changes to the source code, you do not need to reinstall the
-package for the changes to take effect. Install on Google Colab ```bash !git
-clone https://@github.com/aiplanethub/beyondllm.git %cd /content/beyondllm/ pip
-install . ``` ## Quickstart Guide- Chat with YouTube Video In this quick start
-guide, we'll demonstrate how to create a Chat with YouTube video RAG
-application using Beyond LLM with less than 8 lines of code. This 8 lines of
-code includes: * Getting custom data source * Retrieving documents * Generating
-LLM responses * Evaluating embeddings * Evaluating LLM responses ### Approach-
-1: Using Default LLM and Embeddings Build customised RAG in less than ``5 lines
-of code`` using Beyond LLM. ```python from beyondllm import
-source,retrieve,generator import os os.environ['GOOGLE_API_KEY'] = "Your Google
-API Key:" data = source.fit("https://www.youtube.com/
+colab.research.google.com/drive/1S1UL2uCahHkfJsurRA3f7dcR6IHjg-IM?usp=sharing)
+## Quick install ```bash pip install beyondllm ``` ## Quickstart Guide- Chat
+with YouTube Video In this quick start guide, we'll demonstrate how to create a
+Chat with YouTube video RAG application using Beyond LLM with less than 8 lines
+of code. This 8 lines of code includes: * Getting custom data source *
+Retrieving documents * Generating LLM responses * Evaluating embeddings *
+Evaluating LLM responses ### Approach-1: Using Default LLM and Embeddings Build
+customised RAG in less than ``5 lines of code`` using Beyond LLM. ```python
+from beyondllm import source,retrieve,generator import os os.environ
+['GOOGLE_API_KEY'] = "Your Google API Key:" data = source.fit("https://
+www.youtube.com/
 watch?v=oJJyTztI_6g",dtype="youtube",chunk_size=512,chunk_overlap=50) retriever
 = retrieve.auto_retriever(data,type="normal",top_k=3) pipeline =
 generator.Generate(question="what tool is video mentioning
 about?",retriever=retriever) print(pipeline.call()) ``` ### Approach-2: With
 Custom LLM and Embeddings Beyond LLM support various Embeddings and LLMs that
 are two very important components in Retrieval Augmented Generation. ```python
 from beyondllm import source,retrieve,embeddings,llms,generator import os from
@@ -69,17 +58,23 @@
 ```bash The tool mentioned in the context is called Jupiter, which is an AI
 Guru designed to simplify the learning of complex data science topics. Users
 can access Jupiter by logging into AI Planet, accessing any course for free,
 and then requesting explanations of topics from Jupiter in various styles, such
 as in the form of a movie plot. Jupiter aims to make AI education more
 accessible and interactive for everyone. Hit_rate:1.0 MRR:1.0 Context relevancy
 Score: 8.0 Answer relevancy Score: 7.0 Groundness score: 7.666666666666667 ```
-## Get in Touch You can schedule a 1:1 meeting with our Team to get started
-with GenAI Stack, OpenAGI, AI Planet Open Source LLMs(Buddhi, effi and Panda
-Coder) and Beyond LLM. Schedule the call here: [https://calendly.com/jaintarun]
-(https://calendly.com/jaintarun) ## Contribution guidelines Beyond LLM thrives
-in the rapidly evolving landscape of open-source projects. We wholeheartedly
-welcome contributions in various capacities, be it through innovative features,
-enhanced infrastructure, or refined documentation. ## Acknowledgements *
-[HuggingFace](https://github.com/huggingface) * [LlamaIndex](https://
-github.com/jerryjliu/llama_index) * [OpenAI](https://github.com/openai) *
-[Google Gemini](https://ai.google.dev/) and the entire OpenSource community.
+## Documentation See the [beyondllm.aiplanet.com](https://
+beyondllm.aiplanet.com/) for complete documentation. ## Contribution guidelines
+Beyond LLM thrives in the rapidly evolving landscape of open-source projects.
+We wholeheartedly welcome contributions in various capacities, be it through
+innovative features, enhanced infrastructure, or refined documentation. See
+[Contributing guide](https://github.com/aiplanethub/beyondllm/blob/main/
+CONTRIBUTING.md) for more information on contributing to the BeyondLLM library.
+## Acknowledgements * [HuggingFace](https://github.com/huggingface) *
+[LlamaIndex](https://github.com/jerryjliu/llama_index) * [OpenAI](https://
+github.com/openai) * [Google Gemini](https://ai.google.dev/) and the entire
+OpenSource community. ## License The contents of this repository are licensed
+under the [Apache License, version 2.0](https://github.com/aiplanethub/
+beyondllm/blob/main/LICENSE). ## Get in Touch You can schedule a 1:1 meeting
+with our Team to get started with GenAI Stack, OpenAGI, AI Planet Open Source
+LLMs(Buddhi, effi and Panda Coder) and Beyond LLM. Schedule the call here:
+[https://calendly.com/jaintarun](https://calendly.com/jaintarun)
```

