# Comparing `tmp/llm-guard-0.3.7.tar.gz` & `tmp/llm-guard-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-guard-0.3.7.tar", last modified: Mon Jan 15 09:18:50 2024, max compression
+gzip compressed data, was "llm-guard-0.3.9.tar", last modified: Thu Feb  8 14:46:26 2024, max compression
```

## Comparing `llm-guard-0.3.7.tar` & `llm-guard-0.3.9.tar`

### file list

```diff
@@ -1,168 +1,177 @@
-drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-01-15 09:18:50.786158 llm-guard-0.3.7/
--rw-r--r--   0 asofter    (501) staff       (20)     1105 2023-08-08 19:47:28.000000 llm-guard-0.3.7/LICENSE
--rw-r--r--   0 asofter    (501) staff       (20)    10859 2024-01-15 09:18:50.785770 llm-guard-0.3.7/PKG-INFO
--rw-r--r--   0 asofter    (501) staff       (20)     6663 2024-01-13 14:25:25.000000 llm-guard-0.3.7/README.md
-drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-01-15 09:18:50.753341 llm-guard-0.3.7/llm_guard/
--rw-r--r--   0 asofter    (501) staff       (20)       71 2024-01-14 21:02:48.000000 llm-guard-0.3.7/llm_guard/__init__.py
--rw-r--r--   0 asofter    (501) staff       (20)     4773 2024-01-13 15:16:51.000000 llm-guard-0.3.7/llm_guard/evaluate.py
--rw-r--r--   0 asofter    (501) staff       (20)       52 2024-01-13 14:33:14.000000 llm-guard-0.3.7/llm_guard/exception.py
-drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-01-15 09:18:50.757741 llm-guard-0.3.7/llm_guard/input_scanners/
--rw-r--r--   0 asofter    (501) staff       (20)      783 2024-01-12 14:52:32.000000 llm-guard-0.3.7/llm_guard/input_scanners/__init__.py
--rw-r--r--   0 asofter    (501) staff       (20)    12422 2024-01-14 21:39:13.000000 llm-guard-0.3.7/llm_guard/input_scanners/anonymize.py
-drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-01-15 09:18:50.759113 llm-guard-0.3.7/llm_guard/input_scanners/anonymize_helpers/
--rw-r--r--   0 asofter    (501) staff       (20)      324 2023-11-04 21:00:55.000000 llm-guard-0.3.7/llm_guard/input_scanners/anonymize_helpers/__init__.py
--rw-r--r--   0 asofter    (501) staff       (20)     3130 2024-01-13 15:12:02.000000 llm-guard-0.3.7/llm_guard/input_scanners/anonymize_helpers/analyzer.py
--rw-r--r--   0 asofter    (501) staff       (20)     2278 2023-11-13 20:40:50.000000 llm-guard-0.3.7/llm_guard/input_scanners/anonymize_helpers/faker.py
--rw-r--r--   0 asofter    (501) staff       (20)     1689 2023-12-18 14:24:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/anonymize_helpers/ner_mapping.py
--rw-r--r--   0 asofter    (501) staff       (20)    13834 2023-12-18 20:57:23.000000 llm-guard-0.3.7/llm_guard/input_scanners/anonymize_helpers/transformers_recognizer.py
--rw-r--r--   0 asofter    (501) staff       (20)     3198 2024-01-13 15:12:02.000000 llm-guard-0.3.7/llm_guard/input_scanners/ban_competitors.py
--rw-r--r--   0 asofter    (501) staff       (20)     3761 2024-01-13 15:16:51.000000 llm-guard-0.3.7/llm_guard/input_scanners/ban_substrings.py
--rw-r--r--   0 asofter    (501) staff       (20)     3779 2024-01-14 21:39:16.000000 llm-guard-0.3.7/llm_guard/input_scanners/ban_topics.py
--rw-r--r--   0 asofter    (501) staff       (20)      765 2024-01-13 14:45:04.000000 llm-guard-0.3.7/llm_guard/input_scanners/base.py
--rw-r--r--   0 asofter    (501) staff       (20)     4257 2024-01-14 21:39:19.000000 llm-guard-0.3.7/llm_guard/input_scanners/code.py
--rw-r--r--   0 asofter    (501) staff       (20)     1155 2024-01-13 14:50:58.000000 llm-guard-0.3.7/llm_guard/input_scanners/invisible_text.py
--rw-r--r--   0 asofter    (501) staff       (20)     3012 2024-01-13 15:16:51.000000 llm-guard-0.3.7/llm_guard/input_scanners/language.py
--rw-r--r--   0 asofter    (501) staff       (20)     3315 2024-01-14 21:39:22.000000 llm-guard-0.3.7/llm_guard/input_scanners/prompt_injection.py
--rw-r--r--   0 asofter    (501) staff       (20)     2919 2024-01-13 15:16:51.000000 llm-guard-0.3.7/llm_guard/input_scanners/regex.py
--rw-r--r--   0 asofter    (501) staff       (20)    16462 2024-01-13 14:40:14.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets.py
-drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-01-15 09:18:50.778413 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/
--rw-r--r--   0 asofter    (501) staff       (20)        0 2023-09-21 12:28:09.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/__init__.py
--rw-r--r--   0 asofter    (501) staff       (20)      477 2023-10-01 20:39:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/adafruit.py
--rw-r--r--   0 asofter    (501) staff       (20)      621 2023-10-07 13:13:41.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/adobe.py
--rw-r--r--   0 asofter    (501) staff       (20)      349 2023-10-01 20:39:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/age_secret_key.py
--rw-r--r--   0 asofter    (501) staff       (20)      486 2023-10-01 20:39:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/airtable_api_key.py
--rw-r--r--   0 asofter    (501) staff       (20)      353 2023-10-07 13:23:14.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/algolia_api_key.py
--rw-r--r--   0 asofter    (501) staff       (20)      652 2023-10-07 13:33:19.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/alibaba.py
--rw-r--r--   0 asofter    (501) staff       (20)      761 2023-10-01 20:39:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/asana.py
--rw-r--r--   0 asofter    (501) staff       (20)      549 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/atlassian_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      571 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/authress_access_key.py
--rw-r--r--   0 asofter    (501) staff       (20)      521 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/beamer_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      812 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/bitbucket.py
--rw-r--r--   0 asofter    (501) staff       (20)      786 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/bittrex.py
--rw-r--r--   0 asofter    (501) staff       (20)      361 2023-10-02 18:26:12.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/clojars_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      534 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/codecov_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      542 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/coinbase_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      827 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/confluent.py
--rw-r--r--   0 asofter    (501) staff       (20)      525 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/contentful_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      370 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/databricks_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      502 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/datadog_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      558 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/defined_networking_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      631 2023-10-02 18:49:36.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/digitalocean.py
--rw-r--r--   0 asofter    (501) staff       (20)     1009 2023-10-03 13:16:49.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/discord.py
--rw-r--r--   0 asofter    (501) staff       (20)      361 2023-10-07 13:41:56.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/doppler_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      534 2023-10-03 13:16:50.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/droneci_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)     1046 2023-10-03 13:16:50.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/dropbox.py
--rw-r--r--   0 asofter    (501) staff       (20)      371 2023-10-07 13:41:56.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/duffel_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      385 2023-10-07 13:41:56.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/dynatrace_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      437 2023-10-07 13:41:56.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/easypost.py
--rw-r--r--   0 asofter    (501) staff       (20)      516 2023-10-03 13:16:50.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/etsy_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      540 2023-10-03 13:16:50.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/facebook_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      507 2023-10-03 13:16:50.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/fastly_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      802 2023-10-03 13:16:50.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/finicity.py
--rw-r--r--   0 asofter    (501) staff       (20)      534 2023-10-05 19:56:34.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/finnhub_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      528 2023-10-05 19:56:34.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/flickr_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      563 2023-10-07 13:41:56.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/flutterwave.py
--rw-r--r--   0 asofter    (501) staff       (20)      367 2023-10-07 13:41:56.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/frameio_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      552 2023-10-07 11:13:45.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/freshbooks_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      366 2023-10-07 11:13:45.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/gcp_api_key.py
--rw-r--r--   0 asofter    (501) staff       (20)      637 2023-10-01 20:39:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/github_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      539 2023-10-05 19:56:34.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/gitlab.py
--rw-r--r--   0 asofter    (501) staff       (20)      530 2023-10-07 11:13:45.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/gitter_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      570 2023-10-07 13:41:56.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/gocardless_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      682 2023-10-05 19:56:34.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/grafana.py
--rw-r--r--   0 asofter    (501) staff       (20)      462 2023-10-07 11:13:45.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/hashicorp_tf_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      526 2023-10-07 11:52:29.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/heroku_api_key.py
--rw-r--r--   0 asofter    (501) staff       (20)      567 2023-10-07 11:52:29.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/hubspot_api_key.py
--rw-r--r--   0 asofter    (501) staff       (20)      557 2023-10-07 11:52:29.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/huggingface.py
--rw-r--r--   0 asofter    (501) staff       (20)      500 2023-10-07 11:52:29.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/intercom_api_key.py
--rw-r--r--   0 asofter    (501) staff       (20)      827 2023-10-07 11:52:29.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/jfrog.py
--rw-r--r--   0 asofter    (501) staff       (20)     1145 2023-10-07 11:52:29.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/jwt.py
--rw-r--r--   0 asofter    (501) staff       (20)      539 2023-10-07 11:52:29.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/kraken_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      829 2023-10-07 12:06:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/kucoin.py
--rw-r--r--   0 asofter    (501) staff       (20)      531 2023-10-07 12:06:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/launchdarkly_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      609 2023-10-07 13:41:56.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/linear.py
--rw-r--r--   0 asofter    (501) staff       (20)      804 2023-10-07 12:06:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/linkedin.py
--rw-r--r--   0 asofter    (501) staff       (20)      778 2023-10-07 12:06:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/lob.py
--rw-r--r--   0 asofter    (501) staff       (20)     1099 2023-10-07 12:06:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/mailgun.py
--rw-r--r--   0 asofter    (501) staff       (20)      531 2023-10-07 12:06:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/mapbox_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      552 2023-10-07 12:06:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/mattermost_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      891 2023-10-07 12:06:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/messagebird.py
--rw-r--r--   0 asofter    (501) staff       (20)      608 2023-10-07 12:06:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/microsoft_teams_webhook.py
--rw-r--r--   0 asofter    (501) staff       (20)      541 2023-10-07 12:06:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/netlify_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)     1115 2023-10-07 12:06:47.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/new_relic.py
--rw-r--r--   0 asofter    (501) staff       (20)      556 2023-10-07 12:20:46.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/nytimes_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      491 2023-10-07 12:20:46.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/okta_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      395 2023-10-07 12:20:46.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/openai_api_key.py
--rw-r--r--   0 asofter    (501) staff       (20)      689 2023-10-07 13:41:56.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/planetscale.py
--rw-r--r--   0 asofter    (501) staff       (20)      374 2023-10-07 13:41:56.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/postman_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      346 2023-10-07 12:20:46.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/prefect_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      342 2023-10-07 12:20:46.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/pulumi_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      337 2023-10-07 12:20:46.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/pypi_upload_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      509 2023-10-07 12:20:46.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/rapidapi_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      343 2023-10-07 12:20:46.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/readme_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      352 2023-10-07 12:20:46.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/rubygems_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      325 2023-10-07 12:20:46.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/scalingo_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      832 2023-10-07 12:20:46.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/sendbird.py
--rw-r--r--   0 asofter    (501) staff       (20)      356 2023-10-07 19:40:22.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/sendgrid_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      389 2023-10-07 19:40:22.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/sendinblue_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      497 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/sentry_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      371 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/shippo_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      766 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/shopify.py
--rw-r--r--   0 asofter    (501) staff       (20)      804 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/sidekiq.py
--rw-r--r--   0 asofter    (501) staff       (20)     1217 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/slack.py
--rw-r--r--   0 asofter    (501) staff       (20)      523 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/snyk_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      570 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/squarespace_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      652 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/sumologic.py
--rw-r--r--   0 asofter    (501) staff       (20)      397 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/telegram_bot_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      508 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/travisci_access_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      485 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/twitch_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)     1512 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/twitter.py
--rw-r--r--   0 asofter    (501) staff       (20)      505 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/typeform_api_token.py
--rw-r--r--   0 asofter    (501) staff       (20)      470 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/vault.py
--rw-r--r--   0 asofter    (501) staff       (20)     1028 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/yandex.py
--rw-r--r--   0 asofter    (501) staff       (20)      494 2023-10-07 19:38:25.000000 llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/zendesk_secret_key.py
--rw-r--r--   0 asofter    (501) staff       (20)     1704 2024-01-13 14:45:04.000000 llm-guard-0.3.7/llm_guard/input_scanners/sentiment.py
--rw-r--r--   0 asofter    (501) staff       (20)     2313 2024-01-13 15:12:02.000000 llm-guard-0.3.7/llm_guard/input_scanners/token_limit.py
--rw-r--r--   0 asofter    (501) staff       (20)     3082 2024-01-13 14:45:04.000000 llm-guard-0.3.7/llm_guard/input_scanners/toxicity.py
--rw-r--r--   0 asofter    (501) staff       (20)     2035 2024-01-13 14:40:14.000000 llm-guard-0.3.7/llm_guard/input_scanners/util.py
-drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-01-15 09:18:50.783114 llm-guard-0.3.7/llm_guard/output_scanners/
--rw-r--r--   0 asofter    (501) staff       (20)     1113 2024-01-13 14:25:25.000000 llm-guard-0.3.7/llm_guard/output_scanners/__init__.py
--rw-r--r--   0 asofter    (501) staff       (20)     1401 2024-01-13 15:16:49.000000 llm-guard-0.3.7/llm_guard/output_scanners/ban_competitors.py
--rw-r--r--   0 asofter    (501) staff       (20)     2201 2024-01-13 15:16:51.000000 llm-guard-0.3.7/llm_guard/output_scanners/ban_substrings.py
--rw-r--r--   0 asofter    (501) staff       (20)     1439 2024-01-13 15:16:51.000000 llm-guard-0.3.7/llm_guard/output_scanners/ban_topics.py
--rw-r--r--   0 asofter    (501) staff       (20)      802 2023-09-23 11:51:50.000000 llm-guard-0.3.7/llm_guard/output_scanners/base.py
--rw-r--r--   0 asofter    (501) staff       (20)     2640 2024-01-13 14:45:04.000000 llm-guard-0.3.7/llm_guard/output_scanners/bias.py
--rw-r--r--   0 asofter    (501) staff       (20)     1436 2024-01-13 15:16:49.000000 llm-guard-0.3.7/llm_guard/output_scanners/code.py
--rw-r--r--   0 asofter    (501) staff       (20)     4954 2024-01-13 14:50:58.000000 llm-guard-0.3.7/llm_guard/output_scanners/deanonymize.py
--rw-r--r--   0 asofter    (501) staff       (20)     2200 2024-01-13 14:50:56.000000 llm-guard-0.3.7/llm_guard/output_scanners/factual_consistency.py
--rw-r--r--   0 asofter    (501) staff       (20)     3404 2024-01-13 14:50:56.000000 llm-guard-0.3.7/llm_guard/output_scanners/json.py
--rw-r--r--   0 asofter    (501) staff       (20)     1350 2024-01-13 15:16:49.000000 llm-guard-0.3.7/llm_guard/output_scanners/language.py
--rw-r--r--   0 asofter    (501) staff       (20)     2334 2024-01-13 14:50:56.000000 llm-guard-0.3.7/llm_guard/output_scanners/language_same.py
--rw-r--r--   0 asofter    (501) staff       (20)     2410 2024-01-13 14:50:56.000000 llm-guard-0.3.7/llm_guard/output_scanners/malicious_urls.py
--rw-r--r--   0 asofter    (501) staff       (20)     1830 2024-01-13 14:50:56.000000 llm-guard-0.3.7/llm_guard/output_scanners/no_refusal.py
--rw-r--r--   0 asofter    (501) staff       (20)     1445 2024-01-13 14:50:56.000000 llm-guard-0.3.7/llm_guard/output_scanners/reading_time.py
--rw-r--r--   0 asofter    (501) staff       (20)     1493 2024-01-13 15:16:49.000000 llm-guard-0.3.7/llm_guard/output_scanners/regex.py
--rw-r--r--   0 asofter    (501) staff       (20)     4911 2024-01-13 14:50:59.000000 llm-guard-0.3.7/llm_guard/output_scanners/relevance.py
--rw-r--r--   0 asofter    (501) staff       (20)     3382 2024-01-13 15:16:52.000000 llm-guard-0.3.7/llm_guard/output_scanners/sensitive.py
--rw-r--r--   0 asofter    (501) staff       (20)     1008 2024-01-13 14:50:56.000000 llm-guard-0.3.7/llm_guard/output_scanners/sentiment.py
--rw-r--r--   0 asofter    (501) staff       (20)     1189 2024-01-13 14:50:56.000000 llm-guard-0.3.7/llm_guard/output_scanners/toxicity.py
--rw-r--r--   0 asofter    (501) staff       (20)     1665 2024-01-13 14:50:56.000000 llm-guard-0.3.7/llm_guard/output_scanners/url_reachabitlity.py
--rw-r--r--   0 asofter    (501) staff       (20)     2731 2024-01-13 14:45:04.000000 llm-guard-0.3.7/llm_guard/output_scanners/util.py
-drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-01-15 09:18:50.783962 llm-guard-0.3.7/llm_guard/resources/
--rw-r--r--   0 asofter    (501) staff       (20)      529 2023-08-08 19:49:15.000000 llm-guard-0.3.7/llm_guard/resources/output_stop_substrings.json
--rw-r--r--   0 asofter    (501) staff       (20)      805 2023-08-08 19:49:16.000000 llm-guard-0.3.7/llm_guard/resources/prompt_stop_substrings.json
--rw-r--r--   0 asofter    (501) staff       (20)     1118 2023-10-10 19:42:29.000000 llm-guard-0.3.7/llm_guard/resources/sensisitive_patterns.json
--rw-r--r--   0 asofter    (501) staff       (20)     6108 2024-01-14 21:35:10.000000 llm-guard-0.3.7/llm_guard/transformers_helpers.py
--rw-r--r--   0 asofter    (501) staff       (20)     4537 2024-01-12 08:52:59.000000 llm-guard-0.3.7/llm_guard/util.py
--rw-r--r--   0 asofter    (501) staff       (20)      854 2023-10-05 19:14:21.000000 llm-guard-0.3.7/llm_guard/vault.py
--rw-r--r--   0 asofter    (501) staff       (20)       22 2024-01-14 21:37:47.000000 llm-guard-0.3.7/llm_guard/version.py
-drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-01-15 09:18:50.784538 llm-guard-0.3.7/llm_guard.egg-info/
--rw-r--r--   0 asofter    (501) staff       (20)    10859 2024-01-15 09:18:50.000000 llm-guard-0.3.7/llm_guard.egg-info/PKG-INFO
--rw-r--r--   0 asofter    (501) staff       (20)     7926 2024-01-15 09:18:50.000000 llm-guard-0.3.7/llm_guard.egg-info/SOURCES.txt
--rw-r--r--   0 asofter    (501) staff       (20)        1 2024-01-15 09:18:50.000000 llm-guard-0.3.7/llm_guard.egg-info/dependency_links.txt
--rw-r--r--   0 asofter    (501) staff       (20)      745 2024-01-15 09:18:50.000000 llm-guard-0.3.7/llm_guard.egg-info/requires.txt
--rw-r--r--   0 asofter    (501) staff       (20)       10 2024-01-15 09:18:50.000000 llm-guard-0.3.7/llm_guard.egg-info/top_level.txt
--rw-r--r--   0 asofter    (501) staff       (20)     2964 2024-01-14 21:23:16.000000 llm-guard-0.3.7/pyproject.toml
--rw-r--r--   0 asofter    (501) staff       (20)       38 2024-01-15 09:18:50.786224 llm-guard-0.3.7/setup.cfg
-drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-01-15 09:18:50.784205 llm-guard-0.3.7/tests/
--rw-r--r--   0 asofter    (501) staff       (20)     3162 2024-01-11 15:01:46.000000 llm-guard-0.3.7/tests/test_evaluate.py
+drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-02-08 14:46:26.195208 llm-guard-0.3.9/
+-rw-r--r--   0 asofter    (501) staff       (20)     1105 2023-08-08 19:47:28.000000 llm-guard-0.3.9/LICENSE
+-rw-r--r--   0 asofter    (501) staff       (20)    10469 2024-02-08 14:46:26.194808 llm-guard-0.3.9/PKG-INFO
+-rw-r--r--   0 asofter    (501) staff       (20)     6243 2024-02-06 08:20:37.000000 llm-guard-0.3.9/README.md
+drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-02-08 14:46:26.148160 llm-guard-0.3.9/llm_guard/
+-rw-r--r--   0 asofter    (501) staff       (20)       71 2024-01-14 21:02:48.000000 llm-guard-0.3.9/llm_guard/__init__.py
+-rw-r--r--   0 asofter    (501) staff       (20)     4880 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/evaluate.py
+-rw-r--r--   0 asofter    (501) staff       (20)       52 2024-01-13 14:33:14.000000 llm-guard-0.3.9/llm_guard/exception.py
+drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-02-08 14:46:26.155552 llm-guard-0.3.9/llm_guard/input_scanners/
+-rw-r--r--   0 asofter    (501) staff       (20)      783 2024-01-12 14:52:32.000000 llm-guard-0.3.9/llm_guard/input_scanners/__init__.py
+-rw-r--r--   0 asofter    (501) staff       (20)    14533 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize.py
+drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-02-08 14:46:26.157187 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/
+-rw-r--r--   0 asofter    (501) staff       (20)      324 2023-11-04 21:00:55.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/__init__.py
+-rw-r--r--   0 asofter    (501) staff       (20)     4892 2024-02-02 11:43:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/analyzer.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2278 2023-11-13 20:40:50.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/faker.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2583 2024-02-06 08:49:03.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/ner_mapping.py
+drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-02-08 14:46:26.158217 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/
+-rw-r--r--   0 asofter    (501) staff       (20)      483 2024-01-31 14:06:17.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/__init__.py
+-rw-r--r--   0 asofter    (501) staff       (20)      233 2024-01-31 14:06:17.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/phone_recognizer.py
+drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-02-08 14:46:26.160315 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/zh/
+-rw-r--r--   0 asofter    (501) staff       (20)      380 2024-01-31 14:06:17.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/zh/__init__.py
+-rw-r--r--   0 asofter    (501) staff       (20)      288 2024-01-31 14:06:17.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/zh/crypto_recognizer.py
+-rw-r--r--   0 asofter    (501) staff       (20)      626 2024-01-31 14:06:17.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/zh/custom_pattern_recognizer.py
+-rw-r--r--   0 asofter    (501) staff       (20)      359 2024-01-31 14:06:17.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/zh/email_recognizer.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1282 2024-01-31 14:06:17.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/zh/ip_recognizer.py
+-rw-r--r--   0 asofter    (501) staff       (20)    14094 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/transformers_recognizer.py
+-rw-r--r--   0 asofter    (501) staff       (20)     3321 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/input_scanners/ban_competitors.py
+-rw-r--r--   0 asofter    (501) staff       (20)     3841 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/input_scanners/ban_substrings.py
+-rw-r--r--   0 asofter    (501) staff       (20)     4177 2024-02-05 07:35:35.000000 llm-guard-0.3.9/llm_guard/input_scanners/ban_topics.py
+-rw-r--r--   0 asofter    (501) staff       (20)      765 2024-01-13 14:45:04.000000 llm-guard-0.3.9/llm_guard/input_scanners/base.py
+-rw-r--r--   0 asofter    (501) staff       (20)     4969 2024-02-05 07:53:30.000000 llm-guard-0.3.9/llm_guard/input_scanners/code.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1193 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/input_scanners/invisible_text.py
+-rw-r--r--   0 asofter    (501) staff       (20)     3385 2024-02-06 08:47:12.000000 llm-guard-0.3.9/llm_guard/input_scanners/language.py
+-rw-r--r--   0 asofter    (501) staff       (20)     3647 2024-02-06 08:47:41.000000 llm-guard-0.3.9/llm_guard/input_scanners/prompt_injection.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2964 2024-02-02 11:06:21.000000 llm-guard-0.3.9/llm_guard/input_scanners/regex.py
+-rw-r--r--   0 asofter    (501) staff       (20)    16507 2024-02-02 11:06:21.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets.py
+drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-02-08 14:46:26.185325 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/
+-rw-r--r--   0 asofter    (501) staff       (20)        0 2023-09-21 12:28:09.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/__init__.py
+-rw-r--r--   0 asofter    (501) staff       (20)      477 2023-10-01 20:39:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/adafruit.py
+-rw-r--r--   0 asofter    (501) staff       (20)      621 2023-10-07 13:13:41.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/adobe.py
+-rw-r--r--   0 asofter    (501) staff       (20)      349 2023-10-01 20:39:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/age_secret_key.py
+-rw-r--r--   0 asofter    (501) staff       (20)      486 2023-10-01 20:39:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/airtable_api_key.py
+-rw-r--r--   0 asofter    (501) staff       (20)      353 2023-10-07 13:23:14.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/algolia_api_key.py
+-rw-r--r--   0 asofter    (501) staff       (20)      652 2023-10-07 13:33:19.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/alibaba.py
+-rw-r--r--   0 asofter    (501) staff       (20)      761 2023-10-01 20:39:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/asana.py
+-rw-r--r--   0 asofter    (501) staff       (20)      549 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/atlassian_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      571 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/authress_access_key.py
+-rw-r--r--   0 asofter    (501) staff       (20)      521 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/beamer_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      812 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/bitbucket.py
+-rw-r--r--   0 asofter    (501) staff       (20)      786 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/bittrex.py
+-rw-r--r--   0 asofter    (501) staff       (20)      361 2023-10-02 18:26:12.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/clojars_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      534 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/codecov_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      542 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/coinbase_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      827 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/confluent.py
+-rw-r--r--   0 asofter    (501) staff       (20)      525 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/contentful_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      370 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/databricks_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      502 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/datadog_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      558 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/defined_networking_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      631 2023-10-02 18:49:36.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/digitalocean.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1009 2023-10-03 13:16:49.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/discord.py
+-rw-r--r--   0 asofter    (501) staff       (20)      361 2023-10-07 13:41:56.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/doppler_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      534 2023-10-03 13:16:50.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/droneci_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1046 2023-10-03 13:16:50.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/dropbox.py
+-rw-r--r--   0 asofter    (501) staff       (20)      371 2023-10-07 13:41:56.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/duffel_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      385 2023-10-07 13:41:56.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/dynatrace_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      437 2023-10-07 13:41:56.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/easypost.py
+-rw-r--r--   0 asofter    (501) staff       (20)      516 2023-10-03 13:16:50.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/etsy_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      540 2023-10-03 13:16:50.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/facebook_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      507 2023-10-03 13:16:50.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/fastly_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      802 2023-10-03 13:16:50.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/finicity.py
+-rw-r--r--   0 asofter    (501) staff       (20)      534 2023-10-05 19:56:34.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/finnhub_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      528 2023-10-05 19:56:34.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/flickr_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      563 2023-10-07 13:41:56.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/flutterwave.py
+-rw-r--r--   0 asofter    (501) staff       (20)      367 2023-10-07 13:41:56.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/frameio_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      552 2023-10-07 11:13:45.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/freshbooks_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      366 2023-10-07 11:13:45.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/gcp_api_key.py
+-rw-r--r--   0 asofter    (501) staff       (20)      637 2023-10-01 20:39:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/github_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      539 2023-10-05 19:56:34.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/gitlab.py
+-rw-r--r--   0 asofter    (501) staff       (20)      530 2023-10-07 11:13:45.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/gitter_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      570 2023-10-07 13:41:56.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/gocardless_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      682 2023-10-05 19:56:34.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/grafana.py
+-rw-r--r--   0 asofter    (501) staff       (20)      462 2023-10-07 11:13:45.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/hashicorp_tf_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      526 2023-10-07 11:52:29.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/heroku_api_key.py
+-rw-r--r--   0 asofter    (501) staff       (20)      567 2023-10-07 11:52:29.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/hubspot_api_key.py
+-rw-r--r--   0 asofter    (501) staff       (20)      557 2023-10-07 11:52:29.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/huggingface.py
+-rw-r--r--   0 asofter    (501) staff       (20)      500 2023-10-07 11:52:29.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/intercom_api_key.py
+-rw-r--r--   0 asofter    (501) staff       (20)      827 2023-10-07 11:52:29.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/jfrog.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1145 2023-10-07 11:52:29.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/jwt.py
+-rw-r--r--   0 asofter    (501) staff       (20)      539 2023-10-07 11:52:29.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/kraken_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      829 2023-10-07 12:06:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/kucoin.py
+-rw-r--r--   0 asofter    (501) staff       (20)      531 2023-10-07 12:06:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/launchdarkly_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      609 2023-10-07 13:41:56.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/linear.py
+-rw-r--r--   0 asofter    (501) staff       (20)      804 2023-10-07 12:06:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/linkedin.py
+-rw-r--r--   0 asofter    (501) staff       (20)      778 2023-10-07 12:06:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/lob.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1099 2023-10-07 12:06:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/mailgun.py
+-rw-r--r--   0 asofter    (501) staff       (20)      531 2023-10-07 12:06:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/mapbox_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      552 2023-10-07 12:06:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/mattermost_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      891 2023-10-07 12:06:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/messagebird.py
+-rw-r--r--   0 asofter    (501) staff       (20)      608 2023-10-07 12:06:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/microsoft_teams_webhook.py
+-rw-r--r--   0 asofter    (501) staff       (20)      541 2023-10-07 12:06:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/netlify_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1115 2023-10-07 12:06:47.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/new_relic.py
+-rw-r--r--   0 asofter    (501) staff       (20)      556 2023-10-07 12:20:46.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/nytimes_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      491 2023-10-07 12:20:46.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/okta_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      395 2023-10-07 12:20:46.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/openai_api_key.py
+-rw-r--r--   0 asofter    (501) staff       (20)      689 2023-10-07 13:41:56.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/planetscale.py
+-rw-r--r--   0 asofter    (501) staff       (20)      374 2023-10-07 13:41:56.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/postman_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      346 2023-10-07 12:20:46.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/prefect_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      342 2023-10-07 12:20:46.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/pulumi_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      337 2023-10-07 12:20:46.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/pypi_upload_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      509 2023-10-07 12:20:46.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/rapidapi_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      343 2023-10-07 12:20:46.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/readme_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      352 2023-10-07 12:20:46.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/rubygems_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      325 2023-10-07 12:20:46.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/scalingo_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      832 2023-10-07 12:20:46.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/sendbird.py
+-rw-r--r--   0 asofter    (501) staff       (20)      356 2023-10-07 19:40:22.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/sendgrid_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      389 2023-10-07 19:40:22.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/sendinblue_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      497 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/sentry_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      371 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/shippo_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      766 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/shopify.py
+-rw-r--r--   0 asofter    (501) staff       (20)      804 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/sidekiq.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1217 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/slack.py
+-rw-r--r--   0 asofter    (501) staff       (20)      523 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/snyk_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      570 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/squarespace_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      652 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/sumologic.py
+-rw-r--r--   0 asofter    (501) staff       (20)      397 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/telegram_bot_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      508 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/travisci_access_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      485 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/twitch_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1512 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/twitter.py
+-rw-r--r--   0 asofter    (501) staff       (20)      505 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/typeform_api_token.py
+-rw-r--r--   0 asofter    (501) staff       (20)      470 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/vault.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1028 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/yandex.py
+-rw-r--r--   0 asofter    (501) staff       (20)      494 2023-10-07 19:38:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/zendesk_secret_key.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1892 2024-02-02 11:21:25.000000 llm-guard-0.3.9/llm_guard/input_scanners/sentiment.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2420 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/input_scanners/token_limit.py
+-rw-r--r--   0 asofter    (501) staff       (20)     3468 2024-02-06 08:47:41.000000 llm-guard-0.3.9/llm_guard/input_scanners/toxicity.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2035 2024-01-13 14:40:14.000000 llm-guard-0.3.9/llm_guard/input_scanners/util.py
+drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-02-08 14:46:26.191616 llm-guard-0.3.9/llm_guard/output_scanners/
+-rw-r--r--   0 asofter    (501) staff       (20)     1113 2024-01-13 14:25:25.000000 llm-guard-0.3.9/llm_guard/output_scanners/__init__.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1401 2024-01-13 15:16:49.000000 llm-guard-0.3.9/llm_guard/output_scanners/ban_competitors.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2201 2024-01-13 15:16:51.000000 llm-guard-0.3.9/llm_guard/output_scanners/ban_substrings.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1726 2024-02-05 07:53:30.000000 llm-guard-0.3.9/llm_guard/output_scanners/ban_topics.py
+-rw-r--r--   0 asofter    (501) staff       (20)      802 2023-09-23 11:51:50.000000 llm-guard-0.3.9/llm_guard/output_scanners/base.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2886 2024-02-06 08:50:19.000000 llm-guard-0.3.9/llm_guard/output_scanners/bias.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1650 2024-02-05 07:53:30.000000 llm-guard-0.3.9/llm_guard/output_scanners/code.py
+-rw-r--r--   0 asofter    (501) staff       (20)     5016 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/output_scanners/deanonymize.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2250 2024-02-05 07:52:15.000000 llm-guard-0.3.9/llm_guard/output_scanners/factual_consistency.py
+-rw-r--r--   0 asofter    (501) staff       (20)     3825 2024-02-05 09:49:52.000000 llm-guard-0.3.9/llm_guard/output_scanners/json.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1578 2024-02-05 07:53:30.000000 llm-guard-0.3.9/llm_guard/output_scanners/language.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2795 2024-02-05 07:53:30.000000 llm-guard-0.3.9/llm_guard/output_scanners/language_same.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2859 2024-02-06 08:50:19.000000 llm-guard-0.3.9/llm_guard/output_scanners/malicious_urls.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2966 2024-02-06 08:54:10.000000 llm-guard-0.3.9/llm_guard/output_scanners/no_refusal.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1608 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/output_scanners/reading_time.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1493 2024-01-13 15:16:49.000000 llm-guard-0.3.9/llm_guard/output_scanners/regex.py
+-rw-r--r--   0 asofter    (501) staff       (20)     4938 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/output_scanners/relevance.py
+-rw-r--r--   0 asofter    (501) staff       (20)     3469 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/output_scanners/sensitive.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1008 2024-01-13 14:50:56.000000 llm-guard-0.3.9/llm_guard/output_scanners/sentiment.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1464 2024-02-05 07:53:30.000000 llm-guard-0.3.9/llm_guard/output_scanners/toxicity.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1705 2024-02-02 11:06:21.000000 llm-guard-0.3.9/llm_guard/output_scanners/url_reachabitlity.py
+-rw-r--r--   0 asofter    (501) staff       (20)     2731 2024-01-13 14:45:04.000000 llm-guard-0.3.9/llm_guard/output_scanners/util.py
+drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-02-08 14:46:26.192469 llm-guard-0.3.9/llm_guard/resources/
+-rw-r--r--   0 asofter    (501) staff       (20)      529 2023-08-08 19:49:15.000000 llm-guard-0.3.9/llm_guard/resources/output_stop_substrings.json
+-rw-r--r--   0 asofter    (501) staff       (20)      805 2023-08-08 19:49:16.000000 llm-guard-0.3.9/llm_guard/resources/prompt_stop_substrings.json
+-rw-r--r--   0 asofter    (501) staff       (20)     8901 2024-02-06 08:54:10.000000 llm-guard-0.3.9/llm_guard/resources/sensisitive_patterns.json
+-rw-r--r--   0 asofter    (501) staff       (20)     6203 2024-02-08 14:45:42.000000 llm-guard-0.3.9/llm_guard/transformers_helpers.py
+-rw-r--r--   0 asofter    (501) staff       (20)     5668 2024-02-02 11:06:39.000000 llm-guard-0.3.9/llm_guard/util.py
+-rw-r--r--   0 asofter    (501) staff       (20)     1065 2024-01-31 14:06:17.000000 llm-guard-0.3.9/llm_guard/vault.py
+-rw-r--r--   0 asofter    (501) staff       (20)       22 2024-02-08 14:46:13.000000 llm-guard-0.3.9/llm_guard/version.py
+drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-02-08 14:46:26.193302 llm-guard-0.3.9/llm_guard.egg-info/
+-rw-r--r--   0 asofter    (501) staff       (20)    10469 2024-02-08 14:46:26.000000 llm-guard-0.3.9/llm_guard.egg-info/PKG-INFO
+-rw-r--r--   0 asofter    (501) staff       (20)     8534 2024-02-08 14:46:26.000000 llm-guard-0.3.9/llm_guard.egg-info/SOURCES.txt
+-rw-r--r--   0 asofter    (501) staff       (20)        1 2024-02-08 14:46:26.000000 llm-guard-0.3.9/llm_guard.egg-info/dependency_links.txt
+-rw-r--r--   0 asofter    (501) staff       (20)      753 2024-02-08 14:46:26.000000 llm-guard-0.3.9/llm_guard.egg-info/requires.txt
+-rw-r--r--   0 asofter    (501) staff       (20)       10 2024-02-08 14:46:26.000000 llm-guard-0.3.9/llm_guard.egg-info/top_level.txt
+-rw-r--r--   0 asofter    (501) staff       (20)     2986 2024-02-05 17:48:04.000000 llm-guard-0.3.9/pyproject.toml
+-rw-r--r--   0 asofter    (501) staff       (20)       38 2024-02-08 14:46:26.195278 llm-guard-0.3.9/setup.cfg
+drwxr-xr-x   0 asofter    (501) staff       (20)        0 2024-02-08 14:46:26.192803 llm-guard-0.3.9/tests/
+-rw-r--r--   0 asofter    (501) staff       (20)     3162 2024-01-11 15:01:46.000000 llm-guard-0.3.9/tests/test_evaluate.py
```

### Comparing `llm-guard-0.3.7/LICENSE` & `llm-guard-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/PKG-INFO` & `llm-guard-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: llm-guard
-Version: 0.3.7
+Version: 0.3.9
 Summary: LLM-Guard is a comprehensive tool designed to fortify the security of Large Language Models (LLMs). By offering sanitization, detection of harmful language, prevention of data leakage, and resistance against prompt injection attacks, LLM-Guard ensures that your interactions with LLMs remain safe and secure.
