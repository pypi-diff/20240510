# Comparing `tmp/browsergym_core-0.1.0rc7.tar.gz` & `tmp/browsergym_core-0.2.0.tar.gz`

## Comparing `browsergym_core-0.1.0rc7.tar` & `browsergym_core-0.2.0.tar`

### file list

```diff
@@ -1,70 +1,74 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/requirements.txt
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/__init__.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/chat.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/constants.py
--rw-r--r--   0        0        0    16748 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/env.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/observation.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/registration.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/spaces.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/task.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/action/base.py
--rw-r--r--   0        0        0    16206 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/action/functions.py
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/action/highlevel.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/action/parsers.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/action/python.py
--rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/action/utils.py
--rw-r--r--   0        0        0   133496 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/chat_files/assistant.png
--rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/chat_files/chatbox.html
--rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/javascript/frame_mark_elements.js
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/core/javascript/frame_unmark_elements.js
--rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/src/browsergym/utils/obs.py
--rw-r--r--   0        0        0    38868 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/test_actions_highlevel.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/test_actions_python.py
--rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/test_gym_envs.py
--rw-r--r--   0        0        0    18661 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/test_observation.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/utils.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/example.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/hover.html
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/long_page.html
--rw-r--r--   0        0        0    26054 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/screenshot.png
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/test_page.html
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/textbox.html
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/basic_iframe_site/basic_iframe.html
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/basic_iframe_site/basic_iframe_2.html
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/basic_iframe_site/inner-iframe.html
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/basic_iframe_site/outer-iframe.html
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/basic_shadow_dom_site/basic_shadow_dom.html
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/basic_shadow_dom_site/simple_shadow_dom.html
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/basic_shadow_iframe_site/basic_iframe.html
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/basic_shadow_iframe_site/basic_iframe_2.html
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/basic_shadow_iframe_site/inner-iframe.html
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/basic_shadow_iframe_site/outer-iframe.html
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/button_input.html
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/checkbox_input.html
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/color_picker_input.html
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/date_input.html
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/date_min_max_input.html
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/date_time_local_input.html
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/email_input.html
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/file_input.html
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/hidden_field_input.html
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/image_input.html
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/img_submit.gif
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/number_input.html
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/number_step_input.html
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/password_input.html
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/radio_input.html
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/range_input.html
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/reset_input.html
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/search_input.html
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/submit_input.html
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/submit_nn_input.html
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/telephone_input.html
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/text_input.html
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/time_input.html
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/url_input.html
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/tests/data/input_type/week_input.html
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/.gitignore
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/pyproject.toml
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 browsergym_core-0.1.0rc7/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/constants.py
+-rw-r--r--   0        0        0    21281 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/env.py
+-rw-r--r--   0        0        0    20773 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/observation.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/registration.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/spaces.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/action/__init__.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/action/base.py
+-rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/action/functions.py
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/action/highlevel.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/action/parsers.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/action/python.py
+-rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/action/utils.py
+-rw-r--r--   0        0        0   133496 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/chat_files/assistant.png
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/chat_files/chatbox.html
+-rw-r--r--   0        0        0    10578 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/chat_files/chatbox_modern.html
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/chat_files/img/send.svg
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/javascript/frame_mark_elements.js
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/core/javascript/frame_unmark_elements.js
+-rw-r--r--   0        0        0    18053 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/src/browsergym/utils/obs.py
+-rw-r--r--   0        0        0    39100 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/test_actions_highlevel.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/test_actions_python.py
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/test_gym_envs.py
+-rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/test_observation.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/example.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/hover.html
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/long_page.html
+-rw-r--r--   0        0        0    26054 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/screenshot.png
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/test_page.html
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/test_page_2.html
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/textbox.html
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/basic_iframe_site/basic_iframe.html
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/basic_iframe_site/basic_iframe_2.html
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/basic_iframe_site/inner-iframe.html
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/basic_iframe_site/outer-iframe.html
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/basic_shadow_dom_site/basic_shadow_dom.html
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/basic_shadow_dom_site/simple_shadow_dom.html
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/basic_shadow_iframe_site/basic_iframe.html
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/basic_shadow_iframe_site/basic_iframe_2.html
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/basic_shadow_iframe_site/inner-iframe.html
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/basic_shadow_iframe_site/outer-iframe.html
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/button_input.html
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/checkbox_input.html
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/color_picker_input.html
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/date_input.html
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/date_min_max_input.html
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/date_time_local_input.html
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/email_input.html
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/file_input.html
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/hidden_field_input.html
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/image_input.html
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/img_submit.gif
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/number_input.html
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/number_step_input.html
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/password_input.html
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/radio_input.html
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/range_input.html
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/reset_input.html
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/search_input.html
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/submit_input.html
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/submit_nn_input.html
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/telephone_input.html
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/text_input.html
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/time_input.html
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/url_input.html
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/tests/data/input_type/week_input.html
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/.gitignore
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 browsergym_core-0.2.0/PKG-INFO
```

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/__init__.py` & `browsergym_core-0.2.0/src/browsergym/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0rc7"
+__version__ = "0.2.0"
 
 import playwright.sync_api
 
 # we use a global playwright instance
 _PLAYWRIGHT = None
```

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/chat.py` & `browsergym_core-0.2.0/src/browsergym/core/chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 import base64
 from pathlib import Path
 from typing import Literal
 import logging
 import playwright.sync_api
 import re
+import time
 
 from importlib import resources
 
 from . import _get_global_playwright, chat_files
 
 
-CHATBOX_HTML_PATH = str(resources.files(chat_files).joinpath("chatbox.html"))
-ASSISTANT_IMG_PATH = str(resources.files(chat_files).joinpath("assistant.png"))
+CHATBOX_DIR = resources.files(chat_files)
 
 
 class Chat:
-    def __init__(self, headless: bool, chat_size=(500, 800), record_video_dir=None) -> None:
+    def __init__(
+        self, headless: bool, chat_size=(500, 800), record_video_dir=None, modern=True
+    ) -> None:
         self.messages = []
 
         # create a new browser, browser context and page for the chat
         pw: playwright.sync_api.Playwright = _get_global_playwright()
         self.browser = pw.chromium.launch(
             headless=headless, args=[f"--window-size={chat_size[0]},{chat_size[1]}"]
         )
         self.context = self.browser.new_context(
             no_viewport=True,
             record_video_dir=Path(record_video_dir) / "chat_video" if record_video_dir else None,
             record_video_size=dict(width=chat_size[0], height=chat_size[1]),
         )
         self.page = self.context.new_page()
+        self.recording_start_time = time.time() if record_video_dir else None
 
         # setup the chat page
         self.page.expose_function(
             "send_user_message", lambda msg: self.add_message(role="user", msg=msg, from_js=True)
         )
 
-        self.page.set_content(get_chatbox_html())
+        if modern:
+            self.page.set_content(get_chatbox_modern(CHATBOX_DIR))
+        else:
+            self.page.set_content(get_chatbox_classic(CHATBOX_DIR))
 
     def add_message(
         self, role: Literal["user", "assistant", "info"], msg: str, from_js: bool = False
     ):
 
         if role not in ("user", "assistant", "info"):
             raise ValueError(f"Invalid role: {role}")
         if role in ("user", "assistant"):
             self.messages.append({"role": role, "message": msg})
         if not from_js:
-            # change new lines to html
-            msg = msg.replace("\n", "<br>")
             self.page.evaluate(f"addChatMessage({repr(role)}, {repr(msg)});")
 
     def wait_for_user_message(self):
         logging.info("Waiting for message from user...")
         # reset flag
         self.page.evaluate("USER_MESSAGE_RECEIVED = false;")
         # wait for flag to be raised
@@ -59,20 +63,23 @@
         logging.info("Message received.")
 
     def close(self):
         self.context.close()
         self.browser.close()
 
 
-def get_chatbox_html() -> str:
-    with open(CHATBOX_HTML_PATH, "r") as file:
+def get_chatbox_modern(chatbox_dir) -> str:
+    with open(chatbox_dir / "chatbox_modern.html", "r") as file:
         chatbox_html = file.read()
 
-    with open(ASSISTANT_IMG_PATH, "rb") as f:
-        # image = Image.open(f)
+    return chatbox_html
+
+
+def get_chatbox_classic(chatbox_dir) -> str:
+    with open(chatbox_dir / "chatbox.html", "r") as file:
+        chatbox_html = file.read()
+    with open(chatbox_dir / "assistant.png", "rb") as f:
         image_base64 = base64.b64encode(f.read()).decode("utf-8")
 
-    # hard-code the assistant image in the HTML
     assistant_image_url = f"data:image/png;base64,{image_base64}"
     chatbox_html = re.sub("<ASSISTANT_IMAGE_URL>", assistant_image_url, chatbox_html)
-
     return chatbox_html
```

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/env.py` & `browsergym_core-0.2.0/src/browsergym/core/env.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,99 @@
 import copy
 import gymnasium as gym
 import logging
 import numpy as np
 import playwright.sync_api
 import time
+import re
 
 from abc import ABC
 from pathlib import Path
-from typing import Optional, Literal
+from typing import Optional
 
 from .chat import Chat
 from .task import AbstractBrowserTask
-from .spaces import Unicode, AnyDict
+from .spaces import Unicode, AnyDict, AnyBox
 from .constants import TEXT_MAX_LENGTH, BROWSERGYM_ID_ATTRIBUTE, EXTRACT_OBS_MAX_TRIES
 from .observation import (
     _pre_extract,
     _post_extract,
     extract_screenshot,
     extract_dom_snapshot,
+    extract_dom_extra_properties,
     extract_merged_axtree,
     extract_focused_element_bid,
+    MarkingError,
 )
 from .action.base import execute_python_code
 from .action.highlevel import HighLevelActionSet
 from .action.base import execute_python_code
 from . import _get_global_playwright
 
 
 class BrowserEnv(gym.Env, ABC):
+    """The main BrowserGym class, which encapsulates instruction-following Web browsing into a Gymnasium environment."""
+
     # gym metadata
     metadata = {"render_modes": None}
 
     def __init__(
         self,
+        # task-related arguments
         task_entrypoint: type[AbstractBrowserTask],
+        task_kwargs: dict = {},
+        viewport: Optional[dict] = None,  # will override the task's viewport
+        slow_mo: Optional[int] = None,  # will override the task's slow_mo
+        timeout: Optional[int] = None,  # will override the task's timeout
+        # interactive / debugging arguments
         headless: bool = True,
-        viewport: dict = {"width": 1280, "height": 720},
-        slow_mo: int = 1000,  # in milliseconds
-        timeout: int = 5000,
         wait_for_user_message: bool = False,
-        demo_mode: Literal["off", "default", "only_visible_elements"] = "off",
-        record_video_dir: str = None,
-        playwright_kwargs: dict = {},
+        resizeable_window: bool = False,
+        record_video_dir: Optional[str] = None,
+        pw_chromium_kwargs: dict = {},
+        pw_context_kwargs: dict = {},
+        # agent-related arguments
         action_mapping: Optional[callable] = HighLevelActionSet().to_python_code,
-        **task_kwargs,
     ):
