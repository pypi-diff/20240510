# Comparing `tmp/turkish-lm-tuner-0.1.1.tar.gz` & `tmp/turkish_lm_tuner-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turkish-lm-tuner-0.1.1.tar", last modified: Mon Feb  5 07:53:32 2024, max compression
+gzip compressed data, was "turkish_lm_tuner-0.1.2.tar", last modified: Fri May 10 08:32:52 2024, max compression
```

## Comparing `turkish-lm-tuner-0.1.1.tar` & `turkish_lm_tuner-0.1.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 07:53:32.204254 turkish-lm-tuner-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 07:53:32.188254 turkish-lm-tuner-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 07:53:32.188254 turkish-lm-tuner-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/BuildREADME.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-02-05 07:53:32.200254 turkish-lm-tuner-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 07:53:32.192254 turkish-lm-tuner-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 07:53:32.192254 turkish-lm-tuner-0.1.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/docs/tutorials/evaluation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/docs/tutorials/finetuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/docs/tutorials/getting-started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/docs/tutorials/inference.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 07:53:32.192254 turkish-lm-tuner-0.1.1/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/compute_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 07:53:32.196254 turkish-lm-tuner-0.1.1/experiments/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/class_prod_reviews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/class_ttc4900.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/class_tweet_sentiment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/default_classification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/default_cond_gen.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/ner_milliyet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/ner_milliyet_token.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/ner_wikiann.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/ner_wikiann_token.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/nli_multinli_tr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/nli_snli_tr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/nli_tr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/paraphrasing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/pos_boun.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/pos_boun_token.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/pos_imst.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/pos_imst_token.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/qa_exams.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/qa_mkqa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/qa_tquad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/semantic_similarity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/summarization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/conf/title_generation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/finetune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 07:53:32.200254 turkish-lm-tuner-0.1.1/experiments/generation_conf/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/class_prod_reviews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/class_ttc4900.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/default_classification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/default_cond_gen.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/ner_milliyet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/ner_wikiann.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/nli_snli_tr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/nli_tr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/paraphrasing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/pos_boun.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/pos_imst.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/qa_exams.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/qa_mkqa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/qa_tquad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/semantic_similarity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/summarization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/generation_conf/title_generation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/ner_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/push_to_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 07:53:32.200254 turkish-lm-tuner-0.1.1/experiments/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/scripts/compute_lengths.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/scripts/evaluate.sh
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/experiments/scripts/finetune.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 07:53:32.204254 turkish-lm-tuner-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 07:53:32.200254 turkish-lm-tuner-0.1.1/turkish_lm_tuner/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner/dataset_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner/t5_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    33575 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner/tr_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-02-05 07:53:22.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 07:53:32.200254 turkish-lm-tuner-0.1.1/turkish_lm_tuner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-02-05 07:53:32.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-02-05 07:53:32.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 07:53:32.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 07:53:31.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-05 07:53:32.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 07:53:32.000000 turkish-lm-tuner-0.1.1/turkish_lm_tuner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:52.164789 turkish_lm_tuner-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:52.148789 turkish_lm_tuner-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:52.152789 turkish_lm_tuner-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/BuildREADME.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-10 08:32:52.164789 turkish_lm_tuner-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:52.152789 turkish_lm_tuner-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:52.152789 turkish_lm_tuner-0.1.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/docs/tutorials/evaluation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/docs/tutorials/finetuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/docs/tutorials/getting-started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/docs/tutorials/inference.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:52.156789 turkish_lm_tuner-0.1.2/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/compute_lengths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:52.160789 turkish_lm_tuner-0.1.2/experiments/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/class_prod_reviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/class_ttc4900.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/class_tweet_sentiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/default_classification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/default_cond_gen.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/ner_milliyet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/ner_milliyet_token.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/ner_wikiann.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/ner_wikiann_token.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/nli_multinli_tr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/nli_snli_tr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/nli_tr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/paraphrasing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/pos_boun.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/pos_boun_token.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/pos_imst.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/pos_imst_token.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/qa_exams.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/qa_mkqa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/qa_tquad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/semantic_similarity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/summarization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/conf/title_generation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/finetune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:52.160789 turkish_lm_tuner-0.1.2/experiments/generation_conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/class_prod_reviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/class_ttc4900.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/default_classification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/default_cond_gen.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/ner_milliyet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/ner_wikiann.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/nli_snli_tr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/nli_tr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/paraphrasing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/pos_boun.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/pos_imst.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/qa_exams.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/qa_mkqa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/qa_tquad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/semantic_similarity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/summarization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/generation_conf/title_generation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/ner_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/push_to_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:52.164789 turkish_lm_tuner-0.1.2/experiments/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/scripts/compute_lengths.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/scripts/evaluate.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/experiments/scripts/finetune.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:32:52.164789 turkish_lm_tuner-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:52.164789 turkish_lm_tuner-0.1.2/turkish_lm_tuner/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner/dataset_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner/t5_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33724 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner/tr_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-05-10 08:32:47.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:32:52.164789 turkish_lm_tuner-0.1.2/turkish_lm_tuner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-10 08:32:52.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-10 08:32:52.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:32:52.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:32:51.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-10 08:32:52.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 08:32:52.000000 turkish_lm_tuner-0.1.2/turkish_lm_tuner.egg-info/top_level.txt
```

### Comparing `turkish-lm-tuner-0.1.1/.github/workflows/doc.yml` & `turkish_lm_tuner-0.1.2/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/.github/workflows/publish.yml` & `turkish_lm_tuner-0.1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/.gitignore` & `turkish_lm_tuner-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/BuildREADME.md` & `turkish_lm_tuner-0.1.2/BuildREADME.md`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/LICENSE` & `turkish_lm_tuner-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/PKG-INFO` & `turkish_lm_tuner-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkish-lm-tuner
-Version: 0.1.1
+Version: 0.1.2
 Summary: Implementation of the Turkish LM Tuner
 Author-email: Gökçe Uludoğan <gokceuludogan@gmail.com>, Zeynep Yirmibeşoğlu Balal <yirmibesogluz@gmail.com>, Furkan Akkurt <furkanakkurt9285@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/boun-tabi-LMG/turkish-lm-tuner
 Project-URL: Bug Tracker, https://github.com/boun-tabi-LMG/turkish-lm-tuner/issues
 Project-URL: Documentation, https://turkish-lm-tuner-docs.boun-tabi-LMG.github.io/
 Keywords: nlp,turkish,language models,finetuning
@@ -121,15 +121,15 @@
 )
 
 train_dataset = dataset_processor.load_and_preprocess_data(split='train')
 eval_dataset = dataset_processor.load_and_preprocess_data(split='validation')
 test_dataset = dataset_processor.load_and_preprocess_data(split="test")
 
 training_params = {
-    'num_train_epochs': 10
+    'num_train_epochs': 10,
     'per_device_train_batch_size': 4,
     'per_device_eval_batch_size': 4,
     'output_dir': './', 
     'evaluation_strategy': 'epoch',
     'save_strategy': 'epoch',
     'predict_with_generate': True    
 }
@@ -170,15 +170,17 @@
     dataset_name, task, task_format, task_mode,
     model_name, max_input_length, max_target_length
 )
 
 test_dataset = dataset_processor.load_and_preprocess_data(split="test")
 
 test_params = {
-    'per_device_eval_batch_size': 4
+    'per_device_eval_batch_size': 4,
+    'output_dir': './',
+    'predict_with_generate': True
 }
 
 model_path = "turna_tr_news_summarization"
 generation_params = {
     'num_beams': 4,
     'length_penalty': 2.0,
     'no_repeat_ngram_size': 3,
@@ -195,15 +197,15 @@
 ```
 
 ## Reference
 
 If you use this repository, please cite the following related [paper](https://arxiv.org/abs/2401.14373):
 
 ```bibtex
-@misc{uludoğan2024turna,
+@misc{uludogan2024turna,
       title={TURNA: A Turkish Encoder-Decoder Language Model for Enhanced Understanding and Generation}, 
       author={Gökçe Uludoğan and Zeynep Yirmibeşoğlu Balal and Furkan Akkurt and Melikşah Türker and Onur Güngör and Susan Üsküdarlı},
       year={2024},
       eprint={2401.14373},
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
```

### Comparing `turkish-lm-tuner-0.1.1/README.md` & `turkish_lm_tuner-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 )
 
 train_dataset = dataset_processor.load_and_preprocess_data(split='train')
 eval_dataset = dataset_processor.load_and_preprocess_data(split='validation')
 test_dataset = dataset_processor.load_and_preprocess_data(split="test")
 
 training_params = {
-    'num_train_epochs': 10
+    'num_train_epochs': 10,
     'per_device_train_batch_size': 4,
     'per_device_eval_batch_size': 4,
     'output_dir': './', 
     'evaluation_strategy': 'epoch',
     'save_strategy': 'epoch',
     'predict_with_generate': True    
 }
@@ -124,15 +124,17 @@
     dataset_name, task, task_format, task_mode,
     model_name, max_input_length, max_target_length
 )
 
 test_dataset = dataset_processor.load_and_preprocess_data(split="test")
 
 test_params = {
-    'per_device_eval_batch_size': 4
+    'per_device_eval_batch_size': 4,
+    'output_dir': './',
+    'predict_with_generate': True
 }
 
 model_path = "turna_tr_news_summarization"
 generation_params = {
     'num_beams': 4,
     'length_penalty': 2.0,
     'no_repeat_ngram_size': 3,
@@ -149,15 +151,15 @@
 ```
 
 ## Reference
 
 If you use this repository, please cite the following related [paper](https://arxiv.org/abs/2401.14373):
 
 ```bibtex
-@misc{uludoğan2024turna,
+@misc{uludogan2024turna,
       title={TURNA: A Turkish Encoder-Decoder Language Model for Enhanced Understanding and Generation}, 
       author={Gökçe Uludoğan and Zeynep Yirmibeşoğlu Balal and Furkan Akkurt and Melikşah Türker and Onur Güngör and Susan Üsküdarlı},
       year={2024},
       eprint={2401.14373},
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
```

### Comparing `turkish-lm-tuner-0.1.1/docs/index.md` & `turkish_lm_tuner-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/docs/license.md` & `turkish_lm_tuner-0.1.2/docs/license.md`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/docs/tutorials/evaluation.ipynb` & `turkish_lm_tuner-0.1.2/docs/tutorials/evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/docs/tutorials/finetuning.ipynb` & `turkish_lm_tuner-0.1.2/docs/tutorials/finetuning.ipynb`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/docs/tutorials/getting-started.ipynb` & `turkish_lm_tuner-0.1.2/docs/tutorials/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/docs/tutorials/inference.ipynb` & `turkish_lm_tuner-0.1.2/docs/tutorials/inference.ipynb`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/env.yml` & `turkish_lm_tuner-0.1.2/env.yml`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/experiments/README.md` & `turkish_lm_tuner-0.1.2/experiments/README.md`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/experiments/compute_lengths.py` & `turkish_lm_tuner-0.1.2/experiments/compute_lengths.py`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/experiments/conf/class_prod_reviews.yaml` & `turkish_lm_tuner-0.1.2/experiments/conf/class_prod_reviews.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 max_target_length: 4
 num_labels: 2
 training_params:
   per_device_train_batch_size: 32 # for ultramarine
   per_device_eval_batch_size: 32 # for ultramarine
   # Conditional generation mode: classification/cg/tr_product_reviews
   # Classification mode: classification/tc/tr_product_reviews
-  output_dir: /stratch/bounllm/finetuned-models/ul2tr/classification/cg/tr_product_reviews
+  output_dir: /finetuned-models/turna/classification/cg/tr_product_reviews
```

### Comparing `turkish-lm-tuner-0.1.1/experiments/conf/class_tweet_sentiment.yaml` & `turkish_lm_tuner-0.1.2/experiments/conf/class_tweet_sentiment.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 defaults:
   #- default_classification  
   - default_cond_gen # switch to this line for Conditional Generation
 
 dataset_name: 17bintweet_sentiment 
 task: classification
-dataset_loc: "/stratch/bounllm/supervised/17bintweet_sentiment/"
+dataset_loc: "/supervised/17bintweet_sentiment/"
 max_input_length: 160
 max_target_length: 4
 num_labels: 3
 training_params:
   per_device_train_batch_size: 32 # for ultramarine
   per_device_eval_batch_size: 32 # for ultramarine
   # Conditional generation mode: classification/cg/17bintweet_sentiment
   # Classification mode: classification/tc/17bintweet_sentiment
-  output_dir: /stratch/bounllm/finetuned-models/ul2tr/classification/cg/17bintweet_sentiment
+  output_dir: /finetuned-models/turna/classification/cg/17bintweet_sentiment
```

### Comparing `turkish-lm-tuner-0.1.1/experiments/eval.py` & `turkish_lm_tuner-0.1.2/experiments/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     task_format = cfg.task_format
     task_mode = cfg.task_mode
     max_input_length = cfg.max_input_length
     max_target_length = cfg.max_target_length
     test_params = cfg.test_params
     generation_params = cfg.generation_params
     dataset_location = cfg.dataset_loc
+    
+    if "num_labels" in cfg.keys():
+        num_labels = cfg.num_labels
 
     logger.info("Loading test dataset")
     dataset_processor = DatasetProcessor(dataset_name, task, task_format, task_mode, tokenizer_path, max_input_length, max_target_length, dataset_location)
     
     try:
         test_dataset = dataset_processor.load_and_preprocess_data(split="test")  # Use split="test[:10]" to test for small sample
         test_exists = True
@@ -65,15 +68,15 @@
     
 
     if task_format == 'conditional_generation':
         logger.info("Evaluating in conditional generation mode")
         evaluator = EvaluatorForConditionalGeneration(model_path, tokenizer_path, task, max_input_length, max_target_length, test_params, generation_params, postprocess_fn)
     elif task_format == 'classification':
         logger.info("Evaluating in classification mode")
-        evaluator = EvaluatorForClassification(model_path, tokenizer_path, task, test_params)
+        evaluator = EvaluatorForClassification(model_path, tokenizer_path, task, max_input_length, test_params, num_labels, postprocess_fn)
 
   
     logger.info("Evaluating model")
     results = evaluator.evaluate_model(test_dataset)
     logger.info("Result: %s", results)    
     json.dump(results.metrics, open(os.path.join(test_params['output_dir'], "results.json"), "w"))
```

### Comparing `turkish-lm-tuner-0.1.1/experiments/finetune.py` & `turkish_lm_tuner-0.1.2/experiments/finetune.py`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/experiments/ner_classification.py` & `turkish_lm_tuner-0.1.2/experiments/ner_classification.py`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/experiments/push_to_hub.py` & `turkish_lm_tuner-0.1.2/experiments/push_to_hub.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from huggingface_hub import create_repo
 
 # Set up the Hugging Face authentication token
 HF_AUTH_TOKEN = os.getenv('HF_AUTH_TOKEN')
 
 # Tokenizer mapping and model paths
 tokenizer_mapping = {
-    'ul2tr': '/stratch/bounllm/pretrained_checkpoints/ckpt-1.74M/',
+    'ul2tr': '/pretrained_checkpoints/ckpt-1.74M/',
     'mbart': 'facebook/mbart-large-cc25', 
     'mt5-large': 'google/mt5-large'
 }
 
 # List of completed tasks
 completed_tasks = ['summarization', 'paraphrasing', 'title_generation', 'semantic_similarity', 'nli', 'ner', 'pos']
 
@@ -31,20 +31,20 @@
         tokenizer.push_to_hub(repo_name, private=True, token=HF_AUTH_TOKEN)
     except Exception as e:
         print(f'Error during pushing {model_path}. Repo exists or an error occurred, check error: {e}')
 
 # Push pretrained models
 pretrained_models = ['1.74M', '1M', '500K']
 for model_version in pretrained_models:
-    model_path = f'/stratch/bounllm/pretrained_checkpoints/ckpt-{model_version}'
+    model_path = f'/pretrained_checkpoints/ckpt-{model_version}'
     repo_name = f'{organization}/turna-{model_version}'
     push_model_to_hub(repo_name, model_path, tokenizer_mapping['ul2tr'])
 
 # Push finetuned models
-path = Path('/stratch/bounllm/finetuned-models/')
+path = Path('/finetuned-models/')
 for model_dir in path.iterdir():
     if model_dir.name not in tokenizer_mapping:
         continue
 
     for task in model_dir.iterdir():
         if task.name not in completed_tasks:
             continue
```

### Comparing `turkish-lm-tuner-0.1.1/experiments/scripts/evaluate.sh` & `turkish_lm_tuner-0.1.2/experiments/scripts/evaluate.sh`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/experiments/scripts/finetune.sh` & `turkish_lm_tuner-0.1.2/experiments/scripts/finetune.sh`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/mkdocs.yml` & `turkish_lm_tuner-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/pyproject.toml` & `turkish_lm_tuner-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/turkish_lm_tuner/dataset_processor.py` & `turkish_lm_tuner-0.1.2/turkish_lm_tuner/dataset_processor.py`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/turkish_lm_tuner/evaluator.py` & `turkish_lm_tuner-0.1.2/turkish_lm_tuner/evaluator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from transformers import (
     AutoTokenizer, AutoModelForSeq2SeqLM, AutoModelForSequenceClassification,
     Seq2SeqTrainer, Seq2SeqTrainingArguments,
     Trainer, TrainingArguments,
-    EvalPrediction
+    EvalPrediction,
+    AutoConfig, AutoModel,
+    AutoModelForTokenClassification,
 )
 
+from .t5_classifier import T5ForClassification, T5ForClassificationConfig
+
+
 from .metrics import load_task_metrics
 import pandas as pd
 import numpy as np
 import os
 import logging
 
 logger = logging.getLogger(__name__)
@@ -59,19 +64,39 @@
         for metric in self.metrics:
             metric_scores = metric.compute(preds, labels)
             scores.update(metric_scores)
         return scores
 
 class EvaluatorForClassification(BaseEvaluator):
 
+    def __init__(self, model_path, tokenizer_path, task, max_input_length, test_params, num_labels, postprocess_fn=None):
+        super().__init__(model_path, tokenizer_path, task, test_params, postprocess_fn)
+        self.max_input_length = max_input_length
+        self.num_labels = num_labels
+    
     def initialize_model(self):
-        # If used without fine-tuning, model should be loaded from the model save path
-        return AutoModelForSequenceClassification.from_pretrained(self.model_path)
+        AutoConfig.register("t5_turna_enc", T5ForClassificationConfig)
+        AutoModel.register(T5ForClassificationConfig, T5ForClassification)
+        config = AutoConfig.from_pretrained(self.model_path)
+
+        if config.model_type in ["t5", "mt5", "t5_turna_enc"]:
+            if self.task == "classification":
+                return T5ForClassification.from_pretrained(self.model_path, config, self.num_labels, "single_label_classification")
+            elif self.task in ["ner", "pos_tagging"]:
+                return T5ForClassification.from_pretrained(self.model_path, config, self.num_labels, "token_classification")
+            else:
+                return T5ForClassification.from_pretrained(self.model_path, config, 1, "regression")
+        else:
+            if self.task == "classification":
+                return AutoModelForSequenceClassification.from_pretrained(self.model_path, num_labels=self.num_labels)
+            elif self.task in ["ner", "pos_tagging"]:
+                return AutoModelForTokenClassification.from_pretrained(self.model_path, num_labels=self.num_labels)
 
     def initialize_trainer(self, model):
+
         test_args = TrainingArguments(
             **self.test_params)
 
         trainer = Trainer(
             model=model,
             args=test_args,
             compute_metrics=self.compute_metrics,
```

### Comparing `turkish-lm-tuner-0.1.1/turkish_lm_tuner/metrics.py` & `turkish_lm_tuner-0.1.2/turkish_lm_tuner/metrics.py`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/turkish_lm_tuner/predictor.py` & `turkish_lm_tuner-0.1.2/turkish_lm_tuner/predictor.py`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/turkish_lm_tuner/t5_classifier.py` & `turkish_lm_tuner-0.1.2/turkish_lm_tuner/t5_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from torch import nn
-from transformers import T5EncoderModel
+from transformers import T5EncoderModel, PretrainedConfig
 from torch import nn
 from torch.nn import BCEWithLogitsLoss, CrossEntropyLoss, MSELoss
 from transformers.models.t5.modeling_t5 import T5PreTrainedModel
 
+class T5ForClassificationConfig(PretrainedConfig):
+    model_type="t5_turna_enc"
 
 class T5ForClassification(T5PreTrainedModel):   # nn.Module
+    config_class = T5ForClassificationConfig
     """
     T5 encoder adapted for classification
     Args:
         pretrained_model_name: Pretrained model name or path
         config: T5Config
         num_labels: Number of labels
         problem_type: Problem type. It can be either 'single_label_classification', 'multi_label_classification', 'token_classification' or 'regression'
         dropout_prob: Dropout probability
     """
     def __init__(self, pretrained_model_name, config, num_labels, problem_type, dropout_prob=0.1):
         super().__init__(config)
 
-        self.encoder = T5EncoderModel.from_pretrained(pretrained_model_name)
+        try:
+            self.encoder = T5EncoderModel.from_pretrained(pretrained_model_name)
+        except Exception as e:
+            pretrained_model_name = config._name_or_path
+            self.encoder = T5EncoderModel.from_pretrained(pretrained_model_name)
+
         self.dropout = nn.Dropout(dropout_prob)
         self.classifier = nn.Linear(self.encoder.config.d_model, num_labels)
         self.config = self.encoder.config
         self.config.num_labels = num_labels
         self.config.problem_type = problem_type
         self.config.dropout_prob = dropout_prob
```

### Comparing `turkish-lm-tuner-0.1.1/turkish_lm_tuner/tr_datasets.py` & `turkish_lm_tuner-0.1.2/turkish_lm_tuner/tr_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,19 @@
         return {"input_text": input, "target_text": output}
 
     def postprocess_data(self, examples):
         def convert_sts_label(label):
             try:
                 return(float(label.strip()))
             except:
-                return 0
+                try:
+                    return(float(label))
+                except:
+                    return 0
+
         return [convert_sts_label(ex) for ex in examples]
 
 class NLI_TRDataset(BaseDataset):
     DATASET_INFO = ("nli_tr", None)
     IN_LABEL_DICT = {0: "gereklilik", 1: "nötr", 2:"çelişki"}
     OUT_LABEL_DICT = {v: k for k, v in IN_LABEL_DICT.items()}
     def __init__(self, dataset_name=None):
@@ -656,15 +660,20 @@
     OUT_LABEL_DICT = None
 
     def __init__(self, dataset_name=None):
         super().__init__(dataset_name)
         self.OUT_LABEL_DICT = {v: k for k, v in self.IN_LABEL_DICT.items()}
 
     def postprocess_data(self, examples):
-        return [self.OUT_LABEL_DICT.get(ex.strip(), -1) for ex in examples]
+        def convert_class_label(label):
+            if type(label) == type(""):
+                return self.OUT_LABEL_DICT.get(label.strip(), -1)
+            else:
+                return label
+        return [convert_class_label(ex) for ex in examples]
 
     def load_dataset(self, split=None):
         return super().load_dataset(split)
 
 class TTC4900Dataset(ClassificationDataset):
     DATASET_NAME = "ttc4900"
     DATASET_INFO = "ttc4900"
@@ -717,17 +726,14 @@
     def preprocess_data(self, examples, skip_output_processing=False):
         # If used with the classification mode, don't process the output
         if skip_output_processing:
             return {"input_text": examples["text"], "label": examples["label"]}
         output = [self.IN_LABEL_DICT[ex] for ex in examples["label"]]
         return {"input_text": examples["text"], "target_text": output}
 
-    def postprocess_data(self, examples):
-        return [self.OUT_LABEL_DICT.get(ex.strip(), -1) for ex in examples]
-
     def load_dataset(self, split=None):
         dataset = LocalDataset.load_dataset(self, split)
         #dataset = datasets.load_dataset(self.dataset_loc, data_files=self.dataset_info, split=split)
         print("Deduplicating data")
         return super().deduplicate_data(dataset, "text")
 
 DATASET_MAPPING_NAMES = [
```

### Comparing `turkish-lm-tuner-0.1.1/turkish_lm_tuner/trainer.py` & `turkish_lm_tuner-0.1.2/turkish_lm_tuner/trainer.py`

 * *Files identical despite different names*

### Comparing `turkish-lm-tuner-0.1.1/turkish_lm_tuner.egg-info/PKG-INFO` & `turkish_lm_tuner-0.1.2/turkish_lm_tuner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkish-lm-tuner
-Version: 0.1.1
+Version: 0.1.2
 Summary: Implementation of the Turkish LM Tuner
 Author-email: Gökçe Uludoğan <gokceuludogan@gmail.com>, Zeynep Yirmibeşoğlu Balal <yirmibesogluz@gmail.com>, Furkan Akkurt <furkanakkurt9285@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/boun-tabi-LMG/turkish-lm-tuner
 Project-URL: Bug Tracker, https://github.com/boun-tabi-LMG/turkish-lm-tuner/issues
 Project-URL: Documentation, https://turkish-lm-tuner-docs.boun-tabi-LMG.github.io/
 Keywords: nlp,turkish,language models,finetuning
@@ -121,15 +121,15 @@
 )
 
 train_dataset = dataset_processor.load_and_preprocess_data(split='train')
 eval_dataset = dataset_processor.load_and_preprocess_data(split='validation')
 test_dataset = dataset_processor.load_and_preprocess_data(split="test")
 
 training_params = {
-    'num_train_epochs': 10
+    'num_train_epochs': 10,
     'per_device_train_batch_size': 4,
     'per_device_eval_batch_size': 4,
     'output_dir': './', 
     'evaluation_strategy': 'epoch',
     'save_strategy': 'epoch',
     'predict_with_generate': True    
 }
@@ -170,15 +170,17 @@
     dataset_name, task, task_format, task_mode,
     model_name, max_input_length, max_target_length
 )
 
 test_dataset = dataset_processor.load_and_preprocess_data(split="test")
 
 test_params = {
-    'per_device_eval_batch_size': 4
+    'per_device_eval_batch_size': 4,
+    'output_dir': './',
+    'predict_with_generate': True
 }
 
 model_path = "turna_tr_news_summarization"
 generation_params = {
     'num_beams': 4,
     'length_penalty': 2.0,
     'no_repeat_ngram_size': 3,
@@ -195,15 +197,15 @@
 ```
 
 ## Reference
 
 If you use this repository, please cite the following related [paper](https://arxiv.org/abs/2401.14373):
 
 ```bibtex
-@misc{uludoğan2024turna,
+@misc{uludogan2024turna,
       title={TURNA: A Turkish Encoder-Decoder Language Model for Enhanced Understanding and Generation}, 
       author={Gökçe Uludoğan and Zeynep Yirmibeşoğlu Balal and Furkan Akkurt and Melikşah Türker and Onur Güngör and Susan Üsküdarlı},
       year={2024},
       eprint={2401.14373},
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
```

### Comparing `turkish-lm-tuner-0.1.1/turkish_lm_tuner.egg-info/SOURCES.txt` & `turkish_lm_tuner-0.1.2/turkish_lm_tuner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

