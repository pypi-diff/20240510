# Comparing `tmp/ofscraper-3.9.5.tar.gz` & `tmp/ofscraper-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.9.5.tar", max compression
+gzip compressed data, was "ofscraper-3.9.6.tar", max compression
```

## Comparing `ofscraper-3.9.5.tar` & `ofscraper-3.9.6.tar`

### file list

```diff
@@ -1,205 +1,230 @@
--rw-r--r--   0        0        0     1067 2024-05-07 17:03:44.537793 ofscraper-3.9.5/LICENSE
--rw-r--r--   0        0        0     4213 2024-05-07 17:03:44.537793 ofscraper-3.9.5/README.md
--rwxr-xr-x   0        0        0      283 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/__main__.py
--rw-r--r--   0        0        0     1690 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/__version__.py
--rw-r--r--   0        0        0     1625 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/actions/__init__.py
--rw-r--r--   0        0        0     8505 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/actions/like.py
--rw-r--r--   0        0        0    10057 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/actions/process.py
--rw-r--r--   0        0        0    21617 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/actions/scraper.py
--rw-r--r--   0        0        0    16237 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/archive.py
--rw-r--r--   0        0        0      274 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/common/logs.py
--rw-r--r--   0        0        0    14697 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1479 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/init.py
--rw-r--r--   0        0        0    14238 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/labels.py
--rw-r--r--   0        0        0     2912 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/me.py
--rw-r--r--   0        0        0    18538 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/messages.py
--rw-r--r--   0        0        0    13861 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/paid.py
--rw-r--r--   0        0        0     8717 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     6176 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1718 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/subscriptions/helpers.py
--rw-r--r--   0        0        0     3381 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/subscriptions/individual.py
--rw-r--r--   0        0        0    12660 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/subscriptions/lists.py
--rw-r--r--   0        0        0     8171 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/subscriptions/subscriptions.py
--rw-r--r--   0        0        0    17241 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     1460 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/base.py
--rw-r--r--   0        0        0      876 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/labels.py
--rw-r--r--   0        0        0    15560 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/media.py
--rw-r--r--   0        0        0     6005 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/models.py
--rw-r--r--   0        0        0     1771 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0    20499 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     5156 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/posts.py
--rw-r--r--   0        0        0    18427 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/sessionmanager.py
--rw-r--r--   0        0        0      156 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/button.py
--rw-r--r--   0        0        0     1689 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/boolfield.py
--rw-r--r--   0        0        0     1370 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/datefield.py
--rw-r--r--   0        0        0      629 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/mediafield.py
--rw-r--r--   0        0        0      694 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/numfield.py
--rw-r--r--   0        0        0     1302 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/pricefield.py
--rw-r--r--   0        0        0      678 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/responsefield.py
--rw-r--r--   0        0        0     1417 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/selectfield.py
--rw-r--r--   0        0        0     1487 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/fields/textsearch.py
--rw-r--r--   0        0        0     2460 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/fields/timefield.py
--rw-r--r--   0        0        0     1893 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/inputs/filterinput.py
--rw-r--r--   0        0        0      117 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/inputs/intergerinput.py
--rw-r--r--   0        0        0      113 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/inputs/strinput.py
--rw-r--r--   0        0        0      297 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/row_names.py
--rw-r--r--   0        0        0     4583 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/status.py
--rw-r--r--   0        0        0    21258 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/table.py
--rw-r--r--   0        0        0      156 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/table_console.py
--rw-r--r--   0        0        0    26132 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/commands/check.py
--rw-r--r--   0        0        0    11014 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/commands/manual.py
--rw-r--r--   0        0        0      430 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/commands/picker.py
--rwxr-xr-x   0        0        0     3810 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0       53 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/binary.py
--rw-r--r--   0        0        0     1655 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/config.py
--rw-r--r--   0        0        0     1628 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/constants.py
--rw-r--r--   0        0        0       74 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/date.py
--rw-r--r--   0        0        0      190 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/download.py
--rw-r--r--   0        0        0      204 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/files.py
--rw-r--r--   0        0        0     1375 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/general.py
--rw-r--r--   0        0        0       93 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/logger.py
--rw-r--r--   0        0        0       69 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/metadata.py
--rw-r--r--   0        0        0      862 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/other_url.py
--rw-r--r--   0        0        0     1908 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/prompts.py
--rw-r--r--   0        0        0     1808 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/req.py
--rw-r--r--   0        0        0      271 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/table.py
--rw-r--r--   0        0        0   265533 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/test_constants.py
--rw-r--r--   0        0        0      248 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/time.py
--rw-r--r--   0        0        0     3594 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/url.py
--rw-r--r--   0        0        0        1 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    15609 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations.py
--rw-r--r--   0        0        0      206 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/helpers.py
--rw-r--r--   0        0        0     8568 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/labels.py
--rw-r--r--   0        0        0    19443 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/media.py
--rw-r--r--   0        0        0    11553 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/merge.py
--rw-r--r--   0        0        0     8494 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/messages.py
--rw-r--r--   0        0        0     8928 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/others.py
--rw-r--r--   0        0        0    10366 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/posts.py
--rw-r--r--   0        0        0     6725 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/profile.py
--rw-r--r--   0        0        0     7485 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/stories.py
--rw-r--r--   0        0        0     4810 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/wrapper.py
--rw-r--r--   0        0        0    10881 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/alt_download.py
--rw-r--r--   0        0        0    10682 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/alt_downloadbatch.py
--rw-r--r--   0        0        0     4901 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/download.py
--rw-r--r--   0        0        0    17167 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/downloadbatch.py
--rw-r--r--   0        0        0     9077 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/downloadnormal.py
--rw-r--r--   0        0        0    10787 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/main_download.py
--rw-r--r--   0        0        0    11235 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/main_downloadbatch.py
--rw-r--r--   0        0        0     1414 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/shared/classes/retries.py
--rw-r--r--   0        0        0     1356 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/shared/classes/session.py
--rw-r--r--   0        0        0     3795 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/shared/common/alt_common.py
--rw-r--r--   0        0        0     6372 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/common/general.py
--rw-r--r--   0        0        0     2063 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/common/main_common.py
--rw-r--r--   0        0        0     2341 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/globals.py
--rw-r--r--   0        0        0     9440 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/keyhelpers.py
--rw-r--r--   0        0        0     3431 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/log.py
--rw-r--r--   0        0        0      317 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/media.py
--rw-r--r--   0        0        0      790 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/message.py
--rw-r--r--   0        0        0     3927 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/metadata.py
--rw-r--r--   0        0        0     2590 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/paths.py
--rw-r--r--   0        0        0      453 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/progress.py
--rw-r--r--   0        0        0     1155 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/text.py
--rw-r--r--   0        0        0     8075 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/media/helpers.py
--rw-r--r--   0        0        0     5019 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/media/main.py
--rw-r--r--   0        0        0     3136 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/date.py
--rw-r--r--   0        0        0     3143 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/flags.py
--rw-r--r--   0        0        0      957 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/helpers.py
--rw-r--r--   0        0        0      726 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/other.py
--rw-r--r--   0        0        0     7561 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/price.py
--rw-r--r--   0        0        0     1538 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/sort.py
--rw-r--r--   0        0        0     1454 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/subtype.py
--rw-r--r--   0        0        0     3414 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/models/retriver.py
--rw-r--r--   0        0        0     8105 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/models/selector.py
--rw-r--r--   0        0        0     2466 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/helpers/model_helpers.py
--rw-r--r--   0        0        0    15219 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/helpers/prompt_helpers.py
--rw-r--r--   0        0        0      846 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     7747 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0      917 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/actions.py
--rw-r--r--   0        0        0     6595 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/area.py
--rw-r--r--   0        0        0     8257 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/auth.py
--rw-r--r--   0        0        0     4438 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/binary.py
--rw-r--r--   0        0        0    27916 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/config.py
--rw-r--r--   0        0        0     1879 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/menu.py
--rw-r--r--   0        0        0     3112 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/merge.py
--rw-r--r--   0        0        0    16090 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/model.py
--rw-r--r--   0        0        0     4135 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/profile.py
--rw-r--r--   0        0        0     7609 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    10346 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0     1342 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      567 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/runner/exit.py
--rw-r--r--   0        0        0     1578 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/runner/load.py
--rw-r--r--   0        0        0     2743 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/runner/run.py
--rw-r--r--   0        0        0        1 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3803 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/actions.py
--rw-r--r--   0        0        0     1838 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/areas.py
--rw-r--r--   0        0        0       12 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/globals.py
--rw-r--r--   0        0        0     8419 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/common_args.py
--rw-r--r--   0        0        0    18709 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/main_args.py
--rw-r--r--   0        0        0     1349 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/manual_args.py
--rw-r--r--   0        0        0     1618 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/message_args.py
--rw-r--r--   0        0        0     1619 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/paid_args.py
--rw-r--r--   0        0        0     1986 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/post_args.py
--rw-r--r--   0        0        0     1672 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/story_args.py
--rw-r--r--   0        0        0     5571 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/helpers.py
--rw-r--r--   0        0        0     1928 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/parse.py
--rw-r--r--   0        0        0      395 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/quality.py
--rw-r--r--   0        0        0      960 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/read.py
--rw-r--r--   0        0        0      721 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/user.py
--rw-r--r--   0        0        0      403 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/write.py
--rw-r--r--   0        0        0     2148 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/context.py
--rw-r--r--   0        0        0     1680 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/data.py
--rw-r--r--   0        0        0     2034 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/file.py
--rw-r--r--   0        0        0     2844 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/helpers.py
--rw-r--r--   0        0        0     1669 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/make.py
--rw-r--r--   0        0        0     6902 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/request.py
--rw-r--r--   0        0        0      802 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/schema.py
--rw-r--r--   0        0        0     9824 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0     1780 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/cache.py
--rw-r--r--   0        0        0     1612 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/checkers.py
--rw-r--r--   0        0        0     2856 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/config.py
--rw-r--r--   0        0        0     1442 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/context.py
--rw-r--r--   0        0        0      522 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/custom.py
--rw-r--r--   0        0        0    24693 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/data.py
--rw-r--r--   0        0        0     2146 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/file.py
--rw-r--r--   0        0        0     2073 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/menu.py
--rw-r--r--   0        0        0     4797 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/schema.py
--rw-r--r--   0        0        0      409 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/wrapper.py
--rw-r--r--   0        0        0      499 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/console.py
--rw-r--r--   0        0        0      788 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/constants.py
--rw-r--r--   0        0        0     3401 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/context/exit.py
--rw-r--r--   0        0        0     1135 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/context/run_async.py
--rw-r--r--   0        0        0     1004 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/context/stdout.py
--rw-r--r--   0        0        0     3460 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/dates.py
--rw-r--r--   0        0        0     1040 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     1745 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/hash.py
--rw-r--r--   0        0        0     7226 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/classes.py
--rw-r--r--   0        0        0     2588 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/close.py
--rw-r--r--   0        0        0      477 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/globals.py
--rw-r--r--   0        0        0     1670 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/helpers.py
--rw-r--r--   0        0        0     2098 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/logger.py
--rw-r--r--   0        0        0     1672 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/logs.py
--rw-r--r--   0        0        0     5955 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/other.py
--rw-r--r--   0        0        0     3652 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/stdout.py
--rw-r--r--   0        0        0      601 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/manager.py
--rw-r--r--   0        0        0      576 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/me.py
--rw-r--r--   0        0        0     4161 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/menu.py
--rw-r--r--   0        0        0     1022 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/merge.py
--rw-r--r--   0        0        0     1710 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/paths/check.py
--rw-r--r--   0        0        0     3091 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/paths/common.py
--rw-r--r--   0        0        0      703 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/paths/manage.py
--rw-r--r--   0        0        0     4912 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/paths/paths.py
--rw-r--r--   0        0        0     1034 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/profiles/data.py
--rw-r--r--   0        0        0     2785 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/profiles/manage.py
--rw-r--r--   0        0        0     1583 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/profiles/tools.py
--rw-r--r--   0        0        0    10893 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/progress.py
--rw-r--r--   0        0        0     4406 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/run.py
--rw-r--r--   0        0        0        1 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/sems.py
--rw-r--r--   0        0        0     1672 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     4691 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/settings.py
--rw-r--r--   0        0        0      417 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/system/free.py
--rw-r--r--   0        0        0     3279 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/system/network.py
--rw-r--r--   0        0        0     2472 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/system/system.py
--rw-r--r--   0        0        0     2002 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/text.py
--rw-r--r--   0        0        0     2117 2024-05-07 17:04:09.753831 ofscraper-3.9.5/pyproject.toml
--rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 ofscraper-3.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-10 19:08:59.308061 ofscraper-3.9.6/LICENSE
+-rw-r--r--   0        0        0     4213 2024-05-10 19:08:59.308061 ofscraper-3.9.6/README.md
+-rwxr-xr-x   0        0        0      283 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1064 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/__version__.pye
+-rw-r--r--   0        0        0    15951 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/api/archive.py
+-rw-r--r--   0        0        0      274 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/api/common/logs.py
+-rw-r--r--   0        0        0    14697 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1479 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/api/init.py
+-rw-r--r--   0        0        0    14238 2024-05-10 19:08:59.312061 ofscraper-3.9.6/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2912 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/me.py
+-rw-r--r--   0        0        0    18146 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    13861 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     8581 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     6176 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1718 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/subscriptions/helpers.py
+-rw-r--r--   0        0        0     3381 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/subscriptions/individual.py
+-rw-r--r--   0        0        0    12660 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/subscriptions/lists.py
+-rw-r--r--   0        0        0     8171 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/subscriptions/subscriptions.py
+-rw-r--r--   0        0        0    17037 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     1460 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/base.py
+-rw-r--r--   0        0        0      876 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0    15560 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     6005 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/models.py
+-rw-r--r--   0        0        0     1771 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0    20597 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     5156 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0    18427 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/sessionmanager.py
+-rw-r--r--   0        0        0      156 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/button.py
+-rw-r--r--   0        0        0     1689 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/boolfield.py
+-rw-r--r--   0        0        0     1370 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/datefield.py
+-rw-r--r--   0        0        0      629 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/mediafield.py
+-rw-r--r--   0        0        0      694 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/numfield.py
+-rw-r--r--   0        0        0     1302 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/pricefield.py
+-rw-r--r--   0        0        0      678 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/responsefield.py
+-rw-r--r--   0        0        0     1417 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/selectfield.py
+-rw-r--r--   0        0        0     1487 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/textsearch.py
+-rw-r--r--   0        0        0     2460 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/fields/timefield.py
+-rw-r--r--   0        0        0     1893 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/inputs/filterinput.py
+-rw-r--r--   0        0        0      117 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/inputs/intergerinput.py
+-rw-r--r--   0        0        0      113 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/inputs/strinput.py
+-rw-r--r--   0        0        0      297 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/row_names.py
+-rw-r--r--   0        0        0     4583 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/status.py
+-rw-r--r--   0        0        0    21258 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/table.py
+-rw-r--r--   0        0        0      156 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/classes/table/table_console.py
+-rw-r--r--   0        0        0        1 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/actions/__init__.py
+-rw-r--r--   0        0        0     6447 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/actions/download/download.py
+-rw-r--r--   0        0        0    21813 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/actions/download/post.py
+-rw-r--r--   0        0        0    11597 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/actions/like.py
+-rw-r--r--   0        0        0     1545 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/actions/scrape_context.py
+-rw-r--r--   0        0        0     1039 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/add_select/add_selected.py
+-rw-r--r--   0        0        0    26132 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/check.py
+-rw-r--r--   0        0        0    11014 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/manual.py
+-rw-r--r--   0        0        0     8188 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/metadata.py
+-rw-r--r--   0        0        0      556 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/picker.py
+-rwxr-xr-x   0        0        0     3785 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0       53 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/binary.py
+-rw-r--r--   0        0        0     1655 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/config.py
+-rw-r--r--   0        0        0     1002 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/constants.py
+-rw-r--r--   0        0        0       74 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/date.py
+-rw-r--r--   0        0        0      190 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/download.py
+-rw-r--r--   0        0        0      204 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/files.py
+-rw-r--r--   0        0        0     1375 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/general.py
+-rw-r--r--   0        0        0       93 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/logger.py
+-rw-r--r--   0        0        0      120 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/metadata.py
+-rw-r--r--   0        0        0      862 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/other_url.py
+-rw-r--r--   0        0        0     1908 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/prompts.py
+-rw-r--r--   0        0        0     1807 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/req.py
+-rw-r--r--   0        0        0      271 2024-05-10 19:08:59.316061 ofscraper-3.9.6/ofscraper/const/table.py
+-rw-r--r--   0        0        0   265533 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/const/test_constants.py
+-rw-r--r--   0        0        0      248 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/const/time.py
+-rw-r--r--   0        0        0     3594 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/const/url.py
+-rw-r--r--   0        0        0        1 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    15609 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations.py
+-rw-r--r--   0        0        0      206 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/helpers.py
+-rw-r--r--   0        0        0     8568 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/labels.py
+-rw-r--r--   0        0        0    19876 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/media.py
+-rw-r--r--   0        0        0    11553 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/merge.py
+-rw-r--r--   0        0        0     8494 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/messages.py
+-rw-r--r--   0        0        0     8928 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/others.py
+-rw-r--r--   0        0        0    10366 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/posts.py
+-rw-r--r--   0        0        0     6725 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/profile.py
+-rw-r--r--   0        0        0     7485 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/stories.py
+-rw-r--r--   0        0        0     4810 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/db/operations_/wrapper.py
+-rw-r--r--   0        0        0    10881 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/alt_download.py
+-rw-r--r--   0        0        0    10682 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/alt_downloadbatch.py
+-rw-r--r--   0        0        0     4914 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/download.py
+-rw-r--r--   0        0        0    17191 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/downloadbatch.py
+-rw-r--r--   0        0        0     9077 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/downloadnormal.py
+-rw-r--r--   0        0        0    10787 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/main_download.py
+-rw-r--r--   0        0        0    11235 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/main_downloadbatch.py
+-rw-r--r--   0        0        0     1414 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/classes/retries.py
+-rw-r--r--   0        0        0     1356 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/classes/session.py
+-rw-r--r--   0        0        0     3795 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/common/alt_common.py
+-rw-r--r--   0        0        0     6372 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/common/general.py
+-rw-r--r--   0        0        0     2063 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/common/main_common.py
+-rw-r--r--   0        0        0     2341 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/globals.py
+-rw-r--r--   0        0        0     9440 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/keyhelpers.py
+-rw-r--r--   0        0        0     3431 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/log.py
+-rw-r--r--   0        0        0      317 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/media.py
+-rw-r--r--   0        0        0      790 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/message.py
+-rw-r--r--   0        0        0     5698 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/metadata.py
+-rw-r--r--   0        0        0     2590 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/paths.py
+-rw-r--r--   0        0        0      453 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/progress.py
+-rw-r--r--   0        0        0     1155 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/download/shared/utils/text.py
+-rw-r--r--   0        0        0     8075 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/media/helpers.py
+-rw-r--r--   0        0        0     5019 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/media/main.py
+-rw-r--r--   0        0        0     3136 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/date.py
+-rw-r--r--   0        0        0     3143 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/flags.py
+-rw-r--r--   0        0        0      957 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/helpers.py
+-rw-r--r--   0        0        0      726 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/other.py
+-rw-r--r--   0        0        0     7561 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/price.py
+-rw-r--r--   0        0        0     1538 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/sort.py
+-rw-r--r--   0        0        0     1454 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/filters/models/subtype.py
+-rw-r--r--   0        0        0     3414 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/models/retriver.py
+-rw-r--r--   0        0        0     8105 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/models/selector.py
+-rw-r--r--   0        0        0     2466 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/helpers/model_helpers.py
+-rw-r--r--   0        0        0    15219 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/helpers/prompt_helpers.py
+-rw-r--r--   0        0        0      846 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     7747 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0      917 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/actions.py
+-rw-r--r--   0        0        0     6834 2024-05-10 19:08:59.320061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/area.py
+-rw-r--r--   0        0        0     8257 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/auth.py
+-rw-r--r--   0        0        0     4438 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/binary.py
+-rw-r--r--   0        0        0    27916 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/config.py
+-rw-r--r--   0        0        0     1879 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/menu.py
+-rw-r--r--   0        0        0     3112 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/merge.py
+-rw-r--r--   0        0        0    16090 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/model.py
+-rw-r--r--   0        0        0     4135 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_groups/profile.py
+-rw-r--r--   0        0        0     7609 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    10346 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0     1342 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      567 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/runner/exit.py
+-rw-r--r--   0        0        0     1578 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/runner/load.py
+-rw-r--r--   0        0        0     2743 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/runner/run.py
+-rw-r--r--   0        0        0        1 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3803 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/actions.py
+-rw-r--r--   0        0        0     1838 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/areas.py
+-rw-r--r--   0        0        0     1089 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/advanced_processing.py
+-rw-r--r--   0        0        0     1546 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/advanced_program.py
+-rw-r--r--   0        0        0     4411 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/advanced_user_filter.py
+-rw-r--r--   0        0        0      997 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/automatic.py
+-rw-r--r--   0        0        0     5183 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/content.py
+-rw-r--r--   0        0        0      944 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/download.py
+-rw-r--r--   0        0        0      905 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/file.py
+-rw-r--r--   0        0        0     1185 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/logging.py
+-rw-r--r--   0        0        0     1282 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/media_type.py
+-rw-r--r--   0        0        0      935 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/program.py
+-rw-r--r--   0        0        0     3825 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/user_list.py
+-rw-r--r--   0        0        0     2683 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/user_select.py
+-rw-r--r--   0        0        0      971 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/arguments/user_sort.py
+-rw-r--r--   0        0        0      319 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/advanced_common.py
+-rw-r--r--   0        0        0      661 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/common.py
+-rw-r--r--   0        0        0     1020 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/main.py
+-rw-r--r--   0        0        0     1579 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/manual.py
+-rw-r--r--   0        0        0     2281 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/message_check.py
+-rw-r--r--   0        0        0     4145 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/metadata.py
+-rw-r--r--   0        0        0     1862 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/paid_check.py
+-rw-r--r--   0        0        0     2277 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/post_check.py
+-rw-r--r--   0        0        0     1928 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/bundles/story_check.py
+-rw-r--r--   0        0        0      502 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/main.py
+-rw-r--r--   0        0        0      189 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/manual.py
+-rw-r--r--   0        0        0      217 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/message.py
+-rw-r--r--   0        0        0      197 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/metadata.py
+-rw-r--r--   0        0        0      205 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/paid.py
+-rw-r--r--   0        0        0      205 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/post.py
+-rw-r--r--   0        0        0      209 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/commands/story.py
+-rw-r--r--   0        0        0       12 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/globals.py
+-rw-r--r--   0        0        0     5616 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/helpers.py
+-rw-r--r--   0        0        0     2031 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/parse.py
+-rw-r--r--   0        0        0      395 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/quality.py
+-rw-r--r--   0        0        0      960 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/read.py
+-rw-r--r--   0        0        0      721 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/user.py
+-rw-r--r--   0        0        0      403 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/args/write.py
+-rw-r--r--   0        0        0     2148 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/context.py
+-rw-r--r--   0        0        0     1680 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/data.py
+-rw-r--r--   0        0        0     2034 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/file.py
+-rw-r--r--   0        0        0     2844 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/helpers.py
+-rw-r--r--   0        0        0     1669 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/make.py
+-rw-r--r--   0        0        0     6902 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/request.py
+-rw-r--r--   0        0        0      802 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/auth/schema.py
+-rw-r--r--   0        0        0     9824 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0     1780 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/cache.py
+-rw-r--r--   0        0        0     1612 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/checkers.py
+-rw-r--r--   0        0        0     2952 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/config.py
+-rw-r--r--   0        0        0     1442 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/context.py
+-rw-r--r--   0        0        0      522 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/custom.py
+-rw-r--r--   0        0        0    24693 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/data.py
+-rw-r--r--   0        0        0     2146 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/file.py
+-rw-r--r--   0        0        0     2073 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/menu.py
+-rw-r--r--   0        0        0     4797 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/schema.py
+-rw-r--r--   0        0        0      409 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/config/wrapper.py
+-rw-r--r--   0        0        0      499 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      788 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/constants.py
+-rw-r--r--   0        0        0     3401 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/context/exit.py
+-rw-r--r--   0        0        0     1135 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/context/run_async.py
+-rw-r--r--   0        0        0     1004 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/context/stdout.py
+-rw-r--r--   0        0        0     3460 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0     1040 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     1745 2024-05-10 19:08:59.324061 ofscraper-3.9.6/ofscraper/utils/hash.py
+-rw-r--r--   0        0        0     7226 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/classes.py
+-rw-r--r--   0        0        0     2588 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/close.py
+-rw-r--r--   0        0        0      477 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/globals.py
+-rw-r--r--   0        0        0     1670 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/helpers.py
+-rw-r--r--   0        0        0     2098 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/logger.py
+-rw-r--r--   0        0        0     1672 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/logs.py
+-rw-r--r--   0        0        0     5955 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/other.py
+-rw-r--r--   0        0        0     3652 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/logs/stdout.py
+-rw-r--r--   0        0        0      601 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/manager.py
+-rw-r--r--   0        0        0      576 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/me.py
+-rw-r--r--   0        0        0     4167 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/menu.py
+-rw-r--r--   0        0        0     1022 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/merge.py
+-rw-r--r--   0        0        0     1710 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/paths/check.py
+-rw-r--r--   0        0        0     3091 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/paths/common.py
+-rw-r--r--   0        0        0      703 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/paths/manage.py
+-rw-r--r--   0        0        0     4912 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/paths/paths.py
+-rw-r--r--   0        0        0     1034 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/profiles/data.py
+-rw-r--r--   0        0        0     2785 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/profiles/manage.py
+-rw-r--r--   0        0        0     1583 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/profiles/tools.py
+-rw-r--r--   0        0        0    10893 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/progress.py
+-rw-r--r--   0        0        0     4406 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/run.py
+-rw-r--r--   0        0        0        1 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/sems.py
+-rw-r--r--   0        0        0     1672 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     4691 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/settings.py
+-rw-r--r--   0        0        0      417 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/system/free.py
+-rw-r--r--   0        0        0     3279 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/system/network.py
+-rw-r--r--   0        0        0     2472 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/system/system.py
+-rw-r--r--   0        0        0     2055 2024-05-10 19:08:59.328061 ofscraper-3.9.6/ofscraper/utils/text.py
+-rw-r--r--   0        0        0     2117 2024-05-10 19:09:27.052271 ofscraper-3.9.6/pyproject.toml
+-rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 ofscraper-3.9.6/PKG-INFO
```

### Comparing `ofscraper-3.9.5/LICENSE` & `ofscraper-3.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/README.md` & `ofscraper-3.9.6/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/__version__.py` & `ofscraper-3.9.6/ofscraper/prompts/prompts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,22 @@
 r"""
-        _____                                               
-r"""
                                                              
  _______  _______         _______  _______  _______  _______  _______  _______  _______ 
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
-                 \/     \/           \/            \/       
-"""
-
-__title__ = "ofscraper"
-__author__ = "datawhores"
-__author_email__ = "datawhores@riseup.net"
-__description__ = (
-    "A command-line program to quickly download,like or unlike posts, and more"
-)
-__url__ = "https://github.com/datawhores/OF-Scraper"
-__license__ = "GNU General Public License v3 or later (GPLv3+)"
-__copyright__ = "Copyright 2023"
-
-try:
-    from dunamai import Version
-
-    __hardcoded__ = None
-    __version__ = __hardcoded__ or Version.from_git(
-        pattern="(?P<base>\d+\.\d+\.((\d+\.\w+)|\w+))"
-    ).serialize(format="{base}+{branch}.{commit}", metadata=False)
-except:
-    import pkg_resources
 
-    __version__ = pkg_resources.get_distribution("ofscraper").version
+from ofscraper.prompts.prompt_groups.actions import *
+from ofscraper.prompts.prompt_groups.area import *
+from ofscraper.prompts.prompt_groups.auth import *
+from ofscraper.prompts.prompt_groups.binary import *
+from ofscraper.prompts.prompt_groups.config import *
+from ofscraper.prompts.prompt_groups.menu import *
+from ofscraper.prompts.prompt_groups.merge import *
+from ofscraper.prompts.prompt_groups.model import *
+from ofscraper.prompts.prompt_groups.profile import *
```

### Comparing `ofscraper-3.9.5/ofscraper/__version__.pye` & `ofscraper-3.9.6/ofscraper/utils/separate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 r"""
-        _____                                               
-r"""
                                                              
  _______  _______         _______  _______  _______  _______  _______  _______  _______ 
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
-                 \/     \/           \/            \/       
-"""
 