+        """
+        Instantiate a ready to use BrowserEnv gym environment.
+
+        Args:
+            task_entrypoint: a callable that returns a new task object from a seed. Used for creating a new task during `reset()`.
+            task_kwargs: additional arguments passed to `task_entrypoint`.
+            viewport: desired viewport size. This will override the value defined by the task, which might change its behaviour and difficulty. Should only be set for debugging/testing.
+            slow_mo: desired slow_mo value for Playwright. This will override the value defined by the task, which might change its behaviour and difficulty. Should only be set for debugging/testing.
+            timeout: desired timeout value for Playwright. This will override the value defined by the task, which might change its behaviour and difficulty. Should only be set for debugging/testing.
+            headless: whether the browser should run in headless mode or not. This will affect the viewport size, which might change the behaviour and difficulty of the task. Headless mode should only be disabled for debugging/testing.
+            wait_for_user_message: whether the environment should pause and wait for a user message in the chat after a new message is sent by the agent. Useful for running agents in interactive mode.
+            resizeable_window: whether the browser window should be resizeable or not. This will affect the viewport size, which might change the behaviour and difficulty of the task. Should only be set for debugging/testing.
+            record_video_dir: if set, indicates a directory to which viewport videos will be recorded.
+            pw_chromium_kwargs: extra parameters for the playwright Browser. Should only be used for debugging/testing.
+            pw_context_kwargs: extra parameters for the playwright BrowserContext. Should only be used for debugging/testing.
+            action_mapping: if set, the environment will use this function to map every received action to executable Python code.
+
+        """
         super().__init__()
         self.task_entrypoint = task_entrypoint
-        self.task_kwargs = task_kwargs
-        self.headless = headless
+        self.task_kwargs = dict(**task_kwargs)
         self.viewport = viewport
         self.slow_mo = slow_mo
         self.timeout = timeout
+        self.headless = headless
         self.wait_for_user_message = wait_for_user_message
-        self.demo_mode = demo_mode
-        self.action_mapping = action_mapping
+        self.resizeable_window = resizeable_window
         self.record_video_dir = record_video_dir
+        self.pw_chromium_kwargs = pw_chromium_kwargs
+        self.pw_context_kwargs = pw_context_kwargs
+        self.action_mapping = action_mapping
 
         # task
         self.task = None
 
         # playwright
-        self.playwright_kwargs = playwright_kwargs
-        self.playwright_kwargs.setdefault("headless", self.headless)
-        self.playwright_kwargs.setdefault("slow_mo", self.slow_mo)
-        self.playwright_kwargs.setdefault(
-            "args", [f"--window-size={self.viewport['width']},{self.viewport['height']}"]
-        )
         self.browser: playwright.sync_api.Browser = None
         self.context: playwright.sync_api.BrowserContext = None
         self.page: playwright.sync_api.Page = None
         self.page_history: dict = {}
 
         # chat
         self.chat: Chat = None
@@ -89,22 +112,23 @@
                 # TODO: this is redundant with chat messages, to be removed
                 "goal": Unicode(min_length=0, max_length=TEXT_MAX_LENGTH),
                 "open_pages_urls": gym.spaces.Sequence(
                     Unicode(min_length=0, max_length=TEXT_MAX_LENGTH)
                 ),
                 "active_page_index": gym.spaces.Box(low=0, high=255, dtype=int),
                 "url": Unicode(min_length=0, max_length=TEXT_MAX_LENGTH),
-                "screenshot": gym.spaces.Box(
-                    0,
-                    255,
-                    shape=(viewport["height"], viewport["width"], 3),
+                "screenshot": AnyBox(
+                    low=0,
+                    high=255,
+                    shape=(-1, -1, 3),
                     dtype=np.uint8,
-                ),  # swapped axes (height first)
+                ),  # swapped axes (height, width, RGB)
                 "dom_object": AnyDict(),
                 "axtree_object": AnyDict(),
+                "extra_element_properties": AnyDict(),
                 "focused_element_bid": Unicode(min_length=0, max_length=TEXT_MAX_LENGTH),
                 "last_action": Unicode(min_length=0, max_length=TEXT_MAX_LENGTH),
                 "last_action_error": Unicode(min_length=0, max_length=TEXT_MAX_LENGTH),
                 "elapsed_time": gym.spaces.Box(low=0, high=np.inf, dtype=float),
             }
         )
 
@@ -120,47 +144,75 @@
             # close the browser context
             self.context.close()
             # close the browser
             self.browser.close()
             self.task = None
 
     def reset(self, seed=None, *args, **kwargs):
-        # we need the following line to seed self.np_random
         super().reset(seed=seed, *args, **kwargs)
+        self.np_random = None  # make sure all randomness is handled by the task
 
         if self.task:
             self.task.teardown()
             self.context.close()
             self.chat.close()
-        else:
-            pw: playwright.sync_api.Playwright = _get_global_playwright()
-            # important: change playwright's test id attribute from "data-testid" to "bid"
-            pw.selectors.set_test_id_attribute(BROWSERGYM_ID_ATTRIBUTE)
-            self.browser = pw.chromium.launch(**self.playwright_kwargs)
+            self.browser.close()
+
+        # create a new task
+        self.task = self.task_entrypoint(seed=seed, **self.task_kwargs)
+
+        def override_property(task, env, property):
+            """Extract property value from env if not None, otherwise from task."""
+            env_value = getattr(env, property)
+            task_value = getattr(task, property)
+            if env_value is None:
+                return task_value
+            else:
+                logging.warning(
+                    f"Overriding the task's {property} parameter ({repr(task_value)} => {repr(env_value)}). This might change the task's behaviour and difficulty."
+                )
+                return env_value
+
+        # fetch task's desired parameters for browser setup
+        viewport = override_property(self.task, self, "viewport")
+        slow_mo = override_property(self.task, self, "slow_mo")
+        timeout = override_property(self.task, self, "timeout")
+
+        # use the global Playwright instance
+        pw: playwright.sync_api.Playwright = _get_global_playwright()
+        # important: change playwright's test id attribute from "data-testid" to "bid"
+        pw.selectors.set_test_id_attribute(BROWSERGYM_ID_ATTRIBUTE)
+
+        # create a new browser
+        self.browser = pw.chromium.launch(
+            headless=self.headless,
+            slow_mo=slow_mo,
+            args=(
+                [f"--window-size={viewport['width']},{viewport['height']}"]
+                if self.resizeable_window
+                else None
+            ),
+            # will raise an Exception if above args are overriden
+            **self.pw_chromium_kwargs,
+        )
 
         # create a new browser context for pages
-        t_before = time.time()
         self.context = self.browser.new_context(
-            no_viewport=True,
+            no_viewport=True if self.resizeable_window else None,
+            viewport=viewport,
             record_video_dir=(
                 Path(self.record_video_dir) / "task_video" if self.record_video_dir else None
             ),
-            record_video_size=self.viewport,
+            record_video_size=viewport,
+            # will raise an Exception if above args are overriden
+            **self.pw_context_kwargs,
         )
-        # create the chat at the same time to make sure videos are synced
-        self.chat = Chat(
-            headless=self.playwright_kwargs["headless"],
-            chat_size=(500, max(self.viewport["height"], 800)),
-            record_video_dir=self.record_video_dir,
-        )
-        t_after = time.time()
-        recording_start_time = (t_before + t_after) / 2  # recording start time
 
         # set default timeout
-        self.context.set_default_timeout(self.timeout)
+        self.context.set_default_timeout(timeout)
 
         # hack: keep track of the active page with a javascript callback
         # there is no concept of active page in playwright
         # https://github.com/microsoft/playwright/issues/2603
         self.context.expose_binding(
             "browsergym_page_activated", lambda source: self._activate_page_from_js(source["page"])
         )