-Author-email: "Laiyer.ai" <hello@laiyer.ai>
+Author-email: Protect AI <community@protectai.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -21,18 +21,18 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://github.com/laiyer-ai/llm-guard
+Project-URL: homepage, https://github.com/protectai/llm-guard
 Project-URL: documentation, https://llm-guard.com/
-Project-URL: repository, https://github.com/laiyer-ai/llm-guard
-Project-URL: issues, https://github.com/laiyer-ai/llm-guard/issues
+Project-URL: repository, https://github.com/protectai/llm-guard
+Project-URL: issues, https://github.com/protectai/llm-guard/issues
 Project-URL: changelog, https://llm-guard.com/changelog/
 Keywords: llm,language model,security,adversarial attacks,prompt injection,prompt leakage,PII detection,self-hardening,firewall
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -40,69 +40,69 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: detect-secrets==1.4.0
 Requires-Dist: faker<23,>=22
 Requires-Dist: fuzzysearch==0.7.3
-Requires-Dist: json-repair==0.4.5
+Requires-Dist: json-repair==0.8.0
 Requires-Dist: nltk<4,>=3.8
 Requires-Dist: presidio-analyzer<3,>=2.2
 Requires-Dist: presidio-anonymizer<3,>=2.2
-Requires-Dist: protobuf<4,>=3.20
+Requires-Dist: protobuf>=4
 Requires-Dist: regex==2023.12.25
 Requires-Dist: sentencepiece==0.1.99
 Requires-Dist: tiktoken<0.6,>=0.5
 Requires-Dist: torch==2.0.1
 Requires-Dist: transformers==4.36.2
 Requires-Dist: xformers==0.0.22
 Requires-Dist: span-marker==1.5.0
+Requires-Dist: structlog>=24
 Provides-Extra: onnxruntime
 Requires-Dist: optimum[onnxruntime]; extra == "onnxruntime"
 Provides-Extra: onnxruntime-gpu
 Requires-Dist: optimum[onnxruntime-gpu]; extra == "onnxruntime-gpu"
 Provides-Extra: docs-dev
 Requires-Dist: mkdocs<2,>=1.5; extra == "docs-dev"
 Requires-Dist: mkdocs-autorefs==0.5.0; extra == "docs-dev"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.2; extra == "docs-dev"
 Requires-Dist: mkdocs-jupyter==0.24.6; extra == "docs-dev"
-Requires-Dist: mkdocs-material==9.5.3; extra == "docs-dev"
+Requires-Dist: mkdocs-material==9.5.6; extra == "docs-dev"
 Requires-Dist: mkdocs-material-extensions==1.3.1; extra == "docs-dev"
-Requires-Dist: mkdocs-swagger-ui-tag==0.6.7; extra == "docs-dev"
+Requires-Dist: mkdocs-swagger-ui-tag==0.6.8; extra == "docs-dev"
 Requires-Dist: mkdocstrings==0.24.0; extra == "docs-dev"
 Requires-Dist: mkdocstrings-python==1.8.0; extra == "docs-dev"
 Provides-Extra: dev
 Requires-Dist: llm_guard[docs-dev]; extra == "dev"
 Requires-Dist: autoflake<3,>=2; extra == "dev"
 Requires-Dist: black<24,>=23; extra == "dev"
 Requires-Dist: isort<6,>5; extra == "dev"
-Requires-Dist: pytest<8,>=7.4; extra == "dev"
+Requires-Dist: pytest<9,>=7.4; extra == "dev"
 Requires-Dist: pytest-cov<5,>=4.1; extra == "dev"
 Requires-Dist: pre-commit<4,>=3.6; extra == "dev"
 
 # LLM Guard - The Security Toolkit for LLM Interactions
 