-__title__ = 'ofscraper'
-__author__ = 'datawhores'
-__author_email__ = 'datawhores@riseup.net'
-__description__ = 'A command-line program to quickly download,like or unlike posts, and more'
-__url__ = 'https://github.com/datawhores/OF-Scraper'
-__license__ = 'GNU General Public License v3 or later (GPLv3+)'
-__copyright__ = 'Copyright 2023'
-
-try:
-      from dunamai import Version,Pattern
-      __version__ = Version.from_git(pattern=Pattern.DefaultUnprefixed).serialize(format="{base}+{branch}.{commit}",metadata=False)
-except:
-      import pkg_resources
-      __version__= pkg_resources.get_distribution('ofscraper').version
+import ofscraper.utils.cache as cache
+import ofscraper.utils.constants as constants
+import ofscraper.utils.me as me_util
+
+
+def separate_by_id(data: list, media_ids: list) -> list:
+    media_ids = set(media_ids)
+    return list(filter(lambda x: x.id not in media_ids, data))
+
+
+def seperate_avatars(data):
+    return list(filter(lambda x: seperate_avatar_helper(x) is False, data))
+
+
+def seperate_avatar_helper(ele):
+    # id for avatar comes from xxh32 of url
+    if ele.postid and ele.responsetype == "profile":
+        value = cache.get(ele.postid, default=False)
+        cache.close()
+        return value
+    return False
+
+
+def seperate_by_self(data):
+    my_id = me_util.get_id()
+    if constants.getattr("FILTER_SELF_MEDIA"):
+        return list(filter(lambda x: x.post.fromuser != my_id, data))
```

### Comparing `ofscraper-3.9.5/ofscraper/actions/like.py` & `ofscraper-3.9.6/ofscraper/commands/actions/like.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,30 +22,95 @@
     Progress,
     SpinnerColumn,
     TextColumn,
 )
 from rich.style import Style
 
 import ofscraper.api.archive as archive