@@ -184,21 +236,27 @@
     if (document.visibilityState === "visible") {
         window.browsergym_page_activated();
     }
 }, {capture: true});
 """
         )
 
+        # create the chat
+        self.chat = Chat(
+            headless=self.headless,
+            chat_size=(500, max(viewport["height"], 800)),
+            record_video_dir=self.record_video_dir,
+        )
+
         # create a new page
         self.page = self.context.new_page()
+        recording_start_time = time.time()
 
-        # create and setup a new task
-        task_seed = self.np_random.integers(np.iinfo(np.int32).max + 1)
-        self.task = self.task_entrypoint(**self.task_kwargs)
-        goal, info = self.task.setup(seed=task_seed, page=self.page)
+        # setup the task
+        goal, task_info = self.task.setup(page=self.page)
 
         # initialize the chat
         self.chat.add_message(
             role="assistant",
             msg="Hi! I am your UI assistant, I can perform web tasks for you. What can I help you with?",
         )
         # if any, add the task's goal to the chat
@@ -220,36 +278,54 @@
 
         # if asked, wait for user message
         self._wait_for_user_message()
 
         # extract obs and info from environment
         obs = self._get_obs()
 
+        info = {}
+        info["task_info"] = task_info
+
+        # TODO this is a bit hacky, find a better solution to record videos
         if self.record_video_dir:
             info["recording_start_time"] = recording_start_time
+            info["recording_file"] = str(self.page.video.path())
+            info["chat"] = {
+                "recording_start_time": self.chat.recording_start_time,
+                "recording_file": str(self.chat.page.video.path()),
+            }
 
         return obs, info
 
     def step(self, action: str) -> tuple:
         self.last_action = action
 
+        info = {}
+        info["action_exec_start"] = time.time()
+        info["action_exec_timeout"] = 0
+
         # try to execute the action
         try:
             if self.action_mapping:
                 code = self.action_mapping(action)
             else:
                 code = action
             execute_python_code(
                 code,
                 self.page,
                 send_message_to_user=lambda text: self.chat.add_message(role="assistant", msg=text),
             )
             self.last_action_error = ""
         except Exception as e:
             self.last_action_error = f"{type(e).__name__}: {e}"
+            match = re.match("TimeoutError: Timeout ([0-9]+)ms exceeded.", self.last_action_error)
+            if match:
+                info["action_exec_timeout"] = float(match.groups()[0]) / 1000  # ms to sec
+
+        info["action_exec_stop"] = time.time()
 
         # wait a bit (for the JavaScript callback to set the active page)
         time.sleep(0.5)  # wait for JS events to be fired (half a second)
         self.context.cookies()  # trigger all waiting Playwright callbacks on the stack (hack, see https://playwright.dev/java/docs/multithreading)
 
         # wait for the network to idle before extracting the observation, reward etc.
         self._wait_dom_loaded()
@@ -258,15 +334,16 @@
         # perform a safety check
         self._active_page_check()
 
         # if asked, wait for user message
         self._wait_for_user_message()
 
         # extract reward, done, user_message, info (task-specific)
-        reward, done, user_message, info = self._task_validate()
+        reward, done, user_message, task_info = self._task_validate()
+        info["task_info"] = task_info
 
         # add any user message sent by the task to the chat
         if user_message:
             self.chat.add_message(role="user", msg=user_message)
 
         # extract observation (generic)
         obs = self._get_obs()
@@ -283,15 +360,15 @@
         prev_page_history = self.page_history.copy()
 
         # call validate
         reward, done, user_message, info = self.task.validate(self.page, self.chat.messages)
 
         # safety fix, in case validate() did mess up the active page and/or page history
         if prev_active_page != self.page or prev_page_history != self.page_history:
-            logging.warning(
+            logging.info(
                 "The active page and / or page history has changed during task.validate(). A recovery fix will be applied."
             )
             self.page = prev_active_page
             self.page_history = prev_page_history
 
         return reward, done, user_message, info
 
@@ -359,21 +436,24 @@
             try:
                 # pre-extraction, mark dom elements (set bid, set dynamic attributes like value and checked)
                 _pre_extract(self.page)
 
                 dom = extract_dom_snapshot(self.page)
                 axtree = extract_merged_axtree(self.page)
                 focused_element_bid = extract_focused_element_bid(self.page)
-            except playwright.sync_api.Error as e:
+                extra_properties = extract_dom_extra_properties(dom)
+            except (playwright.sync_api.Error, MarkingError) as e:
                 err_msg = str(e)
                 # try to add robustness to async events (detached / deleted frames)
                 if retries_left > 0 and (
                     "Frame was detached" in err_msg
                     or "Frame with the given frameId is not found" in err_msg
                     or "Execution context was destroyed" in err_msg
+                    or "Frame has been detached" in err_msg
+                    or "Cannot mark a child frame without a bid" in err_msg
                 ):
                     logging.warning(
                         f"An error occured while extracting the dom and axtree. Retrying ({retries_left}/{EXTRACT_OBS_MAX_TRIES} tries left).\n{repr(e)}"
                     )
                     # post-extract cleanup (aria-roledescription attribute)
                     _post_extract(self.page)
                     time.sleep(0.5)
@@ -398,14 +478,15 @@
             "goal": goal,  # TODO: redundant with chat messages, to be removed?
             "open_pages_urls": [page.url for page in self.context.pages],
             "active_page_index": np.asarray([self.context.pages.index(self.page)]),
             "url": self.page.url,
             "screenshot": extract_screenshot(self.page),
             "dom_object": dom,
             "axtree_object": axtree,
+            "extra_element_properties": extra_properties,
             "focused_element_bid": focused_element_bid,
             "last_action": self.last_action,
             "last_action_error": self.last_action_error,
             "elapsed_time": np.asarray([time.time() - self.start_time]),
         }
 
         return obs
```

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/spaces.py` & `browsergym_core-0.2.0/src/browsergym/core/spaces.py`

 * *Files 17% similar despite different names*

```diff
@@ -73,7 +73,46 @@
     def __repr__(self) -> str:
         """Gives a string representation of this space."""
         return f"AnyDict()"
 
     def __eq__(self, other: Any) -> bool:
         """Check whether ``other`` is equivalent to this instance."""
         return isinstance(other, AnyDict)
+
+
+class AnyBox(Space[NDArray[Any]]):
+    """A space representing an arbitrary dictionary object."""
+
+    def __init__(self, low, high, shape, dtype):
+        super().__init__(shape, dtype)
+        self.low = low
+        self.high = high
+
+    def contains(self, x: Any) -> bool:
+        """Return boolean specifying if x is a valid member of this space."""
+        if not isinstance(x, np.ndarray):
+            try:
+                x = np.asarray(x, dtype=self.dtype)
+            except (ValueError, TypeError):
+                return False
+
+        return bool(
+            np.can_cast(x.dtype, self.dtype)
+            and len(x.shape) == len(self.shape)
+            and all([dim in (xdim, -1) for xdim, dim in zip(x.shape, self.shape)])
+            and np.all(x >= self.low)
+            and np.all(x <= self.high)
+        )
+
+    def __repr__(self) -> str:
+        """Gives a string representation of this space."""
+        return f"AnyBox(low={repr(self.low)}, high={repr(self.high)}, shape={repr(self.shape)}, dtype={repr(self.dtype)})"
+
+    def __eq__(self, other: Any) -> bool:
+        """Check whether ``other`` is equivalent to this instance."""
+        return (
+            isinstance(other, AnyBox)
+            and self.low == other.low
+            and self.high == other.high
+            and self.shape == other.shape
+            and self.dtype == other.dtype
+        )
```

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/task.py` & `browsergym_core-0.2.0/src/browsergym/core/task.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,41 @@
+import numpy as np
 import playwright.sync_api
 
 from abc import ABC, abstractmethod
 from typing import Tuple
 
 
 class AbstractBrowserTask(ABC):
     """
     Abstract class for browsergym tasks.
 
     """
 
-    # gym metadata (default values, can be overloaded)
-    nondeterministic: bool = True
-
     @classmethod
     @abstractmethod
     def get_task_id(cls):
         pass
 
+    def __init__(self, seed: int) -> None:
+        # initiate a random number generator
+        self.random = np.random.RandomState(seed)
+
+        # task properties, will be used to set up the browsergym environment
+        # default values, can be overriden in children classes
+        self.viewport = {"width": 1280, "height": 720}
+        self.slow_mo = 1000  # ms
+        self.timeout = 5000  # ms
+
     @abstractmethod
-    def setup(self, seed: int, page: playwright.sync_api.Page) -> tuple[str, dict]:
+    def setup(self, page: playwright.sync_api.Page) -> tuple[str, dict]:
         """
         Set up everything needed to execute the task.
 
         Args:
-            seed: a seed for the task's randomness.
             page: the active playwright page.
 
         Returns:
             goal: str, goal of the task.
             info: dict, custom information from the task.
         """
 
@@ -67,25 +74,27 @@
 
 
 class OpenEndedTask(AbstractBrowserTask):
     @classmethod
     def get_task_id(cls):
         return "openended"
 
-    def __init__(self, start_url: str, goal: str = None) -> None:
+    def __init__(self, seed: int, start_url: str, goal: str = None) -> None:
         """
         Args:
+            seed: random seed.
             start_url: str, the url for the starting page.
             goal: str, the initial goal.
 
         """
+        super().__init__(seed)
         self.start_url = start_url
         self.goal = goal
 
-    def setup(self, seed: int, page: playwright.sync_api.Page) -> tuple[str, dict]:
+    def setup(self, page: playwright.sync_api.Page) -> tuple[str, dict]:
         page.goto(self.start_url, timeout=10000)
         return self.goal, {}
 
     def teardown(self) -> None:
         pass
 
     def validate(
```

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/action/base.py` & `browsergym_core-0.2.0/src/browsergym/core/action/base.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/action/functions.py` & `browsergym_core-0.2.0/src/browsergym/core/action/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # these are placeholders
 # all these symbols will be available in browsergym actions
 import playwright.sync_api
 from typing import Literal
 
 from .utils import (
     add_demo_mode_effects,
-    check_for_overlay,
     get_elem_by_bid,
     highlight_by_box,
     smooth_move_visual_cursor_to,
 )
 
 page: playwright.sync_api.Page = None
 send_message_to_user: callable = None
-demo_mode: Literal["off", "default", "only_visible_elements"] = "off"
+demo_mode: Literal["off", "default", "all_blue", "only_visible_elements"] = None
 
 """IMPORTANT
 The following primitives are meant to be included in the browsergym action using
 inspect.getsource().
 """
 
 
@@ -47,126 +46,120 @@
     """
     Fill out a form field. It focuses the element and triggers an input event with the entered text.
     It works for <input>, <textarea> and [contenteditable] elements.
 
     Examples:
         fill('237', 'example value')
         fill('45', "multi-line\\nexample")
-        fill('32-12', "example with \\"quotes\\"")
+        fill('a12', "example with \\"quotes\\"")
     """
-    elem = get_elem_by_bid(page, bid, demo_mode)
+    elem = get_elem_by_bid(page, bid, demo_mode != "off")
+    add_demo_mode_effects(page, elem, bid, demo_mode=demo_mode, move_cursor=False)
     if demo_mode != "off":
-        add_demo_mode_effects(page, elem, bid, demo_mode_type=demo_mode, move_cursor=False)
         elem.clear()
         delay = max(2000 / len(value), 10)
         elem.type(value, delay=delay)
     else:
-        elem.fill(value)
+        elem.fill(value, timeout=500)
 
 
 # https://playwright.dev/python/docs/api/class-locator#locator-check
 def check(bid: str):
     """
     Ensure a checkbox or radio element is checked.
 
     Examples:
         check('55')
     """
-    elem = get_elem_by_bid(page, bid, demo_mode)
-    if demo_mode != "off":
-        add_demo_mode_effects(page, elem, bid, demo_mode_type=demo_mode, move_cursor=True)
-    elem.check()
+    elem = get_elem_by_bid(page, bid, demo_mode != "off")
+    add_demo_mode_effects(page, elem, bid, demo_mode=demo_mode, move_cursor=True)
+    elem.check(timeout=500)
 
 
 # https://playwright.dev/python/docs/api/class-locator#locator-uncheck
 def uncheck(bid: str):
     """
     Ensure a checkbox or radio element is unchecked.
 
     Examples:
-        uncheck('65-5289')
+        uncheck('a5289')
     """
-    elem = get_elem_by_bid(page, bid, demo_mode)
-    if demo_mode != "off":
-        add_demo_mode_effects(page, elem, bid, demo_mode_type=demo_mode, move_cursor=True)
-    elem.uncheck()
+    elem = get_elem_by_bid(page, bid, demo_mode != "off")
+    add_demo_mode_effects(page, elem, bid, demo_mode=demo_mode, move_cursor=True)
+    elem.uncheck(timeout=500)
 
 
 # https://playwright.dev/docs/input#select-options
 def select_option(bid: str, options: str | list[str]):
     """
     Select one or multiple options in a <select> element. You can specify
     option value or label to select. Multiple options can be selected.
 
     Examples:
         select_option('48', "blue")
         select_option('48', ["red", "green", "blue"])
     """
-    elem = get_elem_by_bid(page, bid, demo_mode)
-    if demo_mode != "off":
-        add_demo_mode_effects(page, elem, bid, demo_mode_type=demo_mode, move_cursor=False)
-    elem.select_option(options)
+    elem = get_elem_by_bid(page, bid, demo_mode != "off")
+    add_demo_mode_effects(page, elem, bid, demo_mode=demo_mode, move_cursor=False)
+    elem.select_option(options, timeout=500)
 
 
 # https://playwright.dev/python/docs/api/class-locator#locator-click
 def click(
     bid: str,
     button: Literal["left", "middle", "right"] = "left",
     modifiers: list[Literal["Alt", "Control", "Meta", "Shift"]] = [],
 ):
     """
     Click an element.
 
     Examples:
         click('51')
-        click('69-2', button="right")
+        click('b22', button="right")
         click('48', button="middle", modifiers=["Shift"])
     """
-    elem = get_elem_by_bid(page, bid, demo_mode)
-    if demo_mode != "off":
-        add_demo_mode_effects(page, elem, bid, demo_mode_type=demo_mode, move_cursor=True)
-
+    elem = get_elem_by_bid(page, bid, demo_mode != "off")
+    add_demo_mode_effects(page, elem, bid, demo_mode=demo_mode, move_cursor=True)
     elem.click(button=button, modifiers=modifiers)
 
 
 # https://playwright.dev/python/docs/api/class-locator#locator-dblclick
 def dblclick(
     bid: str,
     button: Literal["left", "middle", "right"] = "left",
     modifiers: list[Literal["Alt", "Control", "Meta", "Shift"]] = [],
 ):
     """
     Double click an element.
 
     Examples:
         dblclick('12')