-LLM Guard by [Laiyer.ai](https://laiyer.ai) is a comprehensive tool designed to fortify the security of Large Language Models (LLMs).
+LLM Guard by [Protect AI](https://protectai.com/llm-guard) is a comprehensive tool designed to fortify the security of Large Language Models (LLMs).
 
-[**Documentation**](https://laiyer-ai.github.io/llm-guard/) | [**Playground**](https://huggingface.co/spaces/laiyer/llm-guard-playground) | [**Changelog**](https://llm-guard.com/changelog/) | [**Blog**](https://substack.com/@laiyer)
+[**Documentation**](https://llm-guard.com/) | [**Playground**](https://huggingface.co/spaces/ProtectAI/llm-guard-playground) | [**Changelog**](https://llm-guard.com/changelog/)
 
 [![GitHub
-stars](https://img.shields.io/github/stars/laiyer-ai/llm-guard.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/laiyer-ai/llm-guard/stargazers/)
+stars](https://img.shields.io/github/stars/protectai/llm-guard.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/protectai/llm-guard/stargazers/)
 [![MIT license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](http://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Python Version](https://img.shields.io/pypi/v/llm-guard)](https://pypi.org/project/llm-guard)
 [![Downloads](https://static.pepy.tech/badge/llm-guard)](https://pepy.tech/project/llm-guard)
 [![Downloads](https://static.pepy.tech/badge/llm-guard/month)](https://pepy.tech/project/llm-guard)
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/laiyer_ai.svg?style=social&label=Follow%20%40Laiyer_AI)](https://twitter.com/laiyer_ai)
 
-<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/laiyer-ai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
+<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/protectai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
 
 ## What is LLM Guard?
 
-![LLM-Guard](https://github.com/laiyer-ai/llm-guard/blob/main/docs/assets/flow.png?raw=true)
+![LLM-Guard](https://github.com/protectai/llm-guard/blob/main/docs/assets/flow.png?raw=true)
 
 By offering sanitization, detection of harmful language, prevention of data leakage, and resistance against prompt
 injection attacks, LLM-Guard ensures that your interactions with LLMs remain safe and secure.
 
 ## Installation
 
 Begin your journey with LLM Guard by downloading the package:
@@ -177,30 +177,23 @@
 We are committed to a transparent development process and highly appreciate any contributions.
 Whether you are helping us fix bugs, propose new features, improve our documentation or spread the word,
 we would love to have you as part of our community.
 
 - Give us a ⭐️ github star ⭐️ on the top of this page to support what we're doing,
   it means a lot for open source projects!
 - Read our
-  [docs](https://laiyer-ai.github.io/llm-guard/)
+  [docs](https://llm-guard.com/)
   for more info about how to use and customize LLM Guard, and for step-by-step tutorials.
 - Post a [Github
-  Issue](https://github.com/laiyer-ai/llm-guard/issues) to submit a bug report, feature request, or suggest an improvement.
+  Issue](https://github.com/protectai/llm-guard/issues) to submit a bug report, feature request, or suggest an improvement.
 - To contribute to the package, check out our [contribution guidelines](CONTRIBUTING.md), and open a PR.
 
 Join our Slack to give us feedback, connect with the maintainers and fellow users, ask questions,
 get help for package usage or contributions, or engage in discussions about LLM security!
 
-<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/laiyer-ai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
+<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/protectai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
 
 ### Production Support
 
 We're eager to provide personalized assistance when deploying your LLM Guard to a production environment.
 
-- [Send Email ✉️](mailto:hello@laiyer.ai)
-
-## Supporters
-
-LLM Guard is supported by the following organizations:
-
-- [Google Patch Rewards program](https://bughunters.google.com/open-source-security/patch-rewards)
-- [JetBrains](https://jb.gg/OpenSourceSupport)
+- [Send Email ✉️](mailto:community@protectai.com)
```

### Comparing `llm-guard-0.3.7/README.md` & `llm-guard-0.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # LLM Guard - The Security Toolkit for LLM Interactions
 
-LLM Guard by [Laiyer.ai](https://laiyer.ai) is a comprehensive tool designed to fortify the security of Large Language Models (LLMs).
+LLM Guard by [Protect AI](https://protectai.com/llm-guard) is a comprehensive tool designed to fortify the security of Large Language Models (LLMs).
 
-[**Documentation**](https://laiyer-ai.github.io/llm-guard/) | [**Playground**](https://huggingface.co/spaces/laiyer/llm-guard-playground) | [**Changelog**](https://llm-guard.com/changelog/) | [**Blog**](https://substack.com/@laiyer)
+[**Documentation**](https://llm-guard.com/) | [**Playground**](https://huggingface.co/spaces/ProtectAI/llm-guard-playground) | [**Changelog**](https://llm-guard.com/changelog/)
 
 [![GitHub
-stars](https://img.shields.io/github/stars/laiyer-ai/llm-guard.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/laiyer-ai/llm-guard/stargazers/)
+stars](https://img.shields.io/github/stars/protectai/llm-guard.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/protectai/llm-guard/stargazers/)
 [![MIT license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](http://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Python Version](https://img.shields.io/pypi/v/llm-guard)](https://pypi.org/project/llm-guard)
 [![Downloads](https://static.pepy.tech/badge/llm-guard)](https://pepy.tech/project/llm-guard)
 [![Downloads](https://static.pepy.tech/badge/llm-guard/month)](https://pepy.tech/project/llm-guard)
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/laiyer_ai.svg?style=social&label=Follow%20%40Laiyer_AI)](https://twitter.com/laiyer_ai)
 
-<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/laiyer-ai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
+<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/protectai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
 
 ## What is LLM Guard?
 
-![LLM-Guard](https://github.com/laiyer-ai/llm-guard/blob/main/docs/assets/flow.png?raw=true)
+![LLM-Guard](https://github.com/protectai/llm-guard/blob/main/docs/assets/flow.png?raw=true)
 
 By offering sanitization, detection of harmful language, prevention of data leakage, and resistance against prompt
 injection attacks, LLM-Guard ensures that your interactions with LLMs remain safe and secure.
 
 ## Installation
 
 Begin your journey with LLM Guard by downloading the package:
@@ -96,30 +95,23 @@
 We are committed to a transparent development process and highly appreciate any contributions.
 Whether you are helping us fix bugs, propose new features, improve our documentation or spread the word,
 we would love to have you as part of our community.
 
 - Give us a ⭐️ github star ⭐️ on the top of this page to support what we're doing,
   it means a lot for open source projects!
 - Read our
-  [docs](https://laiyer-ai.github.io/llm-guard/)
+  [docs](https://llm-guard.com/)
   for more info about how to use and customize LLM Guard, and for step-by-step tutorials.
 - Post a [Github
-  Issue](https://github.com/laiyer-ai/llm-guard/issues) to submit a bug report, feature request, or suggest an improvement.
+  Issue](https://github.com/protectai/llm-guard/issues) to submit a bug report, feature request, or suggest an improvement.
 - To contribute to the package, check out our [contribution guidelines](CONTRIBUTING.md), and open a PR.
 
 Join our Slack to give us feedback, connect with the maintainers and fellow users, ask questions,
 get help for package usage or contributions, or engage in discussions about LLM security!
 
-<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/laiyer-ai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
+<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/protectai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
 
 ### Production Support
 
 We're eager to provide personalized assistance when deploying your LLM Guard to a production environment.
 
-- [Send Email ✉️](mailto:hello@laiyer.ai)
-
-## Supporters
-
-LLM Guard is supported by the following organizations:
-
-- [Google Patch Rewards program](https://bughunters.google.com/open-source-security/patch-rewards)
-- [JetBrains](https://jb.gg/OpenSourceSupport)
+- [Send Email ✉️](mailto:community@protectai.com)
```

#### html2text {}

```diff
@@ -1,45 +1,42 @@
-# LLM Guard - The Security Toolkit for LLM Interactions LLM Guard by
-[Laiyer.ai](https://laiyer.ai) is a comprehensive tool designed to fortify the
-security of Large Language Models (LLMs). [**Documentation**](https://laiyer-
-ai.github.io/llm-guard/) | [**Playground**](https://huggingface.co/spaces/
-laiyer/llm-guard-playground) | [**Changelog**](https://llm-guard.com/changelog/
-) | [**Blog**](https://substack.com/@laiyer) [![GitHub stars](https://
-img.shields.io/github/stars/laiyer-ai/llm-
-guard.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/laiyer-
-ai/llm-guard/stargazers/) [![MIT license](https://img.shields.io/badge/license-
-MIT-brightgreen.svg)](http://opensource.org/licenses/MIT) [![Code style: black]
-(https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black) [![PyPI - Python Version](https://img.shields.io/pypi/v/
-llm-guard)](https://pypi.org/project/llm-guard) [![Downloads](https://
-static.pepy.tech/badge/llm-guard)](https://pepy.tech/project/llm-guard) [!
-[Downloads](https://static.pepy.tech/badge/llm-guard/month)](https://pepy.tech/
-project/llm-guard) [![Twitter](https://img.shields.io/twitter/url/https/
-twitter.com/laiyer_ai.svg?style=social&label=Follow%20%40Laiyer_AI)](https://
-twitter.com/laiyer_ai) _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_a_i_y_e_r_-_a_i_/_l_l_m_-_g_u_a_r_d_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/
-_a_s_s_e_t_s_/_j_o_i_n_-_o_u_r_-_s_l_a_c_k_-_c_o_m_m_u_n_i_t_y_._p_n_g_?_r_a_w_=_t_r_u_e_]## What is LLM Guard? ![LLM-Guard]
-(https://github.com/laiyer-ai/llm-guard/blob/main/docs/assets/
-flow.png?raw=true) By offering sanitization, detection of harmful language,
-prevention of data leakage, and resistance against prompt injection attacks,
-LLM-Guard ensures that your interactions with LLMs remain safe and secure. ##
-Installation Begin your journey with LLM Guard by downloading the package:
-```sh pip install llm-guard ``` ## Getting Started **Important Notes**: - LLM
-Guard is designed for easy integration and deployment in production
-environments. While it's ready to use out-of-the-box, please be informed that
-we're constantly improving and updating the repository. - Base functionality
-requires a limited number of libraries. As you explore more advanced features,
-necessary libraries will be automatically installed. - Ensure you're using
-Python version 3.9 or higher. Confirm with: `python --version`. - Library
-installation issues? Consider upgrading pip: `python -m pip install --upgrade
-pip`. **Examples**: - Get started with [ChatGPT and LLM Guard](./examples/
-openai_api.py). - Deploy LLM Guard as [API](https://llm-guard.com/usage/api/
-) ## Supported scanners ### Prompt scanners - [Anonymize](https://llm-
-guard.com/input_scanners/anonymize/) - [BanCompetitors](https://llm-guard.com/
-input_scanners/ban_competitors/) - [BanSubstrings](https://llm-guard.com/
-input_scanners/ban_substrings/) - [BanTopics](https://llm-guard.com/
+# LLM Guard - The Security Toolkit for LLM Interactions LLM Guard by [Protect
+AI](https://protectai.com/llm-guard) is a comprehensive tool designed to
+fortify the security of Large Language Models (LLMs). [**Documentation**]
+(https://llm-guard.com/) | [**Playground**](https://huggingface.co/spaces/
+ProtectAI/llm-guard-playground) | [**Changelog**](https://llm-guard.com/
+changelog/) [![GitHub stars](https://img.shields.io/github/stars/protectai/llm-
+guard.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/
+protectai/llm-guard/stargazers/) [![MIT license](https://img.shields.io/badge/
+license-MIT-brightgreen.svg)](http://opensource.org/licenses/MIT) [![Code
+style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
+(https://github.com/psf/black) [![PyPI - Python Version](https://
+img.shields.io/pypi/v/llm-guard)](https://pypi.org/project/llm-guard) [!
+[Downloads](https://static.pepy.tech/badge/llm-guard)](https://pepy.tech/
+project/llm-guard) [![Downloads](https://static.pepy.tech/badge/llm-guard/
+month)](https://pepy.tech/project/llm-guard) _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_p_r_o_t_e_c_t_a_i_/_l_l_m_-
+_g_u_a_r_d_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_a_s_s_e_t_s_/_j_o_i_n_-_o_u_r_-_s_l_a_c_k_-_c_o_m_m_u_n_i_t_y_._p_n_g_?_r_a_w_=_t_r_u_e_]## What is
+LLM Guard? ![LLM-Guard](https://github.com/protectai/llm-guard/blob/main/docs/
+assets/flow.png?raw=true) By offering sanitization, detection of harmful
+language, prevention of data leakage, and resistance against prompt injection
+attacks, LLM-Guard ensures that your interactions with LLMs remain safe and
+secure. ## Installation Begin your journey with LLM Guard by downloading the
+package: ```sh pip install llm-guard ``` ## Getting Started **Important
+Notes**: - LLM Guard is designed for easy integration and deployment in
+production environments. While it's ready to use out-of-the-box, please be
+informed that we're constantly improving and updating the repository. - Base
+functionality requires a limited number of libraries. As you explore more
+advanced features, necessary libraries will be automatically installed. -
+Ensure you're using Python version 3.9 or higher. Confirm with: `python --
+version`. - Library installation issues? Consider upgrading pip: `python -m pip
+install --upgrade pip`. **Examples**: - Get started with [ChatGPT and LLM
+Guard](./examples/openai_api.py). - Deploy LLM Guard as [API](https://llm-
+guard.com/usage/api/) ## Supported scanners ### Prompt scanners - [Anonymize]
+(https://llm-guard.com/input_scanners/anonymize/) - [BanCompetitors](https://
+llm-guard.com/input_scanners/ban_competitors/) - [BanSubstrings](https://llm-
+guard.com/input_scanners/ban_substrings/) - [BanTopics](https://llm-guard.com/
 input_scanners/ban_topics/) - [Code](https://llm-guard.com/input_scanners/code/
 ) - [InvisibleText](https://llm-guard.com/input_scanners/invisible_text/) -
 [Language](https://llm-guard.com/input_scanners/language/) - [PromptInjection]
 (https://llm-guard.com/input_scanners/prompt_injection/) - [Regex](https://llm-
 guard.com/input_scanners/regex/) - [Secrets](https://llm-guard.com/
 input_scanners/secrets/) - [Sentiment](https://llm-guard.com/input_scanners/
 sentiment/) - [TokenLimit](https://llm-guard.com/input_scanners/token_limit/) -
@@ -65,21 +62,18 @@
 contribute or create issues, it helps us improve LLM Guard! ## Community,
 Contributing, Docs & Support LLM Guard is an open source solution. We are
 committed to a transparent development process and highly appreciate any
 contributions. Whether you are helping us fix bugs, propose new features,
 improve our documentation or spread the word, we would love to have you as part
 of our community. - Give us a â­ï¸ github star â­ï¸ on the top of this page
 to support what we're doing, it means a lot for open source projects! - Read
-our [docs](https://laiyer-ai.github.io/llm-guard/) for more info about how to
-use and customize LLM Guard, and for step-by-step tutorials. - Post a [Github
-Issue](https://github.com/laiyer-ai/llm-guard/issues) to submit a bug report,
-feature request, or suggest an improvement. - To contribute to the package,
-check out our [contribution guidelines](CONTRIBUTING.md), and open a PR. Join
-our Slack to give us feedback, connect with the maintainers and fellow users,
-ask questions, get help for package usage or contributions, or engage in
-discussions about LLM security! _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_a_i_y_e_r_-_a_i_/_l_l_m_-_g_u_a_r_d_/_b_l_o_b_/
-_m_a_i_n_/_d_o_c_s_/_a_s_s_e_t_s_/_j_o_i_n_-_o_u_r_-_s_l_a_c_k_-_c_o_m_m_u_n_i_t_y_._p_n_g_?_r_a_w_=_t_r_u_e_]### Production Support
-We're eager to provide personalized assistance when deploying your LLM Guard to
-a production environment. - [Send Email âï¸](mailto:hello@laiyer.ai) ##
-Supporters LLM Guard is supported by the following organizations: - [Google
-Patch Rewards program](https://bughunters.google.com/open-source-security/
-patch-rewards) - [JetBrains](https://jb.gg/OpenSourceSupport)
+our [docs](https://llm-guard.com/) for more info about how to use and customize
+LLM Guard, and for step-by-step tutorials. - Post a [Github Issue](https://
+github.com/protectai/llm-guard/issues) to submit a bug report, feature request,
+or suggest an improvement. - To contribute to the package, check out our
+[contribution guidelines](CONTRIBUTING.md), and open a PR. Join our Slack to
+give us feedback, connect with the maintainers and fellow users, ask questions,
+get help for package usage or contributions, or engage in discussions about LLM
+security! _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_p_r_o_t_e_c_t_a_i_/_l_l_m_-_g_u_a_r_d_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_a_s_s_e_t_s_/_j_o_i_n_-
+_o_u_r_-_s_l_a_c_k_-_c_o_m_m_u_n_i_t_y_._p_n_g_?_r_a_w_=_t_r_u_e_]### Production Support We're eager to provide
+personalized assistance when deploying your LLM Guard to a production
+environment. - [Send Email âï¸](mailto:community@protectai.com)
```

### Comparing `llm-guard-0.3.7/llm_guard/evaluate.py` & `llm-guard-0.3.9/llm_guard/evaluate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import time
 from typing import Dict, List, Optional
 
 from .input_scanners.base import Scanner as InputScanner
 from .output_scanners.base import Scanner as OutputScanner
-from .util import logger
+from .util import get_logger
 
 """
 This file contains main functionality for scanning both prompts and outputs of Large Language Models (LLMs).
 There are two primary functions: 'scan_prompt' and 'scan_output'.
 Each function takes a list of scanner objects and applies each scanner to the input string(s).
 
 An Scanner in this context is an object of a class that inherits from either `input_scanners.Scanner` or `output_scanners.Scanner` base classes.
 These base classes define an `scan` method that takes in a string and returns a processed string and a boolean value indicating the validity of the input string.
 
 These functions return the processed string after all scanners have been applied, along with a dictionary mapping the name of each scanner to its validity result.
 """
 
+LOGGER = get_logger(__name__)
+
 
 def scan_prompt(
     scanners: List[InputScanner], prompt: str, fail_fast: Optional[bool] = False
 ) -> (str, Dict[str, bool], Dict[str, float]):
     """
     Scans a given prompt using the provided scanners.
 
@@ -43,27 +45,29 @@
         return sanitized_prompt, results_valid, results_score
 
     start_time = time.time()
     for scanner in scanners:
         start_time_scanner = time.time()
         sanitized_prompt, is_valid, risk_score = scanner.scan(sanitized_prompt)
         elapsed_time_scanner = time.time() - start_time_scanner
-        logger.debug(
-            f"Scanner {type(scanner).__name__}: Valid={is_valid}. Elapsed time: {elapsed_time_scanner:.6f} seconds"
+
+        LOGGER.debug(
+            "Scanner completed",
+            scanner=type(scanner).__name__,
+            is_valid=is_valid,
+            elapsed_time_seconds=round(elapsed_time_scanner, 6),
         )
 
         results_valid[type(scanner).__name__] = is_valid
         results_score[type(scanner).__name__] = risk_score
         if fail_fast and not is_valid:
             break
 
     elapsed_time = time.time() - start_time
-    logger.info(
-        f"Scanned prompt with the score: {results_score}. Elapsed time: {elapsed_time:.6f} seconds"
-    )
+    LOGGER.info("Scanned prompt", scores=results_score, elapsed_time_seconds=round(elapsed_time, 6))
 
     return sanitized_prompt, results_valid, results_score
 
 
 def scan_output(
     scanners: List[OutputScanner], prompt: str, output: str, fail_fast: Optional[bool] = False
 ) -> (str, Dict[str, bool], Dict[str, float]):
@@ -91,22 +95,24 @@
         return sanitized_output, results_valid, results_score
 
     start_time = time.time()
     for scanner in scanners:
         start_time_scanner = time.time()
         sanitized_output, is_valid, risk_score = scanner.scan(prompt, sanitized_output)
         elapsed_time_scanner = time.time() - start_time_scanner
-        logger.debug(
-            f"Scanner {type(scanner).__name__}: Valid={is_valid}. Elapsed time: {elapsed_time_scanner:.6f} seconds"
+
+        LOGGER.debug(
+            "Scanner completed",
+            scanner=type(scanner).__name__,
+            is_valid=is_valid,
+            elapsed_time_seconds=round(elapsed_time_scanner, 6),
         )
 
         results_valid[type(scanner).__name__] = is_valid
         results_score[type(scanner).__name__] = risk_score
         if fail_fast and not is_valid:
             break
 
     elapsed_time = time.time() - start_time
-    logger.info(
-        f"Scanned output with the score: {results_score}. Elapsed time: {elapsed_time:.6f} seconds"
-    )
+    LOGGER.info("Scanned output", scores=results_score, elapsed_time_seconds=round(elapsed_time, 6))
 
     return sanitized_output, results_valid, results_score
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/__init__.py` & `llm-guard-0.3.9/llm_guard/input_scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/anonymize.py` & `llm-guard-0.3.9/llm_guard/input_scanners/anonymize.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 import os
 import re
 from typing import Dict, List, Optional, Sequence
 
 from presidio_anonymizer.core.text_replace_builder import TextReplaceBuilder
 from presidio_anonymizer.entities import PIIEntity, RecognizerResult
 
-from llm_guard.util import logger
-from llm_guard.vault import Vault
-
+from ..exception import LLMGuardValidationError
+from ..util import get_logger
+from ..vault import Vault
 from .anonymize_helpers import (
     BERT_BASE_NER_CONF,
     get_analyzer,
     get_fake_value,
     get_transformers_recognizer,
 )
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 sensitive_patterns_path = os.path.join(
     os.path.dirname(os.path.abspath(__file__)),
     "..",
     "resources",
     "sensisitive_patterns.json",
 )
+
 default_entity_types = [
     "CREDIT_CARD",
     "CRYPTO",
     "EMAIL_ADDRESS",
     "IBAN_CODE",
     "IP_ADDRESS",
     "PERSON",
@@ -35,14 +38,16 @@
     "US_BANK_NUMBER",
     "CREDIT_CARD_RE",
     "UUID",
     "EMAIL_ADDRESS_RE",
     "US_SSN_RE",
 ]
 
+ALL_SUPPORTED_LANGUAGES = ["en", "zh"]
+
 
 class Anonymize(Scanner):
     """
     Anonymize sensitive data in the text using NLP (English only) and predefined regex patterns.
 
     Anonymizes detected entities with placeholders like [REDACTED_PERSON_1] and stores the real values in a Vault.
     Deanonymizer can be used to replace the placeholders back to their original values.
@@ -57,14 +62,15 @@
         entity_types: Optional[Sequence[str]] = None,
         preamble: str = "",
         regex_pattern_groups_path: str = sensitive_patterns_path,
         use_faker: bool = False,
         recognizer_conf: Optional[Dict] = BERT_BASE_NER_CONF,
         threshold: float = 0,
         use_onnx: bool = False,
+        language: str = "en",
     ):
         """
         Initialize an instance of Anonymize class.
 
         Parameters:
             vault (Vault): A vault instance to store the anonymized data.
             hidden_names (Optional[Sequence[str]]): List of names to be anonymized e.g. [REDACTED_CUSTOM_1].
@@ -72,38 +78,54 @@
             entity_types (Optional[Sequence[str]]): List of entity types to be detected. If not provided, defaults to all.
             preamble (str): Text to prepend to sanitized prompt. If not provided, defaults to an empty string.
             regex_pattern_groups_path (str): Path to a JSON file with regex pattern groups. If not provided, defaults to sensisitive_patterns.json.
             use_faker (bool): Whether to use faker instead of placeholders in applicable cases. If not provided, defaults to False, replaces with placeholders [REDACTED_PERSON_1].
             recognizer_conf (Optional[Dict]): Configuration to recognize PII data. Default is dslim/bert-base-NER.
             threshold (float): Acceptance threshold. Default is 0.
             use_onnx (bool): Whether to use ONNX runtime for inference. Default is False.
+            language (str): Language of the anonymize detect. Default is "en".
         """
 
+        if language not in ALL_SUPPORTED_LANGUAGES:
+            raise LLMGuardValidationError(
+                f"Language must be in the list of allowed: {ALL_SUPPORTED_LANGUAGES}"
+            )
+
         os.environ["TOKENIZERS_PARALLELISM"] = "false"  # Disables huggingface/tokenizers warning
 
         if not entity_types:
-            logger.debug(f"No entity types provided, using default: {default_entity_types}")
+            LOGGER.debug(
+                "No entity types provided, using default", default_entities=default_entity_types
+            )
             entity_types = default_entity_types.copy()
+
         entity_types.append("CUSTOM")
 
         if not hidden_names:
             hidden_names = []
 
         self._vault = vault
         self._entity_types = entity_types
         self._allowed_names = allowed_names
         self._preamble = preamble
         self._use_faker = use_faker
         self._threshold = threshold
+        self._language = language
+
+        transformers_recognizer = get_transformers_recognizer(
+            recognizer_conf=recognizer_conf,
+            use_onnx=use_onnx,
+            supported_language=language,
+        )
 
-        transformers_recognizer = get_transformers_recognizer(recognizer_conf, use_onnx)
         self._analyzer = get_analyzer(
-            transformers_recognizer,
-            Anonymize.get_regex_patterns(regex_pattern_groups_path),
-            hidden_names,
+            recognizer=transformers_recognizer,
+            regex_groups=Anonymize.get_regex_patterns(regex_pattern_groups_path),
+            custom_names=hidden_names,
+            supported_languages=list(set(["en", language])),
         )
 
     @staticmethod
     def get_regex_patterns(json_path: str) -> List[dict]:
         """
         Load regex patterns from a specified JSON file.
 
@@ -118,24 +140,26 @@
         try:
             with open(json_path, "r") as myfile:
                 pattern_groups_raw = json.load(myfile)
             for group in pattern_groups_raw:
                 regex_groups.append(
                     {
                         "name": group["name"].upper(),
-                        "expressions": group["expressions"],
-                        "context": group["context"],
-                        "score": group["score"],
+                        "expressions": group.get("expressions", []),
+                        "context": group.get("context", []),
+                        "score": group.get("score", 0.75),
+                        "languages": group.get("languages", ["en"]),
+                        "reuse": group.get("reuse", False),
                     }
                 )
-                logger.debug(f"Loaded regex pattern for {group['name']}")
+                LOGGER.debug("Loaded regex pattern", group_name=group["name"])
         except FileNotFoundError:
-            logger.warning(f"Could not find {json_path}")
+            LOGGER.warning("Could not find file", path=json_path)
         except json.decoder.JSONDecodeError as json_error:
-            logger.warning(f"Could not parse {json_path}: {json_error}")
+            LOGGER.warning("Could not parse file", path=json_path, error=json_error)
         return regex_groups
 
     @staticmethod
     def _remove_conflicts_and_get_text_manipulation_data(
         analyzer_results: List[RecognizerResult],
     ) -> List[RecognizerResult]:
         """
@@ -161,15 +185,15 @@
                 other_element.score = max(result.score, other_element.score)
                 is_merge_same_entity_type = True
                 break
             if not is_merge_same_entity_type:
                 other_elements.append(result)
                 tmp_analyzer_results.append(result)
             else:
-                logger.debug(f"removing element {result} from " f"results list due to merge")
+                LOGGER.debug("Removing element the results list due to merge", result=result)
 
         unique_text_metadata_elements = []
         # This list contains all elements which we need to check a single result
         # against. If a result is dropped, it can also be dropped from this list
         # since it is intersecting with another result, and we selected the other one.
         other_elements = tmp_analyzer_results.copy()
         for result in tmp_analyzer_results:
@@ -177,15 +201,17 @@
             result_conflicted = Anonymize.__is_result_conflicted_with_other_elements(
                 other_elements, result
             )
             if not result_conflicted:
                 other_elements.append(result)
                 unique_text_metadata_elements.append(result)
             else:
-                logger.debug(f"removing element {result} from results list due to conflict")
+                LOGGER.debug(
+                    "Removing element from the results list due to conflict", result=result
+                )
         return unique_text_metadata_elements
 
     @staticmethod
     def __is_result_conflicted_with_other_elements(other_elements, result):
         """
         Check if the given result conflicts with any other elements.
         """
@@ -216,44 +242,61 @@
         if use_faker:
             result = get_fake_value(entity_type) or result
 
         return result
 
     @staticmethod
     def _anonymize(
-        prompt: str, pii_entities: List[PIIEntity], use_faker: bool
+        prompt: str, pii_entities: List[PIIEntity], vault: Vault, use_faker: bool
     ) -> (str, List[tuple]):
         """
         Replace detected entities in the prompt with anonymized placeholders.
 
         Parameters:
             prompt (str): Original text prompt.
             pii_entities (List[PIIEntity]): List of entities detected in the prompt.
+            vault (Vault): A vault instance with the anonymized data stored.
             use_faker (bool): Whether to use faker to generate fake data.
 
         Returns:
             str: Sanitized text.
             List[tuple]: List of tuples representing the replaced entities and their corresponding placeholders.
         """
         text_replace_builder = TextReplaceBuilder(original_text=prompt)
 
-        entity_type_counter = {}
+        entity_type_counter, new_entity_counter = {}, {}
         for pii_entity in pii_entities:
             entity_type = pii_entity.entity_type
             entity_value = text_replace_builder.get_text_in_position(
                 pii_entity.start, pii_entity.end
             )
 
             if entity_type not in entity_type_counter:
                 entity_type_counter[entity_type] = {}
 
             if entity_value not in entity_type_counter[entity_type]:
-                entity_type_counter[entity_type][entity_value] = (
-                    len(entity_type_counter[entity_type]) + 1
-                )
+                vault_entities = [
+                    (entity_placeholder, entity_vault_value)
+                    for entity_placeholder, entity_vault_value in vault.get()
+                    if entity_type in entity_placeholder
+                ]
+                entity_placeholder = [
+                    entity_placeholder
+                    for entity_placeholder, entity_vault_value in vault_entities
+                    if entity_vault_value == entity_value
+                ]
+                if len(entity_placeholder) > 0:
+                    entity_type_counter[entity_type][entity_value] = int(
+                        entity_placeholder[0].split("_")[-1][:-1]
+                    )
+                else:
+                    entity_type_counter[entity_type][entity_value] = (
+                        len(vault_entities) + new_entity_counter.get(entity_type, 0) + 1
+                    )
+                    new_entity_counter[entity_type] = new_entity_counter.get(entity_type, 0) + 1
 
         results = []
         sorted_pii_entities = sorted(pii_entities, reverse=True)
         for pii_entity in sorted_pii_entities:
             entity_type = pii_entity.entity_type
             entity_value = text_replace_builder.get_text_in_position(
                 pii_entity.start, pii_entity.end
@@ -278,15 +321,15 @@
     def scan(self, prompt: str) -> (str, bool, float):
         risk_score = 0.0
         if prompt.strip() == "":
             return prompt, True, risk_score
 
         analyzer_results = self._analyzer.analyze(
             text=Anonymize.remove_single_quotes(prompt),
-            language="en",
+            language=self._language,
             entities=self._entity_types,
             allow_list=self._allowed_names,
             score_threshold=self._threshold,
         )
 
         risk_score = round(
             max(analyzer_result.score for analyzer_result in analyzer_results)
@@ -294,20 +337,24 @@
             else 0.0,
             1,
         )
         analyzer_results = self._remove_conflicts_and_get_text_manipulation_data(analyzer_results)
         merged_results = self._merge_entities_with_whitespace_between(prompt, analyzer_results)
 
         sanitized_prompt, anonymized_results = self._anonymize(
-            prompt, merged_results, self._use_faker
+            prompt, merged_results, self._vault, self._use_faker
         )
 
         if prompt != sanitized_prompt:
-            logger.warning(
-                f"Found sensitive data in the prompt and replaced it: {merged_results}, risk score: {risk_score}"
+            LOGGER.warning(
+                "Found sensitive data in the prompt and replaced it",
+                merged_results=merged_results,
+                risk_score=risk_score,
             )
-            self._vault.extend(anonymized_results)
+            for entity_placeholder, entity_value in anonymized_results:
+                if not self._vault.placeholder_exists(entity_placeholder):
+                    self._vault.append((entity_placeholder, entity_value))
             return self._preamble + sanitized_prompt, False, risk_score
 
-        logger.debug(f"Prompt does not have sensitive data to replace. Risk score is {risk_score}")
+        LOGGER.debug("Prompt does not have sensitive data to replace", risk_score=risk_score)
 
         return prompt, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/anonymize_helpers/faker.py` & `llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/faker.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/anonymize_helpers/ner_mapping.py` & `llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/ner_mapping.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 BERT_BASE_NER_CONF = {
     "PRESIDIO_SUPPORTED_ENTITIES": [
         "LOCATION",
         "PERSON",
         "ORGANIZATION",
     ],
     "DEFAULT_MODEL_PATH": "dslim/bert-base-NER",
-    "ONNX_MODEL_PATH": "laiyer/bert-base-NER-onnx",
+    "ONNX_MODEL_PATH": "dslim/bert-base-NER",
     "LABELS_TO_IGNORE": ["O", "CARDINAL"],
     "DEFAULT_EXPLANATION": "Identified as {} by the dslim/bert-base-NER NER model",
     "SUB_WORD_AGGREGATION": "simple",
     "DATASET_TO_PRESIDIO_MAPPING": {
         "MISC": "O",
         "LOC": "LOCATION",
         "ORG": "ORGANIZATION",
@@ -30,15 +30,15 @@
 BERT_LARGE_NER_CONF = {
     "PRESIDIO_SUPPORTED_ENTITIES": [
         "LOCATION",
         "PERSON",
         "ORGANIZATION",
     ],
     "DEFAULT_MODEL_PATH": "dslim/bert-large-NER",
-    "ONNX_MODEL_PATH": "laiyer/bert-large-NER-onnx",
+    "ONNX_MODEL_PATH": "dslim/bert-large-NER",
     "LABELS_TO_IGNORE": ["O", "CARDINAL"],
     "DEFAULT_EXPLANATION": "Identified as {} by the dslim/bert-large-NER NER model",
     "SUB_WORD_AGGREGATION": "simple",
     "DATASET_TO_PRESIDIO_MAPPING": {
         "MISC": "O",
         "LOC": "LOCATION",
         "ORG": "ORGANIZATION",
@@ -52,11 +52,41 @@
     },
     "CHUNK_OVERLAP_SIZE": 40,
     "CHUNK_SIZE": 600,
     "ID_SCORE_MULTIPLIER": 0.4,
     "ID_ENTITY_NAME": "ID",
 }
 
+BERT_ZH_NER_CONF = {
+    "PRESIDIO_SUPPORTED_ENTITIES": [
+        "LOCATION",
+        "PERSON",
+        "ORGANIZATION",
+    ],
+    "DEFAULT_MODEL_PATH": "gyr66/bert-base-chinese-finetuned-ner",
+    "ONNX_MODEL_PATH": "ProtectAI/gyr66-bert-base-chinese-finetuned-ner-onnx",
+    "LABELS_TO_IGNORE": ["O", "CARDINAL"],
+    "DEFAULT_EXPLANATION": "Identified as {} by the gyr66/bert-base-chinese-finetuned-ner NER model",
+    "SUB_WORD_AGGREGATION": "simple",
+    "DATASET_TO_PRESIDIO_MAPPING": {
+        "MISC": "O",
+        "address": "LOCATION",
+        "company": "ORGANIZATION",
+        "name": "PERSON",
+    },
+    "MODEL_TO_PRESIDIO_MAPPING": {
+        "MISC": "O",
+        "address": "LOCATION",
+        "company": "ORGANIZATION",
+        "name": "PERSON",
+    },
+    "CHUNK_OVERLAP_SIZE": 40,
+    "CHUNK_SIZE": 600,
+    "ID_SCORE_MULTIPLIER": 0.4,
+    "ID_ENTITY_NAME": "ID",
+}
+
 ALL_RECOGNIZER_CONF = [
     BERT_BASE_NER_CONF,
     BERT_LARGE_NER_CONF,
+    BERT_ZH_NER_CONF,
 ]
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/anonymize_helpers/transformers_recognizer.py` & `llm-guard-0.3.9/llm_guard/input_scanners/anonymize_helpers/transformers_recognizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from typing import List, Optional
 
 from presidio_analyzer import AnalysisExplanation, EntityRecognizer, RecognizerResult
 from presidio_analyzer.nlp_engine import NlpArtifacts
 from transformers import TokenClassificationPipeline
 
 from llm_guard.transformers_helpers import pipeline
-from llm_guard.util import logger
+from llm_guard.util import get_logger
 
 from .ner_mapping import BERT_BASE_NER_CONF
 
+LOGGER = get_logger(__name__)
+
 
 class TransformersRecognizer(EntityRecognizer):
     """
     Wrapper for a transformers_rec model, if needed to be used within Presidio Analyzer.
     The class loads models hosted on HuggingFace - https://huggingface.co/
     and loads the model and tokenizer into a TokenClassification pipeline.
     Samples are split into short text chunks, ideally shorter than max_length input_ids of the individual model,
@@ -49,14 +51,15 @@
         pass
 
     def __init__(
         self,
         model_path: Optional[str] = None,
         pipeline: Optional[TokenClassificationPipeline] = None,
         supported_entities: Optional[List[str]] = None,
+        supported_language: str = "en",
     ):
         if not supported_entities:
             supported_entities = BERT_BASE_NER_CONF["PRESIDIO_SUPPORTED_ENTITIES"]
         super().__init__(
             supported_entities=supported_entities,
             name=f"Transformers model {model_path}",
         )
@@ -71,14 +74,15 @@
         self.entity_mapping = None
         self.default_explanation = None
         self.text_overlap_length = None
         self.chunk_length = None
         self.id_entity_name = None
         self.id_score_reduction = None
         self.onnx_model_path = None
+        self.supported_language = supported_language
 
     def load_transformer(self, use_onnx: bool = False, **kwargs) -> None:
         """Load external configuration parameters and set default values.
 
         :param kwargs: define default values for class attributes and modify pipeline behavior
         **DATASET_TO_PRESIDIO_MAPPING (dict) - defines mapping entity strings from dataset format to Presidio format
         **MODEL_TO_PRESIDIO_MAPPING (dict) -  defines mapping entity strings from chosen model format to Presidio format
@@ -104,16 +108,17 @@
         self.id_score_reduction = kwargs.get("ID_SCORE_REDUCTION", 0.5)
         self.onnx_model_path = kwargs.get("ONNX_MODEL_PATH", None)
 
         if not self.pipeline:
             if not self.model_path:
                 self.model_path = "dslim/bert-base-NER"
                 self.onnx_model_path = "optimum/bert-base-NER"
-                logger.warning(
-                    f"Both 'model' and 'model_path' arguments are None. Using default model_path={self.model_path}"
+                LOGGER.warning(
+                    "Both 'model' and 'model_path' arguments are None. Using default",
+                    model_path=self.model_path,
                 )
 
         self._load_pipeline(use_onnx)
 
     def _load_pipeline(self, use_onnx: bool = False) -> None:
         """Initialize NER transformers_rec pipeline using the model_path provided"""
         self.pipeline = pipeline(
@@ -155,19 +160,21 @@
 
         for res in ner_results:
             res["entity_group"] = self.__check_label_transformer(res["entity_group"])
             if not res["entity_group"]:
                 continue
 
             if res["entity_group"] not in entities:
-                logger.debug(f"Ignoring entity {res['entity_group']}")
+                LOGGER.debug("Ignoring entity", entity_group=res["entity_group"])
                 continue
 
             if res["entity_group"] == self.id_entity_name:
-                logger.debug(f"ID entity found, multiplying score by {self.id_score_reduction}")
+                LOGGER.debug(
+                    "ID entity found, multiplying score", score_reduction=self.id_score_reduction
+                )
                 res["score"] = res["score"] * self.id_score_reduction
 
             textual_explanation = self.default_explanation.format(res["entity_group"])
             explanation = self.build_transformers_explanation(
                 float(round(res["score"], 2)), textual_explanation, res["word"]
             )
             transformers_result = self._convert_to_recognizer_result(res, explanation)
@@ -192,15 +199,15 @@
         :type overlap_length: int
         :return: List of start and end positions for individual text chunks
         :rtype: List[List]
         """
         if input_length < chunk_length:
             return [[0, input_length]]
         if chunk_length <= overlap_length:
-            logger.warning(
+            LOGGER.warning(
                 "overlap_length should be shorter than chunk_length, setting overlap_length to by half of chunk_length"
             )
             overlap_length = chunk_length // 2
         return [
             [i, min([i + chunk_length, input_length])]
             for i in range(0, input_length - overlap_length, chunk_length - overlap_length)
         ]
@@ -218,16 +225,18 @@
         model_max_length = self.pipeline.tokenizer.model_max_length
         # calculate inputs based on the text
         text_length = len(text)
         # split text into chunks
         if text_length <= model_max_length:
             predictions = self.pipeline(text)
         else:
-            logger.info(
-                f"splitting the text into chunks, length {text_length} > {model_max_length}"
+            LOGGER.info(
+                "splitting the text into chunks",
+                length=text_length,
+                model_max_length=model_max_length,
             )
             predictions = list()
             chunk_indexes = TransformersRecognizer.split_text_to_word_chunks(
                 text_length, self.chunk_length, self.text_overlap_length
             )
 
             # iterate over text chunks and run inference
@@ -305,14 +314,14 @@
         # convert model label to presidio label
         entity = self.model_to_presidio_mapping.get(label, None)
 
         if entity in self.ignore_labels:
             return None
 
         if entity is None:
-            logger.warning(f"Found unrecognized label {label}, returning entity as is")
+            LOGGER.warning("Found unrecognized label, returning entity as is", label=label)
             return label
 
         if entity not in self.supported_entities:
-            logger.warning(f"Found entity {entity} which is not supported by Presidio")
+            LOGGER.warning("Found entity which is not supported by Presidio", entity=entity)
             return entity
         return entity
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/ban_competitors.py` & `llm-guard-0.3.9/llm_guard/input_scanners/ban_competitors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Dict, Optional, Sequence
 
 from presidio_anonymizer.core.text_replace_builder import TextReplaceBuilder
 
 from llm_guard.exception import LLMGuardValidationError
-from llm_guard.util import device, lazy_load_dep, logger
+from llm_guard.util import device, get_logger, lazy_load_dep
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 MODEL_BASE = {
     "path": "tomaarsen/span-marker-bert-base-orgs",
 }
 
 MODEL_SMALL = {
     "path": "tomaarsen/span-marker-bert-small-orgs",
 }
@@ -69,29 +71,33 @@
         entities = self._ner_pipeline.predict(prompt)
         entities = sorted(entities, key=lambda x: x["char_end_index"], reverse=True)
         for entity in entities:
             if entity["span"] not in self._competitors:
                 continue
 
             if entity["score"] < self._threshold:
-                logger.debug(
-                    f"Competitor {entity['span']} detected but the score is below threshold: {entity['score']}"
+                LOGGER.debug(
+                    "Competitor detected but the score is below threshold",
+                    entity=entity["span"],
+                    score=entity["score"],
                 )
                 continue
 
             is_detected = True
 
             if self._redact:
                 text_replace_builder.replace_text_get_insertion_index(
                     "[REDACTED]",
                     entity["char_start_index"],
                     entity["char_end_index"],
                 )
 
-            logger.warning(f"Competitor {entity['span']} detected with score: {entity['score']}")
+            LOGGER.warning(
+                "Competitor detected with score", entity=entity["span"], score=entity["score"]
+            )
 
         if is_detected:
             return text_replace_builder.output_text, False, 1.0
 
-        logger.debug(f"None of the competitors were detected")
+        LOGGER.debug("None of the competitors were detected")
 
         return prompt, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/ban_substrings.py` & `llm-guard-0.3.9/llm_guard/input_scanners/ban_substrings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import re
 from enum import Enum
 from typing import Sequence, Union
 
-from llm_guard.util import logger
+from llm_guard.util import get_logger
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 stop_file_path = os.path.join(
     os.path.dirname(os.path.abspath(__file__)),
     "..",
     "resources",
     "prompt_stop_substrings.json",
 )
 
@@ -84,32 +86,34 @@
             if self._match_type.match(prompt, s):
                 matched_substrings.append(s)
             else:
                 missing_substrings.append(s)
 
         if self._contains_all:
             if len(missing_substrings) > 0:
-                logger.debug(f"Some substrings were not found: " + ", ".join(missing_substrings))
+                LOGGER.debug(
+                    "Some substrings were not found", missing_substrings=missing_substrings
+                )
                 return sanitized_prompt, True, 0.0
 
             if self._redact:
                 sanitized_prompt = self._redact_text(sanitized_prompt, matched_substrings)
-                logger.debug("Redacted banned substrings")
+                LOGGER.debug("Redacted banned substrings")
 
-            logger.warning(f"All substrings were found")
+            LOGGER.warning("All substrings were found")
 
             return sanitized_prompt, False, 1.0
 
         if matched_substrings:
-            logger.warning(
-                f"Found the following banned substrings: " + ", ".join(matched_substrings)
+            LOGGER.warning(
+                "Found the following banned substrings", matched_substrings=matched_substrings
             )
 
             if self._redact:
                 sanitized_prompt = self._redact_text(sanitized_prompt, matched_substrings)
-                logger.debug("Redacted banned substrings")
+                LOGGER.debug("Redacted banned substrings")
 
             return sanitized_prompt, False, 1.0
 
-        logger.debug("No banned substrings found")
+        LOGGER.debug("No banned substrings found")
 
         return sanitized_prompt, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/ban_topics.py` & `llm-guard-0.3.9/llm_guard/input_scanners/ban_topics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Dict, Optional, Sequence
 
 from llm_guard.exception import LLMGuardValidationError
 from llm_guard.transformers_helpers import pipeline
-from llm_guard.util import logger
+from llm_guard.util import get_logger
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 # This model was trained on a mixture of 33 datasets and 389 classes reformatted in the universal NLI format.
 # The model is English only. You can also use it for multilingual zeroshot classification by first machine translating texts to English.
 MODEL_LARGE = {
     "path": "MoritzLaurer/deberta-v3-large-zeroshot-v1.1-all-33",
     "onnx_path": "MoritzLaurer/deberta-v3-large-zeroshot-v1.1-all-33",
     "max_length": 512,
 }
@@ -47,57 +49,66 @@
     def __init__(
         self,
         topics: Sequence[str],
         *,
         threshold: float = 0.6,
         model: Optional[Dict] = None,
         use_onnx: bool = False,
+        transformers_kwargs: Optional[Dict] = None,
     ):
         """
         Initialize BanTopics object.
 
         Parameters:
             topics (Sequence[str]): List of topics to ban.
             threshold (float, optional): Threshold to determine if a topic is present in the prompt. Default is 0.75.
             model (Dict, optional): Model to use for zero-shot classification. Default is deberta-v3-base-zeroshot-v1.
             use_onnx (bool, optional): Whether to use ONNX for inference. Default is False.
+            transformers_kwargs (Dict, optional): Additional kwargs to pass to the transformers pipeline. Default is None.
 
         Raises:
             ValueError: If no topics are provided.
         """
         if model is None:
             model = MODEL_BASE
 
         if model not in ALL_MODELS:
             raise LLMGuardValidationError(f"Model must be in the list of allowed: {ALL_MODELS}")
 
         self._topics = topics
         self._threshold = threshold
 
+        transformers_kwargs = transformers_kwargs or {}
+        transformers_kwargs["max_length"] = model["max_length"]
+        transformers_kwargs["truncation"] = True
+
         self._classifier = pipeline(
             task="zero-shot-classification",
             model=model["path"],
             onnx_model=model["onnx_path"],
             use_onnx=use_onnx,
-            max_length=model["max_length"],
-            truncation=True,
+            **transformers_kwargs,
         )
 
     def scan(self, prompt: str) -> (str, bool, float):
         if prompt.strip() == "":
             return prompt, True, 0.0
 
         output_model = self._classifier(prompt, self._topics, multi_label=False)
 
         max_score = round(max(output_model["scores"]) if output_model["scores"] else 0, 2)
         if max_score > self._threshold:
-            logger.warning(
-                f"Topics detected for the prompt {output_model['labels']} with scores: {output_model['scores']}"
+            LOGGER.warning(
+                "Topics detected for the prompt",
+                labels=output_model["labels"],
+                scores=output_model["scores"],
             )
 
             return prompt, False, max_score
 
-        logger.debug(
-            f"No banned topics detected ({output_model['labels']}, scores: {output_model['scores']})"
+        LOGGER.debug(
+            "No banned topics detected",
+            labels=output_model["labels"],
+            scores=output_model["scores"],
         )
 
         return prompt, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/base.py` & `llm-guard-0.3.9/llm_guard/input_scanners/base.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/code.py` & `llm-guard-0.3.9/llm_guard/input_scanners/code.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,48 @@
 import re
-from typing import List, Sequence
+from typing import Dict, List, Optional, Sequence
 
 from llm_guard.exception import LLMGuardValidationError
 from llm_guard.transformers_helpers import pipeline
-from llm_guard.util import calculate_risk_score, logger
+from llm_guard.util import calculate_risk_score, get_logger
 
 from .base import Scanner
 
-_model_path = (
-    "huggingface/CodeBERTa-language-id",
-    "laiyer/CodeBERTa-language-id-onnx",  # ONNX model
-)
+LOGGER = get_logger(__name__)
 
-SUPPORTED_LANGUAGES = ["go", "java", "javascript", "php", "python", "ruby"]
+_model_path = "philomath-1209/programming-language-identification"
+
+SUPPORTED_LANGUAGES = [
+    "ARM Assembly",
+    "AppleScript",
+    "C",
+    "C#",
+    "C++",
+    "COBOL",
+    "Erlang",
+    "Fortran",
+    "Go",
+    "Java",
+    "JavaScript",
+    "Kotlin",
+    "Lua",
+    "Mathematica/Wolfram Language",
+    "PHP",
+    "Pascal",
+    "Perl",
+    "PowerShell",
+    "Python",
+    "R",
+    "Ruby",
+    "Rust",
+    "Scala",
+    "Swift",
+    "Visual Basic .NET",
+    "jq",
+]
 
 
 class Code(Scanner):
     """
     A class for scanning if the prompt includes code in specific programming languages.
 
     This class uses the transformers library to detect code snippets in the output of the language model.
@@ -26,40 +52,45 @@
     def __init__(
         self,
         languages: Sequence[str],
         *,
         is_blocked: bool = True,
         threshold: float = 0.5,
         use_onnx: bool = False,
+        transformers_kwargs: Optional[Dict] = None,
     ):
         """
         Initializes Code with the allowed and denied languages.
 
         Parameters:
             languages (Sequence[str]): The list of programming languages to allow or deny.
             is_blocked (bool): Whether the languages are blocked or allowed. Default is True.
             threshold (float): The threshold for the risk score. Default is 0.5.
             use_onnx (bool): Whether to use ONNX for inference. Default is False.
+            transformers_kwargs (Optional[Dict]): Optional keyword arguments for the transformers pipeline.
 
         Raises:
-            ValueError: If both 'allowed' and 'denied' lists are provided or if both are empty.
+            LLMGuardValidationError: If the languages are not a subset of SUPPORTED_LANGUAGES.
         """
         if not set(languages).issubset(set(SUPPORTED_LANGUAGES)):
             raise LLMGuardValidationError(f"Languages must be a subset of {SUPPORTED_LANGUAGES}")
 
         self._languages = languages
         self._is_blocked = is_blocked
         self._threshold = threshold
 
+        transformers_kwargs = transformers_kwargs or {}
+        transformers_kwargs["truncation"] = True
+
         self._pipeline = pipeline(
             task="text-classification",
-            model=_model_path[0],
-            onnx_model=_model_path[1],
+            model=_model_path,
+            onnx_model=_model_path,
             use_onnx=use_onnx,
-            truncation=True,
+            **transformers_kwargs,
         )
 
         self._fenced_code_regex = re.compile(r"```(?:[a-zA-Z0-9]*\n)?(.*?)```", re.DOTALL)
         self._inline_code_regex = re.compile(r"`(.*?)`")
 
     def _extract_code_blocks(self, markdown: str) -> List[str]:
         # Extract fenced code blocks (between triple backticks)
@@ -79,38 +110,42 @@
     def scan(self, prompt: str) -> (str, bool, float):
         if prompt.strip() == "":
             return prompt, True, 0.0
 
         # Try to extract code snippets from Markdown
         code_blocks = self._extract_code_blocks(prompt)
         if len(code_blocks) == 0:
-            logger.debug("No Markdown code blocks found in the output")
+            LOGGER.debug("No Markdown code blocks found in the output")
             return prompt, True, 0.0
 
-        logger.debug(f"Code blocks found in the output: {code_blocks}")
+        LOGGER.debug("Code blocks found in the output", code_blocks=code_blocks)
 
         # Only check when the code is detected
         for code_block in code_blocks:
             languages = self._pipeline(code_block)
-            logger.debug(f"Detected languages {languages} in the code: {code_block}")
+            LOGGER.debug(
+                "Detected languages in the code", languages=languages, code_block=code_block
+            )
 
             for language in languages:
                 language_name = language["label"]
                 score = round(language["score"], 2)
 
                 if score < self._threshold or language_name not in self._languages:
                     continue
 
                 if self._is_blocked:
-                    logger.warning(f"Language {language_name} is not allowed (score {score})")
+                    LOGGER.warning(
+                        "Language is not allowed", language_name=language_name, score=score
+                    )
                     return prompt, False, calculate_risk_score(score, self._threshold)
 
                 if not self._is_blocked:
-                    logger.debug(f"Language {language_name} is allowed (score {score})")
+                    LOGGER.debug("Language is allowed", language_name=language_name, score=score)
                     return prompt, True, 0.0
 
         if self._is_blocked:
-            logger.debug(f"No blocked languages detected")
+            LOGGER.debug("No blocked languages detected")
             return prompt, True, 0.0
 
-        logger.warning(f"No allowed languages detected")
+        LOGGER.warning("No allowed languages detected")
         return prompt, False, 1.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/invisible_text.py` & `llm-guard-0.3.9/llm_guard/input_scanners/invisible_text.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import unicodedata
 
-from llm_guard.util import logger
+from llm_guard.util import get_logger
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 
 class InvisibleText(Scanner):
     """
     A class for scanning if the prompt includes invisible characters.
 
     This class uses the unicodedata library to detect invisible characters in the output of the language model.
     """
@@ -31,13 +33,13 @@
             if unicodedata.category(char) not in self._banned_categories:
                 continue
 
             chars.append(char)
             prompt = prompt.replace(char, "")
 
         if chars:
-            logger.warning(f"Found invisible characters {chars} in the prompt")
+            LOGGER.warning("Found invisible characters in the prompt", chars=chars)
 
             return prompt, False, 1.0
 
-        logger.debug(f"No invisible characters found")
+        LOGGER.debug("No invisible characters found")
         return prompt, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/language.py` & `llm-guard-0.3.9/llm_guard/input_scanners/language.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from enum import Enum
-from typing import List, Sequence, Union
+from typing import Dict, List, Optional, Sequence, Union
 
 from llm_guard.transformers_helpers import pipeline
-from llm_guard.util import calculate_risk_score, logger, split_text_by_sentences
+from llm_guard.util import calculate_risk_score, get_logger, split_text_by_sentences
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 model_path = (
     "papluca/xlm-roberta-base-language-detection",
-    "laiyer/xlm-roberta-base-language-detection-onnx",
+    "ProtectAI/xlm-roberta-base-language-detection-onnx",
 )
 
 
 class MatchType(Enum):
     SENTENCE = "sentence"
     FULL = "full"
 
@@ -34,39 +36,44 @@
     def __init__(
         self,
         valid_languages: Sequence[str],
         *,
         threshold: float = 0.6,
         match_type: Union[MatchType, str] = MatchType.FULL,
         use_onnx: bool = False,
+        transformers_kwargs: Optional[Dict] = None,
     ):
         """
         Initializes the Language scanner with a list of valid languages.
 
         Parameters:
             valid_languages (Sequence[str]): A list of valid language codes in ISO 639-1.
             threshold (float): Minimum confidence score.
             match_type (MatchType): Whether to match the full text or individual sentences. Default is MatchType.FULL.
             use_onnx (bool): Whether to use ONNX for inference. Default is False.
+            transformers_kwargs (Optional[Dict]): Optional keyword arguments for the transformers pipeline.
         """
         if isinstance(match_type, str):
             match_type = MatchType(match_type)
 
         self._threshold = threshold
         self._valid_languages = valid_languages
         self._match_type = match_type
 
+        transformers_kwargs = transformers_kwargs or {}
+        transformers_kwargs["max_length"] = 512
+        transformers_kwargs["truncation"] = True
+        transformers_kwargs["top_k"] = None
+
         self._pipeline = pipeline(
             task="text-classification",
             model=model_path[0],
             onnx_model=model_path[1],
-            top_k=None,
             use_onnx=use_onnx,
-            truncation=True,
-            max_length=512,
+            **transformers_kwargs,
         )
 
     def scan(self, prompt: str) -> (str, bool, float):
         if prompt.strip() == "":
             return prompt, True, 0.0
 
         results_all = self._pipeline(self._match_type.get_inputs(prompt))
@@ -75,16 +82,16 @@
                 result["label"] for result in result_chunk if result["score"] > self._threshold
             ]
 
             highest_score = max([result["score"] for result in result_chunk])
 
             # Check if any of the languages above threshold are not valid
             if len(set(languages_above_threshold) - set(self._valid_languages)) > 0:
-                logger.warning(
-                    f"Languages {languages_above_threshold} are found with high confidence"
+                LOGGER.warning(
+                    "Languages are found with high confidence", languages=languages_above_threshold
                 )
 
                 return prompt, False, calculate_risk_score(highest_score, self._threshold)
 
-        logger.debug(f"Only valid languages are found in the text.")
+        LOGGER.debug("Only valid languages are found in the text.")
 
         return prompt, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/prompt_injection.py` & `llm-guard-0.3.9/llm_guard/input_scanners/prompt_injection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from enum import Enum
 from typing import Dict, List, Optional, Union
 
 from llm_guard.exception import LLMGuardValidationError
 from llm_guard.transformers_helpers import pipeline
-from llm_guard.util import calculate_risk_score, logger, split_text_by_sentences
+from llm_guard.util import calculate_risk_score, get_logger, split_text_by_sentences
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 # This model is proprietary but open source.
 MODEL_LAIYER = {
-    "path": "laiyer/deberta-v3-base-prompt-injection",
-    "onnx_path": "laiyer/deberta-v3-base-prompt-injection",  # extract from onnx folder
+    "path": "ProtectAI/deberta-v3-base-prompt-injection",
+    "onnx_path": "ProtectAI/deberta-v3-base-prompt-injection",  # extract from onnx folder
     "label": "INJECTION",
     "max_length": 512,
 }
 
 ALL_MODELS = [
     MODEL_LAIYER,
 ]
@@ -40,23 +42,25 @@
     def __init__(
         self,
         *,
         model: Optional[Dict] = None,
         threshold: float = 0.9,
         match_type: Union[MatchType, str] = MatchType.FULL,
         use_onnx: bool = False,
+        transformers_kwargs: Optional[Dict] = None,
     ):
         """
         Initializes PromptInjection with a threshold.
 
         Parameters:
             model (Dict, optional): Chosen model to classify prompt. Default is Laiyer's one.
             threshold (float): Threshold for the injection score. Default is 0.9.
             match_type (MatchType): Whether to match the full text or individual sentences. Default is MatchType.FULL.
             use_onnx (bool): Whether to use ONNX for inference. Defaults to False.
+            transformers_kwargs (Optional[Dict]): Optional keyword arguments for the transformers pipeline.
 
         Raises:
             ValueError: If non-existent models were provided.
         """
         if model is None:
             model = MODEL_LAIYER
 
@@ -65,21 +69,25 @@
 
         if isinstance(match_type, str):
             match_type = MatchType(match_type)
 
         self._threshold = threshold
         self._match_type = match_type
         self._model = model
+
+        transformers_kwargs = transformers_kwargs or {}
+        transformers_kwargs["max_length"] = model["max_length"]
+        transformers_kwargs["truncation"] = True
+
         self._pipeline = pipeline(
             task="text-classification",
             model=model["path"],
             use_onnx=use_onnx,
             onnx_model=model["onnx_path"],
-            truncation=True,
-            max_length=model["max_length"],
+            **transformers_kwargs,
         )
 
     def scan(self, prompt: str) -> (str, bool, float):
         if prompt.strip() == "":
             return prompt, True, 0.0
 
         highest_score = 0.0
@@ -90,14 +98,14 @@
                 2,
             )
 
             if injection_score > highest_score:
                 highest_score = injection_score
 
             if injection_score > self._threshold:
-                logger.warning(f"Detected prompt injection with score: {injection_score}")
+                LOGGER.warning("Detected prompt injection", injection_score=injection_score)
 
                 return prompt, False, calculate_risk_score(injection_score, self._threshold)
 
-        logger.debug(f"No prompt injection detected, highest score: {highest_score}")
+        LOGGER.debug("No prompt injection detected", highest_score=highest_score)
 
         return prompt, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/regex.py` & `llm-guard-0.3.9/llm_guard/input_scanners/regex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import re
 from enum import Enum
 from typing import Pattern, Sequence, Union
 
 from presidio_anonymizer.core.text_replace_builder import TextReplaceBuilder
 
-from llm_guard.util import logger
+from llm_guard.util import get_logger
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 
 class MatchType(Enum):
     SEARCH = "search"
     FULL_MATCH = "fullmatch"
 
     def match(self, pattern: Pattern[str], text: str):
         return getattr(pattern, self.value)(text)
@@ -60,27 +62,27 @@
         text_replace_builder = TextReplaceBuilder(original_text=prompt)
         for pattern in self._patterns:
             match = self._match_type.match(pattern, prompt)
             if match is None:
                 continue
 
             if self._is_blocked:
-                logger.warning(f"Pattern {pattern} was detected in the text")
+                LOGGER.warning("Pattern was detected in the text", pattern=pattern)
 
                 if self._redact:
                     text_replace_builder.replace_text_get_insertion_index(
                         "[REDACTED]",
                         match.start(),
                         match.end(),
                     )
 
                 return text_replace_builder.output_text, False, 1.0
 
-            logger.debug(f"Pattern {pattern} matched the text")
+            LOGGER.debug("Pattern matched the text", pattern=pattern)
             return text_replace_builder.output_text, True, 0.0
 
         if self._is_blocked:
-            logger.debug(f"None of the patterns were found in the text")
+            LOGGER.debug("None of the patterns were found in the text")
             return text_replace_builder.output_text, True, 0.0
 
-        logger.warning(f"None of the patterns matched the text")
+        LOGGER.warning("None of the patterns matched the text")
         return text_replace_builder.output_text, False, 1.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 import os
 import tempfile
 
 from detect_secrets.core.secrets_collection import SecretsCollection
 from detect_secrets.settings import transient_settings
 from presidio_anonymizer.core.text_replace_builder import TextReplaceBuilder
 
-from llm_guard.util import logger
+from llm_guard.util import get_logger
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 _custom_plugins_path = "file://" + os.path.join(
     os.path.dirname(os.path.abspath(__file__)), "secrets_plugins"
 )
 _default_detect_secrets_config = {
     "plugins_used": [
         {"name": "SoftlayerDetector"},
         {"name": "StripeDetector"},
@@ -482,13 +484,13 @@
                     character_start_index,
                     character_end_index,
                 )
 
         os.remove(temp_file.name)
 
         if secret_types:
-            logger.warning(f"Detected secrets in prompt: {secret_types}")
+            LOGGER.warning("Detected secrets in prompt", secret_types=secret_types)
             return text_replace_builder.output_text, False, 1.0
 
-        logger.debug("No secrets detected in the prompt")
+        LOGGER.debug("No secrets detected in the prompt")
 
         return prompt, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/adobe.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/adobe.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/alibaba.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/alibaba.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/asana.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/asana.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/atlassian_api_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/atlassian_api_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/authress_access_key.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/authress_access_key.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/beamer_api_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/beamer_api_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/bitbucket.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/bitbucket.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/bittrex.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/bittrex.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/codecov_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/codecov_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/coinbase_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/coinbase_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/confluent.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/confluent.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/contentful_api_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/contentful_api_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/defined_networking_api_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/defined_networking_api_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/digitalocean.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/digitalocean.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/discord.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/discord.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/droneci_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/droneci_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/dropbox.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/dropbox.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/etsy_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/etsy_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/facebook_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/facebook_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/finicity.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/finicity.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/finnhub_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/finnhub_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/flickr_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/flickr_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/flutterwave.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/flutterwave.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/freshbooks_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/freshbooks_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/github_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/github_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/gitlab.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/gitlab.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/gitter_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/gitter_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/gocardless_api_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/gocardless_api_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/grafana.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/grafana.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/heroku_api_key.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/heroku_api_key.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/hubspot_api_key.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/hubspot_api_key.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/huggingface.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/huggingface.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/jfrog.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/jfrog.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/jwt.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/jwt.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/kraken_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/kraken_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/kucoin.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/kucoin.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/launchdarkly_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/launchdarkly_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/linear.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/linear.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/linkedin.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/linkedin.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/lob.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/lob.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/mailgun.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/mailgun.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/mapbox_api_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/mapbox_api_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/mattermost_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/mattermost_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/messagebird.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/messagebird.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/microsoft_teams_webhook.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/microsoft_teams_webhook.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/netlify_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/netlify_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/new_relic.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/new_relic.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/nytimes_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/nytimes_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/planetscale.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/planetscale.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/sendbird.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/sendbird.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/shopify.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/shopify.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/sidekiq.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/sidekiq.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/slack.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/slack.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/snyk_api_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/snyk_api_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/squarespace_access_token.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/squarespace_access_token.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/sumologic.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/sumologic.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/twitter.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/twitter.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/secrets_plugins/yandex.py` & `llm-guard-0.3.9/llm_guard/input_scanners/secrets_plugins/yandex.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/sentiment.py` & `llm-guard-0.3.9/llm_guard/input_scanners/sentiment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from llm_guard.util import lazy_load_dep, logger
+from llm_guard.util import get_logger, lazy_load_dep
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
 _lexicon = "vader_lexicon"
 
 
 class Sentiment(Scanner):
     """
     A sentiment scanner based on the NLTK's SentimentIntensityAnalyzer. It is used to detect if a prompt
     has a sentiment score lower than the threshold, indicating a negative sentiment.
@@ -30,18 +31,24 @@
         self._sentiment_analyzer = sentiment.SentimentIntensityAnalyzer()
         self._threshold = threshold
 
     def scan(self, prompt: str) -> (str, bool, float):
         sentiment_score = self._sentiment_analyzer.polarity_scores(prompt)
         sentiment_score_compound = sentiment_score["compound"]
         if sentiment_score_compound > self._threshold:
-            logger.debug(f"Sentiment score: {sentiment_score}, threshold: {self._threshold}")
+            LOGGER.debug(
+                "Sentiment score is below the threshold",
+                sentiment_score=sentiment_score_compound,
+                threshold=self._threshold,
+            )
 
             return prompt, True, 0.0
 
-        logger.warning(
-            f"Sentiment score is over threshold: {sentiment_score}, threshold: {self._threshold}"
+        LOGGER.warning(
+            "Sentiment score is above the threshold",
+            sentiment_score=sentiment_score_compound,
+            threshold=self._threshold,
         )
 
         # Normalize such that -1 maps to 1 and threshold maps to 0
         score = round((sentiment_score_compound - (-1)) / (self._threshold - (-1)), 2)
         return prompt, False, score
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/token_limit.py` & `llm-guard-0.3.9/llm_guard/input_scanners/token_limit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import List, Optional
 
-from llm_guard.util import lazy_load_dep, logger
+from llm_guard.util import get_logger, lazy_load_dep
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 
 class TokenLimit(Scanner):
     """
     A token limit scanner based on the tiktoken library. It checks if a prompt exceeds a specific token limit
     and can split a large prompt into chunks of text that each fit within the limit.
     """
 
@@ -53,13 +55,17 @@
 
     def scan(self, prompt: str) -> (str, bool, float):
         if prompt.strip() == "":
             return prompt, True, 0.0
 
         chunks, num_tokens = self._split_text_on_tokens(text=prompt)
         if num_tokens < self._limit:
-            logger.debug(f"Prompt fits the maximum tokens: {num_tokens}, max: {self._limit}")
+            LOGGER.debug(
+                "Prompt fits the maximum tokens", num_tokens=num_tokens, threshold=self._limit
+            )
             return prompt, True, 0.0
 
-        logger.warning(f"Prompt is too big ({num_tokens} tokens). Split into chunks: {chunks}")
+        LOGGER.warning(
+            "Prompt is too big. Splitting into chunks", num_tokens=num_tokens, chunks=chunks
+        )
 
         return chunks[0], False, 1.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/toxicity.py` & `llm-guard-0.3.9/llm_guard/input_scanners/toxicity.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from enum import Enum
-from typing import List, Union
+from typing import Dict, List, Optional, Union
 
 from llm_guard.transformers_helpers import pipeline
-from llm_guard.util import calculate_risk_score, logger, split_text_by_sentences
+from llm_guard.util import calculate_risk_score, get_logger, split_text_by_sentences
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 _model_path = (
     "unitary/unbiased-toxic-roberta",
-    "laiyer/unbiased-toxic-roberta-onnx",  # ONNX model
+    "ProtectAI/unbiased-toxic-roberta-onnx",  # ONNX model
 )
 _toxic_labels = [
     "toxicity",
     "severe_toxicity",
     "obscene",
     "threat",
     "insult",
@@ -42,38 +44,43 @@
 
     def __init__(
         self,
         *,
         threshold: float = 0.5,
         match_type: Union[MatchType, str] = MatchType.FULL,
         use_onnx: bool = False,
+        transformers_kwargs: Optional[Dict] = None,
     ):
         """
         Initializes Toxicity with a threshold for toxicity.
 
         Parameters:
            threshold (float): Threshold for toxicity. Default is 0.5.
            match_type (MatchType): Whether to match the full text or individual sentences. Default is MatchType.FULL.
            use_onnx (bool): Whether to use ONNX for inference. Default is False.
+           transformers_kwargs (Optional[Dict]): Optional keyword arguments for the transformers pipeline.
         """
         if isinstance(match_type, str):
             match_type = MatchType(match_type)
 
         self._threshold = threshold
         self._match_type = match_type
 
+        transformers_kwargs = transformers_kwargs or {}
+        transformers_kwargs["truncation"] = True
+        transformers_kwargs["padding"] = "max_length"
+        transformers_kwargs["top_k"] = None
+        transformers_kwargs["function_to_apply"] = "sigmoid"
+
         self._pipeline = pipeline(
             task="text-classification",
             model=_model_path[0],
             onnx_model=_model_path[1],
-            top_k=None,
             use_onnx=use_onnx,
-            padding="max_length",
-            function_to_apply="sigmoid",
-            truncation=True,
+            **transformers_kwargs,
         )
 
     def scan(self, prompt: str) -> (str, bool, float):
         if prompt.strip() == "":
             return prompt, True, 0.0
 
         inputs = self._match_type.get_inputs(prompt)
@@ -89,14 +96,14 @@
                 if result["score"] > self._threshold:
                     toxicity_above_threshold.append(result)
 
                 if result["score"] > highest_toxicity_score:
                     highest_toxicity_score = result["score"]
 
         if len(toxicity_above_threshold) > 0:
-            logger.warning(f"Detected toxicity in the text: {toxicity_above_threshold}")
+            LOGGER.warning("Detected toxicity in the text", results=toxicity_above_threshold)
 
             return prompt, False, calculate_risk_score(highest_toxicity_score, self._threshold)
 
-        logger.debug(f"Not toxicity found in the text. Results: {results_all}")
+        LOGGER.debug("Not toxicity found in the text", results=results_all)
 
         return prompt, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/input_scanners/util.py` & `llm-guard-0.3.9/llm_guard/input_scanners/util.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/__init__.py` & `llm-guard-0.3.9/llm_guard/output_scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/ban_competitors.py` & `llm-guard-0.3.9/llm_guard/output_scanners/ban_competitors.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/ban_substrings.py` & `llm-guard-0.3.9/llm_guard/output_scanners/ban_substrings.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/ban_topics.py` & `llm-guard-0.3.9/llm_guard/output_scanners/ban_topics.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,25 +15,33 @@
     def __init__(
         self,
         topics: Sequence[str],
         *,
         threshold: float = 0.75,
         model: Optional[Dict] = None,
         use_onnx: bool = False,
+        transformers_kwargs: Optional[Dict] = None,
     ):
         """
         Initializes BanTopics with a list of topics and a probability threshold.
 
         Parameters:
             topics (Sequence[str]): The list of topics to be banned from the text.
             threshold (float): The minimum probability required for a topic to be considered present in the text.
                                Default is 0.75.
             model (Dict, optional): The name of the zero-shot-classification model to be used. Default is MODEL_BASE.
             use_onnx (bool, optional): Whether to use ONNX for inference. Default is False.
+            transformers_kwargs (Dict, optional): Additional kwargs to pass to the transformers pipeline. Default is None.
 
         Raises:
             ValueError: If no topics are provided.
         """
-        self._scanner = InputBanTopics(topics, threshold=threshold, model=model, use_onnx=use_onnx)
+        self._scanner = InputBanTopics(
+            topics,
+            threshold=threshold,
+            model=model,
+            use_onnx=use_onnx,
+            transformers_kwargs=transformers_kwargs,
+        )
 
     def scan(self, prompt: str, output: str) -> (str, bool, float):
         return self._scanner.scan(output)
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/base.py` & `llm-guard-0.3.9/llm_guard/output_scanners/base.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/bias.py` & `llm-guard-0.3.9/llm_guard/output_scanners/bias.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from enum import Enum
-from typing import List, Union
+from typing import Dict, List, Optional, Union
 
 from llm_guard.transformers_helpers import pipeline
-from llm_guard.util import calculate_risk_score, logger, split_text_by_sentences
+from llm_guard.util import calculate_risk_score, get_logger, split_text_by_sentences
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 _model_path = (
     "valurank/distilroberta-bias",
-    "laiyer/distilroberta-bias-onnx",  # ONNX model
+    "ProtectAI/distilroberta-bias-onnx",  # ONNX model
 )
 
 
 class MatchType(Enum):
     SENTENCE = "sentence"
     FULL = "full"
 
@@ -30,35 +32,40 @@
 
     def __init__(
         self,
         *,
         threshold: float = 0.7,
         match_type: Union[MatchType, str] = MatchType.FULL,
         use_onnx: bool = False,
+        transformers_kwargs: Optional[Dict] = None,
     ):
         """
         Initializes the Bias scanner with a probability threshold for bias detection.
 
         Parameters:
            threshold (float): The threshold above which a text is considered biased. Default is 0.7.
            match_type (MatchType): Whether to match the full text or individual sentences. Default is MatchType.FULL.
            use_onnx (bool): Whether to use ONNX instead of PyTorch for inference.
+           transformers_kwargs (dict): Additional keyword arguments to pass to the transformers pipeline.
         """
         if isinstance(match_type, str):
             match_type = MatchType(match_type)
 
         self._threshold = threshold
         self._match_type = match_type
 
+        transformers_kwargs = transformers_kwargs or {}
+        transformers_kwargs["truncation"] = True
+
         self._classifier = pipeline(
             task="text-classification",
             model=_model_path[0],
             onnx_model=_model_path[1],
-            truncation=True,
             use_onnx=use_onnx,
+            **transformers_kwargs,
         )
 
     def scan(self, prompt: str, output: str) -> (str, bool, float):
         if output.strip() == "":
             return output, True, 0.0
 
         highest_score = 0.0
@@ -69,18 +76,14 @@
                 2,
             )
 
             if score > highest_score:
                 highest_score = score
 
             if score > self._threshold:
-                logger.warning(
-                    f"Detected biased text with score: {score}, threshold: {self._threshold}"
-                )
+                LOGGER.warning("Detected biased text", score=score, threshold=self._threshold)
 
                 return output, False, calculate_risk_score(score, self._threshold)
 
-        logger.debug(
-            f"Not biased result. Highest score: {highest_score}, threshold: {self._threshold}"
-        )
+        LOGGER.debug("Not biased result", highest_score=highest_score, threshold=self._threshold)
 
         return output, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/code.py` & `llm-guard-0.3.9/llm_guard/output_scanners/code.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Sequence
+from typing import Dict, Optional, Sequence
 
 from llm_guard.input_scanners.code import Code as InputCode
 
 from .base import Scanner
 
 
 class Code(Scanner):
@@ -16,27 +16,33 @@
     def __init__(
         self,
         languages: Sequence[str],
         *,
         is_blocked: bool = True,
         threshold: float = 0.5,
         use_onnx: bool = False,
+        transformers_kwargs: Optional[Dict] = None,
     ):
         """
         Initializes an instance of the Code class.
 
         Parameters:
             languages (Sequence[str]): The list of programming languages to allow or deny.
             is_blocked (bool): Whether the languages are blocked or allowed. Default is True.
             threshold (float): The threshold for the model output to be considered valid. Default is 0.5.
             use_onnx (bool): Whether to use ONNX for inference. Default is False.
+            transformers_kwargs: Optional[Dict] = None,
 
         Raises:
             ValueError: If both 'allowed' and 'denied' lists are provided or if both are empty.
         """
 
         self._scanner = InputCode(
-            languages, is_blocked=is_blocked, threshold=threshold, use_onnx=use_onnx
+            languages,
+            is_blocked=is_blocked,
+            threshold=threshold,
+            use_onnx=use_onnx,
+            transformers_kwargs=transformers_kwargs,
         )
 
     def scan(self, prompt: str, output: str) -> (str, bool, float):
         return self._scanner.scan(output)
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/deanonymize.py` & `llm-guard-0.3.9/llm_guard/output_scanners/deanonymize.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import re
 from enum import Enum
 from typing import List, Tuple, Union
 
-from llm_guard.util import lazy_load_dep, logger
+from llm_guard.util import get_logger, lazy_load_dep
 from llm_guard.vault import Vault
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 
 class MatchingStrategy(Enum):
     """
     An enum for the different matching strategies used to find placeholders in the model output.
     """
 
     EXACT = "exact"
@@ -24,15 +26,15 @@
         Replaces placeholders in the model output with real values from the vault.
 
         Parameters:
             text (str): The model output.
             vault_items (List[Tuple]): The list of items in the vault.
         """
         for vault_item in vault_items:
-            logger.debug(f"Replaced placeholder ${vault_item[0]} with real value")
+            LOGGER.debug("Replaced placeholder with real value", placeholder=vault_item[0])
             text = text.replace(vault_item[0], vault_item[1])
 
         return text
 
     @staticmethod
     def _match_case_insensitive(text: str, vault_items: List[Tuple]) -> str:
         """
@@ -44,15 +46,15 @@
             JOHN F. KENNEDY -> John F. Kennedy
 
         Parameters:
             text (str): The model output.
             vault_items (List[Tuple]): The list of items in the vault.
         """
         for vault_item in vault_items:
-            logger.debug(f"Replaced placeholder ${vault_item[0]} with real value")
+            LOGGER.debug("Replaced placeholder with real value", placeholder=vault_item[0])
             # Use regular expressions for case-insensitive matching and replacing
             text = re.sub(vault_item[0], vault_item[1], text, flags=re.IGNORECASE)
 
         return text
 
     @staticmethod
     def _match_fuzzy(text: str, vault_items: List[Tuple], max_l_dist: int = 3) -> str:
@@ -67,15 +69,15 @@
         Parameters:
             text (str): The model output.
             vault_items (List[Tuple]): The list of items in the vault.
         """
 
         fuzzysearch = lazy_load_dep("fuzzysearch")
         for vault_item in vault_items:
-            logger.debug(f"Replaced placeholder ${vault_item[0]} with real value")
+            LOGGER.debug("Replaced placeholder with real value", placeholder=vault_item[0])
 
             matches = fuzzysearch.find_near_matches(vault_item[0], text, max_l_dist=max_l_dist)
 
             new_text = ""
             last_end = 0
             for m in matches:
                 # add the text that isn't part of a match
@@ -133,12 +135,12 @@
 
         self._vault = vault
         self._matching_strategy = matching_strategy
 
     def scan(self, prompt: str, output: str) -> (str, bool, float):
         vault_items = self._vault.get()
         if len(vault_items) == 0:
-            logger.warning("No items found in the Vault")
+            LOGGER.warning("No items found in the Vault")
 
         output = self._matching_strategy.match(output, vault_items)
 
         return output, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/factual_consistency.py` & `llm-guard-0.3.9/llm_guard/output_scanners/factual_consistency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from llm_guard.input_scanners.ban_topics import MODEL_BASE
 from llm_guard.transformers_helpers import get_tokenizer_and_model_for_classification
-from llm_guard.util import device, lazy_load_dep, logger
+from llm_guard.util import device, get_logger, lazy_load_dep
 
 from .base import Scanner
 
 torch = lazy_load_dep("torch")
+LOGGER = get_logger(__name__)
 
 _model = MODEL_BASE
 
 
 class FactualConsistency(Scanner):
     """
     FactualConsistency Class:
@@ -49,14 +50,14 @@
         label_names = ["entailment", "not_entailment"]
         prediction = {
             name: round(float(pred), 2) for pred, name in zip(model_prediction, label_names)
         }
 
         entailment_score = prediction["entailment"]
         if entailment_score < self._minimum_score:
-            logger.warning(f"Entailment score is below the threshold: {prediction}")
+            LOGGER.warning("Entailment score is below the threshold", prediction=prediction)
 
             return output, False, prediction["not_entailment"]
 
-        logger.debug(f"The output is factually consistent: {prediction}")
+        LOGGER.debug("The output is factually consistent", prediction=prediction)
 
         return output, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/json.py` & `llm-guard-0.3.9/llm_guard/output_scanners/json.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import json
 import re
 
 import regex
 
-from llm_guard.util import lazy_load_dep, logger
+from llm_guard.util import get_logger, lazy_load_dep
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+JSON_PATTERN = r"(?<!\\)(?:\\\\)*\{(?:[^{}]|(?R))*\}"
+
 
 class JSON(Scanner):
     """
     A scanner class to detect, validate and repair JSON structures within a given output.
 
     It primarily serves to detect JSON objects and arrays using regular expressions,
     then to validate them to ensure their correctness and finally to repair them if necessary.
@@ -22,29 +25,31 @@
         Parameters:
             required_elements (int, optional): The minimum number of JSON elements
             that should be present. Defaults to 0.
             repair (bool, optional): Whether to repair the broken JSON. Defaults to False.
         """
         self._required_elements = required_elements
         self._repair = repair
+        self._pattern = regex.compile(JSON_PATTERN, re.DOTALL)
 
     @staticmethod
     def is_valid_json(json_str: str) -> bool:
         """Check if the input string is a valid JSON.
 
         Parameters:
             json_str (str): The input string to check.
 
         Returns:
             bool: True if the input string is a valid JSON, False otherwise.
         """
         try:
             json.loads(json_str)
             return True
-        except ValueError:
+        except ValueError as e:
+            LOGGER.warning("Invalid JSON", error=e)
             return False
 
     @staticmethod
     def repair_json(json_str: str) -> str:
         """Repair a broken JSON string.
 
         Parameters:
@@ -65,41 +70,52 @@
         return repaired_json
 
     def scan(self, prompt: str, output: str) -> (str, bool, float):
         if prompt.strip() == "":
             return output, True, 0.0
 
         # Find JSON object and array candidates using regular expressions
-        json_candidates = regex.findall(r"(?<!\\)(?:\\\\)*\{(?:[^{}]|(?R))*\}", output, re.DOTALL)
+        json_candidates = self._pattern.findall(output)
 
         # Validate each JSON
         valid_jsons = []
         for json_candidate in json_candidates:
             if self.is_valid_json(json_candidate):
                 valid_jsons.append(json_candidate)
                 continue
 
             if self._repair:
-                logger.warning(f"Found invalid JSON: {json_candidate}. Trying to repair it...")
+                LOGGER.warning(
+                    "Found invalid JSON. Trying to repair it...", json_candidate=json_candidate
+                )
 
                 repaired_json = self.repair_json(json_candidate)
                 if not self.is_valid_json(repaired_json):
-                    logger.warning(f"Could not repair JSON: {repaired_json}. Skipping...")
+                    LOGGER.warning(
+                        "Could not repair JSON. Skipping...", repaired_json=repaired_json
+                    )
+
                     continue
 
                 valid_jsons.append(repaired_json)
                 output = output.replace(json_candidate, repaired_json)
 
         # Check if there are enough valid JSONs
         if len(valid_jsons) < self._required_elements:
-            logger.warning(
-                f"There should be at least {self._required_elements} JSONs but {len(valid_jsons)} found"
+            LOGGER.warning(
+                "Not all required JSON elements are found",
+                num_required_elements=self._required_elements,
+                num_found=len(valid_jsons),
             )
             return output, False, 1.0
 
         # Compare
         if len(valid_jsons) != len(json_candidates):
-            logger.warning(f"Only {len(valid_jsons)}/{len(json_candidates)} JSONs are valid")
+            LOGGER.warning(
+                "Only some JSONs are valid",
+                num_valid=len(valid_jsons),
+                num_total=len(json_candidates),
+            )
 
             return output, False, 1.0
 
         return output, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/language.py` & `llm-guard-0.3.9/llm_guard/output_scanners/language.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Sequence, Union
+from typing import Dict, Optional, Sequence, Union
 
 from llm_guard.input_scanners.language import Language as InputLanguage
 from llm_guard.input_scanners.language import MatchType
 
 from .base import Scanner
 
 
@@ -15,27 +15,30 @@
     def __init__(
         self,
         valid_languages: Sequence[str],
         *,
         threshold: float = 0.7,
         match_type: Union[MatchType, str] = MatchType.FULL,
         use_onnx: bool = False,
+        transformers_kwargs: Optional[Dict] = None,
     ):
         """
         Initializes the Language scanner with a list of valid languages.
 
         Parameters:
             valid_languages (Sequence[str]): A list of valid language codes.
             threshold (float): Minimum confidence score.
             match_type (MatchType): Whether to match the full text or individual sentences. Default is MatchType.FULL.
             use_onnx (bool): Whether to use ONNX for inference. Default is False.
+            transformers_kwargs (dict): Additional keyword arguments to pass to the transformers pipeline.
         """
 
         self._scanner = InputLanguage(
             valid_languages,
             threshold=threshold,
             match_type=match_type,
             use_onnx=use_onnx,
+            transformers_kwargs=transformers_kwargs,
         )
 
     def scan(self, prompt: str, output: str) -> (str, bool, float):
         return self._scanner.scan(output)
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/language_same.py` & `llm-guard-0.3.9/llm_guard/output_scanners/language_same.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,52 @@
+from typing import Dict, Optional
+
 from llm_guard.input_scanners.language import model_path
 from llm_guard.transformers_helpers import pipeline
-from llm_guard.util import logger
+from llm_guard.util import get_logger
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 
 class LanguageSame(Scanner):
     """
     LanguageSame class is responsible for detecting and comparing the language of given prompt and model output to ensure they are the same.
     """
 
     def __init__(
         self,
         *,
         threshold: float = 0.1,
         use_onnx: bool = False,
+        transformers_kwargs: Optional[Dict] = None,
     ):
         """
         Initializes the LanguageSame scanner.
 
         Parameters:
             threshold (float): Minimum confidence score
             use_onnx (bool): Whether to use ONNX for inference. Default is False.
+            transformers_kwargs (dict): Additional keyword arguments to pass to the transformers pipeline.
         """
 
         self._threshold = threshold
+
+        transformers_kwargs = transformers_kwargs or {}
+        transformers_kwargs["max_length"] = 512
+        transformers_kwargs["truncation"] = True
+        transformers_kwargs["top_k"] = None
+
         self._pipeline = pipeline(
             task="text-classification",
             model=model_path[0],
             onnx_model=model_path[1],
-            top_k=None,
             use_onnx=use_onnx,
-            truncation=True,
-            max_length=512,
+            **transformers_kwargs,
         )
 
     def scan(self, prompt: str, output: str) -> (str, bool, float):
         if prompt.strip() == "" or output.strip() == "":
             return prompt, True, 0.0
 
         detected_languages = self._pipeline([prompt, output])
@@ -48,21 +58,25 @@
         output_languages = [
             detected_language["label"]
             for detected_language in detected_languages[1]
             if detected_language["score"] > self._threshold
         ]
 
         if len(prompt_languages) == 0:
-            logger.warning(f"None of languages are above found in the prompt")
+            LOGGER.warning("None of languages are above found in the prompt")
             return output, False, 1.0
 
         if len(output_languages) == 0:
-            logger.warning(f"None of languages are above threshold found in the output")
+            LOGGER.warning("None of languages are above threshold found in the output")
             return output, False, 1.0
 
         common_languages = list(set(prompt_languages).intersection(output_languages))
         if len(common_languages) == 0:
-            logger.warning(f"No common languages in the output and prompt: {common_languages}")
+            LOGGER.warning(
+                "No common languages in the output and prompt", common_languages=common_languages
+            )
             return output, False, 1.0
 
-        logger.debug(f"Languages {common_languages} are found in the prompt and output")
+        LOGGER.debug(
+            "Languages are found in the prompt and output", common_languages=common_languages
+        )
         return output, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/malicious_urls.py` & `llm-guard-0.3.9/llm_guard/output_scanners/malicious_urls.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from typing import Dict, Optional
+
 from llm_guard.transformers_helpers import pipeline
-from llm_guard.util import calculate_risk_score, extract_urls, logger
+from llm_guard.util import calculate_risk_score, extract_urls, get_logger
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
 _model_path = (
     "DunnBC22/codebert-base-Malicious_URLs",
-    "laiyer/codebert-base-Malicious_URLs-onnx",  # ONNX version
+    "ProtectAI/codebert-base-Malicious_URLs-onnx",  # ONNX version
 )
 
 _malicious_labels = [
     "defacement",
     "phishing",
     "malware",
 ]
@@ -20,53 +23,62 @@
     This scanner is used to scan and detect malicious URLs in the text.
 
     Large Language Models can occasionally produce malicious URLs in their outputs.
     Using the "DunnBC22/codebert-base-Malicious_URLs" model from HuggingFace, this class classifies
     URLs as either malicious or benign to safeguard users from potential threats.
     """
 
-    def __init__(self, *, threshold=0.5, use_onnx: bool = False):
+    def __init__(
+        self, *, threshold=0.5, use_onnx: bool = False, transformers_kwargs: Optional[Dict] = None
+    ):
         """
         Initializes an instance of the MaliciousURLs class.
 
         Parameters:
             threshold (float): The threshold used to determine if the website is malicious. Defaults to 0.5.
             use_onnx (bool): Whether to use the ONNX version of the model. Defaults to False.
+            transformers_kwargs (dict): Additional keyword arguments to pass to the transformers pipeline.
         """
 
         self._threshold = threshold
+
+        transformers_kwargs = transformers_kwargs or {}
+        transformers_kwargs["max_length"] = 512
+        transformers_kwargs["truncation"] = True
+        transformers_kwargs["top_k"] = None
+
         self._classifier = pipeline(
             task="text-classification",
             model=_model_path[0],
             onnx_model=_model_path[1],
-            truncation=True,
             use_onnx=use_onnx,
-            top_k=None,
-            max_length=512,
+            **transformers_kwargs,
         )
 
     def scan(self, prompt: str, output: str) -> (str, bool, float):
         if output.strip() == "":
             return output, True, 0.0
 
         urls = extract_urls(output)
         if len(urls) == 0:
             return output, True, 0.0
 
-        logger.debug(f"Found {len(urls)} URLs in the output")
+        LOGGER.debug("Found URLs in the output", len=len(urls))
 
         results = self._classifier(urls)
         for url, result in zip(urls, results):
             malicious_scores = [
                 item["score"] for item in result if item["label"] in _malicious_labels
             ]
             highest_malicious_score = max(malicious_scores)
             if highest_malicious_score > self._threshold:
-                logger.warning(
-                    f"Detected malware URL '{url}' with score: {highest_malicious_score}"
+                LOGGER.warning(
+                    "Detected malware URL",
+                    url=url,
+                    highest_malicious_score=highest_malicious_score,
                 )
 
                 return output, False, calculate_risk_score(highest_malicious_score, self._threshold)
 
-        logger.debug(f"Not malware URLs in the output: {results}")
+        LOGGER.debug("Not malware URLs in the output", results=results)
 
         return output, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/reading_time.py` & `llm-guard-0.3.9/llm_guard/output_scanners/reading_time.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from llm_guard.util import logger
+from llm_guard.util import get_logger
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 
 class ReadingTime(Scanner):
     """
     Scanner that checks the reading time of the output against a maximum time.
 
     If the output exceeds the maximum time, the output will be truncated to fit within the time limit.
     """
@@ -22,17 +24,21 @@
 
     def scan(self, prompt: str, output: str) -> (str, bool, float):
         words = output.split()
         word_count = len(words)
         reading_time_minutes = word_count / self._words_per_minute
 
         if reading_time_minutes > self._max_time:
-            logger.warning(f"Output exceeded maximum reading time of {self._max_time} minutes")
+            LOGGER.warning(
+                "Output exceeded maximum reading time",
+                reading_time_minutes=reading_time_minutes,
+                max_reading_time_minutes=self._max_time,
+            )
             if self._truncate:
                 # Calculate the maximum number of words to fit within the time limit
                 max_words = int(self._max_time * self._words_per_minute)
                 output = " ".join(words[:max_words])
 
             return output, False, 1.0
 
-        logger.debug(f"Output reading time: {reading_time_minutes} minutes")
+        LOGGER.debug("Output reading time", reading_time_minutes=reading_time_minutes)
         return output, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/regex.py` & `llm-guard-0.3.9/llm_guard/output_scanners/regex.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/relevance.py` & `llm-guard-0.3.9/llm_guard/output_scanners/relevance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Tuple
 
 from llm_guard.exception import LLMGuardValidationError
 from llm_guard.transformers_helpers import get_tokenizer, is_onnx_supported
-from llm_guard.util import device, lazy_load_dep, logger
+from llm_guard.util import device, get_logger, lazy_load_dep
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 MODEL_EN_BGE_BASE = (
     "BAAI/bge-base-en-v1.5",
     "zeroshot/bge-base-en-v1.5-quant",  # Quantized and converted to ONNX version of BGE base
 )
 MODEL_EN_BGE_LARGE = (
     "BAAI/bge-large-en-v1.5",
     "zeroshot/bge-large-en-v1.5-quant",  # Quantized and converted to ONNX version of BGE large
@@ -53,15 +55,15 @@
 
         model_path = model[0]
 
         self.pooling_method = "cls"
         self.normalize_embeddings = True
 
         if use_onnx and is_onnx_supported() is False:
-            logger.warning("ONNX is not supported on this machine. Using PyTorch instead of ONNX.")
+            LOGGER.warning("ONNX is not supported on this machine. Using PyTorch instead of ONNX.")
             use_onnx = False
 
         if use_onnx:
             model_path = model[1]
             optimum_onnxruntime = lazy_load_dep(
                 "optimum.onnxruntime",
                 "optimum[onnxruntime-gpu]" if device().type == "cuda" else "optimum[onnxruntime]",
@@ -70,19 +72,19 @@
                 model_path,
                 export=False,
                 provider="CUDAExecutionProvider"
                 if device().type == "cuda"
                 else "CPUExecutionProvider",
                 use_io_binding=True if device().type == "cuda" else False,
             )
-            logger.debug(f"Initialized ONNX model {model_path} on device {device()}")
+            LOGGER.debug("Initialized ONNX model", model=model_path, device=device())
         else:
             transformers = lazy_load_dep("transformers")
             self._model = transformers.AutoModel.from_pretrained(model_path).to(device())
-            logger.debug(f"Initialized model {model_path} on device {device()}")
+            LOGGER.debug("Initialized model", model=model_path, device=device())
             self._model.eval()
 
         self._tokenizer = get_tokenizer(model_path)
 
     def pooling(self, last_hidden_state: torch.Tensor, attention_mask: torch.Tensor = None):
         if self.pooling_method == "cls":
             return last_hidden_state[:, 0]
@@ -113,14 +115,14 @@
             return output, True, 0.0
 
         prompt_embedding = self._encode(prompt)
         output_embedding = self._encode(output)
         similarity = prompt_embedding @ output_embedding.T
 
         if similarity < self._threshold:
-            logger.warning(f"Result is not similar to the prompt. Similarity score: {similarity}")
+            LOGGER.warning("Result is not similar to the prompt", similarity_score=similarity)
 
             return output, False, round(1 - similarity, 2)
 
-        logger.debug(f"Result is similar to the prompt. Similarity score: {similarity}")
+        LOGGER.debug("Result is similar to the prompt", similarity_score=similarity)
 
         return output, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/sensitive.py` & `llm-guard-0.3.9/llm_guard/output_scanners/sensitive.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,20 @@
     sensitive_patterns_path,
 )
 from llm_guard.input_scanners.anonymize_helpers import (
     BERT_BASE_NER_CONF,
     get_analyzer,
     get_transformers_recognizer,
 )
-from llm_guard.util import logger
+from llm_guard.util import get_logger
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 
 class Sensitive(Scanner):
     """
     A class used to detect sensitive (PII) data in the output of a language model.
 
     This class uses the Presidio Analyzer Engine and predefined internally patterns (sensitive_patterns.json) to analyze the output for specified entity types.
     If no entity types are specified, it defaults to checking for all entity types.
@@ -44,15 +46,17 @@
            regex_pattern_groups_path (str): Path to the regex patterns file. Default is sensitive_patterns.json.
            redact (bool): Redact found sensitive entities. Default to False.
            recognizer_conf (Optional[Dict]): Configuration to recognize PII data. Default is dslim/bert-base-NER.
            threshold (float): Acceptance threshold. Default is 0.
            use_onnx (bool): Use ONNX model for inference. Default is False.
         """
         if not entity_types:
-            logger.debug(f"No entity types provided, using default: {default_entity_types}")
+            LOGGER.debug(
+                "No entity types provided, using default", default_entity_types=default_entity_types
+            )
             entity_types = default_entity_types.copy()
         entity_types.append("CUSTOM")
 
         self._entity_types = entity_types
         self._redact = redact
         self._threshold = threshold
 
@@ -71,17 +75,17 @@
             language="en",
             entities=self._entity_types,
             score_threshold=self._threshold,
         )
 
         if analyzer_results:
             if self._redact:
-                logger.debug(f"Redacting sensitive entities")
+                LOGGER.debug("Redacting sensitive entities")
                 result = self._anonymizer.anonymize(text=output, analyzer_results=analyzer_results)
                 output = result.text
 
             risk_score = max(analyzer_result.score for analyzer_result in analyzer_results)
-            logger.warning(f"Found sensitive data in the output {analyzer_results}")
+            LOGGER.warning("Found sensitive data in the output", results=analyzer_results)
             return output, False, risk_score
 
-        logger.debug(f"No sensitive data found in the output")
+        LOGGER.debug("No sensitive data found in the output")
         return output, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/sentiment.py` & `llm-guard-0.3.9/llm_guard/output_scanners/sentiment.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/toxicity.py` & `llm-guard-0.3.9/llm_guard/output_scanners/toxicity.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union
+from typing import Dict, Optional, Union
 
 from llm_guard.input_scanners.toxicity import MatchType
 from llm_guard.input_scanners.toxicity import Toxicity as InputToxicity
 
 from .base import Scanner
 
 
@@ -15,21 +15,28 @@
 
     def __init__(
         self,
         *,
         threshold: float = 0.7,
         match_type: Union[MatchType, str] = MatchType.FULL,
         use_onnx: bool = False,
+        transformers_kwargs: Optional[Dict] = None,
     ):
         """
         Initializes an instance of the Toxicity class.
 
         Parameters:
             threshold (float): The threshold used to determine toxicity. Defaults to 0.7.
             match_type (MatchType): Whether to match the full text or individual sentences. Defaults to MatchType.FULL.
             use_onnx (bool): Whether to use ONNX for inference. Defaults to False.
+            transformers_kwargs (dict): Additional keyword arguments to pass to the transformers pipeline.
         """
 
-        self._scanner = InputToxicity(threshold=threshold, match_type=match_type, use_onnx=use_onnx)
+        self._scanner = InputToxicity(
+            threshold=threshold,
+            match_type=match_type,
+            use_onnx=use_onnx,
+            transformers_kwargs=transformers_kwargs,
+        )
 
     def scan(self, prompt: str, output: str) -> (str, bool, float):
         return self._scanner.scan(output)
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/url_reachabitlity.py` & `llm-guard-0.3.9/llm_guard/output_scanners/url_reachabitlity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import List
 
 import requests
 
-from llm_guard.util import extract_urls, logger
+from llm_guard.util import extract_urls, get_logger
 
 from .base import Scanner
 
+LOGGER = get_logger(__name__)
+
 
 class URLReachability(Scanner):
     """
     This scanner checks URLs for their reachability.
     """
 
     def __init__(self, *, success_status_codes: List[int] = None, timeout: int = 5):
@@ -39,17 +41,17 @@
             return False
 
     def scan(self, prompt: str, output: str) -> (str, bool, float):
         urls = extract_urls(output)
         if not urls:
             return output, True, 0.0
 
-        logger.debug(f"Found {len(urls)} URLs in the output")
+        LOGGER.debug("Found URLs in the output", len=len(urls))
 
         unreachable_urls = [url for url in urls if not self.is_reachable(url)]
 
         if unreachable_urls:
-            logger.warning(f"Unreachable URLs detected: {unreachable_urls}")
+            LOGGER.warning(f"Unreachable URLs detected", urls=unreachable_urls)
             return output, False, 1.0
 
-        logger.debug("All URLs are reachable.")
+        LOGGER.debug("All URLs are reachable.")
         return output, True, 0.0
```

### Comparing `llm-guard-0.3.7/llm_guard/output_scanners/util.py` & `llm-guard-0.3.9/llm_guard/output_scanners/util.py`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/resources/output_stop_substrings.json` & `llm-guard-0.3.9/llm_guard/resources/output_stop_substrings.json`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/resources/prompt_stop_substrings.json` & `llm-guard-0.3.9/llm_guard/resources/prompt_stop_substrings.json`

 * *Files identical despite different names*

### Comparing `llm-guard-0.3.7/llm_guard/transformers_helpers.py` & `llm-guard-0.3.9/llm_guard/transformers_helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import importlib
 from functools import lru_cache
 from typing import Literal, Optional, get_args
 
 from .exception import LLMGuardValidationError
-from .util import device, lazy_load_dep, logger
+from .util import device, get_logger, lazy_load_dep
+
+LOGGER = get_logger(__name__)
 
 
 @lru_cache(maxsize=None)  # Set maxsize=None for an unbounded cache
 def get_tokenizer(model_identifier: str):
     """
     This function loads a tokenizer given a model identifier and caches it.
     Subsequent calls with the same model_identifier will return the cached tokenizer.
@@ -20,15 +22,15 @@
     return tokenizer
 
 
 @lru_cache(maxsize=None)  # Unbounded cache
 def is_onnx_supported() -> bool:
     is_supported = importlib.util.find_spec("optimum.onnxruntime") is not None
     if not is_supported:
-        logger.warning(
+        LOGGER.warning(
             "ONNX Runtime is not available. "
             "Please install optimum: "
             "`pip install llm-guard[onnxruntime]` for CPU or "
             "`pip install llm-guard[onnxruntime-gpu]` for GPU to enable ONNX Runtime optimizations."
         )
 
     return is_supported
@@ -42,26 +44,26 @@
             export=export,
             subfolder=subfolder,
             file_name="model.onnx",
             provider="CUDAExecutionProvider",
             use_io_binding=True,
         )
 
-        logger.debug(f"Initialized classification ONNX model {model} on CUDA device {device()}")
+        LOGGER.debug("Initialized classification ONNX model", model=model, device=device())
 
         return tf_model
 
     optimum_onnxruntime = lazy_load_dep("optimum.onnxruntime", "optimum[onnxruntime]")
     tf_model = optimum_onnxruntime.ORTModelForSequenceClassification.from_pretrained(
         model,
         export=export,
         subfolder=subfolder,
         file_name="model.onnx",
     )
-    logger.debug(f"Initialized classification ONNX model {model} on device {device()}")
+    LOGGER.debug("Initialized classification ONNX model", model=model, device=device())
 
     return tf_model
 
 
 def get_tokenizer_and_model_for_classification(
     model: str, onnx_model: Optional[str] = None, use_onnx: bool = False, **kwargs
 ):
@@ -78,20 +80,20 @@
     tf_tokenizer = get_tokenizer(model)
     transformers = lazy_load_dep("transformers")
 
     if kwargs.get("max_length", None) is None:
         kwargs["max_length"] = tf_tokenizer.model_max_length
 
     if use_onnx and is_onnx_supported() is False:
-        logger.warning("ONNX is not supported on this machine. Using PyTorch instead of ONNX.")
+        LOGGER.warning("ONNX is not supported on this machine. Using PyTorch instead of ONNX.")
         use_onnx = False
 
     if use_onnx is False:
         tf_model = transformers.AutoModelForSequenceClassification.from_pretrained(model)
-        logger.debug(f"Initialized classification model {model} on device {device()}")
+        LOGGER.debug("Initialized classification model", model=model, device=device())
 
         return tf_tokenizer, tf_model
 
     subfolder = "onnx" if onnx_model == model else ""
     if onnx_model is not None:
         model = onnx_model
 
@@ -133,35 +135,37 @@
 
 
 def _pipeline_ner(model: str, onnx_model: Optional[str] = None, use_onnx: bool = False, **kwargs):
     transformers = lazy_load_dep("transformers")
     tf_tokenizer = get_tokenizer(model)
 
     if use_onnx and is_onnx_supported() is False:
-        logger.warning("ONNX is not supported on this machine. Using PyTorch instead of ONNX.")
+        LOGGER.warning("ONNX is not supported on this machine. Using PyTorch instead of ONNX.")
         use_onnx = False
 
     if use_onnx:
+        subfolder = "onnx" if onnx_model == model else ""
         if onnx_model is not None:
             model = onnx_model
 
         optimum_onnxruntime = lazy_load_dep(
             "optimum.onnxruntime",
             "optimum[onnxruntime]" if device().type != "cuda" else "optimum[onnxruntime-gpu]",
         )
         tf_model = optimum_onnxruntime.ORTModelForTokenClassification.from_pretrained(
             model,
             export=onnx_model is None,
+            subfolder=subfolder,
             provider="CUDAExecutionProvider" if device().type == "cuda" else "CPUExecutionProvider",
             use_io_binding=True if device().type == "cuda" else False,
         )
-        logger.debug(f"Initialized ner pipeline for ONNX model {model} on device {device()}")
+        LOGGER.debug("Initialized NER ONNX model", model=model, device=device())
     else:
         tf_model = transformers.AutoModelForTokenClassification.from_pretrained(model)
-        logger.debug(f"Initialized ner pipeline for model {model} on device {device()}")
+        LOGGER.debug("Initialized NER model", model=model, device=device())
 
     return transformers.pipeline(
         "ner",
         model=tf_model,
         tokenizer=tf_tokenizer,
         device=device(),
         batch_size=1,
```

### Comparing `llm-guard-0.3.7/llm_guard/util.py` & `llm-guard-0.3.9/llm_guard/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,66 @@
 import importlib
 import json
 import logging
 import re
+import sys
 from functools import lru_cache
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Literal, Optional
 
-logging.basicConfig(level=logging.INFO)
-logger = logging.getLogger("llm-guard")
+import structlog
+
+LOGGER = structlog.getLogger(__name__)
 
 """
 This file contains utility functions.
 This is meant for internal use and not part of the public API.
 """
 
+LOG_LEVELS = Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
+EXTERNAL_LOGGERS = {
+    "transformers",
+}
+
+
+def configure_logger(log_level: LOG_LEVELS = "INFO"):
+    """
+    Configures the logger for the package.
+
+    Args:
+        log_level: The log level to use for the logger. It should be one of the following strings:
+            "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL".
+    """
+    logging.basicConfig(
+        format="[%(asctime)s - %(name)s - %(levelname)s] %(message)s",
+        level=log_level,
+        stream=sys.stdout,
+    )
+    structlog.configure(logger_factory=structlog.stdlib.LoggerFactory())
+    for log_name in EXTERNAL_LOGGERS:
+        logging.getLogger(log_name).setLevel(logging.WARNING)
+
+
+def _get_library_name() -> str:
+    return __name__.split(".")[0]
+
+
+def _get_library_root_logger() -> logging.Logger:
+    return logging.getLogger(_get_library_name())
+
+
+def get_logger(name: Optional[str] = None) -> Any:
+    """
+    Return a logger with the specified name.
+    """
+
+    if name is None:
+        name = _get_library_name()
+
+    return structlog.getLogger(name)
+
 
 # Detect pytorch device
 @lru_cache(maxsize=None)  # Unbounded cache
 def device():
     torch = lazy_load_dep("torch")
     if torch.cuda.is_available():
         return torch.device("cuda:0")
@@ -42,19 +86,19 @@
         json.decoder.JSONDecodeError: If the provided file cannot be parsed as JSON.
     """
 
     result = {}
     try:
         with open(json_path, "r") as myfile:
             result = json.load(myfile)
-            logger.debug(f"Loaded json file {json_path}")
+            LOGGER.debug("Loaded json file", path=json_path)
     except FileNotFoundError:
-        logger.error(f"Could not find {json_path}")
+        LOGGER.error("Could not find file", path=json_path)
     except json.decoder.JSONDecodeError as json_error:
-        logger.error(f"Could not parse {json_path}: {json_error}")
+        LOGGER.error("Could not parse file", path=json_path, error=json_error)
     return result
 
 
 def combine_json_results(results: Dict[str, List[str]]) -> List[str]:
     """
     Combines values from a dictionary with list values into a single list.
 
@@ -79,15 +123,15 @@
     """
 
     if package_name is None:
         package_name = import_name
 
     spec = importlib.util.find_spec(import_name)
     if spec is None:
-        logger.warning(
+        LOGGER.warning(
             f"Optional feature dependent on missing package: {import_name} was initialized.\n"
             f"Use `pip install {package_name}` to install the package if running locally."
         )
 
     return importlib.import_module(import_name)
```

### Comparing `llm-guard-0.3.7/llm_guard/vault.py` & `llm-guard-0.3.9/llm_guard/vault.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,7 +23,13 @@
         self._tuples.extend(new_tuples)
 
     def remove(self, tuple_to_remove: Tuple):
         self._tuples.remove(tuple_to_remove)
 
     def get(self) -> List[Tuple]:
         return self._tuples
+
+    def placeholder_exists(self, placeholder: str) -> bool:
+        for entity_placeholder, _ in self._tuples:
+            if placeholder == entity_placeholder:
+                return True
+        return False
```

### Comparing `llm-guard-0.3.7/llm_guard.egg-info/PKG-INFO` & `llm-guard-0.3.9/llm_guard.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: llm-guard
-Version: 0.3.7
+Version: 0.3.9
 Summary: LLM-Guard is a comprehensive tool designed to fortify the security of Large Language Models (LLMs). By offering sanitization, detection of harmful language, prevention of data leakage, and resistance against prompt injection attacks, LLM-Guard ensures that your interactions with LLMs remain safe and secure.
-Author-email: "Laiyer.ai" <hello@laiyer.ai>
+Author-email: Protect AI <community@protectai.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -21,18 +21,18 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://github.com/laiyer-ai/llm-guard
+Project-URL: homepage, https://github.com/protectai/llm-guard
 Project-URL: documentation, https://llm-guard.com/
-Project-URL: repository, https://github.com/laiyer-ai/llm-guard
-Project-URL: issues, https://github.com/laiyer-ai/llm-guard/issues
+Project-URL: repository, https://github.com/protectai/llm-guard
+Project-URL: issues, https://github.com/protectai/llm-guard/issues
 Project-URL: changelog, https://llm-guard.com/changelog/
 Keywords: llm,language model,security,adversarial attacks,prompt injection,prompt leakage,PII detection,self-hardening,firewall
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -40,69 +40,69 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: detect-secrets==1.4.0
 Requires-Dist: faker<23,>=22
 Requires-Dist: fuzzysearch==0.7.3
-Requires-Dist: json-repair==0.4.5
+Requires-Dist: json-repair==0.8.0
 Requires-Dist: nltk<4,>=3.8
 Requires-Dist: presidio-analyzer<3,>=2.2
 Requires-Dist: presidio-anonymizer<3,>=2.2
-Requires-Dist: protobuf<4,>=3.20
+Requires-Dist: protobuf>=4
 Requires-Dist: regex==2023.12.25
 Requires-Dist: sentencepiece==0.1.99
 Requires-Dist: tiktoken<0.6,>=0.5
 Requires-Dist: torch==2.0.1
 Requires-Dist: transformers==4.36.2
 Requires-Dist: xformers==0.0.22
 Requires-Dist: span-marker==1.5.0
+Requires-Dist: structlog>=24
 Provides-Extra: onnxruntime
 Requires-Dist: optimum[onnxruntime]; extra == "onnxruntime"
 Provides-Extra: onnxruntime-gpu
 Requires-Dist: optimum[onnxruntime-gpu]; extra == "onnxruntime-gpu"
 Provides-Extra: docs-dev
 Requires-Dist: mkdocs<2,>=1.5; extra == "docs-dev"
 Requires-Dist: mkdocs-autorefs==0.5.0; extra == "docs-dev"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.2; extra == "docs-dev"
 Requires-Dist: mkdocs-jupyter==0.24.6; extra == "docs-dev"
-Requires-Dist: mkdocs-material==9.5.3; extra == "docs-dev"
+Requires-Dist: mkdocs-material==9.5.6; extra == "docs-dev"
 Requires-Dist: mkdocs-material-extensions==1.3.1; extra == "docs-dev"
-Requires-Dist: mkdocs-swagger-ui-tag==0.6.7; extra == "docs-dev"
+Requires-Dist: mkdocs-swagger-ui-tag==0.6.8; extra == "docs-dev"
 Requires-Dist: mkdocstrings==0.24.0; extra == "docs-dev"
 Requires-Dist: mkdocstrings-python==1.8.0; extra == "docs-dev"
 Provides-Extra: dev
 Requires-Dist: llm_guard[docs-dev]; extra == "dev"
 Requires-Dist: autoflake<3,>=2; extra == "dev"
 Requires-Dist: black<24,>=23; extra == "dev"
 Requires-Dist: isort<6,>5; extra == "dev"
-Requires-Dist: pytest<8,>=7.4; extra == "dev"
+Requires-Dist: pytest<9,>=7.4; extra == "dev"
 Requires-Dist: pytest-cov<5,>=4.1; extra == "dev"
 Requires-Dist: pre-commit<4,>=3.6; extra == "dev"
 
 # LLM Guard - The Security Toolkit for LLM Interactions
 
-LLM Guard by [Laiyer.ai](https://laiyer.ai) is a comprehensive tool designed to fortify the security of Large Language Models (LLMs).
+LLM Guard by [Protect AI](https://protectai.com/llm-guard) is a comprehensive tool designed to fortify the security of Large Language Models (LLMs).
 
-[**Documentation**](https://laiyer-ai.github.io/llm-guard/) | [**Playground**](https://huggingface.co/spaces/laiyer/llm-guard-playground) | [**Changelog**](https://llm-guard.com/changelog/) | [**Blog**](https://substack.com/@laiyer)
+[**Documentation**](https://llm-guard.com/) | [**Playground**](https://huggingface.co/spaces/ProtectAI/llm-guard-playground) | [**Changelog**](https://llm-guard.com/changelog/)
 
 [![GitHub
-stars](https://img.shields.io/github/stars/laiyer-ai/llm-guard.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/laiyer-ai/llm-guard/stargazers/)
+stars](https://img.shields.io/github/stars/protectai/llm-guard.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/protectai/llm-guard/stargazers/)
 [![MIT license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](http://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Python Version](https://img.shields.io/pypi/v/llm-guard)](https://pypi.org/project/llm-guard)
 [![Downloads](https://static.pepy.tech/badge/llm-guard)](https://pepy.tech/project/llm-guard)
 [![Downloads](https://static.pepy.tech/badge/llm-guard/month)](https://pepy.tech/project/llm-guard)
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/laiyer_ai.svg?style=social&label=Follow%20%40Laiyer_AI)](https://twitter.com/laiyer_ai)
 
-<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/laiyer-ai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
+<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/protectai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
 
 ## What is LLM Guard?
 
-![LLM-Guard](https://github.com/laiyer-ai/llm-guard/blob/main/docs/assets/flow.png?raw=true)
+![LLM-Guard](https://github.com/protectai/llm-guard/blob/main/docs/assets/flow.png?raw=true)
 
 By offering sanitization, detection of harmful language, prevention of data leakage, and resistance against prompt
 injection attacks, LLM-Guard ensures that your interactions with LLMs remain safe and secure.
 
 ## Installation
 
 Begin your journey with LLM Guard by downloading the package:
@@ -177,30 +177,23 @@
 We are committed to a transparent development process and highly appreciate any contributions.
 Whether you are helping us fix bugs, propose new features, improve our documentation or spread the word,
 we would love to have you as part of our community.
 
 - Give us a ⭐️ github star ⭐️ on the top of this page to support what we're doing,
   it means a lot for open source projects!
 - Read our
-  [docs](https://laiyer-ai.github.io/llm-guard/)
+  [docs](https://llm-guard.com/)
   for more info about how to use and customize LLM Guard, and for step-by-step tutorials.
 - Post a [Github
-  Issue](https://github.com/laiyer-ai/llm-guard/issues) to submit a bug report, feature request, or suggest an improvement.
+  Issue](https://github.com/protectai/llm-guard/issues) to submit a bug report, feature request, or suggest an improvement.
 - To contribute to the package, check out our [contribution guidelines](CONTRIBUTING.md), and open a PR.
 
 Join our Slack to give us feedback, connect with the maintainers and fellow users, ask questions,
 get help for package usage or contributions, or engage in discussions about LLM security!
 
-<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/laiyer-ai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
+<a href="https://join.slack.com/t/laiyerai/shared_invite/zt-28jv3ci39-sVxXrLs3rQdaN3mIl9IT~w"><img src="https://github.com/protectai/llm-guard/blob/main/docs/assets/join-our-slack-community.png?raw=true" width="200"></a>
 
 ### Production Support
 
 We're eager to provide personalized assistance when deploying your LLM Guard to a production environment.
 
-- [Send Email ✉️](mailto:hello@laiyer.ai)
-
-## Supporters
-
-LLM Guard is supported by the following organizations:
-
-- [Google Patch Rewards program](https://bughunters.google.com/open-source-security/patch-rewards)
-- [JetBrains](https://jb.gg/OpenSourceSupport)
+- [Send Email ✉️](mailto:community@protectai.com)
```

### Comparing `llm-guard-0.3.7/llm_guard.egg-info/SOURCES.txt` & `llm-guard-0.3.9/llm_guard.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,21 @@
 llm_guard/input_scanners/toxicity.py
 llm_guard/input_scanners/util.py
 llm_guard/input_scanners/anonymize_helpers/__init__.py
 llm_guard/input_scanners/anonymize_helpers/analyzer.py
 llm_guard/input_scanners/anonymize_helpers/faker.py
 llm_guard/input_scanners/anonymize_helpers/ner_mapping.py
 llm_guard/input_scanners/anonymize_helpers/transformers_recognizer.py
+llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/__init__.py
+llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/phone_recognizer.py
+llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/zh/__init__.py
+llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/zh/crypto_recognizer.py
+llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/zh/custom_pattern_recognizer.py
+llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/zh/email_recognizer.py
+llm_guard/input_scanners/anonymize_helpers/predefined_recognizers/zh/ip_recognizer.py
 llm_guard/input_scanners/secrets_plugins/__init__.py
 llm_guard/input_scanners/secrets_plugins/adafruit.py
 llm_guard/input_scanners/secrets_plugins/adobe.py
 llm_guard/input_scanners/secrets_plugins/age_secret_key.py
 llm_guard/input_scanners/secrets_plugins/airtable_api_key.py
 llm_guard/input_scanners/secrets_plugins/algolia_api_key.py
 llm_guard/input_scanners/secrets_plugins/alibaba.py
```

### Comparing `llm-guard-0.3.7/llm_guard.egg-info/requires.txt` & `llm-guard-0.3.9/llm_guard.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 detect-secrets==1.4.0
 faker<23,>=22
 fuzzysearch==0.7.3
-json-repair==0.4.5
+json-repair==0.8.0
 nltk<4,>=3.8
 presidio-analyzer<3,>=2.2
 presidio-anonymizer<3,>=2.2
-protobuf<4,>=3.20
+protobuf>=4
 regex==2023.12.25
 sentencepiece==0.1.99
 tiktoken<0.6,>=0.5
 torch==2.0.1
 transformers==4.36.2
 xformers==0.0.22
 span-marker==1.5.0
+structlog>=24
 
 [dev]
 llm_guard[docs-dev]
 autoflake<3,>=2
 black<24,>=23
 isort<6,>5
-pytest<8,>=7.4
+pytest<9,>=7.4
 pytest-cov<5,>=4.1
 pre-commit<4,>=3.6
 
 [docs-dev]
 mkdocs<2,>=1.5
 mkdocs-autorefs==0.5.0
 mkdocs-git-revision-date-localized-plugin==1.2.2
 mkdocs-jupyter==0.24.6
-mkdocs-material==9.5.3
+mkdocs-material==9.5.6
 mkdocs-material-extensions==1.3.1
-mkdocs-swagger-ui-tag==0.6.7
+mkdocs-swagger-ui-tag==0.6.8
 mkdocstrings==0.24.0
 mkdocstrings-python==1.8.0
 
 [onnxruntime]
 optimum[onnxruntime]
 
 [onnxruntime-gpu]
```

### Comparing `llm-guard-0.3.7/pyproject.toml` & `llm-guard-0.3.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "llm-guard"
 description = "LLM-Guard is a comprehensive tool designed to fortify the security of Large Language Models (LLMs). By offering sanitization, detection of harmful language, prevention of data leakage, and resistance against prompt injection attacks, LLM-Guard ensures that your interactions with LLMs remain safe and secure."
 authors = [
-  { name = "Laiyer.ai", email = "hello@laiyer.ai"}
+  { name = "Protect AI", email = "community@protectai.com"}
 ]
 keywords = ["llm", "language model", "security", "adversarial attacks", "prompt injection", "prompt leakage", "PII detection", "self-hardening", "firewall"]
 license = { file = "LICENSE" }
 readme = "README.md"
 dynamic = ["version"]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -19,61 +19,62 @@
 ]
 requires-python = ">=3.9"
 
 dependencies = [
   "detect-secrets==1.4.0",
   "faker>=22,<23",
   "fuzzysearch==0.7.3",
-  "json-repair==0.4.5",
+  "json-repair==0.8.0",
   "nltk>=3.8,<4",
   "presidio-analyzer>=2.2,<3",
   "presidio-anonymizer>=2.2,<3",
-  "protobuf>=3.20,<4",
+  "protobuf>=4",
   "regex==2023.12.25",
   "sentencepiece==0.1.99",
   "tiktoken>=0.5,<0.6",
   "torch==2.0.1",
   "transformers==4.36.2",
   "xformers==0.0.22",
-  "span-marker==1.5.0"
+  "span-marker==1.5.0",
+  "structlog>=24"
 ]
 
 [project.optional-dependencies]
 onnxruntime = [
   "optimum[onnxruntime]",
 ]
 onnxruntime-gpu = [
   "optimum[onnxruntime-gpu]",
 ]
 docs-dev = [
   "mkdocs>=1.5,<2",
   "mkdocs-autorefs==0.5.0",
   "mkdocs-git-revision-date-localized-plugin==1.2.2",
   "mkdocs-jupyter==0.24.6",
-  "mkdocs-material==9.5.3",
+  "mkdocs-material==9.5.6",
   "mkdocs-material-extensions==1.3.1",
-  "mkdocs-swagger-ui-tag==0.6.7",
+  "mkdocs-swagger-ui-tag==0.6.8",
   "mkdocstrings==0.24.0",
   "mkdocstrings-python==1.8.0"
 ]
 dev = [
   "llm_guard[docs-dev]",
   "autoflake>=2,<3",
   "black>=23,<24",
   "isort>5,<6",
-  "pytest>=7.4,<8",
+  "pytest>=7.4,<9",
   "pytest-cov>=4.1,<5",
   "pre-commit>=3.6,<4",
 ]
 
 [project.urls]
-homepage = "https://github.com/laiyer-ai/llm-guard"
+homepage = "https://github.com/protectai/llm-guard"
 documentation = "https://llm-guard.com/"
-repository = "https://github.com/laiyer-ai/llm-guard"
-issues = "https://github.com/laiyer-ai/llm-guard/issues"
+repository = "https://github.com/protectai/llm-guard"
+issues = "https://github.com/protectai/llm-guard/issues"
 changelog = "https://llm-guard.com/changelog/"
 
 [tool.setuptools]
 packages = {find = {where=["."], include=["llm_guard", "llm_guard.*"]}}
 license-files = [
   "LICENSE"
 ]
```

### Comparing `llm-guard-0.3.7/tests/test_evaluate.py` & `llm-guard-0.3.9/tests/test_evaluate.py`

 * *Files identical despite different names*