+import ofscraper.api.init as init
 import ofscraper.api.labels as labels_api
 import ofscraper.api.pinned as pinned
+import ofscraper.api.profile as profile
 import ofscraper.api.timeline as timeline
 import ofscraper.classes.posts as posts_
 import ofscraper.classes.sessionmanager as sessionManager
+import ofscraper.db.operations as operations
+import ofscraper.filters.media.main as filters
+import ofscraper.models.selector as userselector
 import ofscraper.utils.args.areas as areas
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.console as console
 import ofscraper.utils.constants as constants
+import ofscraper.utils.context.exit as exit
+import ofscraper.utils.context.stdout as stdout
+import ofscraper.utils.profiles.tools as profile_tools
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.system.system as system
+from ofscraper.commands.actions.scrape_context import scrape_context_manager
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 
 
+@exit.exit_wrapper
+def process_like():
+    with scrape_context_manager():
+        profile_tools.print_current_profile()
+        init.print_sign_status()
+        userdata = userselector.getselected_usernames(rescan=False)
+        active = list(filter(lambda x: x.active, userdata))
+        length = len(active)
+        log.debug(f"Number of Active Accounts selected {length}")
+        with stdout.lowstdout():
+            for count, ele in enumerate(active):
+                log.info(f"Like action progressing on model {count+1}/{length}")
+                if constants.getattr("SHOW_AVATAR") and ele.avatar:
+                    log.warning(f"Avatar : {ele.avatar}")
+                log.warning(
+                    f"Getting {','.join(areas.get_like_area())} for [bold]{ele.name}[/bold]\n[bold]Subscription Active:[/bold] {ele.active}"
+                )
+                model_id = ele.id
+                operations.table_init_create(model_id=model_id, username=ele.name)
+                unfavorited_posts = get_post_for_like(
+                    model_id=model_id, username=ele.name
+                )
+                unfavorited_posts = filters.post_filter_for_like(
+                    unfavorited_posts, like=True
+                )
+                post_ids = get_post_ids(unfavorited_posts)
+                like(model_id, post_ids)
+
+
+@exit.exit_wrapper
+def process_unlike():
+    with scrape_context_manager():
+        profile_tools.print_current_profile()
+        init.print_sign_status()
+        userdata = userselector.getselected_usernames(rescan=False)
+        active = list(filter(lambda x: x.active, userdata))
+        length = len(active)
+        log.debug(f"Number of Active Accounts selected {length}")
+        with stdout.lowstdout():
+            for count, ele in enumerate(active):
+                log.info(f"Unlike action progressing on model {count+1}/{length}")
+                if constants.getattr("SHOW_AVATAR") and ele.avatar:
+                    log.warning(f"Avatar : {ele.avatar}")
+                log.warning(
+                    f"Getting {','.join(areas.get_like_area())} for [bold]{ele.name}[/bold]\n[bold]Subscription Active:[/bold] {ele.active}"
+                )
+                model_id = profile.get_id(ele.name)
+                operations.table_init_create(model_id=model_id, username=ele.name)
+                favorited_posts = get_posts_for_unlike(model_id, ele.name)
+                favorited_posts = filters.post_filter_for_like(
+                    favorited_posts, like=False
+                )
+                post_ids = get_post_ids(favorited_posts)
+                unlike(model_id, post_ids)
+
+
 @run
 async def get_posts(model_id, username):
     responses = []
     final_post_areas = set(areas.get_like_area())
     tasks = []
     with progress_utils.setup_api_split_progress_live():
         async with sessionManager.sessionManager(
@@ -57,14 +122,15 @@
         ) as c:
             while True:
                 max_count = min(
                     constants.getattr("API_MAX_AREAS"),
                     system.getcpu_count(),
                     len(final_post_areas),
                 )