-        dblclick('289-5-42', button="right")
+        dblclick('ca42', button="right")
         dblclick('178', button="middle", modifiers=["Shift"])
     """
-    elem = get_elem_by_bid(page, bid, demo_mode)
-    if demo_mode != "off":
-        add_demo_mode_effects(page, elem, bid, demo_mode_type=demo_mode, move_cursor=True)
-    elem.dblclick(button=button, modifiers=modifiers, force=True)
+    elem = get_elem_by_bid(page, bid, demo_mode != "off")
+    add_demo_mode_effects(page, elem, bid, demo_mode=demo_mode, move_cursor=True)
+    elem.dblclick(button=button, modifiers=modifiers, timeout=500)
 
 
 # https://playwright.dev/python/docs/api/class-locator#locator-hover
 def hover(bid: str):
     """
     Hover over an element.
 
     Examples:
-        hover('12-8')
+        hover('b8')
     """
-    elem = get_elem_by_bid(page, bid, demo_mode)
+    elem = get_elem_by_bid(page, bid, demo_mode != "off")
     if demo_mode != "off":
         box = elem.bounding_box()
         if box:
             center_x, center_y = box["x"] + box["width"] / 2, box["y"] + box["height"] / 2
             smooth_move_visual_cursor_to(page, center_x, center_y)
-    elem.hover()
+    elem.hover(timeout=500)
 
 
 # https://playwright.dev/python/docs/input#keys-and-shortcuts
 def press(bid: str, key_comb: str):
     """
     Focus the matching element and press a combination of keys. It accepts
     the logical key names that are emitted in the keyboardEvent.key property
@@ -175,78 +168,73 @@
     ArrowRight, ArrowUp, F1 - F12, Digit0 - Digit9, KeyA - KeyZ, etc. You can
     alternatively specify a single character you'd like to produce such as "a"
     or "#". Following modification shortcuts are also supported: Shift, Control,
     Alt, Meta.
 
     Examples:
         press('88', 'Backspace')
-        press('48-6', 'Control+a')
-        press('48-6', 'Meta+Shift+t')
+        press('a26', 'Control+a')
+        press('a61', 'Meta+Shift+t')
     """
-    elem = get_elem_by_bid(page, bid, demo_mode)
-    if demo_mode != "off":
-        add_demo_mode_effects(page, elem, bid, demo_mode_type=demo_mode, move_cursor=False)
-    elem.press(key_comb)
+    elem = get_elem_by_bid(page, bid, demo_mode != "off")
+    add_demo_mode_effects(page, elem, bid, demo_mode=demo_mode, move_cursor=False)
+    elem.press(key_comb, timeout=500)
 
 
 # https://playwright.dev/python/docs/api/class-locator#locator-focus
 def focus(bid: str):
     """
     Focus the matching element.
 
     Examples:
-        focus('87-455')
+        focus('b455')
     """
-    elem = get_elem_by_bid(page, bid, demo_mode)
-    if demo_mode != "off":
-        add_demo_mode_effects(page, elem, bid, demo_mode_type=demo_mode, move_cursor=False)
-    elem.focus()
+    elem = get_elem_by_bid(page, bid, demo_mode != "off")
+    add_demo_mode_effects(page, elem, bid, demo_mode=demo_mode, move_cursor=False)
+    elem.focus(timeout=500)
 
 
 # https://playwright.dev/python/docs/api/class-locator#locator-clear
 def clear(bid: str):
     """
     Clear the input field.
 
     Examples:
         clear('996')
     """
-    elem = get_elem_by_bid(page, bid, demo_mode)
-    if demo_mode != "off":
-        add_demo_mode_effects(page, elem, bid, demo_mode_type=demo_mode, move_cursor=False)
-    elem.clear()
+    elem = get_elem_by_bid(page, bid, demo_mode != "off")
+    add_demo_mode_effects(page, elem, bid, demo_mode=demo_mode, move_cursor=False)
+    elem.clear(timeout=500)
 
 
 # https://playwright.dev/python/docs/input#drag-and-drop
 def drag_and_drop(from_bid: str, to_bid: str):
     """
     Perform a drag & drop. Hover the element that will be dragged. Press
     left mouse button. Move mouse to the element that will receive the
     drop. Release left mouse button.
 
     Examples:
         drag_and_drop('56', '498')
     """
-    from_elem = get_elem_by_bid(page, from_bid, demo_mode)
-    if demo_mode != "off":
-        add_demo_mode_effects(page, from_elem, from_bid, move_cursor=True)
-    from_elem.hover()
+    from_elem = get_elem_by_bid(page, from_bid, demo_mode != "off")
+    add_demo_mode_effects(page, from_elem, from_bid, demo_mode=demo_mode, move_cursor=True)
+    from_elem.hover(timeout=500)
     page.mouse.down()
 
-    to_elem = get_elem_by_bid(page, to_bid, demo_mode)
-    if demo_mode != "off":
-        add_demo_mode_effects(page, to_elem, to_bid, move_cursor=True)
-    to_elem.hover()
+    to_elem = get_elem_by_bid(page, to_bid, demo_mode != "off")
+    add_demo_mode_effects(page, to_elem, to_bid, demo_mode=demo_mode, move_cursor=True)
+    to_elem.hover(timeout=500)
     page.mouse.up()
 
 
 # https://playwright.dev/python/docs/api/class-mouse#mouse-wheel
 def scroll(delta_x: float, delta_y: float):
     """
-    Scroll horizontally and vertically. Amounts in pixels. Dispatches a wheel event.
+    Scroll horizontally and vertically. Amounts in pixels, positive for right or down scrolling, negative for left or up scrolling. Dispatches a wheel event.
 
     Examples:
         scroll(0, 200)
         scroll(-50.2, -100.5)
     """
     page.mouse.wheel(delta_x, delta_y)
 
@@ -366,14 +354,15 @@
     as "a" or "#". Following modification shortcuts are also supported:
     Shift, Control, Alt, Meta.
 
     Examples:
         keyboard_press('Backspace')
         keyboard_press('Control+a')
         keyboard_press('Meta+Shift+t')
+        page.keyboard.press("PageDown")
     """
     page.keyboard.press(key)
 
 
 # https://playwright.dev/python/docs/api/class-keyboard#keyboard-up
 def keyboard_up(key: str):
     """
@@ -517,7 +506,52 @@
     Examples:
         tab_focus(2)
     """
     global page  # set the focused page as the active page
     page = page.context.pages[index]
     # trigger the callback that sets this page as active in browsergym
     page.locate("html").dispatch_event("pageshow")
+
+
+# https://playwright.dev/python/docs/input#upload-files
+def upload_file(bid: str, file: str | list[str]):
+    """
+    Click an element and wait for a "filechooser" event, then select one
+    or multiple input files for upload. Relative file paths are resolved
+    relative to the current working directory. An empty list clears the
+    selected files.
+
+    Examples:
+        upload_file("572", "my_receipt.pdf")
+        upload_file("63", ["/home/bob/Documents/image.jpg", "/home/bob/Documents/file.zip"])
+    """
+    elem = get_elem_by_bid(page, bid, demo_mode != "off")
+    add_demo_mode_effects(page, elem, bid, demo_mode=demo_mode, move_cursor=True)
+
+    with page.expect_file_chooser() as fc_info:
+        elem.click(timeout=500)
+
+    file_chooser = fc_info.value
+    file_chooser.set_files(file)
+
+
+# https://playwright.dev/python/docs/input#upload-files
+def mouse_upload_file(x: float, y: float, file: str | list[str]):
+    """
+    Click a location and wait for a "filechooser" event, then select one
+    or multiple input files for upload. Relative file paths are resolved
+    relative to the current working directory. An empty list clears the
+    selected files.
+
+    Examples:
+        mouse_upload_file(132.1, 547, "my_receipt.pdf")
+        mouse_upload_file(328, 812, ["/home/bob/Documents/image.jpg", "/home/bob/Documents/file.zip"])
+    """
+    if demo_mode != "off":
+        smooth_move_visual_cursor_to(page, x, y)
+        highlight_by_box(page, {"x": x, "y": y, "width": 1, "height": 1})
+
+    with page.expect_file_chooser() as fc_info:
+        page.mouse.click(x, y)
+
+    file_chooser = fc_info.value
+    file_chooser.set_files(file)
```

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/action/highlevel.py` & `browsergym_core-0.2.0/src/browsergym/core/action/highlevel.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,21 +16,23 @@
     click,
     dblclick,
     hover,
     press,
     focus,
     clear,
     drag_and_drop,
+    upload_file,
     scroll,
     mouse_move,
     mouse_up,
     mouse_down,
     mouse_click,
     mouse_dblclick,
     mouse_drag_and_drop,
+    mouse_upload_file,
     keyboard_down,
     keyboard_up,
     keyboard_press,
     keyboard_type,
     keyboard_insert_text,
     tab_close,
     tab_focus,
@@ -54,24 +56,26 @@
     click,
     dblclick,
     hover,
     press,
     focus,
     clear,
     drag_and_drop,
+    upload_file,
 ]
 
 COORD_ACTIONS = [
     scroll,
     mouse_move,
     mouse_up,
     mouse_down,
     mouse_click,
     mouse_dblclick,
     mouse_drag_and_drop,
+    mouse_upload_file,
     keyboard_down,
     keyboard_up,
     keyboard_press,
     keyboard_type,
     keyboard_insert_text,
 ]
 
@@ -102,15 +106,15 @@
             "chat",
             "bid",
             "nav",
             "tab",
         ],
         custom_actions: Optional[list[callable]] = None,
         multiaction: bool = True,
-        demo_mode: Literal["off", "default", "only_visible_elements"] = "off",
+        demo_mode: Literal["off", "default", "all_blue", "only_visible_elements"] = "off",
         strict: bool = False,
     ):
         super().__init__(strict)
         self.multiaction = multiaction
         self.demo_mode = demo_mode
 
         if not subsets:
@@ -205,45 +209,44 @@
             self.action_set[func.__name__] = HighLevelAction(
                 # entrypoint=func,
                 signature=signature,
                 description=description,
                 examples=examples,
             )
 
-    def example_action(self, abstract: bool) -> str:
+    def example_action(self, abstract: bool, max_examples: int = 3) -> str:
         """
         Returns an example action as a string.
         """
         if abstract:
             if self.multiaction:
                 return """\
 One or several actions, separated by new lines."""
             else:
                 return """\
 One single action to be executed. You can only use one action at a time."""
         else:
             picked_examples = []
 
             # use fill and click examples if action is present
-            if "fill" in self.action_set:
-                picked_examples.extend(self.action_set["fill"].examples)
-            if "click" in self.action_set:
-                picked_examples.extend(self.action_set["click"].examples)
+            for action_name in ["fill", "click", "mouse_click", "keyboard_type"]:
+                if action_name in self.action_set:
+                    picked_examples.extend(self.action_set[action_name].examples)
 
-            # last resort, use all examples
+            # last resort, use all action examples
             if not picked_examples:
                 for _, action in self.action_set.items():
-                    all_examples += action.examples
+                    picked_examples += action.examples
 
             # shuffle examples
             rng = random.Random(1)
             rng.shuffle(picked_examples)
 
             if self.multiaction:
-                return "\n".join(picked_examples[:3])
+                return "\n".join(picked_examples[:max_examples])
             else:
                 return picked_examples[0]
 
     def describe(self, with_long_description: bool = True, with_examples: bool = True):
         """
         Returns a textual description of this action space.
         """
```

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/action/parsers.py` & `browsergym_core-0.2.0/src/browsergym/core/action/parsers.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/action/python.py` & `browsergym_core-0.2.0/src/browsergym/core/action/python.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 ```
 frame = page.frame_locator(".result-frame")
 button = frame.get_by_text("Submit")
 button.click()
 ```
 Here is another example:
 ```
-frame = page.get_by_test_id("35").frame_locator(":scope")
-frame.get_by_test_id("35-776").click()
+frame = page.get_by_test_id("a").frame_locator(":scope")
+frame.get_by_test_id("a776").click()
 ```
 Note that Playwright's `get_by_test_id()` method is configured to use the `bid` attribute to locate HTML elements,
 instead of the default `data-testid`. Also, Playwright's locators can not traverse iframes, so you have to locate
 parent iframes first in order to locate an element in an iframe. The `bid` attribute contains all the information
-required to recursively locate an element. For example, an element with `bid="23-557-2"` can be retrieved as follows:
+required to recursively locate an element. For example, an element with `bid="ac2"` can be retrieved as follows:
 ```
-frame = page.get_by_test_id("23").frame_locator(":scope")
-frame = frame.get_by_test_id("23-557").frame_locator(":scope")
-elem = frame.get_by_test_id("23-557-2")
+frame = page.get_by_test_id("a").frame_locator(":scope")
+frame = frame.get_by_test_id("ac").frame_locator(":scope")
+elem = frame.get_by_test_id("ac2")
 ```
 """
         else:
             description += f"""\
 
 """
         if with_examples:
@@ -73,18 +73,18 @@
         Returns an example action as a string.
         """
         if abstract:
             return """\
 One single bloc of Python code. Do not include any explanation, only valid Python code."""
         else:
             return """\
-frame = page.get_by_test_id("23").frame_locator(":scope")
-frame = page.get_by_test_id("23-557").frame_locator(":scope")
-frame.get_by_test_id("23-557-2").fill("Hello world!")
-frame.get_by_test_id("23-557-3").click()
+frame = page.get_by_test_id("b").frame_locator(":scope")
+frame = page.get_by_test_id("ba").frame_locator(":scope")
+frame.get_by_test_id("ba2").fill("Hello world!")
+frame.get_by_test_id("ba3").click()
 """
 
     def to_python_code(self, action):
         """
         Converts the given code action string to browsergym-compatible playwright code.
 
         Args:
```

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/action/utils.py` & `browsergym_core-0.2.0/src/browsergym/core/action/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import playwright.sync_api
+from typing import Literal
 
 
 def get_elem_by_bid(
     page: playwright.sync_api.Page, bid: str, scroll_into_view: bool = False
 ) -> playwright.sync_api.Locator:
     """
     Parse the given bid to sequentially locate every nested frame leading to the bid, then
-    locate the bid element. Bids are expected to take the form "XX-...-YY-ZZ", which means
-    the element ZZ is located inside frame YY, which is located inside frame ..., which is
-    located inside frame XX, which is located inside the page's main frame.
+    locate the bid element. Bids are expected to take the form "abb123", which means
+    the element abb123 is located inside frame abb, which is located inside frame ab, which is
+    located inside frame a, which is located inside the page's main frame.
 
     Args:
         bid: the browsergym id (playwright testid) of the page element.
         scroll_into_view: try to scroll element into view, unless it is completely visible.
 
     Returns:
         Playwright element.