+                forced_after=read_args.retriveArgs().after or 0
                 if not bool(tasks) and not bool(final_post_areas):
                     break
                 for _ in range(max_count - len(tasks)):
                     if "Pinned" in final_post_areas:
                         tasks.append(
                             asyncio.create_task(
                                 pinned.get_pinned_posts_progress(model_id, c)
@@ -75,39 +141,39 @@
                     elif "Timeline" in final_post_areas:
                         tasks.append(
                             asyncio.create_task(
                                 timeline.get_timeline_posts_progress(
                                     model_id=model_id,
                                     username=username,
                                     c=c,
-                                    forced_after=read_args.retriveArgs().after or 0,
+                                    forced_after=forced_after
                                 )
                             )
                         )
                         progress_utils.timeline_layout.visible = True
                         final_post_areas.remove("Timeline")
                     if "Archived" in final_post_areas:
                         tasks.append(
                             asyncio.create_task(
                                 archive.get_archived_posts_progress(
                                     model_id=model_id,
                                     username=username,
                                     c=c,
-                                    forced_after=read_args.retriveArgs().after or 0,
+                                    forced_after=forced_after
                                 )
                             )
                         )
                         progress_utils.archived_layout.visible = True
                         final_post_areas.remove("Archived")
 
                     elif "Labels" in final_post_areas:
                         tasks.append(
                             asyncio.create_task(
                                 labels_api.get_labels_posts_progress(
-                                    model_id=model_id, c=c
+                                    model_id=model_id, c=c,
                                 )
                             )
                         )
                         progress_utils.labelled_layout.visible = True
                         final_post_areas.remove("Labels")
                 if not bool(tasks):
                     break
```

### Comparing `ofscraper-3.9.5/ofscraper/actions/scraper.py` & `ofscraper-3.9.6/ofscraper/commands/actions/download/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,36 +452,43 @@
             return [item for sublist in output for item in sublist], [
                 post for ele in labelled_posts_labels for post in ele.posts
             ]
     except Exception as E:
         log.traceback_(E)
         log.traceback_(traceback.format_exc())
 
-
 @run
-async def process_areas(ele, model_id) -> list:
+async def process_areas_helper(ele, model_id) -> list:
     with stdout.lowstdout():
         executor = (
             ProcessPoolExecutor()
             if platform.system() not in constants.getattr("API_REQUEST_THREADONLY")
             else ThreadPoolExecutor()
         )
         try:
             with executor:
                 asyncio.get_event_loop().set_default_executor(executor)
                 username = ele.name
                 output = []
                 with progress_utils.setup_api_split_progress_live():
                     medias, posts = await process_task(model_id, username, ele)
                     output.extend(medias)
-            return filters.filterMedia(output), filters.filterPost(posts)
+            return (
+                medias,
+                posts,
+            )
         except Exception as E:
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
 
+@run
+async def process_areas(model_id, username):
+    media, posts = await process_areas_helper(model_id, username)
+    return filters.filterMedia(media), filters.filterPost(posts)
+
 
 async def process_task(model_id, username, ele):
     mediaObjs = []
     postObjs = []
     final_post_areas = set(areas.get_download_area())
     tasks = []
     async with sessionManager.sessionManager(
```

### Comparing `ofscraper-3.9.5/ofscraper/api/archive.py` & `ofscraper-3.9.6/ofscraper/api/archive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 r"""
                                                              
-r"""
-                                                             
  _______  _______         _______  _______  _______  _______  _______  _______  _______ 
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
-                 \/     \/           \/            \/         
-"""
 
 import asyncio
 import logging
 import math
 import traceback
 
 import arrow
@@ -51,15 +47,15 @@
     else:
         oldarchived = []
     trace_log_old(oldarchived)
 
     log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
     oldarchived = list(filter(lambda x: x is not None, oldarchived))
     after = await get_after(model_id, username, forced_after)
-    after_log(username, after)
+    time_log(username, after)
     splitArrays = get_split_array(oldarchived, after)
     tasks = get_tasks(splitArrays, c, model_id, after)
     data = await process_tasks(tasks, model_id, after)
     progress_utils.archived_layout.visible = False
     return data
 
 
@@ -70,15 +66,15 @@
     else:
         oldarchived = []
     trace_log_old(oldarchived)
 
     log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
     oldarchived = list(filter(lambda x: x is not None, oldarchived))
     after = await get_after(model_id, username, forced_after)
-    after_log(username, after)
+    time_log(username, after)
     with progress_utils.set_up_api_archived():
         splitArrays = get_split_array(oldarchived, after)
         tasks = get_tasks(splitArrays, c, model_id, after)
         return await process_tasks(tasks, model_id, after)
 
 
 async def process_tasks(tasks, model_id, after):
@@ -159,14 +155,15 @@
     ]
     return splitArrays
 
 
 def get_tasks(splitArrays, c, model_id, after):
     tasks = []
     job_progress = progress_utils.archived_progress
+    before=arrow.get(read_args.retriveArgs().before or arrow.now()).float_timestamp
     if len(splitArrays) > 2:
         tasks.append(
             asyncio.create_task(
                 scrape_archived_posts(
                     c,
                     model_id,
                     job_progress=job_progress,
@@ -198,36 +195,41 @@
             asyncio.create_task(
                 scrape_archived_posts(
                     c,
                     model_id,
                     job_progress=job_progress,
                     timestamp=splitArrays[-1][0].get("created_at"),
                     offset=True,
+                    required_ids=set([before])
+
                 )
             )
         )
     # use the first split if less then 3
     elif len(splitArrays) > 0:
         tasks.append(
             asyncio.create_task(
                 scrape_archived_posts(
                     c,
                     model_id,
                     job_progress=job_progress,
                     timestamp=splitArrays[0][0].get("created_at"),
                     offset=True,
+                    required_ids=set([before])
+
                 )
             )
         )
     # use after if split is empty i.e no db data
     else:
         tasks.append(
             asyncio.create_task(
                 scrape_archived_posts(
-                    c, model_id, job_progress=job_progress, timestamp=after, offset=True
+                    c, model_id, job_progress=job_progress, timestamp=after, offset=True,
+                    required_ids=set([before])
                 )
             )
         )
     return tasks
 
 
 def set_check(unduped, model_id, after):
@@ -284,26 +286,27 @@
 
 async def scrape_archived_posts(
     c, model_id, job_progress=None, timestamp=None, required_ids=None, offset=False
 ) -> list:
     global sem
     posts = None
     if timestamp and (
-        float(timestamp)
-        > (read_args.retriveArgs().before or arrow.now()).float_timestamp
+        float(timestamp) > (read_args.retriveArgs().before).float_timestamp
     ):
-        return []
+        return [],[]
     timestamp = float(timestamp) - 1000 if timestamp and offset else timestamp
     url = (
         constants.getattr("archivedNextEP").format(model_id, str(timestamp))
         if timestamp
         else constants.getattr("archivedEP").format(model_id)
     )
     log.debug(url)
+    
     new_tasks = []
+    posts=[]
     try:
         task = (
             job_progress.add_task(
                 f"Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp is not None  else 'initial'}",
                 visible=True,
             )
             if job_progress
@@ -311,14 +314,15 @@
         )
         async with c.requests_async(url) as r:
             posts = (await r.json_())["list"]
             log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp is not None  else 'initial'}"
             if not bool(posts):
                 log.debug(f"{log_id} -> no posts found")
                 return [], []
+            
             log.debug(f"{log_id} -> number of archived post found {len(posts)}")
             log.debug(
                 f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}"
             )
             log.debug(
                 f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}"
             )
@@ -333,27 +337,15 @@
                             lambda x: f"scrapeinfo archive: {str(x)}",
                             posts,
                         )
                     ),
                 )
             )
 
-            if not required_ids:
-                new_tasks.append(
-                    asyncio.create_task(
-                        scrape_archived_posts(
-                            c,
-                            model_id,
-                            job_progress=job_progress,
-                            timestamp=posts[-1]["postedAtPrecise"],
-                            offset=False,
-                        )
-                    )
-                )
-            elif max(map(lambda x: float(x["postedAtPrecise"]), posts)) >= max(
+            if max(map(lambda x: float(x["postedAtPrecise"]), posts)) >= max(
                 required_ids
             ):
                 pass
             elif float(timestamp or 0) >= max(required_ids):
                 pass
             else:
                 log.debug(f"{log_id} Required before {required_ids}")
@@ -369,27 +361,26 @@
                                 job_progress=job_progress,
                                 timestamp=posts[-1]["postedAtPrecise"],
                                 required_ids=required_ids,
                                 offset=False,
                             )
                         )
                     )
-            return posts, new_tasks
     except asyncio.TimeoutError as _:
         raise Exception(f"Task timed out {url}")
     except Exception as E:
         log.traceback_(E)
         log.traceback_(traceback.format_exc())
         raise E
-
     finally:
         job_progress.remove_task(task) if job_progress and task else None
     return posts, new_tasks
 
 
+
 def trace_log_task(responseArray):
     if not is_trace():
         return
     chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
     for i in range(1, len(responseArray) + 1, chunk_size):
         # Calculate end index considering potential last chunk being smaller
         end_index = min(
@@ -421,16 +412,16 @@
             )
         )
         # Check if there are more elements remaining after this chunk
         if i + chunk_size > len(responseArray):
             break  # Exit the loop if we've processed all elements
 
 
-def after_log(username, after):
+def time_log(username, after):
     log.info(
         f"""
-Setting initial archived scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
+Setting archived scan range for {username} from {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}  to {arrow.get(read_args.retriveArgs().before or arrow.now()).format((constants.getattr('API_DATE_FORMAT')))}
 [yellow]Hint: append ' --after 2000' to command to force scan of all archived posts + download of new files only[/yellow]
 [yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all archived posts + download/re-download of all files[/yellow]
 
             """
     )
```

### Comparing `ofscraper-3.9.5/ofscraper/api/highlights.py` & `ofscraper-3.9.6/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/api/init.py` & `ofscraper-3.9.6/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/api/labels.py` & `ofscraper-3.9.6/ofscraper/api/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/api/me.py` & `ofscraper-3.9.6/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/api/messages.py` & `ofscraper-3.9.6/ofscraper/api/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     oldmessages = None
     if not settings.get_api_cache_disabled():
         oldmessages = await get_messages_post_info(model_id=model_id, username=username)
     else:
         oldmessages = []
     trace_log_old(oldmessages)
 
-    before = (read_args.retriveArgs().before or arrow.now()).float_timestamp
+    before = (read_args.retriveArgs().before).float_timestamp
     after = await get_after(model_id, username, forced_after)
     log_after_before(after, before, username)
 
     filteredArray = get_filterArray(after, before, oldmessages)
     splitArrays = get_split_array(filteredArray)
     # Set charged sleeper
     get_sleeper()
@@ -65,15 +65,15 @@
     oldmessages = None
     if not settings.get_api_cache_disabled():
         oldmessages = await get_messages_post_info(model_id=model_id, username=username)
     else:
         oldmessages = []
     trace_log_old(oldmessages)
 
-    before = (read_args.retriveArgs().before or arrow.now()).float_timestamp
+    before = (read_args.retriveArgs().before).float_timestamp
     after = await get_after(model_id, username, forced_after)
     log_after_before(after, before, username)
 
     filteredArray = get_filterArray(after, before, oldmessages)
     splitArrays = get_split_array(filteredArray)
     with progress_utils.set_up_api_messages():
         tasks = get_tasks(splitArrays, filteredArray, oldmessages, model_id, c)
@@ -151,15 +151,15 @@
     else:
         return oldmessages[get_i(oldmessages, before) : get_j(oldmessages, after)]
 
 
 def get_i(oldmessages, before):
     """
     iterate through posts until a date less then or equal
-    to before , set index to -1 this point
+    to before , set index to -1 thtemp))nt
     """
     if before >= oldmessages[1].get("created_at"):
         return 0
     if before <= oldmessages[-1].get("created_at"):
         return len(oldmessages) - 2
     # Use a generator expression for efficiency
     return max(
@@ -202,15 +202,15 @@
         for i in range(0, len(filteredArray), min_posts)
     ]
 
 
 def get_tasks(splitArrays, filteredArray, oldmessages, model_id, c):
     tasks = []
     job_progress = progress_utils.messages_progress
-
+    # special case pass after to stop work
     if len(splitArrays) > 2:
         tasks.append(
             asyncio.create_task(
                 scrape_messages(
                     c,
                     model_id,
                     job_progress=job_progress,
@@ -233,39 +233,37 @@
                         message_id=splitArrays[i - 1][-1].get("post_id"),
                         required_ids=set(
                             [ele.get("created_at") for ele in splitArrays[i]]
                         ),
                     )
                 )
             )
-            for i in range(1, len(splitArrays) - 1)
+            for i in range(1, len(splitArrays))
         ]
         # keeping grabbing until nothing left
         tasks.append(
             asyncio.create_task(
                 scrape_messages(
                     c,
                     model_id,
                     job_progress=job_progress,
-                    message_id=splitArrays[-2][-1].get("post_id"),
-                    required_ids=set(
-                        [ele.get("created_at") for ele in splitArrays[-1]]
-                    ),
+                    message_id=splitArrays[-1][-1].get("post_id"),
+                    required_ids=set([after]),
                 )
             )
         )
     # use the first split if less then 3
     elif len(splitArrays) > 0:
         tasks.append(
             asyncio.create_task(
                 scrape_messages(
                     c,
                     model_id,
                     job_progress=job_progress,
-                    required_ids=None,
+                    required_ids=set([after]),
                     message_id=(
                         splitArrays[0][0].get("post_id")
                         if len(filteredArray) != len(oldmessages)
                         else None
                     ),
                 )
             )
@@ -275,15 +273,15 @@
         tasks.append(
             asyncio.create_task(
                 scrape_messages(
                     c,
                     model_id,
                     job_progress=job_progress,
                     message_id=None,
-                    required_ids=None,
+                    required_ids=set([after]),
                 )
             )
         )
     return tasks
 
 
 def set_check(unduped, model_id, after):
@@ -310,15 +308,15 @@
         constants.getattr("messagesNextEP")
         if message_id
         else constants.getattr("messagesEP")
     )
     url = ep.format(model_id, message_id)
     log.debug(f"{message_id if message_id else 'init'} {url}")
     new_tasks = []
-    tasks = None
+    task = None
 
     await asyncio.sleep(1)
     try:
         async with c.requests_async(url=url, sleeper=get_sleeper()) as r:
             task = (
                 job_progress.add_task(
                     f": Message ID-> {message_id if message_id else 'initial'}"
@@ -351,27 +349,16 @@
                             lambda x: f"messages scrapeinfo: {str(x)}",
                             messages,
                         )
                     ),
                 )
             )
 
-            if not required_ids:
-                new_tasks.append(
-                    asyncio.create_task(
-                        scrape_messages(
-                            c,
-                            model_id,
-                            job_progress=job_progress,
-                            message_id=messages[-1]["id"],
-                        )
-                    )
-                )
-
-            elif min(
+            #check if first value(newest) is less then then the required time
+            if max(
                 map(
                     lambda x: arrow.get(
                         x.get("createdAt", 0) or x.get("postedAt", 0)
                     ).float_timestamp,
                     messages,
                 )
             ) <= min(required_ids):
@@ -394,24 +381,25 @@
                                 model_id,
                                 job_progress=job_progress,
                                 message_id=messages[-1]["id"],
                                 required_ids=required_ids,
                             )
                         )
                     )
-        return messages, new_tasks
     except asyncio.TimeoutError:
         raise Exception(f"Task timed out {url}")
     except Exception as E:
         await asyncio.sleep(1)
         log.traceback_(E)
         log.traceback_(traceback.format_exc())
         raise E
     finally:
         (job_progress.remove_task(task) if job_progress and task is not None else None)
+    return messages, new_tasks
+
 
 
 def get_individual_post(model_id, postid):
     with sessionManager.sessionManager(
         backend="httpx",
         retries=constants.getattr("API_INDVIDIUAL_NUM_TRIES"),
         wait_min=constants.getattr("OF_MIN_WAIT_API"),
```

### Comparing `ofscraper-3.9.5/ofscraper/api/paid.py` & `ofscraper-3.9.6/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/api/pinned.py` & `ofscraper-3.9.6/ofscraper/api/pinned.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 r"""
                                                              
-r"""
-                                                             
  _______  _______         _______  _______  _______  _______  _______  _______  _______ 
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
-                 \/     \/           \/            \/         
-"""
 
 import asyncio
 import logging
 import math
 import traceback
 
 import arrow
@@ -164,21 +160,22 @@
 
 async def scrape_pinned_posts(
     c, model_id, job_progress=None, timestamp=None, count=0
 ) -> list:
     posts = None
 
     if timestamp and (
-        float(timestamp)
-        > (read_args.retriveArgs().before or arrow.now()).float_timestamp
+        float(timestamp) > (read_args.retriveArgs().before).float_timestamp
     ):
-        return []
+        return [],[]
     url = constants.getattr("timelinePinnedEP").format(model_id, count)
     log.debug(url)
+    
     new_tasks = []
+    posts=[]
     await asyncio.sleep(1)
     try:
 
         task = (
             job_progress.add_task(
                 f"Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp is not None  else 'initial'}",
                 visible=True,
```

### Comparing `ofscraper-3.9.5/ofscraper/api/profile.py` & `ofscraper-3.9.6/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/api/subscriptions/helpers.py` & `ofscraper-3.9.6/ofscraper/api/subscriptions/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/api/subscriptions/individual.py` & `ofscraper-3.9.6/ofscraper/api/subscriptions/individual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/api/subscriptions/lists.py` & `ofscraper-3.9.6/ofscraper/api/subscriptions/lists.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/api/subscriptions/subscriptions.py` & `ofscraper-3.9.6/ofscraper/api/subscriptions/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/api/timeline.py` & `ofscraper-3.9.6/ofscraper/api/timeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 r"""
                                                              
-r"""
-                                                             
  _______  _______         _______  _______  _______  _______  _______  _______  _______ 
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
-                 \/     \/           \/            \/         
-"""
 
 import asyncio
 import logging
 import math
 import traceback
 
 import arrow
@@ -40,15 +36,15 @@
 log = logging.getLogger("shared")
 
 
 @run
 async def get_timeline_posts_progress(model_id, username, forced_after=None, c=None):
 
     after = await get_after(model_id, username, forced_after)
-    after_log(username, after)
+    time_log(username, after)
     splitArrays = await get_split_array(model_id, username, after)
     tasks = get_tasks(splitArrays, c, model_id, after)
     data = await process_tasks(tasks)
     progress_utils.timeline_layout.visible = False
     return data
 
 
@@ -61,15 +57,15 @@
     else:
         oldtimeline = []
     trace_log_old(oldtimeline)
 
     log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
     oldtimeline = list(filter(lambda x: x is not None, oldtimeline))
     after = await get_after(model_id, username, forced_after)
-    after_log(username, after)
+    time_log(username, after)
 
     with progress_utils.set_up_api_timeline():
         splitArrays = await get_split_array(model_id, username, after)
         tasks = get_tasks(splitArrays, c, model_id, after)
         return await process_tasks(tasks)
 
 
@@ -174,14 +170,16 @@
     ]
     return splitArrays
 
 
 def get_tasks(splitArrays, c, model_id, after):
     tasks = []
     job_progress = progress_utils.timeline_progress
+    # special case pass before to stop work
+    before=arrow.get(read_args.retriveArgs().before or arrow.now()).float_timestamp
 
     if len(splitArrays) > 2:
         tasks.append(
             asyncio.create_task(
                 scrape_timeline_posts(
                     c,
                     model_id,
@@ -214,36 +212,40 @@
             asyncio.create_task(
                 scrape_timeline_posts(
                     c,
                     model_id,
                     job_progress=job_progress,
                     timestamp=splitArrays[-1][0].get("created_at"),
                     offset=True,
+                    required_ids=set([before])
                 )
             )
         )
     # use the first split if less then 3
     elif len(splitArrays) > 0:
         tasks.append(
             asyncio.create_task(
                 scrape_timeline_posts(
                     c,
                     model_id,
                     job_progress=job_progress,
                     timestamp=splitArrays[0][0].get("created_at"),
                     offset=True,
+                    required_ids=set([before])
+
                 )
             )
         )
     # use after if split is empty i.e no db data
     else:
         tasks.append(
             asyncio.create_task(
                 scrape_timeline_posts(
-                    c, model_id, job_progress=job_progress, timestamp=after, offset=True
+                    c, model_id, job_progress=job_progress, timestamp=after, offset=True,
+                                        required_ids=set([before])
                 )
             )
         )
 
     return tasks
 
 
@@ -321,15 +323,15 @@
     url = (
         constants.getattr("timelineNextEP").format(model_id, str(timestamp))
         if timestamp
         else constants.getattr("timelineEP").format(model_id)
     )
     log.debug(url)
     new_tasks = []
-    tasks = None
+    task = None
 
     await asyncio.sleep(1)
 
     try:
         task = (
             job_progress.add_task(
                 f"Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp is not None  else 'initial'}",
@@ -366,28 +368,15 @@
                                 posts,
                             )
                         )
                     ),
                 )
             )
 
-            if not required_ids:
-                new_tasks.append(
-                    asyncio.create_task(
-                        scrape_timeline_posts(
-                            c,
-                            model_id,
-                            job_progress=job_progress,
-                            timestamp=posts[-1]["postedAtPrecise"],
-                            offset=False,
-                        )
-                    )
-                )
-
-            elif max(map(lambda x: float(x["postedAtPrecise"]), posts)) >= max(
+            if min(map(lambda x: float(x["postedAtPrecise"]), posts)) >= max(
                 required_ids
             ):
                 pass
             elif float(timestamp or 0) >= max(required_ids):
                 pass
             else:
                 log.debug(f"{log_id} Required before {required_ids}")
@@ -453,16 +442,16 @@
             )
         )
         # Check if there are more elements remaining after this chunk
         if i + chunk_size > len(responseArray):
             break  # Exit the loop if we've processed all elements
 
 
-def after_log(username, after):
+def time_log(username, after):
     log.info(
         f"""
-Setting initial timeline scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
+Setting timeline scan range for{username} rom {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))} to{arrow.get(read_args.retriveArgs().before or arrow.now()).format((constants.getattr('API_DATE_FORMAT')))}
 [yellow]Hint: append ' --after 2000' to command to force scan of all timeline posts + download of new files only[/yellow]
 [yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all timeline posts + download/re-download of all files[/yellow]
 
             """
     )
```

### Comparing `ofscraper-3.9.5/ofscraper/classes/base.py` & `ofscraper-3.9.6/ofscraper/classes/base.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/labels.py` & `ofscraper-3.9.6/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/media.py` & `ofscraper-3.9.6/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/models.py` & `ofscraper-3.9.6/ofscraper/classes/models.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.9.6/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/placeholder.py` & `ofscraper-3.9.6/ofscraper/classes/placeholder.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,27 +355,29 @@
     @property
     def filepath(self):
         return pathlib.Path(self._filepath)
 
     @property
     def filename(self):
         return pathlib.Path(self._filepath).name
-
+    @property
+    def filedir(self):
+        return pathlib.Path(self._filepath).parent
     @property
     def trunicated_filename(self):
         return pathlib.Path(self.trunicated_filepath).name
 
     @property
     def trunicated_filepath(self):
         if settings.get_trunication(mediatype=self._ele.mediatype):
             return pathlib.Path(paths.truncate(self._filepath))
         return self._filepath
 
     @property
-    def filedir(self):
+    def trunicated_filedir(self):
         return pathlib.Path(paths.truncate(self._filepath)).parent
 
 
 class Textholders(basePlaceholder):
     def __init__(self, ele, ext) -> None:
         super().__init__()
         self._filename = None
```

### Comparing `ofscraper-3.9.5/ofscraper/classes/posts.py` & `ofscraper-3.9.6/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/sessionmanager.py` & `ofscraper-3.9.6/ofscraper/classes/sessionmanager.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/fields/boolfield.py` & `ofscraper-3.9.6/ofscraper/classes/table/fields/boolfield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/fields/datefield.py` & `ofscraper-3.9.6/ofscraper/classes/table/fields/datefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/fields/mediafield.py` & `ofscraper-3.9.6/ofscraper/classes/table/fields/mediafield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/fields/numfield.py` & `ofscraper-3.9.6/ofscraper/classes/table/fields/numfield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/fields/pricefield.py` & `ofscraper-3.9.6/ofscraper/classes/table/fields/pricefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/fields/responsefield.py` & `ofscraper-3.9.6/ofscraper/classes/table/fields/responsefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/fields/selectfield.py` & `ofscraper-3.9.6/ofscraper/classes/table/fields/selectfield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/fields/textsearch.py` & `ofscraper-3.9.6/ofscraper/classes/table/fields/textsearch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/fields/timefield.py` & `ofscraper-3.9.6/ofscraper/classes/table/fields/timefield.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/inputs/filterinput.py` & `ofscraper-3.9.6/ofscraper/classes/table/inputs/filterinput.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/status.py` & `ofscraper-3.9.6/ofscraper/classes/table/status.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/classes/table/table.py` & `ofscraper-3.9.6/ofscraper/classes/table/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/commands/check.py` & `ofscraper-3.9.6/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/commands/manual.py` & `ofscraper-3.9.6/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/commands/scraper.py` & `ofscraper-3.9.6/ofscraper/commands/scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,58 +4,58 @@
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
-                                                                                      
+                                                                                      f
 """
 
 import logging
 import traceback
 
-import ofscraper.actions.process as process_actions
 import ofscraper.prompts.prompts as prompts
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.config.data as data
 import ofscraper.utils.console as console
 import ofscraper.utils.context.exit as exit
 import ofscraper.utils.context.stdout as stdout
 import ofscraper.utils.menu as menu
 import ofscraper.utils.paths.paths as paths
 import ofscraper.utils.run as run
 import ofscraper.utils.system.network as network
 from ofscraper.__version__ import __version__
+from ofscraper.commands.add_select.add_selected import add_selected_areas
 
 log = logging.getLogger("shared")
 
 
 def process_selected_areas():
     log.debug("[bold blue] Running Action Mode [/bold blue]")
-    functs = process_actions.add_selected_areas()
+    functs = add_selected_areas()
     run.run_helper(*functs)
     while True:
         if not data.get_InfiniteLoop() or prompts.continue_prompt() == "No":
             break
         action = prompts.action_prompt()
         if action == "main":
             process_prompts()
             break
         elif action == "quit":
             break
         else:
             menu.get_count() > 0 and menu.reset_menu_helper()
-            functs = process_actions.add_selected_areas()
+            functs = add_selected_areas()
             run.run_helper(*functs)
             menu.update_count()
 
 
 def daemon_process():
-    functs = process_actions.add_selected_areas()
+    functs = add_selected_areas()
     run.daemon_run_helper(*functs)
 
 
 @exit.exit_wrapper
 def process_prompts():
     while True:
         if menu.main_menu_action():
```

### Comparing `ofscraper-3.9.5/ofscraper/const/config.py` & `ofscraper-3.9.6/ofscraper/const/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/const/general.py` & `ofscraper-3.9.6/ofscraper/const/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/const/other_url.py` & `ofscraper-3.9.6/ofscraper/const/other_url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/const/prompts.py` & `ofscraper-3.9.6/ofscraper/const/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/const/req.py` & `ofscraper-3.9.6/ofscraper/const/req.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 OF_MIN_WAIT_SESSION_DEFAULT = 4
 OF_MAX_WAIT_SESSION_DEFAULT = 20
 OF_MIN_WAIT_EXPONENTIAL_SESSION_DEFAULT = 16
 OF_MAX_WAIT_EXPONENTIAL_SESSION_DEFAULT = 128
 OF_NUM_RETRIES_SESSION_DEFAULT = 10
 
 
-OF_MIN_WAIT_API = 10
-OF_MAX_WAIT_API = 20
+OF_MIN_WAIT_API = 3
+OF_MAX_WAIT_API = 12
 OF_AUTH_MIN_WAIT = 3
 OF_AUTH_MAX_WAIT = 10
 GIT_MIN_WAIT = 1
 GIT_MAX_WAIT = 5
 DISCORD_MIN_WAIT = 1
 DISCORD_MAX_WAIT = 5
 CDM_MIN_WAIT = 1
```

### Comparing `ofscraper-3.9.5/ofscraper/const/test_constants.py` & `ofscraper-3.9.6/ofscraper/const/test_constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/const/url.py` & `ofscraper-3.9.6/ofscraper/const/url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/db/operations.py` & `ofscraper-3.9.6/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/db/operations_/labels.py` & `ofscraper-3.9.6/ofscraper/db/operations_/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/db/operations_/media.py` & `ofscraper-3.9.6/ofscraper/db/operations_/media.py`

 * *Files 12% similar despite different names*

```diff
@@ -122,19 +122,26 @@
 
 mediaInsertTransition = """INSERT INTO 'medias'(
 media_id,post_id,link,directory,
 filename,size,api_type,
 media_type,preview,linked,
 downloaded,created_at,posted_at,hash,model_id,duration,unlocked)
             VALUES (?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?);"""
+
+mediaDownloadForce = """
+Update 'medias'
+SET
+unlocked=0
+WHERE media_id=(?) and model_id=(?);
+"""
 mediaDownloadSelect = """
 SELECT  
-directory,filename,size
+directory,filename,size,
 downloaded,hash
-FROM medias where media_id=(?)
+FROM medias where media_id=(?) and model_id=(?)
 """
 allIDCheck = """
 SELECT media_id FROM medias
 """
 allDLIDCheck = """
 SELECT media_id FROM medias where downloaded=(1)
 """
@@ -318,29 +325,36 @@
         return [dict(row)["filename"] for row in cur.fetchall()]
 
 
 @wrapper.operation_wrapper_async
 def download_media_update(
     media,
     model_id=None,
+    username=None,
     conn=None,
+    filepath=None,
     filename=None,
+    directory=None,
     downloaded=None,
     hashdata=None,
     changed=False,
     **kwargs,
 ):
     with contextlib.closing(conn.cursor()) as curr:
+        filename=filename or (filepath.name if filepath!=None else None)
+        directory=directory or (filepath.parent if filepath!=None else None)
         update_media_table_via_api_helper(
             media, curr=curr, model_id=model_id, conn=conn
         )
         update_media_table_download_helper(
             media,
             model_id,
             filename=filename,
+            directory=directory,
+            username=username,
             hashdata=hashdata,
             conn=conn,
             curr=curr,
             downloaded=downloaded,
         )
         return curr.rowcount if changed else None
 
@@ -447,15 +461,15 @@
 
 @wrapper.operation_wrapper_async
 def drop_media_table(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(mediaDrop)
         conn.commit()
 
-
+@run
 @wrapper.operation_wrapper_async
 def get_messages_media(conn=None, model_id=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(getMessagesMedia, [model_id])
         data = [dict(row) for row in cur.fetchall()]
         return [
             dict(
@@ -520,56 +534,61 @@
     conn.commit()
 
 
 def update_media_table_download_helper(
     media,
     model_id,
     filename=None,
+    directory=None,
     hashdata=None,
     conn=None,
     downloaded=None,
     curr=None,
     **kwargs,
 ) -> list:
-    prevData = curr.execute(mediaDownloadSelect, (media.id,)).fetchall()
-    prevData = prevData[0] if isinstance(prevData, list) and bool(prevData) else None
-    insertData = media_exist_insert_helper(
-        filename=filename, hashdata=hashdata, prevData=prevData, downloaded=downloaded
-    )
-    insertData.extend([media.id, model_id])
-    curr.execute(mediaUpdateDownload, insertData)
-    conn.commit()
-
+    size=pathlib.Path(directory,filename).stat().st_size if directory and filename and pathlib.Path(directory,filename).exists() else None
 
-def media_exist_insert_helper(
-    filename=None, downloaded=None, hashdata=None, prevData=None, **kwargs
-):
-    directory = None
-    filename_path = None
-    size = None
-    if filename and pathlib.Path(filename).exists():
-        directory = str(pathlib.Path(filename).parent)
-        filename_path = str(pathlib.Path(filename).name)
-        size = math.ceil(pathlib.Path(filename).stat().st_size)
-    elif filename:
-        directory = str(pathlib.Path(filename).parent)
-        filename_path = str(pathlib.Path(filename).name)
-    elif prevData:
-        directory = prevData[0]
-        filename_path = prevData[1]
-        size = prevData[2]
-        hashdata = prevData[3] or hashdata
+    filename=str(filename) if filename else None
+    directory=str(directory) if directory else None
     insertData = [
         directory,
-        filename_path,
+        filename,
         size,
         downloaded,
         hashdata,
     ]
-    return insertData
+    insertData.extend([media.id, model_id])
+    curr.execute(mediaUpdateDownload, insertData)
+    conn.commit()
+
+@run
+@wrapper.operation_wrapper_async
+def prev_download_media_data(media,model_id=None, username=None, conn=None, **kwargs):
+    with contextlib.closing(conn.cursor()) as curr:
+        prevData = curr.execute(mediaDownloadSelect, (media.id,model_id)).fetchone()
+        prevData = dict(prevData) if prevData else None
+        return prevData
+
+@wrapper.operation_wrapper
+def batch_set_media_downloaded(medias, model_id=None, conn=None, **kwargs):
+    with contextlib.closing(conn.cursor()) as curr:
+        insertData = list(
+            map(
+                lambda media: [
+                    media["media_id"],
+                    model_id,
+                ],
+                medias,
+            )
+        )
+        curr.executemany(mediaDownloadForce, insertData)
+        conn.commit()
+
+
+
 
 
 @run
 async def batch_mediainsert(media, **kwargs):
     curr = set(await get_media_ids(**kwargs) or [])
     mediaDict = {}
     for ele in media:
```

### Comparing `ofscraper-3.9.5/ofscraper/db/operations_/merge.py` & `ofscraper-3.9.6/ofscraper/db/operations_/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/db/operations_/messages.py` & `ofscraper-3.9.6/ofscraper/db/operations_/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/db/operations_/others.py` & `ofscraper-3.9.6/ofscraper/db/operations_/others.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/db/operations_/posts.py` & `ofscraper-3.9.6/ofscraper/db/operations_/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/db/operations_/profile.py` & `ofscraper-3.9.6/ofscraper/db/operations_/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/db/operations_/stories.py` & `ofscraper-3.9.6/ofscraper/db/operations_/stories.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/db/operations_/wrapper.py` & `ofscraper-3.9.6/ofscraper/db/operations_/wrapper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/alt_download.py` & `ofscraper-3.9.6/ofscraper/download/alt_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/alt_downloadbatch.py` & `ofscraper-3.9.6/ofscraper/download/alt_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/download.py` & `ofscraper-3.9.6/ofscraper/download/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         log.debug(f"Final Number of media to download {len(medialist)} ")
 
     return medialist
 
 
 def download_process(username, model_id, medialist, posts=None):
     data = None
-    if read_args.retriveArgs().metadata:
+    if read_args.retriveArgs().command == "metadata":
         medialist = (
             list(filter(lambda x: x.canview, medialist))
             if constants.getattr("REMOVE_UNVIEWABLE_METADATA")
             else medialist
         )
         logging.getLogger().info(f"Final media count for metadata {len(medialist)}")
         medialist = medialist_filter(medialist, model_id, username)
```

### Comparing `ofscraper-3.9.5/ofscraper/download/downloadbatch.py` & `ofscraper-3.9.6/ofscraper/download/downloadbatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         common_globals.reset_globals()
         if not read_args.retriveArgs().item_sort:
             random.shuffle(filtered_medialist)
         manager = manager_.get_manager()
         mediasplits = get_mediasplits(filtered_medialist)
         num_proc = len(mediasplits)
         split_val = min(4, num_proc)
-        log.debug(f"Number of process {num_proc}")
+        log.debug(f"Number of download threads: {num_proc}")
         connect_tuples = [AioPipe() for _ in range(num_proc)]
         shared = list(more_itertools.chunked([i for i in range(num_proc)], split_val))
         # shared with other process + main
         logqueues_ = [manager.Queue() for _ in range(len(shared))]
         # other logger queuesprocesses
         otherqueues_ = [manager.Queue() for _ in range(len(shared))]
         # shared cache
@@ -163,16 +163,16 @@
                         log.debug(f"Number of Log Threads: {len(new_logthreads)}")
                     if len(new_logthreads) == 0:
                         break
                     log_threads = new_logthreads
                     for thread in log_threads:
                         thread.join(timeout=0.1)
                     time.sleep(0.5)
-                log.debug(f"Initial Processes: {processes}")
-                log.debug(f"Initial Number of Processes: {len(processes)}")
+                log.debug(f"Initial download threads: {processes}")
+                log.debug(f"Initial Number of download threads: {len(processes)}")
                 while True:
                     new_proceess = list(filter(lambda x: x and x.is_alive(), processes))
                     if len(new_proceess) != len(processes):
                         log.debug(f"Remaining Processes: {new_proceess}")
                         log.debug(f"Number of Processes: {len(new_proceess)}")
                     if len(new_proceess) == 0:
                         break
```

### Comparing `ofscraper-3.9.5/ofscraper/download/downloadnormal.py` & `ofscraper-3.9.6/ofscraper/download/downloadnormal.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/main_download.py` & `ofscraper-3.9.6/ofscraper/download/main_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/main_downloadbatch.py` & `ofscraper-3.9.6/ofscraper/download/main_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/shared/classes/retries.py` & `ofscraper-3.9.6/ofscraper/download/shared/classes/retries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/shared/classes/session.py` & `ofscraper-3.9.6/ofscraper/download/shared/classes/session.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/shared/common/alt_common.py` & `ofscraper-3.9.6/ofscraper/download/shared/common/alt_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         common_paths.set_time(sharedPlaceholderObj.trunicated_filepath, newDate)
         common_globals.log.debug(
             f"{common_logs.get_medialog(ele)} Date set to {arrow.get(sharedPlaceholderObj.trunicated_filepath.stat().st_mtime).format('YYYY-MM-DD HH:mm')}"
         )
     if ele.id:
         await download_media_update(
             ele,
-            filename=sharedPlaceholderObj.trunicated_filepath,
+            filepath=sharedPlaceholderObj.trunicated_filepath,
             model_id=model_id,
             username=username,
             downloaded=True,
             hashdata=await common.get_hash(
                 sharedPlaceholderObj, mediatype=ele.mediatype
             ),
         )
```

### Comparing `ofscraper-3.9.5/ofscraper/download/shared/common/general.py` & `ofscraper-3.9.6/ofscraper/download/shared/common/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/shared/common/main_common.py` & `ofscraper-3.9.6/ofscraper/download/shared/common/main_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         common_globals.log.debug(
             f"{common_logs.get_medialog(ele)} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}"
         )
 
     if ele.id:
         await download_media_update(
             ele,
-            filename=path_to_file,
+            filepath=path_to_file,
             model_id=model_id,
             username=username,
             downloaded=True,
             hashdata=await common.get_hash(path_to_file, mediatype=ele.mediatype),
         )
     await common.set_profile_cache_helper(ele)
     common.add_additional_data(placeholderObj, ele)
```

### Comparing `ofscraper-3.9.5/ofscraper/download/shared/globals.py` & `ofscraper-3.9.6/ofscraper/download/shared/globals.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/shared/utils/keyhelpers.py` & `ofscraper-3.9.6/ofscraper/download/shared/utils/keyhelpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/shared/utils/log.py` & `ofscraper-3.9.6/ofscraper/download/shared/utils/log.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/shared/utils/message.py` & `ofscraper-3.9.6/ofscraper/download/shared/utils/message.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/shared/utils/paths.py` & `ofscraper-3.9.6/ofscraper/download/shared/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/download/shared/utils/text.py` & `ofscraper-3.9.6/ofscraper/download/shared/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/filters/media/helpers.py` & `ofscraper-3.9.6/ofscraper/filters/media/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/filters/media/main.py` & `ofscraper-3.9.6/ofscraper/filters/media/main.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/filters/models/date.py` & `ofscraper-3.9.6/ofscraper/filters/models/date.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/filters/models/flags.py` & `ofscraper-3.9.6/ofscraper/filters/models/flags.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/filters/models/helpers.py` & `ofscraper-3.9.6/ofscraper/filters/models/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/filters/models/other.py` & `ofscraper-3.9.6/ofscraper/filters/models/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/filters/models/price.py` & `ofscraper-3.9.6/ofscraper/filters/models/price.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/filters/models/sort.py` & `ofscraper-3.9.6/ofscraper/filters/models/sort.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/filters/models/subtype.py` & `ofscraper-3.9.6/ofscraper/filters/models/subtype.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/models/retriver.py` & `ofscraper-3.9.6/ofscraper/models/retriver.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/models/selector.py` & `ofscraper-3.9.6/ofscraper/models/selector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/helpers/model_helpers.py` & `ofscraper-3.9.6/ofscraper/prompts/helpers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/helpers/prompt_helpers.py` & `ofscraper-3.9.6/ofscraper/prompts/helpers/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/keybindings.py` & `ofscraper-3.9.6/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/promptConvert.py` & `ofscraper-3.9.6/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/actions.py` & `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/area.py` & `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/area.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,26 +20,27 @@
 import ofscraper.utils.args.areas as areas
 import ofscraper.utils.args.read as read_args
 
 
 def areas_prompt() -> list:
     args = read_args.retriveArgs()
     name = "value"
-    message = (
-        "Which area(s) would you do you want to download and like"
-        if "like" in args.action and len(args.like_area) == 0
-        else (
-            "Which area(s) would you want to download and unlike"
-            if "unike" in args.action and len(args.like_area) == 0
-            else "Which area(s) would you like to download"
-        )
-    )
+    message = None
+    print(args.command)
+    if "like" in args.action and len(args.like_area) == 0:
+        message = "Which area(s) would you do you want to download and like"
+    elif "unlike" in args.action and len(args.like_area) == 0:
+        message = "Which area(s) would you do you want to download and unlike"
+    elif "download" in args.action and args.command == "OF-Scraper":
+        message = "Which area(s) would you do you want to download"
+    elif "download" in args.action and args.command == "metadata":
+        message = "Which area(s) would you do you want to update metadata for"
     more_instruction = (
         """Hint: Since you have Like or Unlike set
-You must select one or more of Timeline,Pinned,Archived, or Label
+    You must select one or more of Timeline,Pinned,Archived, or Label
 """
         if ("like" or "unlike") in args.action and len(args.like_area) == 0
         else ""
     )
     answers = promptClasses.batchConverter(
         *[
             {
```

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/auth.py` & `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/binary.py` & `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/binary.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/config.py` & `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/menu.py` & `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/merge.py` & `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/model.py` & `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/model.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/profile.py` & `ofscraper-3.9.6/ofscraper/prompts/prompt_groups/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.9.6/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.9.6/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/prompts/prompts.py` & `ofscraper-3.9.6/ofscraper/utils/encoding.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,12 @@
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
-from ofscraper.prompts.prompt_groups.actions import *
-from ofscraper.prompts.prompt_groups.area import *
-from ofscraper.prompts.prompt_groups.auth import *
-from ofscraper.prompts.prompt_groups.binary import *
-from ofscraper.prompts.prompt_groups.config import *
-from ofscraper.prompts.prompt_groups.menu import *
-from ofscraper.prompts.prompt_groups.merge import *
-from ofscraper.prompts.prompt_groups.model import *
-from ofscraper.prompts.prompt_groups.profile import *
+
+def encode_utf_16(string):
+    encoded_string = string.encode("utf-16", "surrogatepass")
+    decoded_string = encoded_string.decode("utf-16")
+    return decoded_string
```

### Comparing `ofscraper-3.9.5/ofscraper/runner/exit.py` & `ofscraper-3.9.6/ofscraper/runner/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/runner/load.py` & `ofscraper-3.9.6/ofscraper/runner/load.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/runner/run.py` & `ofscraper-3.9.6/ofscraper/runner/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/actions.py` & `ofscraper-3.9.6/ofscraper/utils/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/args/areas.py` & `ofscraper-3.9.6/ofscraper/utils/args/areas.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/args/groups/manual_args.py` & `ofscraper-3.9.6/ofscraper/utils/args/bundles/paid_check.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 import itertools
 
 import cloup as click
 
-import ofscraper.utils.args.groups.common_args as common
 import ofscraper.utils.args.helpers as helpers
+from ofscraper.utils.args.bundles.advanced_common import advanced_args
+from ofscraper.utils.args.bundles.common import common_args
 
 
-@click.command(
-    "manual",
-    help="Manually download media by providing a list of urls or IDs",
-    short_help="Manually download media by providing a list of urls or IDs",
-)
-@common.common_params
-@common.common_other_params
-@click.constraints.require_one(
-    click.option(
-        "-u",
-        "--url",
-        help="A space or comma seperated list of urls to download",
-        default=None,
-        multiple=True,
-        type=helpers.check_strhelper,
-        callback=lambda ctx, param, value: (
-            list(set(itertools.chain.from_iterable(value))) if value else []
+def paid_check_args(func):
+    @click.command(
+        "paid_check",
+        short_help="""\b
+                Produces a media table from purchases with filterable entries and quick downloads""",
+        help="""
+    The paid_check subcommand gathers information on media content from purchases
+    It presents this data in a table format with filtering options for focused searches 
+    Allows unlocked media entries to be directly downloaded through the table
+    """,
+    )
+    @common_args
+    @click.constraints.require_one(
+        click.option(
+            "-u",
+            "--usernames",
+            "--username",
+            "check_usernames",
+            help="Scan purchases via username(s)",
+            default=None,
+            multiple=True,
+            type=helpers.check_strhelper,
+            callback=lambda ctx, param, value: (
+                list(set(itertools.chain.d(value))) if value else []
+            ),
         ),
-    ),
-    click.option(
-        "-f",
-        "--file",
-        help="file with line-separated URL(s) for downloading",
-        default=None,
-        type=helpers.check_filehelper,
-        multiple=True,
-        callback=lambda ctx, param, value: (
-            list(set(itertools.chain.from_iterable(value))) if value else []
+        click.option(
+            "-f",
+            "--file",
+            help="Scan pu via a file with line-separated URL(s)",
+            default=None,
+            type=helpers.check_filehelper,
+            multiple=True,
+            callback=lambda ctx, param, value: (
+                list(set(itertools.chain.from_iterable(value))) if value else []
+            ),
         ),
-    ),
-)
-@click.option(
-    "-fo",
-    "--force",
-    help="Force retrieval of new messages info from API",
-    is_flag=True,
-    default=False,
-)
-@common.common_advanced_params
-@click.pass_context
-def manual(ctx, *args, **kwargs):
-    return ctx.params, ctx.info_name
+    )
+    @click.option(
+        "-fo",
+        "--force",
+        help="Force retrieval of new purchases info from API",
+        is_flag=True,
+        default=False,
+    )
+    @advanced_args
+    @click.pass_context
+    def wrapper(ctx, *args, **kwargs):
+        return func(ctx, *args, **kwargs)
+
+    return wrapper
```

### Comparing `ofscraper-3.9.5/ofscraper/utils/args/groups/message_args.py` & `ofscraper-3.9.6/ofscraper/utils/args/bundles/story_check.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 import itertools
 
 import cloup as click
 
-import ofscraper.utils.args.groups.common_args as common
 import ofscraper.utils.args.helpers as helpers
+from ofscraper.utils.args.bundles.advanced_common import advanced_args
+from ofscraper.utils.args.bundles.common import common_args
 
 
-@click.command(
-    "msg_check",
-    short_help="""\b
-               Produces a media table from messages with filterable entries and quick downloads""",
-    help="""
-The msg_check subcommand gathers information on media content from messages
-It presents this data in a table format with filtering options for focused searches 
-Allows unlocked media entries to be directly downloaded through the table
-""",
-)
-@common.common_params
-@common.common_other_params
-@click.constraints.require_one(
-    click.option(
-        "-u",
-        "--url",
-        help="Scan messages via space or comma seperated list of urls",
-        default=None,
-        multiple=True,
-        type=helpers.check_strhelper,
-        callback=lambda ctx, param, value: (
-            list(set(itertools.chain.from_iterable(value))) if value else []
+def story_check_args(func):
+
+    @click.command(
+        "story_check",
+        short_help="""\b
+                Produces a media table from stories and highlights with filterable entries and quick downloads""",
+        help="""
+    The story_check subcommand gathers information on media content from stories and highlights
+    It presents this data in a table format with filtering options for focused searches 
+    Allows unlocked media entries to be directly downloaded through the table
+    """,
+    )
+    @common_args
+    @click.constraints.require_one(
+        click.option(
+            "-u",
+            "--usernames",
+            "--username",
+            "check_usernames",
+            help="Scan stories/highlights via username(s)",
+            default=None,
+            multiple=True,
+            type=helpers.check_strhelper,
+            callback=lambda ctx, param, value: (
+                list(set(itertools.chain.from_iterable(value))) if value else []
+            ),
+        ),
+        click.option(
+            "-f",
+            "--file",
+            help="Scan stories/highlights via a file with line-separated URL(s)",
+            default=None,
+            type=helpers.check_filehelper,
+            multiple=True,
+            callback=lambda ctx, param, value: (
+                list(set(itertools.chain.from_iterable(value))) if value else []
+            ),
         ),
-    ),
-    click.option(
-        "-f",
-        "--file",
-        help="Scan messages via a file with line-separated URL(s)",
-        default=None,
-        type=helpers.check_filehelper,
-        multiple=True,
-        callback=lambda ctx, param, value: (
-            list(set(itertools.chain.from_iterable(value))) if value else []
-        ),  # Open file for reading
-    ),
-)
-@click.option(
-    "-fo",
-    "--force",
-    help="Force retrieval of new messages info from API",
-    is_flag=True,
-    default=False,
-)
-@common.common_advanced_params
-@click.pass_context
-def message_check(ctx, *args, **kwargs):
-    return ctx.params, ctx.info_name
+    )
+    @click.option(
+        "-fo",
+        "--force",
+        help="Force retrieval of new messages info from API",
+        is_flag=True,
+        default=False,
+    )
+    @advanced_args
+    @click.pass_context
+    def wrapper(ctx, *args, **kwargs):
+        return func(ctx, *args, **kwargs)
+
+    return wrapper
```

### Comparing `ofscraper-3.9.5/ofscraper/utils/args/groups/paid_args.py` & `ofscraper-3.9.6/ofscraper/utils/args/arguments/media_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,54 @@
+# Define individual options
 import itertools
 
 import cloup as click
 
-import ofscraper.utils.args.groups.common_args as common
-import ofscraper.utils.args.helpers as helpers
+# import click
+from humanfriendly import parse_size
 
+import ofscraper.utils.args.helpers as helpers
 
-@click.command(
-    "paid_check",
-    short_help="""\b
-               Produces a media table from purchases with filterable entries and quick downloads""",
-    help="""
-The paid_check subcommand gathers information on media content from purchases
-It presents this data in a table format with filtering options for focused searches 
-Allows unlocked media entries to be directly downloaded through the table
-""",
+quality_option = click.option(
+    "-q",
+    "--quality",
+    type=click.Choice(["240", "720", "source"], case_sensitive=False),
 )
-@common.common_params
-@common.common_other_params
-@click.constraints.require_one(
-    click.option(
-        "-u",
-        "--usernames",
-        "--username",
-        "check_usernames",
-        help="Scan purchases via username(s)",
-        default=None,
-        multiple=True,
-        type=helpers.check_strhelper,
-        callback=lambda ctx, param, value: (
-            list(set(itertools.chain.from_iterable(value))) if value else []
-        ),
-    ),
-    click.option(
-        "-f",
-        "--file",
-        help="Scan pu via a file with line-separated URL(s)",
-        default=None,
-        type=helpers.check_filehelper,
-        multiple=True,
-        callback=lambda ctx, param, value: (
-            list(set(itertools.chain.from_iterable(value))) if value else []
-        ),
+
+media_type_option = click.option(
+    "-mt",
+    "--mediatype",
+    help="Filter by media type (Videos, Audios, Images)",
+    default=[],
+    required=False,
+    type=helpers.mediatype_helper,
+    callback=lambda ctx, param, value: (
+        list(set(itertools.chain.from_iterable(value))) if value else []
     ),
+    multiple=True,
 )
-@click.option(
-    "-fo",
-    "--force",
-    help="Force retrieval of new purchases info from API",
-    is_flag=True,
-    default=False,
+
+max_size_option = click.option(
+    "-sx",
+    "--size-max",
+    help="Filter out files larger than the given size (bytes or human-readable, e.g., 10mb)",
+    required=False,
+    type=parse_size,
+)
+
+min_size_option = click.option(
+    "-sm",
+    "--size-min",
+    help="Filter out files smaller than the given size (bytes or human-readable, e.g., 10mb)",
+    required=False,
+    type=parse_size,
+)
+
+# Create the option group
+media_type_options = click.option_group(
+    "Media Filters Options",
+    quality_option,
+    media_type_option,
+    max_size_option,
+    min_size_option,
+    help="Options for controlling which media is downloaded",
 )
-@common.common_advanced_params
-@click.pass_context
-def paid_check(ctx, *args, **kwargs):
-    return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.5/ofscraper/utils/args/groups/post_args.py` & `ofscraper-3.9.6/ofscraper/utils/args/bundles/post_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 import itertools
 
 import cloup as click
 
-import ofscraper.utils.args.groups.common_args as common
 import ofscraper.utils.args.helpers as helpers
+from ofscraper.utils.args.bundles.advanced_common import advanced_args
+from ofscraper.utils.args.bundles.common import common_args
 
 
-@click.command(
-    "post_check",
-    short_help="""\b
-               Produces a media table from posts with filterable entries and quick downloads""",
-    help="""The post_check subcommand gathers information on media content from posts
-It presents this data in a table format with filtering options for focused searches 
-Allows unlocked media entries to be directly downloaded through the table""",
-)
-@common.common_params
-@common.common_other_params
-@click.constraints.require_one(
-    click.option(
-        "-u",
-        "--url",
-        help="Scan posts via space or comma seperated list of urls",
-        default=None,
-        multiple=True,
-        type=helpers.check_strhelper,
-        callback=lambda ctx, param, value: (
-            list(set(itertools.chain.from_iterable(value))) if value else []
+def post_check_args(func):
+    @click.command(
+        "post_check",
+        short_help="""\b
+                Produces a media table from posts with filterable entries and quick downloads""",
+        help="""The post_check subcommand gathers information on media content from posts
+    It presents this data in a table format with filtering options for focused searches 
+    Allows unlocked media entries to be directly downloaded through the table""",
+    )
+    @common_args
+    @click.constraints.require_one(
+        click.option(
+            "-u",
+            "--url",
+            help="Scan posts via space or comma seperated list of urls",
+            default=None,
+            multiple=True,
+            type=helpers.check_strhelper,
+            callback=lambda ctx, param, value: (
+                list(set(itertools.chain.from_iterable(value))) if value else []
+            ),
+        ),
+        click.option(
+            "-f",
+            "--file",
+            help="Scan posts via a file with line-separated URL(s)",
+            default=None,
+            type=helpers.check_filehelper,
+            multiple=True,
+            callback=lambda ctx, param, value: (
+                list(set(itertools.chain.from_iterable(value))) if value else []
+            ),
+        ),
+    )
+    @click.option(
+        "-fo",
+        "--force",
+        help="Force retrieval of new posts info from API",
+        is_flag=True,
+        default=False,
+    )
+    @click.option(
+        "-ca",
+        "--check-area",
+        help="Select areas to check (multiple allowed, separated by spaces)",
+        default=["Timeline", "Pinned", "Archived"],
+        type=click.Choice(
+            ["Timeline", "Pinned", "Archived", "Labels"], case_sensitive=False
         ),
-    ),
-    click.option(
-        "-f",
-        "--file",
-        help="Scan posts via a file with line-separated URL(s)",
-        default=None,
-        type=helpers.check_filehelper,
-        multiple=True,
         callback=lambda ctx, param, value: (
-            list(set(itertools.chain.from_iterable(value))) if value else []
+            list(set(helpers.post_check_area(value))) if value else None
         ),
-    ),
-)
-@click.option(
-    "-fo",
-    "--force",
-    help="Force retrieval of new posts info from API",
-    is_flag=True,
-    default=False,
-)
-@click.option(
-    "-ca",
-    "--check-area",
-    help="Select areas to check (multiple allowed, separated by spaces)",
-    default=["Timeline", "Pinned", "Archived"],
-    type=click.Choice(
-        ["Timeline", "Pinned", "Archived", "Labels"], case_sensitive=False
-    ),
-    callback=lambda ctx, param, value: (
-        list(set(helpers.post_check_area(value))) if value else None
-    ),
-    multiple=True,
-)
-@common.common_advanced_params
-@click.pass_context
-def post_check(ctx, *args, **kwargs):
-    return ctx.params, ctx.info_name
+        multiple=True,
+    )
+    @advanced_args
+    @click.pass_context
+    def wrapper(ctx, *args, **kwargs):
+        return func(ctx, *args, **kwargs)
+
+    return wrapper
```

### Comparing `ofscraper-3.9.5/ofscraper/utils/args/helpers.py` & `ofscraper-3.9.6/ofscraper/utils/args/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
 def username_helper(x):
     temp = None
     if isinstance(x, list):
         temp = x
     elif isinstance(x, str):
         temp = re.split(",| ", x)
-
+    temp=list(filter(lambda x:len(x)>0,temp))
     return list(map(lambda x: x.lower() if not x == "ALL" else x, temp))
 
 
 def label_helper(x):
     temp = None
     if isinstance(x, list):
         temp = x
```

### Comparing `ofscraper-3.9.5/ofscraper/utils/args/parse.py` & `ofscraper-3.9.6/ofscraper/utils/args/parse.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
 import sys
 
-import ofscraper.utils.args.groups.main_args as main
-import ofscraper.utils.args.groups.manual_args as manual
-import ofscraper.utils.args.groups.message_args as message
-import ofscraper.utils.args.groups.paid_args as paid
-import ofscraper.utils.args.groups.post_args as post
-import ofscraper.utils.args.groups.story_args as story
+import ofscraper.utils.args.commands.main as main
+import ofscraper.utils.args.commands.manual as manual
+import ofscraper.utils.args.commands.message as message
+import ofscraper.utils.args.commands.metadata as metadata
+import ofscraper.utils.args.commands.paid as paid
+import ofscraper.utils.args.commands.post as post
+import ofscraper.utils.args.commands.story as story
 import ofscraper.utils.args.write as write_args
 
 
 class AutoDotDict(dict):
     """
     Class that automatically converts a dictionary to an object-like structure
     with dot notation access for top-level keys.
@@ -36,15 +37,15 @@
 def parse_args():
     try:
         main.program.add_command(manual.manual, "manual")
         main.program.add_command(message.message_check, "msg_check")
         main.program.add_command(story.story_check, "story_check")
         main.program.add_command(paid.paid_check, "paid_check")
         main.program.add_command(post.post_check, "post_check")
-
+        main.program.add_command(metadata.metadata, "metadata")
         filter_str = r"\b(multiprocessing|pipe_handle|fork|parent_pid)\b"
         result = main.program(
             standalone_mode=False,
             prog_name="OF-Scraper",
             args=[text for text in sys.argv if not re.search(filter_str, text)][1:],
         )
         if result == 0:
```

### Comparing `ofscraper-3.9.5/ofscraper/utils/args/read.py` & `ofscraper-3.9.6/ofscraper/utils/args/read.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/args/user.py` & `ofscraper-3.9.6/ofscraper/utils/args/user.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/auth/context.py` & `ofscraper-3.9.6/ofscraper/utils/auth/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/auth/data.py` & `ofscraper-3.9.6/ofscraper/utils/auth/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/auth/file.py` & `ofscraper-3.9.6/ofscraper/utils/auth/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/auth/helpers.py` & `ofscraper-3.9.6/ofscraper/utils/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/auth/make.py` & `ofscraper-3.9.6/ofscraper/utils/auth/make.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/auth/request.py` & `ofscraper-3.9.6/ofscraper/utils/auth/request.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/auth/schema.py` & `ofscraper-3.9.6/ofscraper/utils/auth/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/binaries.py` & `ofscraper-3.9.6/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/cache.py` & `ofscraper-3.9.6/ofscraper/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/checkers.py` & `ofscraper-3.9.6/ofscraper/utils/checkers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/config/config.py` & `ofscraper-3.9.6/ofscraper/utils/config/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,72 +4,80 @@
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
-                                                                                      
+                                         
 """
 
 import logging
 
 import ofscraper.prompts.prompts as prompts
 import ofscraper.utils.binaries as binaries
 import ofscraper.utils.config.context as config_context
 import ofscraper.utils.config.file as config_file
 import ofscraper.utils.config.schema as schema
 import ofscraper.utils.console as console_
 
 console = console_.get_shared_console()
 log = logging.getLogger("shared")
+config=None
 
 
 def read_config(update=True):
+    global config
+    if config:
+        return config
     while True:
         with config_context.config_context():
             config = config_file.open_config()
             if update and schema.config_diff(config):
                 config = config_file.auto_update_config(config)
             if config.get("config"):
                 config = config["config"]
             return config
 
 
 def update_config(field: str, value):
+    global config
     config = config_file.open_config()
     if config.get("config"):
         config = config["config"]
     config.update({field: value})
     new_config = schema.get_current_config_schema(config)
     config_file.write_config(new_config)
     log.debug(f"new config: {config}")
     return new_config
 
 
-def update_config_full(config, updated_config):
+def update_config_full(config_, updated_config):
+    global config
     if config.get("config"):
-        config = config["config"]
+        config = config_["config"]
     if updated_config.get("config"):
         updated_config = updated_config["config"]
     config.update(updated_config)
     log.debug(f"new config: {config}")
     config_file.write_config(config)
     return config
 
 
 def update_mp4decrypt():
+    global config
     config = {"config": read_config()}
     if prompts.auto_download_mp4_decrypt() == "Yes":
         config["config"]["mp4decrypt"] = binaries.mp4decrypt_download()
     else:
         config["config"]["mp4decrypt"] = prompts.mp4_prompt()
     config_file.write_config(config)
 
 
 def update_ffmpeg():
+    global config
     config = {"config": read_config()}
     if prompts.auto_download_ffmpeg() == "Yes":
         config["config"]["ffmpeg"] = binaries.ffmpeg_download()
     else:
         config["config"]["ffmpeg"] = prompts.ffmpeg_prompt()
     config_file.write_config(config)
```

### Comparing `ofscraper-3.9.5/ofscraper/utils/config/context.py` & `ofscraper-3.9.6/ofscraper/utils/config/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/config/custom.py` & `ofscraper-3.9.6/ofscraper/utils/config/custom.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/config/data.py` & `ofscraper-3.9.6/ofscraper/utils/config/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/config/file.py` & `ofscraper-3.9.6/ofscraper/utils/config/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/config/menu.py` & `ofscraper-3.9.6/ofscraper/utils/config/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/config/schema.py` & `ofscraper-3.9.6/ofscraper/utils/config/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/constants.py` & `ofscraper-3.9.6/ofscraper/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/context/exit.py` & `ofscraper-3.9.6/ofscraper/utils/context/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/context/run_async.py` & `ofscraper-3.9.6/ofscraper/utils/context/run_async.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/context/stdout.py` & `ofscraper-3.9.6/ofscraper/utils/context/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/dates.py` & `ofscraper-3.9.6/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/encoding.py` & `ofscraper-3.9.6/ofscraper/utils/profiles/tools.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,12 +7,35 @@
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
+import logging
+import re
 
-def encode_utf_16(string):
-    encoded_string = string.encode("utf-16", "surrogatepass")
-    decoded_string = encoded_string.decode("utf-16")
-    return decoded_string
+from rich.console import Console
+
+import ofscraper.utils.profiles.data as profile_data
+
+log = logging.getLogger("shared")
+console = Console()
+currentData = None
+currentProfile = None
+
+
+def print_profiles() -> list:
+    print_current_profile()
+    console.print("\n\nCurrent Profiles\n")
+    profile_fmt = "Profile: [cyan]{}"
+    for name in profile_data.get_profile_names():
+        console.print(profile_fmt.format(name))
+
+
+def print_current_profile():
+    current_profile = profile_data.get_active_profile()
+    log.info("Using profile: [cyan]{}[/cyan]".format(current_profile))
+
+
+def profile_name_fixer(input):
+    return f"{re.sub('_profile','', input)}_profile" if input else None
```

### Comparing `ofscraper-3.9.5/ofscraper/utils/hash.py` & `ofscraper-3.9.6/ofscraper/utils/hash.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/logs/classes.py` & `ofscraper-3.9.6/ofscraper/utils/logs/classes.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/logs/close.py` & `ofscraper-3.9.6/ofscraper/utils/logs/close.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/logs/helpers.py` & `ofscraper-3.9.6/ofscraper/utils/logs/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/logs/logger.py` & `ofscraper-3.9.6/ofscraper/utils/logs/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/logs/logs.py` & `ofscraper-3.9.6/ofscraper/utils/logs/logs.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/logs/other.py` & `ofscraper-3.9.6/ofscraper/utils/logs/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/logs/stdout.py` & `ofscraper-3.9.6/ofscraper/utils/logs/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/manager.py` & `ofscraper-3.9.6/ofscraper/utils/manager.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/me.py` & `ofscraper-3.9.6/ofscraper/utils/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/menu.py` & `ofscraper-3.9.6/ofscraper/utils/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 
-import ofscraper.actions.process as process_actions
 import ofscraper.models.selector as userselector
 import ofscraper.prompts.prompts as prompts
 import ofscraper.utils.actions as actions
 import ofscraper.utils.auth.file as auth_file
 import ofscraper.utils.config.menu as config_menu
 import ofscraper.utils.merge as merge
 import ofscraper.utils.profiles.manage as profiles_manage
 import ofscraper.utils.profiles.tools as profile_tools
 import ofscraper.utils.run as run
+from ofscraper.commands.add_select.add_selected import add_selected_areas
 
 log = logging.getLogger("shared")
 count = 0
 
 
 def update_count():
     global count
@@ -35,15 +35,15 @@
             if action_result_prompt == "quit":
                 return True
             elif action_result_prompt == "main":
                 continue
             else:
                 count > 0 and reset_menu_helper()
                 actions.set_scrape_paid()
-                functs = process_actions.add_selected_areas()
+                functs = add_selected_areas()
                 run.run_helper(*functs)
                 count = count + 1
         elif result_main_prompt == "auth":
             # Edit `auth.json` file
             auth_result_prompt = auth_file.edit_auth()
             if auth_result_prompt == "quit":
                 return True
```

### Comparing `ofscraper-3.9.5/ofscraper/utils/merge.py` & `ofscraper-3.9.6/ofscraper/utils/merge.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/paths/check.py` & `ofscraper-3.9.6/ofscraper/utils/paths/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/paths/common.py` & `ofscraper-3.9.6/ofscraper/utils/paths/common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/paths/manage.py` & `ofscraper-3.9.6/ofscraper/utils/paths/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/paths/paths.py` & `ofscraper-3.9.6/ofscraper/utils/paths/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/profiles/data.py` & `ofscraper-3.9.6/ofscraper/utils/profiles/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/profiles/manage.py` & `ofscraper-3.9.6/ofscraper/utils/profiles/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/progress.py` & `ofscraper-3.9.6/ofscraper/utils/progress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/run.py` & `ofscraper-3.9.6/ofscraper/utils/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/settings.py` & `ofscraper-3.9.6/ofscraper/utils/settings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/system/network.py` & `ofscraper-3.9.6/ofscraper/utils/system/network.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/system/system.py` & `ofscraper-3.9.6/ofscraper/utils/system/system.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.5/ofscraper/utils/text.py` & `ofscraper-3.9.6/ofscraper/utils/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 async def get_text(values):
     with ThreadPoolExecutor(
         max_workers=constants.getattr("MAX_TEXT_WORKER")
     ) as executor:
         asyncio.get_event_loop().set_default_executor(executor)
-        dupe = read_args.retriveArgs().dupe
+        dupe = read_args.retriveArgs().force_all or read_args.retriveArgs().force_model_uniqueme
         async with asyncio.TaskGroup() as tg:
             tasks = [
                 tg.create_task(get_text_process(value, dupe=dupe)) for value in values
             ]
             results = []
         for task in asyncio.as_completed(tasks):
             result = await task
```

### Comparing `ofscraper-3.9.5/pyproject.toml` & `ofscraper-3.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.9.5"
+version = "3.9.6"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.14"
```

### Comparing `ofscraper-3.9.5/PKG-INFO` & `ofscraper-3.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.9.5
+Version: 3.9.6
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ofscraper Version: 3.9.5 Summary: automatically
+Metadata-Version: 2.1 Name: ofscraper Version: 3.9.6 Summary: automatically
 scrape onlyfans Author: datawhores Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: pyinstaller Requires-Dist: aiofiles
 (>=23.2.1,<24.0.0) Requires-Dist: aiohttp (==3.9.4) Requires-Dist:
 aioprocessing (>=2.0.1,<3.0.0) Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: arrow (>=1.3.0,<2.0.0) Requires-Dist: browser-cookie3 (==0.19.1)
```