@@ -20,41 +21,50 @@
     """
     if not isinstance(bid, str):
         raise ValueError(f"expected a string, got {repr(bid)}")
 
     current_frame = page
 
     # dive into each nested frame, to the frame where the element is located
-    for i in range(bid.count("-")):
-        frame_bid = "-".join(bid.split("-")[: i + 1])
+    i = 0
+    while bid[i:] and not bid[i:].isnumeric():
+        i += 1
+        frame_bid = bid[:i]  # bid of the next frame to select
         frame_elem = current_frame.get_by_test_id(frame_bid)
+        if not frame_elem.count():
+            raise ValueError(f'could not find element with bid "{frame_bid}"')
         if scroll_into_view:
-            frame_elem.scroll_into_view_if_needed()
+            frame_elem.scroll_into_view_if_needed(timeout=500)
         current_frame = frame_elem.frame_locator(":scope")
 
     # finally, we should have selected the frame where the target element is
     elem = current_frame.get_by_test_id(bid)
+    if not elem.count():
+        raise ValueError(f'Could not find element with bid "{bid}".')
     if scroll_into_view:
-        elem.scroll_into_view_if_needed()
+        elem.scroll_into_view_if_needed(timeout=500)
     return elem
 
 
-def highlight_by_box(page: playwright.sync_api.Page, box: dict, is_visible: bool = True):
+def highlight_by_box(
+    page: playwright.sync_api.Page, box: dict, color: Literal["blue", "red"] = "blue"
+):
     """Highlights the target element based on its bounding box attributes."""
 
+    assert color in ("blue", "red")
+
     if box:
         left, top, width, height = box["x"], box["y"], box["width"], box["height"]
-        color = "blue" if is_visible else "red"
         page.evaluate(
             f"""\
 const overlay = document.createElement('div');
 document.body.appendChild(overlay);
 overlay.setAttribute('style', `
     all: initial;
-    position: absolute;
+    position: fixed;
     border: 2px solid transparent;  /* Start with transparent border */
     borderRadius: 10px;  /* Add rounded corners */
     boxShadow: 0 0 0px {color};  /* Initial boxShadow with 0px spread */
     left: {left - 2}px;  /* Adjust left position to accommodate initial shadow spread */
     top: {top - 2}px;  /* Adjust top position likewise */
     width: {width}px;
     height: {height}px;
@@ -107,15 +117,15 @@
             cursor.innerHTML = `
                 <svg width="50px" height="50px" viewBox="213 106 713 706" fill="none" xmlns="http://www.w3.org/2000/svg">
                 <path d="M213.333 106.667L426.667 853.333 512 512 853.333 426.667 213.333 106.667z" fill="blue"/>
                 </svg>
 `;
             cursor.setAttribute('style', `
                 all: initial;
-                position: absolute;
+                position: fixed;
                 opacity: 0.7; /* Slightly transparent */
                 z-index: 2147483647; /* Maximum value */
                 pointer-events: none; /* Ensures the SVG doesn't interfere with page interactions */
             `);
 
             // Calculate center position within the viewport
             const centerX = window.innerWidth / 2;
@@ -184,56 +194,78 @@
     }""",
         [x, y, speed],
     )
     page.wait_for_timeout(movement_time)
 
 
 def check_for_overlay(
-    page: playwright.sync_api.Page,
-    bid: str,
-    element: playwright.sync_api.ElementHandle,
+    page: playwright.sync_api.Page, bid: str, element: playwright.sync_api.ElementHandle, box: dict
 ):
-    """Checks in a given element is the topmost element at its center position by default.
+    if not element:
+        return False
+
+    visibility = element.get_attribute("browsergym_visibility_ratio")
+    if visibility is not None:
+        return float(visibility) >= 0.5
+
+    """Checks if a given element is the topmost element at its center position by default.
     If check_corners is True, it checks if any of the corners is visible."""
-    if element:
-        box = element.bounding_box()
-        if box:
-            # corners
-            points_to_check = [
-                (box["x"], box["y"]),
-                (box["x"] + box["width"], box["y"]),
-                (box["x"], box["y"] + box["height"]),
-                (box["x"] + box["width"], box["y"] + box["height"]),
-            ]
-
-            for x, y in points_to_check:
-                # Execute JavaScript to find the topmost element at the point.
-                top_element = page.evaluate(
-                    f"""() => {{
-                    const el = document.elementFromPoint({x}, {y});
-                    return el ? el.outerHTML : '';
-                }}"""
-                )
-
-                # Check if the topmost element is the element we're interested in.
-                if top_element and bid in top_element:
-                    return True
+    if box:
+        # corners
+        points_to_check = [
+            (box["x"], box["y"]),
+            (box["x"] + box["width"], box["y"]),
+            (box["x"], box["y"] + box["height"]),
+            (box["x"] + box["width"], box["y"] + box["height"]),
+        ]
+
+        for x, y in points_to_check:
+            # Execute JavaScript to find the topmost element at the point.
+            top_element = page.evaluate(
+                f"""() => {{
+                const el = document.elementFromPoint({x}, {y});
+                return el ? el.outerHTML : '';
+            }}"""
+            )
+
+            # Check if the topmost element is the element we're interested in.
+            if top_element and bid in top_element:
+                return True
+
     return False
 
 
 def add_demo_mode_effects(
     page: playwright.sync_api.Page,
     elem: playwright.sync_api.ElementHandle,
     bid: str,
+    demo_mode: Literal["off", "default", "all_blue", "only_visible_elements"],
     move_cursor: bool = True,
-    demo_mode_type: str = "default",
 ):
+    if demo_mode == "off":
+        return
+
     """Adds visual effects to the target element"""
     box = elem.bounding_box()
+    # box = extract_bounds_cdp(page, bid)
     if box:
         center_x, center_y = box["x"] + box["width"] / 2, box["y"] + box["height"] / 2
-        is_top_element = check_for_overlay(page, bid, elem)
+        is_top_element = check_for_overlay(page, bid, elem, box)
 
-        if is_top_element or demo_mode_type == "default":
-            if move_cursor:
-                smooth_move_visual_cursor_to(page, center_x, center_y)
-            highlight_by_box(page, box, is_visible=is_top_element)
+        if demo_mode == "only_visible_elements":
+            if not is_top_element:
+                return
+            else:
+                color = "blue"
+
+        elif demo_mode == "default":
+            if is_top_element:
+                color = "blue"
+            else:
+                color = "red"
+
+        elif demo_mode == "all_blue":
+            color = "blue"
+
+        if move_cursor:
+            smooth_move_visual_cursor_to(page, center_x, center_y)
+        highlight_by_box(page, box, color=color)
```

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/chat_files/assistant.png` & `browsergym_core-0.2.0/src/browsergym/core/chat_files/assistant.png`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/chat_files/chatbox.html` & `browsergym_core-0.2.0/src/browsergym/core/chat_files/chatbox.html`

 * *Files 4% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
 <body>
 
 
 
     <div class="chat-container">
         <div class="chat-header">
-            <h2>UI Assistant</h2>
+            <h2>BrowserGym</h2>
         </div>
         <div class="chat-body" id="chatBody"></div>
         <div class="chat-debug" id="chatDebug"></div>
         <div class="chat-input-area">
             <form id="chatForm">
                 <textarea class="input-box" rows="2" id="inputBox"></textarea>
                 <input type="submit" class="submit-button" value="Send">
@@ -147,22 +147,31 @@
 
     <script>
 
         const assistant_image_data = "<ASSISTANT_IMAGE_URL>";
 
         var USER_MESSAGE_RECEIVED = false;
 
+        function escapeHtml(unsafe) {
+            return unsafe
+                .replace(/&/g, "&amp;")
+                .replace(/</g, "&lt;")
+                .replace(/>/g, "&gt;")
+                .replace(/"/g, "&quot;")
+                .replace(/'/g, "&#039;");
+        }
+
         function addChatMessage(role, msg) {
             const chatBody = document.getElementById('chatBody');
             const chatDebug = document.getElementById('chatDebug');
             const msgContainer = document.createElement('div');
             msgContainer.className = 'message';
 
             const text = document.createElement('p');
-            text.innerHTML = msg;
+            text.innerHTML = escapeHtml(msg);
 
             const assistant_img = document.createElement('img');
             assistant_img.src = assistant_image_data;
             assistant_img.alt = 'Assistant';
             assistant_img.className = 'assistant-image';
```

#### html2text {}

```diff
@@ -1,2 +1,2 @@
-********** UUII AAssssiissttaanntt **********
+********** BBrroowwsseerrGGyymm **********
 [Send]
```

### Comparing `browsergym_core-0.1.0rc7/src/browsergym/core/javascript/frame_unmark_elements.js` & `browsergym_core-0.2.0/src/browsergym/core/javascript/frame_unmark_elements.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -19,22 +19,21 @@
         }
         i++;
         // Hack: remove custom data stored inside the aria-roledescription tag
         //  - elem_global_id: global browsergym identifier
         if (elem.hasAttribute("aria-roledescription")) {
             let content = elem.getAttribute("aria-roledescription");
             // TODO: handle more data if needed
-            let n_data_items = 8; // bid, bbox_left, bbox_top, center_x, center_y, bbox_right, bbox_bottom, is_in_viewport
+            let n_data_items = 1; // bid
             let post_data_index = 0;
             for (let j = 0; j < n_data_items; j++) {
                 post_data_index = content.indexOf("_", post_data_index) + 1;
             }
             original_content = content.substring(post_data_index);
             if (original_content) {
                 elem.setAttribute("aria-roledescription", original_content);
             } else {
                 elem.removeAttribute("aria-roledescription");
             }
-
         }
     }
 }
```

### Comparing `browsergym_core-0.1.0rc7/tests/test_actions_highlevel.py` & `browsergym_core-0.2.0/tests/test_actions_highlevel.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 
 def test_valid_action():
     action_set = HighLevelActionSet()
 
     env = gym.make(
         "browsergym/openended",
-        start_url=CHECKBOX_URL,
+        task_kwargs={"start_url": CHECKBOX_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
 
     def get_checkbox_elem(obs):
@@ -284,15 +284,15 @@
 
 
 def test_invalid_action():
     action_set = HighLevelActionSet()
 
     env = gym.make(
         "browsergym/openended",
-        start_url=CHECKBOX_URL,
+        task_kwargs={"start_url": CHECKBOX_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
     obs, info = env.reset()
 
@@ -300,15 +300,15 @@
     action = f"""\
 click("INVALID_BID")
 """
 
     obs, reward, term, trunc, info = env.step(action)
 
     # error
-    assert "TimeoutError" in obs["last_action_error"]
+    assert "ValueError" in obs["last_action_error"]
 
     # invalid bid value type
     action = f"""\
 click(None)
 """
 
     obs, reward, term, trunc, info = env.step(action)
@@ -446,15 +446,15 @@
 
 
 def test_click_through_frames():
     action_set = HighLevelActionSet()
 
     env = gym.make(
         "browsergym/openended",
-        start_url=MULTI_IFRAME_URL,
+        task_kwargs={"start_url": MULTI_IFRAME_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
 
     obs, info = env.reset()
@@ -486,15 +486,15 @@
 
 
 def test_fill_through_iframe():
     action_set = HighLevelActionSet()
 
     env = gym.make(
         "browsergym/openended",
-        start_url=MULTI_IFRAME_URL,
+        task_kwargs={"start_url": MULTI_IFRAME_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
 
     obs, info = env.reset()
@@ -530,15 +530,15 @@
 
 
 def test_click():
     action_set = HighLevelActionSet()
 
     env = gym.make(
         "browsergym/openended",
-        start_url=CHECKBOX_URL,
+        task_kwargs={"start_url": CHECKBOX_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
 
     def get_checkbox_elem(obs):
@@ -602,15 +602,15 @@
 
 
 def test_hover():
     action_set = HighLevelActionSet(subsets=["bid", "coord"])
 
     env = gym.make(
         "browsergym/openended",
-        start_url=HOVER_URL,
+        task_kwargs={"start_url": HOVER_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
 
     def get_button_elem(obs):
@@ -647,15 +647,15 @@
     env.close()
 
 
 def test_fill_type_press():
     action_set = HighLevelActionSet(subsets=["bid", "coord"])
     env = gym.make(
         "browsergym/openended",
-        start_url=TEXT_INPUT_URL,
+        task_kwargs={"start_url": TEXT_INPUT_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
 
     def get_fname_lname_elems(obs):
@@ -802,15 +802,15 @@
 
 # copy/paste text using a sequence of keyboard_press actions
 def test_key_press():
     action_set = HighLevelActionSet(subsets=["bid", "coord"])
 
     env = gym.make(
         "browsergym/openended",
-        start_url=TEXT_INPUT_URL,
+        task_kwargs={"start_url": TEXT_INPUT_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
 
     obs, info = env.reset()
@@ -844,15 +844,15 @@
 
 def test_goto():
     url1 = URL_INPUT_URL
     url2 = TEXT_INPUT_URL
 
     env = gym.make(
         "browsergym/openended",
-        start_url=url1,
+        task_kwargs={"start_url": url1},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
     )
 
     obs, info = env.reset()
 
@@ -892,34 +892,30 @@
 
 
 def test_scroll():
     action_set = HighLevelActionSet(subsets=["coord"])
 
     env = gym.make(
         "browsergym/openended",
-        start_url=LONG_PAGE_URL,
-        headless=False,
+        task_kwargs={"start_url": LONG_PAGE_URL},
+        headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
 
     def extract_coords_from_elem(elem):
-        x, y = map(
-            float,
-            re.search(
-                r"\(([-+]?[0-9\.]+),[\s]*([-+]?[0-9\.]+)\)",
-                elem.get("center"),
-            ).groups(),
-        )
-        return x, y
+        return ast.literal_eval(elem.get("center"))
 
     def get_top_bottom_elems(obs):
         soup = bs4.BeautifulSoup(
-            flatten_dom_to_str(obs["dom_object"], with_center_coords=True), "lxml"
+            flatten_dom_to_str(
+                obs["dom_object"], obs["extra_element_properties"], with_center_coords=True
+            ),
+            "lxml",
         )
         top = soup.find("input", attrs={"type": "checkbox", "id": "top"})
         bottom = soup.find("input", attrs={"type": "checkbox", "id": "bottom"})
         return top, bottom
 
     obs, info = env.reset()
     top, bottom = get_top_bottom_elems(obs)
@@ -1005,15 +1001,15 @@
 
     env.close()
 
 
 # def test_meta_action():
 #     env = BrowserEnv(
 #         task_entrypoint=OpenEndedTask,
-#         start_url=TEXT_INPUT_URL,
+#         task_kwargs={"start_url": TEXT_INPUT_URL},
 #         headless=__HEADLESS__,
 #     )
 #     obs, info = env.reset()
 
 #     soup = bs4.BeautifulSoup(obs["html"], "lxml")
 #     fname = soup.find("input", attrs={"id": "fname"})
 #     lname = soup.find("input", attrs={"id": "lname"})
@@ -1139,15 +1135,15 @@
 #     # assert len(list_li) > 0
 #     # assert list_li[0].text == "Kahului, HI - Island of Maui, (OGG)"
 
 
 # def test_clear_success():
 #     env = BrowserEnv(
 #         task_entrypoint=OpenEndedTask,
-#         start_url=TEXT_INPUT_URL,
+#         task_kwargs={"start_url": TEXT_INPUT_URL},
 #         headless=__HEADLESS__,
 #     )
 #     obs, info = env.reset()
 
 #     fname_element = env.driver.find_element(By.CSS_SELECTOR, value="input[id='fname']")
 #     fname_element.send_keys("Christian")
 
@@ -1209,15 +1205,15 @@
 #     assert not obs["last_action_error"]
 
 
 # def test_clear_error():
 #     """In this test, we try to build a ClearAction but we use invalid args, and we check that the action fails when executed in the environment"""
 #     env = BrowserEnv(
 #         task_entrypoint=OpenEndedTask,
-#         start_url=TEXT_INPUT_URL,
+#         task_kwargs={"start_url": TEXT_INPUT_URL},
 #         headless=__HEADLESS__,
 #     )
 #     obs, info = env.reset()
 
 #     soup = bs4.BeautifulSoup(obs["html"], "lxml")
 #     fname = soup.find("input", attrs={"id": "fname"})
 #     lname = soup.find("input", attrs={"id": "lname"})
@@ -1303,24 +1299,27 @@
 
 
 def test_mouse_down_up():
     action_set = HighLevelActionSet(subsets=["bid", "coord"])
 
     env = gym.make(
         "browsergym/openended",
-        start_url=CHECKBOX_URL,
+        task_kwargs={"start_url": CHECKBOX_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
 
     def get_checkbox_elem(obs):
         soup = bs4.BeautifulSoup(
-            flatten_dom_to_str(obs["dom_object"], with_center_coords=True), "lxml"
+            flatten_dom_to_str(
+                obs["dom_object"], obs["extra_element_properties"], with_center_coords=True
+            ),
+            "lxml",
         )
         checkbox = soup.find("input", attrs={"type": "checkbox", "id": "vehicle1"})
         return checkbox
 
     obs, info = env.reset()
     checkbox = get_checkbox_elem(obs)
```

### Comparing `browsergym_core-0.1.0rc7/tests/test_actions_python.py` & `browsergym_core-0.2.0/tests/test_actions_python.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/test_gym_envs.py` & `browsergym_core-0.2.0/tests/test_gym_envs.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 __SLOW_MO = 1000 if "DISPLAY_BROWSER" in os.environ else None
 __HEADLESS = False if "DISPLAY_BROWSER" in os.environ else True
 __TIMEOUT = 500
 
 __DATA_DIR = pathlib.Path(__file__).resolve().parent / "data"
 TEST_PAGE = f"file://{__DATA_DIR}/test_page.html"
 BASIC_IFRAME_PAGE = f"file://{__DATA_DIR}/basic_iframe_site/basic_iframe_2.html"
-DEMO_MODES = ["default", "only_visible_elements"]
+DEMO_MODES = ["default", "only_visible_elements", "all_blue"]
 
 
 def test_gym_env():
     action_set = PythonActionSet()
 
     env = gym.make(
         "browsergym/openended",
-        start_url=TEST_PAGE,
+        task_kwargs={"start_url": TEST_PAGE},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
     obs, info = env.reset()
 
@@ -88,15 +88,15 @@
     env.close()
 
 
 def test_max_episode_steps():
     # no max_steps
     env = gym.make(
         "browsergym/openended",
-        start_url=TEST_PAGE,
+        task_kwargs={"start_url": TEST_PAGE},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
     )
     obs, info = env.reset()
 
     obs, reward, term, trunc, info = env.step("")
@@ -108,15 +108,15 @@
 
     assert term == False
     assert trunc == False
 
     # max_steps = 2
     env = gym.make(
         "browsergym/openended",
-        start_url=TEST_PAGE,
+        task_kwargs={"start_url": TEST_PAGE},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         max_episode_steps=2,
     )
     obs, info = env.reset()
 
@@ -133,15 +133,15 @@
     env.close()
 
 
 def test_active_page():
     action_set = PythonActionSet()
     env = gym.make(
         "browsergym/openended",
-        start_url=TEST_PAGE,
+        task_kwargs={"start_url": TEST_PAGE},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
     )
     obs, info = env.reset()
 
@@ -187,19 +187,18 @@
 
 
 def test_nested_iframes_default_demo_mode():
     demo_mode = "default"
     action_set = HighLevelActionSet(demo_mode=demo_mode)
     env = gym.make(
         "browsergym/openended",
-        start_url=BASIC_IFRAME_PAGE,
+        task_kwargs={"start_url": BASIC_IFRAME_PAGE},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
-        demo_mode=demo_mode,
         action_mapping=action_set.to_python_code,
     )
     obs, info = env.reset()
     assert not obs["last_action_error"]
 
     soup = bs4.BeautifulSoup(flatten_dom_to_str(obs["dom_object"]), "lxml")
     inner_checkbox = soup.find("input", attrs={"id": "checkbox_2"})
@@ -224,20 +223,19 @@
 
 
 @pytest.mark.parametrize("demo_mode", DEMO_MODES)
 def test_demo_mode(demo_mode):
     action_set = HighLevelActionSet(demo_mode=demo_mode)
     env = gym.make(
         "browsergym/openended",
-        start_url=TEST_PAGE,
+        task_kwargs={"start_url": TEST_PAGE},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=action_set.to_python_code,
-        demo_mode=demo_mode,
     )
     obs, info = env.reset()
     assert not obs["last_action_error"]
 
     # Check that the box can be checked when action is not forced
     soup = bs4.BeautifulSoup(flatten_dom_to_str(obs["dom_object"]), "lxml")
     email_field = soup.find("input", attrs={"id": "email"})
@@ -278,7 +276,27 @@
 
     soup = bs4.BeautifulSoup(flatten_dom_to_str(obs["dom_object"]), "lxml")
     checkbox = soup.find("input", attrs={"type": "checkbox", "id": "subscribe"})
     # box is checked
     assert checkbox.has_attr("checked")
 
     env.close()
+
+
+@pytest.mark.parametrize("resizeable_window", (True, False))
+@pytest.mark.parametrize("size", ((1600, 1200), (800, 800)))
+def test_resizeable_window(resizeable_window, size):
+    env = gym.make(
+        "browsergym/openended",
+        task_kwargs={"start_url": TEST_PAGE},
+        headless=__HEADLESS,
+        slow_mo=__SLOW_MO,
+        timeout=__TIMEOUT,
+        viewport={"width": size[0], "height": size[1]},
+        resizeable_window=resizeable_window,
+    )
+    obs, info = env.reset()
+    assert not obs["last_action_error"]
+
+    assert (obs["screenshot"].shape[1], obs["screenshot"].shape[0]) == size
+
+    env.close()
```

### Comparing `browsergym_core-0.1.0rc7/tests/test_observation.py` & `browsergym_core-0.2.0/tests/test_observation.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from browsergym.utils.obs import (
     _remove_redundant_static_text,
     flatten_axtree_to_str,
     flatten_dom_to_str,
 )
 
 # bugfix: use same playwright instance in browsergym and pytest
-
+from utils import setup_playwright
 
 from browsergym.core.observation import (
     _pre_extract,
     _post_extract,
     extract_all_frame_axtrees,
     extract_dom_snapshot,
     extract_merged_axtree,
@@ -33,14 +33,15 @@
 __HEADLESS = False if "DISPLAY_BROWSER" in os.environ else True
 __TIMEOUT = 500
 __VIEWPORT = {"width": 800, "height": 600}
 
 __DATA_DIR = Path(__file__).resolve().parent / "data"
 
 TEST_PAGE = f"file://{__DATA_DIR}/test_page.html"
+TEST_PAGE_2 = f"file://{__DATA_DIR}/test_page_2.html"
 MULTI_IFRAME_URL = f"file://{__DATA_DIR}/basic_iframe_site/basic_iframe_2.html"
 SHADOW_DOM_URL = f"file://{__DATA_DIR}/basic_shadow_dom_site/basic_shadow_dom.html"
 SIMPLE_SHADOW_DOM_URL = f"file://{__DATA_DIR}/basic_shadow_dom_site/simple_shadow_dom.html"
 BASIC_IFRAME_URL = f"file://{__DATA_DIR}/basic_shadow_iframe_site/basic_iframe.html"
 BASIC_IFRAME_2_URL = f"file://{__DATA_DIR}/basic_shadow_iframe_site/basic_iframe_2.html"
 INNER_IFRAME_URL = f"file://{__DATA_DIR}/basic_shadow_iframe_site/inner-iframe.html"
 OUTER_IFRAME_URL = f"file://{__DATA_DIR}/basic_shadow_iframe_site/outer-iframe.html"
@@ -48,15 +49,15 @@
 MULTI_IFRAME_URL = f"file://{__DATA_DIR}/basic_iframe_site/basic_iframe_2.html"
 
 
 @pytest.mark.skip(reason="TODO: how to get the final viewport size right?")
 def test_extract_screenshot():
     env = gym.make(
         "browsergym/openended",
-        start_url=TEST_PAGE,
+        task_kwargs={"start_url": TEST_PAGE},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         viewport=__VIEWPORT,
         timeout=__TIMEOUT,
     )
     obs, info = env.reset()
 
@@ -74,15 +75,15 @@
 
     env.close()
 
 
 def test_extract_axtree_simple():
     env = gym.make(
         "browsergym/openended",
-        start_url=TEST_PAGE,
+        task_kwargs={"start_url": TEST_PAGE},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         viewport=__VIEWPORT,
         timeout=__TIMEOUT,
     )
     obs, info = env.reset()
 
@@ -97,15 +98,15 @@
 
     env.close()
 
 
 def test_extract_axtree_multi_iframe():
     env = gym.make(
         "browsergym/openended",
-        start_url=MULTI_IFRAME_URL,
+        task_kwargs={"start_url": MULTI_IFRAME_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         viewport=__VIEWPORT,
         timeout=__TIMEOUT,
     )
     obs, info = env.reset()
 
@@ -126,15 +127,15 @@
 
     env.close()
 
 
 def test_extract_dom_simple():
     env = gym.make(
         "browsergym/openended",
-        start_url=TEST_PAGE,
+        task_kwargs={"start_url": TEST_PAGE},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         viewport=__VIEWPORT,
         timeout=__TIMEOUT,
     )
     obs, info = env.reset()
 
@@ -147,15 +148,15 @@
 
     env.close()
 
 
 def test_extract_dom_multi_iframe():
     env = gym.make(
         "browsergym/openended",
-        start_url=MULTI_IFRAME_URL,
+        task_kwargs={"start_url": MULTI_IFRAME_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         viewport=__VIEWPORT,
         timeout=__TIMEOUT,
     )
     obs, info = env.reset()
 
@@ -168,15 +169,15 @@
 
     env.close()
 
 
 def test_simple_shadowdom():
     env = gym.make(
         "browsergym/openended",
-        start_url=SIMPLE_SHADOW_DOM_URL,
+        task_kwargs={"start_url": SIMPLE_SHADOW_DOM_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         viewport=__VIEWPORT,
         timeout=__TIMEOUT,
     )
     obs, info = env.reset()
 
@@ -202,15 +203,15 @@
 
     env.close()
 
 
 def test_nested_shadowdom():
     env = gym.make(
         "browsergym/openended",
-        start_url=SHADOW_DOM_URL,
+        task_kwargs={"start_url": SHADOW_DOM_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         viewport=__VIEWPORT,
         timeout=__TIMEOUT,
     )
     obs, info = env.reset()
 
@@ -248,15 +249,15 @@
         INNER_IFRAME_URL,
         OUTER_IFRAME_URL,
     ],
 )
 def test_dom_has_bids_no_aria(url):
     env = gym.make(
         "browsergym/openended",
-        start_url=url,
+        task_kwargs={"start_url": url},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         viewport=__VIEWPORT,
         timeout=__TIMEOUT,
     )
     obs, info = env.reset()
 
@@ -321,15 +322,15 @@
 
     env.close()
 
 
 def test_dom_to_text():
     env = gym.make(
         "browsergym/openended",
-        start_url=TEST_PAGE,
+        task_kwargs={"start_url": TEST_PAGE_2},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=None,
     )
     obs, info = env.reset()
 
@@ -350,31 +351,76 @@
 """
     )
 
     dom = flatten_dom_to_str(obs["dom_object"])
     assert "Janice" in dom
     assert "janice@mail.com" in dom
 
+    dom = flatten_dom_to_str(
+        obs["dom_object"],
+        extra_properties=obs["extra_element_properties"],
+        with_visible=True,
+        with_clickable=True,
+        with_center_coords=True,
+        with_bounding_box_coords=True,
+        with_som=True,
+    )
+    assert 'box="(' in dom
+    assert 'center="(' in dom
+    assert 'clickable="1" som="1" type="submit" value="Submit" visible="1"' in dom
+    assert 'head bid="1" visible="0"' in dom
+    assert 'clickable="1" for="email" visible="1"' in dom
+    assert "Text within in non-html tag" in dom
+    assert "Text that should not be visible" in dom
+
+    dom = flatten_dom_to_str(
+        obs["dom_object"], extra_properties=obs["extra_element_properties"], filter_som_only=True
+    )
+    assert 'for="email"' not in dom
+    assert 'type="submit" value="Submit"' in dom
+    assert "Text within in non-html tag" not in dom
+    assert "Text that should not be visible" not in dom
+
+    dom = flatten_dom_to_str(
+        obs["dom_object"],
+        extra_properties=obs["extra_element_properties"],
+        filter_visible_only=True,
+    )
+    assert "<title bid=" not in dom
+    assert 'type="submit" value="Submit"' in dom
+    assert "Text within in non-html tag" in dom
+    assert "Text that should not be visible" not in dom
+
+    dom = flatten_dom_to_str(
+        obs["dom_object"],
+        extra_properties=obs["extra_element_properties"],
+        filter_with_bid_only=True,
+    )
+    assert "<title bid=" in dom
+    assert 'type="submit" value="Submit"' in dom
+    assert "Text within in non-html tag" not in dom
+    assert "Text that should not be visible" in dom
+
     env.close()
 
 
 def test_axtree_to_text():
     env = gym.make(
         "browsergym/openended",
-        start_url=TEST_PAGE,
+        task_kwargs={"start_url": TEST_PAGE_2},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
         action_mapping=None,
     )
     obs, info = env.reset()
 
     axtree = flatten_axtree_to_str(obs["axtree_object"])
     assert isinstance(axtree, str)
-    assert "checkbox 'Subscribe to newsletter' checked='false'" in axtree
+    assert "checkbox 'Subscribe to newsletter', checked='false'" in axtree
     assert "Janice" not in axtree
 
     obs, reward, term, trunc, info = env.step(
         f"""\
 page.get_by_label("Name:").click()
 page.get_by_label("Name:").fill("Janice")
 page.get_by_label("Name:").press("Tab")
@@ -385,15 +431,59 @@
 page.get_by_label("Subscribe to newsletter").click()
 """
     )
 
     axtree = flatten_axtree_to_str(obs["axtree_object"])
     assert "Janice" in axtree
     assert "janice@mail.com" in axtree
-    assert "checkbox 'Subscribe to newsletter' focused, checked='true'" in axtree
+    assert "checkbox 'Subscribe to newsletter', focused, checked='true'" in axtree
+
+    axtree = flatten_axtree_to_str(
+        obs["axtree_object"],
+        extra_properties=obs["extra_element_properties"],
+        with_visible=True,
+        with_clickable=True,
+        with_center_coords=True,
+        with_bounding_box_coords=True,
+        with_som=True,
+    )
+    assert 'box="(' in axtree
+    assert 'center="(' in axtree
+    assert ', clickable="1", visible="1", som="1"' in axtree
+    assert "heading 'Simple Form', box=\"(" in axtree
+    assert "textbox 'Email:' value='janice@mail.com'" in axtree
+    assert "Text within in non-html tag" in axtree
+    assert "Text that should not be visible" in axtree
+
+    axtree = flatten_axtree_to_str(
+        obs["axtree_object"], extra_properties=obs["extra_element_properties"], filter_som_only=True
+    )
+    assert "LabelText" not in axtree
+    assert "button 'Submit'" in axtree
+    assert "Text within in non-html tag" not in axtree
+    assert "Text that should not be visible" not in axtree
+
+    axtree = flatten_axtree_to_str(
+        obs["axtree_object"],
+        extra_properties=obs["extra_element_properties"],
+        filter_visible_only=True,
+    )
+    assert "RootWebArea" in axtree
+    assert "button 'Submit'" in axtree
+    assert "Text within in non-html tag" in axtree
+    assert "Text that should not be visible" not in axtree
+
+    axtree = flatten_axtree_to_str(
+        obs["axtree_object"],
+        extra_properties=obs["extra_element_properties"],
+        filter_with_bid_only=True,
+    )
+    assert "button 'Submit'" in axtree
+    assert "Text within in non-html tag" not in axtree
+    assert "Text that should not be visible" in axtree
 
     env.close()
 
 
 def test_remove_redundant():
     test_ax_tree = """\
 [150] main 'Screen content'
@@ -434,92 +524,126 @@
     """
     In this simple unit test, we make sure the retrieved coordinates of a known element
     are correct, by verifing that the element is checked after clicking on it.
 
     """
     env = gym.make(
         "browsergym/openended",
-        start_url=TEST_PAGE,
+        task_kwargs={"start_url": TEST_PAGE},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         viewport=__VIEWPORT,
         timeout=__TIMEOUT,
     )
     obs, info = env.reset()
 
     element = env.page.query_selector('[type="checkbox"]')
 
     assert not element.is_checked()
 
-    x, y = map(float, ast.literal_eval(element.get_attribute("browsergym_center")))
+    soup = bs4.BeautifulSoup(
+        flatten_dom_to_str(
+            obs["dom_object"], obs["extra_element_properties"], with_center_coords=True
+        ),
+        "lxml",
+    )
+    input_elem = soup.find("input", attrs={"type": "checkbox"})
+    x, y = map(float, ast.literal_eval(input_elem.get("center")))
+
+    # click input elem
     env.page.mouse.click(x, y)
 
+    element = env.page.query_selector('[type="checkbox"]')
+
     assert element.is_checked()
 
     env.close()
 
 
 def test_basic_iframe_webpage():
     """
     In this simple unit test, we make sure the retrieved coordinates of a known element
     are correct, by verifing that the element is checked after clicking on it.
 
     """
     env = gym.make(
         "browsergym/openended",
-        start_url=BASIC_IFRAME_2_URL,
+        task_kwargs={"start_url": BASIC_IFRAME_2_URL, "goal": "dummy goal"},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         viewport=__VIEWPORT,
         timeout=__TIMEOUT,
-        goal="dummy goal",
     )
 
     # click on the checkbox in the main frame
     obs, info = env.reset()
 
     element = env.page.query_selector('[type="checkbox"]')
 
     assert not element.is_checked()
 
-    x, y = map(float, ast.literal_eval(element.get_attribute("browsergym_center")))
+    bid = element.get_attribute("bid")
+    soup = bs4.BeautifulSoup(
+        flatten_dom_to_str(
+            obs["dom_object"], obs["extra_element_properties"], with_center_coords=True
+        ),
+        "lxml",
+    )
+    input_elem = soup.find("input", attrs={"bid": bid})
+    x, y = map(float, ast.literal_eval(input_elem.get("center")))
     env.page.mouse.click(x, y)
 
     assert element.is_checked()
 
     # click on the checkbox in the inner_frame
-    _, _, _, _, _ = env.step("")
+    obs, _, _, _, _ = env.step("")
     element = env.page.frames[2].query_selector('[type="checkbox"]')
 
     assert element.is_checked()  # instantiated as checked
 
-    x, y = map(float, ast.literal_eval(element.get_attribute("browsergym_center")))
+    bid = element.get_attribute("bid")
+    soup = bs4.BeautifulSoup(
+        flatten_dom_to_str(
+            obs["dom_object"], obs["extra_element_properties"], with_center_coords=True
+        ),
+        "lxml",
+    )
+    input_elem = soup.find("input", attrs={"bid": bid})
+    x, y = map(float, ast.literal_eval(input_elem.get("center")))
     env.page.mouse.click(x, y)
 
     assert not element.is_checked()
 
     # scroll inside a frame, and click on the checkbox in the inner_frame
     env.page.frames[1].evaluate("window.scrollTo(0, document.body.scrollHeight);")
-    _, _, _, _, _ = env.step("")
+    obs, _, _, _, _ = env.step("")
     element = env.page.frames[2].query_selector('[type="checkbox"]')
 
     assert not element.is_checked()  # instantiated as checked
 
-    x, y = map(float, ast.literal_eval(element.get_attribute("browsergym_center")))
+    bid = element.get_attribute("bid")
+    soup = bs4.BeautifulSoup(
+        flatten_dom_to_str(
+            obs["dom_object"], obs["extra_element_properties"], with_center_coords=True
+        ),
+        "lxml",
+    )
+    input_elem = soup.find("input", attrs={"bid": bid})
+    x, y = map(float, ast.literal_eval(input_elem.get("center")))
     env.page.mouse.click(x, y)
 
     assert element.is_checked()
     env.close()
 
 
 @pytest.mark.skip(reason="HTML file seems missing. Deactivating for now.")
 def test_filter_visible_only():
     env = gym.make(
         "browsergym/openended",
-        start_url=CUSTOM_PAGE_URL,
+        task_kwargs={"start_url": CUSTOM_PAGE_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         viewport=__VIEWPORT,
         timeout=__TIMEOUT,
         goal="dummy goal",
     )
 
@@ -539,15 +663,15 @@
     axtree_txt = flatten_axtree_to_str(obs["axtree_object"])
     assert "textbox" in obs["axtree_txt"]
 
 
 def test_extract_focused_element_bid_through_iframes():
     env = gym.make(
         "browsergym/openended",
-        start_url=MULTI_IFRAME_URL,
+        task_kwargs={"start_url": MULTI_IFRAME_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
     )
 
     obs, info = env.reset()
     soup = bs4.BeautifulSoup(flatten_dom_to_str(obs["dom_object"]), "lxml")
@@ -572,15 +696,15 @@
 
     env.close()
 
 
 def test_extract_focused_element_bid_through_shadowdom():
     env = gym.make(
         "browsergym/openended",
-        start_url=SHADOW_DOM_URL,
+        task_kwargs={"start_url": SHADOW_DOM_URL},
         headless=__HEADLESS,
         slow_mo=__SLOW_MO,
         timeout=__TIMEOUT,
     )
 
     obs, info = env.reset()
     soup = bs4.BeautifulSoup(flatten_dom_to_str(obs["dom_object"]), "lxml")
```

### Comparing `browsergym_core-0.1.0rc7/tests/utils.py` & `browsergym_core-0.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/example.html` & `browsergym_core-0.2.0/tests/data/example.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/long_page.html` & `browsergym_core-0.2.0/tests/data/long_page.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/screenshot.png` & `browsergym_core-0.2.0/tests/data/screenshot.png`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/test_page.html` & `browsergym_core-0.2.0/tests/data/test_page.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/basic_iframe_site/basic_iframe.html` & `browsergym_core-0.2.0/tests/data/basic_iframe_site/basic_iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/basic_iframe_site/inner-iframe.html` & `browsergym_core-0.2.0/tests/data/basic_iframe_site/inner-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/basic_iframe_site/outer-iframe.html` & `browsergym_core-0.2.0/tests/data/basic_iframe_site/outer-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/basic_shadow_dom_site/basic_shadow_dom.html` & `browsergym_core-0.2.0/tests/data/basic_shadow_dom_site/basic_shadow_dom.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/basic_shadow_dom_site/simple_shadow_dom.html` & `browsergym_core-0.2.0/tests/data/basic_shadow_dom_site/simple_shadow_dom.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/basic_shadow_iframe_site/basic_iframe.html` & `browsergym_core-0.2.0/tests/data/basic_shadow_iframe_site/basic_iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/basic_shadow_iframe_site/outer-iframe.html` & `browsergym_core-0.2.0/tests/data/basic_shadow_iframe_site/outer-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/checkbox_input.html` & `browsergym_core-0.2.0/tests/data/input_type/checkbox_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/color_picker_input.html` & `browsergym_core-0.2.0/tests/data/input_type/color_picker_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/date_min_max_input.html` & `browsergym_core-0.2.0/tests/data/input_type/date_min_max_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/date_time_local_input.html` & `browsergym_core-0.2.0/tests/data/input_type/date_time_local_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/image_input.html` & `browsergym_core-0.2.0/tests/data/input_type/image_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/img_submit.gif` & `browsergym_core-0.2.0/tests/data/input_type/img_submit.gif`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/password_input.html` & `browsergym_core-0.2.0/tests/data/input_type/password_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/reset_input.html` & `browsergym_core-0.2.0/tests/data/input_type/reset_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/submit_input.html` & `browsergym_core-0.2.0/tests/data/input_type/submit_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/telephone_input.html` & `browsergym_core-0.2.0/tests/data/input_type/telephone_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/text_input.html` & `browsergym_core-0.2.0/tests/data/input_type/text_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/tests/data/input_type/time_input.html` & `browsergym_core-0.2.0/tests/data/input_type/time_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/pyproject.toml` & `browsergym_core-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.1.0rc7/PKG-INFO` & `browsergym_core-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: browsergym-core
-Version: 0.1.0rc7
+Version: 0.2.0
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

