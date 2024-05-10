# Comparing `tmp/tgbotzero-0.0.7.tar.gz` & `tmp/tgbotzero-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgbotzero-0.0.7.tar", last modified: Tue Nov  7 09:21:26 2023, max compression
+gzip compressed data, was "tgbotzero-0.0.9.tar", last modified: Fri May 10 13:44:09 2024, max compression
```

## Comparing `tgbotzero-0.0.7.tar` & `tgbotzero-0.0.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-11-07 09:21:26.075924 tgbotzero-0.0.7/
--rw-rw-rw-   0        0        0     1103 2023-10-22 11:56:28.000000 tgbotzero-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      138 2022-12-15 21:01:40.000000 tgbotzero-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     7834 2023-11-07 09:21:26.074441 tgbotzero-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6703 2023-11-07 09:18:15.000000 tgbotzero-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-11-07 09:21:26.043043 tgbotzero-0.0.7/docs/
--rw-rw-rw-   0        0        0   118536 2023-10-22 14:34:46.000000 tgbotzero-0.0.7/docs/buttonbot.png
--rw-rw-rw-   0        0        0   137181 2023-11-07 00:57:06.000000 tgbotzero-0.0.7/docs/commands.png
--rw-rw-rw-   0        0        0    22219 2023-10-22 13:01:17.000000 tgbotzero-0.0.7/docs/echobot.png
--rw-rw-rw-   0        0        0   356698 2023-11-07 00:59:31.000000 tgbotzero-0.0.7/docs/gallery.png
--rw-rw-rw-   0        0        0   370371 2023-11-07 00:58:10.000000 tgbotzero-0.0.7/docs/img.png
--rw-rw-rw-   0        0        0    14092 2023-11-07 00:55:06.000000 tgbotzero-0.0.7/docs/onstart.png
--rw-rw-rw-   0        0        0   170574 2023-11-07 01:00:44.000000 tgbotzero-0.0.7/docs/puttext.png
--rw-rw-rw-   0        0        0       42 2023-11-07 09:21:26.075924 tgbotzero-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     3708 2023-10-22 12:55:54.000000 tgbotzero-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-07 09:21:26.031095 tgbotzero-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-11-07 09:21:26.045686 tgbotzero-0.0.7/src/tgbotzero/
--rw-rw-rw-   0        0        0      226 2023-11-07 09:18:15.000000 tgbotzero-0.0.7/src/tgbotzero/__about__.py
--rw-rw-rw-   0        0        0      239 2023-10-31 09:21:27.000000 tgbotzero-0.0.7/src/tgbotzero/__init__.py
--rw-rw-rw-   0        0        0       76 2023-10-22 12:48:30.000000 tgbotzero-0.0.7/src/tgbotzero/__main__.py
-drwxrwxrwx   0        0        0        0 2023-11-07 09:21:26.063897 tgbotzero-0.0.7/src/tgbotzero/examples/
--rw-rw-rw-   0        0        0      223 2023-11-07 08:42:44.000000 tgbotzero-0.0.7/src/tgbotzero/examples/00_echo_bot.py
--rw-rw-rw-   0        0        0      380 2023-10-31 08:55:12.000000 tgbotzero-0.0.7/src/tgbotzero/examples/01_bot_with_button.py
--rw-rw-rw-   0        0        0      732 2023-10-31 08:55:30.000000 tgbotzero-0.0.7/src/tgbotzero/examples/02_bot_with_buttons.py
--rw-rw-rw-   0        0        0      121 2023-11-06 22:39:11.000000 tgbotzero-0.0.7/src/tgbotzero/examples/03_help.py
--rw-rw-rw-   0        0        0      488 2023-10-22 14:00:18.000000 tgbotzero-0.0.7/src/tgbotzero/examples/04_no_on_button_func_error.py
--rw-rw-rw-   0        0        0     2245 2023-10-23 09:48:45.000000 tgbotzero-0.0.7/src/tgbotzero/examples/05_schedule_bot.py
--rw-rw-rw-   0        0        0      352 2023-10-31 08:57:12.000000 tgbotzero-0.0.7/src/tgbotzero/examples/06_on_start.py
--rw-rw-rw-   0        0        0      646 2023-10-31 08:54:55.000000 tgbotzero-0.0.7/src/tgbotzero/examples/07_commands.py
--rw-rw-rw-   0        0        0      190 2023-11-06 22:44:26.000000 tgbotzero-0.0.7/src/tgbotzero/examples/08_send_image.py
--rw-rw-rw-   0        0        0      310 2023-11-06 23:18:28.000000 tgbotzero-0.0.7/src/tgbotzero/examples/09_image_gallery.py
--rw-rw-rw-   0        0        0      291 2023-11-06 23:39:50.000000 tgbotzero-0.0.7/src/tgbotzero/examples/10_on_image.py
--rw-rw-rw-   0        0        0      360 2023-11-07 08:01:01.000000 tgbotzero-0.0.7/src/tgbotzero/examples/11_add_text_on_image.py
--rw-rw-rw-   0        0        0     1064 2023-11-07 09:20:02.000000 tgbotzero-0.0.7/src/tgbotzero/examples/99_demo.py
--rw-rw-rw-   0        0        0        0 2022-12-22 17:18:53.000000 tgbotzero-0.0.7/src/tgbotzero/examples/__init__.py
--rw-rw-rw-   0        0        0   955363 2023-10-31 09:17:57.000000 tgbotzero-0.0.7/src/tgbotzero/examples/cat.png
--rw-rw-rw-   0        0        0  2460972 2023-11-06 23:13:42.000000 tgbotzero-0.0.7/src/tgbotzero/examples/dog.png
-drwxrwxrwx   0        0        0        0 2023-11-07 09:21:26.072306 tgbotzero-0.0.7/src/tgbotzero/utils/
--rw-rw-rw-   0        0        0        0 2023-01-27 12:40:02.000000 tgbotzero-0.0.7/src/tgbotzero/utils/__init__.py
--rw-rw-rw-   0        0        0     8167 2023-11-07 00:17:18.000000 tgbotzero-0.0.7/src/tgbotzero/utils/botzero.py
--rw-rw-rw-   0        0        0     1469 2023-10-22 13:58:32.000000 tgbotzero-0.0.7/src/tgbotzero/utils/check_on_button_functions.py
--rw-rw-rw-   0        0        0      438 2023-10-22 13:04:29.000000 tgbotzero-0.0.7/src/tgbotzero/utils/copy_examples.py
--rw-rw-rw-   0        0        0      716 2023-10-22 13:27:29.000000 tgbotzero-0.0.7/src/tgbotzero/utils/help.py
--rw-rw-rw-   0        0        0     2297 2023-11-07 00:49:06.000000 tgbotzero-0.0.7/src/tgbotzero/utils/images.py
--rw-rw-rw-   0        0        0     1376 2023-10-31 10:22:29.000000 tgbotzero-0.0.7/src/tgbotzero/utils/reply_markup.py
--rw-rw-rw-   0        0        0     1913 2023-11-06 23:53:03.000000 tgbotzero-0.0.7/src/tgbotzero/utils/send_answer.py
-drwxrwxrwx   0        0        0        0 2023-11-07 09:21:26.049989 tgbotzero-0.0.7/src/tgbotzero.egg-info/
--rw-rw-rw-   0        0        0     7834 2023-11-07 09:21:25.000000 tgbotzero-0.0.7/src/tgbotzero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1381 2023-11-07 09:21:26.000000 tgbotzero-0.0.7/src/tgbotzero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-07 09:21:25.000000 tgbotzero-0.0.7/src/tgbotzero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-11-07 09:21:25.000000 tgbotzero-0.0.7/src/tgbotzero.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-11-07 09:21:25.000000 tgbotzero-0.0.7/src/tgbotzero.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-07 09:21:26.073933 tgbotzero-0.0.7/tests/
--rw-rw-rw-   0        0        0      819 2023-10-22 12:59:09.000000 tgbotzero-0.0.7/tests/test_copy_examples.py
--rw-rw-rw-   0        0        0      142 2023-10-22 13:13:05.000000 tgbotzero-0.0.7/tests/test_examples.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:44:09.153282 tgbotzero-0.0.9/
+-rw-rw-rw-   0        0        0     1103 2023-10-22 11:56:28.000000 tgbotzero-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      138 2022-12-15 21:01:40.000000 tgbotzero-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8278 2024-05-10 13:44:09.150806 tgbotzero-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7147 2024-01-10 14:40:24.000000 tgbotzero-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 13:44:09.074784 tgbotzero-0.0.9/docs/
+-rw-rw-rw-   0        0        0   118536 2023-10-22 14:34:46.000000 tgbotzero-0.0.9/docs/buttonbot.png
+-rw-rw-rw-   0        0        0   137181 2023-11-07 00:57:06.000000 tgbotzero-0.0.9/docs/commands.png
+-rw-rw-rw-   0        0        0    22219 2023-10-22 13:01:17.000000 tgbotzero-0.0.9/docs/echobot.png
+-rw-rw-rw-   0        0        0   356698 2023-11-07 00:59:31.000000 tgbotzero-0.0.9/docs/gallery.png
+-rw-rw-rw-   0        0        0   370371 2023-11-07 00:58:10.000000 tgbotzero-0.0.9/docs/img.png
+-rw-rw-rw-   0        0        0    14092 2023-11-07 00:55:06.000000 tgbotzero-0.0.9/docs/onstart.png
+-rw-rw-rw-   0        0        0   170574 2023-11-07 01:00:44.000000 tgbotzero-0.0.9/docs/puttext.png
+-rw-rw-rw-   0        0        0       42 2024-05-10 13:44:09.153282 tgbotzero-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3708 2023-10-22 12:55:54.000000 tgbotzero-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:44:09.045280 tgbotzero-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:44:09.081280 tgbotzero-0.0.9/src/tgbotzero/
+-rw-rw-rw-   0        0        0      226 2024-05-10 13:38:58.000000 tgbotzero-0.0.9/src/tgbotzero/__about__.py
+-rw-rw-rw-   0        0        0      239 2023-10-31 09:21:27.000000 tgbotzero-0.0.9/src/tgbotzero/__init__.py
+-rw-rw-rw-   0        0        0       76 2023-10-22 12:48:30.000000 tgbotzero-0.0.9/src/tgbotzero/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:44:09.123295 tgbotzero-0.0.9/src/tgbotzero/examples/
+-rw-rw-rw-   0        0        0      144 2024-01-10 14:36:47.000000 tgbotzero-0.0.9/src/tgbotzero/examples/00_echo_bot.py
+-rw-rw-rw-   0        0        0      380 2024-01-10 14:16:43.000000 tgbotzero-0.0.9/src/tgbotzero/examples/01_bot_with_button.py
+-rw-rw-rw-   0        0        0      732 2024-01-10 14:17:13.000000 tgbotzero-0.0.9/src/tgbotzero/examples/02_bot_with_buttons.py
+-rw-rw-rw-   0        0        0      121 2023-11-06 22:39:11.000000 tgbotzero-0.0.9/src/tgbotzero/examples/03_help.py
+-rw-rw-rw-   0        0        0      488 2024-01-10 14:11:18.000000 tgbotzero-0.0.9/src/tgbotzero/examples/04_no_on_button_func_error.py
+-rw-rw-rw-   0        0        0     2245 2024-01-10 14:11:18.000000 tgbotzero-0.0.9/src/tgbotzero/examples/05_schedule_bot.py
+-rw-rw-rw-   0        0        0      352 2023-10-31 08:57:12.000000 tgbotzero-0.0.9/src/tgbotzero/examples/06_on_start.py
+-rw-rw-rw-   0        0        0      646 2023-10-31 08:54:55.000000 tgbotzero-0.0.9/src/tgbotzero/examples/07_commands.py
+-rw-rw-rw-   0        0        0      190 2023-11-06 22:44:26.000000 tgbotzero-0.0.9/src/tgbotzero/examples/08_send_image.py
+-rw-rw-rw-   0        0        0      310 2023-11-06 23:18:28.000000 tgbotzero-0.0.9/src/tgbotzero/examples/09_image_gallery.py
+-rw-rw-rw-   0        0        0      291 2023-11-06 23:39:50.000000 tgbotzero-0.0.9/src/tgbotzero/examples/10_on_image.py
+-rw-rw-rw-   0        0        0      360 2023-11-07 08:01:01.000000 tgbotzero-0.0.9/src/tgbotzero/examples/11_add_text_on_image.py
+-rw-rw-rw-   0        0        0      184 2024-01-10 14:36:40.000000 tgbotzero-0.0.9/src/tgbotzero/examples/12_chat_id_bot.py
+-rw-rw-rw-   0        0        0        0 2022-12-22 17:18:53.000000 tgbotzero-0.0.9/src/tgbotzero/examples/__init__.py
+-rw-rw-rw-   0        0        0   955363 2023-10-31 09:17:57.000000 tgbotzero-0.0.9/src/tgbotzero/examples/cat.png
+-rw-rw-rw-   0        0        0  2460972 2023-11-06 23:13:42.000000 tgbotzero-0.0.9/src/tgbotzero/examples/dog.png
+drwxrwxrwx   0        0        0        0 2024-05-10 13:44:09.144280 tgbotzero-0.0.9/src/tgbotzero/utils/
+-rw-rw-rw-   0        0        0        0 2023-01-27 12:40:02.000000 tgbotzero-0.0.9/src/tgbotzero/utils/__init__.py
+-rw-rw-rw-   0        0        0    10219 2024-01-10 14:34:07.000000 tgbotzero-0.0.9/src/tgbotzero/utils/botzero.py
+-rw-rw-rw-   0        0        0     1469 2023-10-22 13:58:32.000000 tgbotzero-0.0.9/src/tgbotzero/utils/check_on_button_functions.py
+-rw-rw-rw-   0        0        0      438 2023-10-22 13:04:29.000000 tgbotzero-0.0.9/src/tgbotzero/utils/copy_examples.py
+-rw-rw-rw-   0        0        0      734 2024-01-10 14:21:21.000000 tgbotzero-0.0.9/src/tgbotzero/utils/help.py
+-rw-rw-rw-   0        0        0     2297 2023-11-07 00:49:06.000000 tgbotzero-0.0.9/src/tgbotzero/utils/images.py
+-rw-rw-rw-   0        0        0     1376 2023-10-31 10:22:29.000000 tgbotzero-0.0.9/src/tgbotzero/utils/reply_markup.py
+-rw-rw-rw-   0        0        0     1913 2024-05-10 13:38:23.000000 tgbotzero-0.0.9/src/tgbotzero/utils/send_answer.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:44:09.148806 tgbotzero-0.0.9/src/tgbotzero.egg-info/
+-rw-rw-rw-   0        0        0     8278 2024-05-10 13:44:08.000000 tgbotzero-0.0.9/src/tgbotzero.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1388 2024-05-10 13:44:08.000000 tgbotzero-0.0.9/src/tgbotzero.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 13:44:08.000000 tgbotzero-0.0.9/src/tgbotzero.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-10 13:44:08.000000 tgbotzero-0.0.9/src/tgbotzero.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-10 13:44:08.000000 tgbotzero-0.0.9/src/tgbotzero.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:44:09.147306 tgbotzero-0.0.9/tests/
+-rw-rw-rw-   0        0        0      819 2023-10-22 12:59:09.000000 tgbotzero-0.0.9/tests/test_copy_examples.py
+-rw-rw-rw-   0        0        0      142 2023-10-22 13:13:05.000000 tgbotzero-0.0.9/tests/test_examples.py
```

### Comparing `tgbotzero-0.0.7/LICENSE` & `tgbotzero-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/PKG-INFO` & `tgbotzero-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgbotzero
-Version: 0.0.7
+Version: 0.0.9
 Summary: A zero-boilerplate simple telegram bots
 Home-page: https://github.com/ShashkovS/tgbotzero
 Author: Sergey Shashkov
 Author-email: sh57@yandex.ru
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -49,15 +49,15 @@
 Токен нужно указать в глобальной переменной TOKEN.
 Для обработки текстовых сообщений нужно создать функцию on_message(msg: str). Функция принимает текст сообщения, и может вернуть либо строку с текстом ответа, либо список из сообщений, описаний кнопок и картинок. Про кнопки и картинки будет дальше.
 Для запуска бота нужно выполнить команду `run_bot()` без параметров.
 
 ``` python
 import tgbotzero
 
-TOKEN = '123123123:tokenFromBotFatherInTelegram'
+TOKEN = '123:tokenHereFromBotFatherInTelegram'
 
 def on_message(msg: str):
     return "Твоё сообщение: " + msg
     
 run_bot()
 ```
 
@@ -196,8 +196,28 @@
 
 run_bot()
 ```
 <img alt="puttext" src="https://github.com/ShashkovS/tgbotzero/blob/main/docs/puttext.png?raw=true" width="323">
 
 
 
+
+### Получение chat_id:
+
+К любой функции-обработчику можно добавить ещё один параметр `chat_id: int`, если хочется различать пользователей.
+
+```python
+from tgbotzero import *
+
+TOKEN = '123:tokenHereFromBotFatherInTelegram'
+
+
+def on_message(msg: str, chat_id: int):
+    return f"Текущий chat id: {chat_id}"
+
+
+run_bot()
+```
+
+
+
 # [Contributing](CONTRIBUTING.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tgbotzero Version: 0.0.7 Summary: A zero-
+Metadata-Version: 2.1 Name: tgbotzero Version: 0.0.9 Summary: A zero-
 boilerplate simple telegram bots Home-page: https://github.com/ShashkovS/
 tgbotzero Author: Sergey Shashkov Author-email: sh57@yandex.ru License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: End Users/Desktop Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -24,15 +24,15 @@
 ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ð¹ Ð½ÑÐ¶Ð½Ð¾ ÑÐ¾Ð·Ð´Ð°ÑÑ ÑÑÐ½ÐºÑÐ¸Ñ on_message(msg:
 str). Ð¤ÑÐ½ÐºÑÐ¸Ñ Ð¿ÑÐ¸Ð½Ð¸Ð¼Ð°ÐµÑ ÑÐµÐºÑÑ ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ñ, Ð¸
 Ð¼Ð¾Ð¶ÐµÑ Ð²ÐµÑÐ½ÑÑÑ Ð»Ð¸Ð±Ð¾ ÑÑÑÐ¾ÐºÑ Ñ ÑÐµÐºÑÑÐ¾Ð¼ Ð¾ÑÐ²ÐµÑÐ°,
 Ð»Ð¸Ð±Ð¾ ÑÐ¿Ð¸ÑÐ¾Ðº Ð¸Ð· ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ð¹, Ð¾Ð¿Ð¸ÑÐ°Ð½Ð¸Ð¹ ÐºÐ½Ð¾Ð¿Ð¾Ðº Ð¸
 ÐºÐ°ÑÑÐ¸Ð½Ð¾Ðº. ÐÑÐ¾ ÐºÐ½Ð¾Ð¿ÐºÐ¸ Ð¸ ÐºÐ°ÑÑÐ¸Ð½ÐºÐ¸ Ð±ÑÐ´ÐµÑ
 Ð´Ð°Ð»ÑÑÐµ. ÐÐ»Ñ Ð·Ð°Ð¿ÑÑÐºÐ° Ð±Ð¾ÑÐ° Ð½ÑÐ¶Ð½Ð¾ Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÑ
 ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ `run_bot()` Ð±ÐµÐ· Ð¿Ð°ÑÐ°Ð¼ÐµÑÑÐ¾Ð². ``` python import
-tgbotzero TOKEN = '123123123:tokenFromBotFatherInTelegram' def on_message(msg:
+tgbotzero TOKEN = '123:tokenHereFromBotFatherInTelegram' def on_message(msg:
 str): return "Ð¢Ð²Ð¾Ñ ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ðµ: " + msg run_bot() ``` [echobot]#
 Ð£ÑÑÐ°Ð½Ð¾Ð²ÐºÐ° ÐÐ²ÐµÐ´Ð¸ÑÐµ Ð² ÑÐµÑÐ¼Ð¸Ð½Ð°Ð»Ðµ: ```shell pip install
 tgbotzero --upgrade --user ``` ÐÐ»Ð¸ Ð·Ð°Ð¿ÑÑÑÐ¸ÑÐµ ÑÑÑ
 Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ: ```python import os, sys python = sys.executable user = '--
 user' if 'venv' not in python and 'envs' not in python else '' cmd = f'"
 {python}" -m pip install tgbotzero --upgrade {user}' os.system(cmd) ``` ###
 ÐÐ¾Ñ Ñ ÐºÐ½Ð¾Ð¿ÐºÐ°Ð¼Ð¸: ÐÐ»Ñ ÑÐ¾Ð³Ð¾ ÑÑÐ¾Ð±Ñ Ð´Ð¾Ð±Ð°Ð²Ð¸ÑÑ Ðº
@@ -83,9 +83,15 @@
 Ð´Ð¾Ð±Ð°Ð²Ð»ÐµÐ½Ð¸Ðµ ÑÐµÐºÑÑÐ°. Ð¡Ð¸Ð½ÑÐ°ÐºÑÐ¸Ñ: `img.put_text(text,
 color)`, Ð³Ð´Ðµ`color` â ÑÑÐ¾ RGB-ÐºÐ¾ÑÑÐµÐ¶, Ð½Ð°Ð¿ÑÐ¸Ð¼ÐµÑ, `(255, 0,
 0)`. ÐÐ·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ Ð¼Ð¾Ð¶Ð½Ð¾ Ð¼Ð¾Ð´Ð¸ÑÐ¸ÑÐ¸ÑÐ¾Ð²Ð°ÑÑ Ð´Ð°Ð¶Ðµ
 ÐµÑÐ»Ð¸ Ð¾Ð½Ð¸ Ð¾ÑÐºÑÑÑÑ Ð¸Ð· ÑÐ°Ð¹Ð»Ð°: `Image(image_filename).put_text
 (text, color)` ```python from tgbotzero import * TOKEN = '123:
 tokenHereFromBotFatherInTelegram' def on_message(msg: str): return 'ÐÐ´Ñ
 ÐºÐ°ÑÑÐ¸Ð½ÐºÑ Ñ Ð¿Ð¾Ð´Ð¿Ð¸ÑÑÑ!' def on_image(msg: str, img: Image):
-return img.put_text(msg, (255, 0, 0)) run_bot() ``` [puttext]# [Contributing]
+return img.put_text(msg, (255, 0, 0)) run_bot() ``` [puttext]###
+ÐÐ¾Ð»ÑÑÐµÐ½Ð¸Ðµ chat_id: Ð Ð»ÑÐ±Ð¾Ð¹ ÑÑÐ½ÐºÑÐ¸Ð¸-Ð¾Ð±ÑÐ°Ð±Ð¾ÑÑÐ¸ÐºÑ
+Ð¼Ð¾Ð¶Ð½Ð¾ Ð´Ð¾Ð±Ð°Ð²Ð¸ÑÑ ÐµÑÑ Ð¾Ð´Ð¸Ð½ Ð¿Ð°ÑÐ°Ð¼ÐµÑÑ `chat_id: int`,
+ÐµÑÐ»Ð¸ ÑÐ¾ÑÐµÑÑÑ ÑÐ°Ð·Ð»Ð¸ÑÐ°ÑÑ Ð¿Ð¾Ð»ÑÐ·Ð¾Ð²Ð°ÑÐµÐ»ÐµÐ¹.
+```python from tgbotzero import * TOKEN = '123:
+tokenHereFromBotFatherInTelegram' def on_message(msg: str, chat_id: int):
+return f"Ð¢ÐµÐºÑÑÐ¸Ð¹ chat id: {chat_id}" run_bot() ``` # [Contributing]
 (CONTRIBUTING.md)
```

### Comparing `tgbotzero-0.0.7/README.md` & `tgbotzero-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 Токен нужно указать в глобальной переменной TOKEN.
 Для обработки текстовых сообщений нужно создать функцию on_message(msg: str). Функция принимает текст сообщения, и может вернуть либо строку с текстом ответа, либо список из сообщений, описаний кнопок и картинок. Про кнопки и картинки будет дальше.
 Для запуска бота нужно выполнить команду `run_bot()` без параметров.
 
 ``` python
 import tgbotzero
 
-TOKEN = '123123123:tokenFromBotFatherInTelegram'
+TOKEN = '123:tokenHereFromBotFatherInTelegram'
 
 def on_message(msg: str):
     return "Твоё сообщение: " + msg
     
 run_bot()
 ```
 
@@ -166,8 +166,28 @@
 
 run_bot()
 ```
 <img alt="puttext" src="https://github.com/ShashkovS/tgbotzero/blob/main/docs/puttext.png?raw=true" width="323">
 
 
 
+
+### Получение chat_id:
+
+К любой функции-обработчику можно добавить ещё один параметр `chat_id: int`, если хочется различать пользователей.
+
+```python
+from tgbotzero import *
+
+TOKEN = '123:tokenHereFromBotFatherInTelegram'
+
+
+def on_message(msg: str, chat_id: int):
+    return f"Текущий chat id: {chat_id}"
+
+
+run_bot()
+```
+
+
+
 # [Contributing](CONTRIBUTING.md)
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ð¹ Ð½ÑÐ¶Ð½Ð¾ ÑÐ¾Ð·Ð´Ð°ÑÑ ÑÑÐ½ÐºÑÐ¸Ñ on_message(msg:
 str). Ð¤ÑÐ½ÐºÑÐ¸Ñ Ð¿ÑÐ¸Ð½Ð¸Ð¼Ð°ÐµÑ ÑÐµÐºÑÑ ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ñ, Ð¸
 Ð¼Ð¾Ð¶ÐµÑ Ð²ÐµÑÐ½ÑÑÑ Ð»Ð¸Ð±Ð¾ ÑÑÑÐ¾ÐºÑ Ñ ÑÐµÐºÑÑÐ¾Ð¼ Ð¾ÑÐ²ÐµÑÐ°,
 Ð»Ð¸Ð±Ð¾ ÑÐ¿Ð¸ÑÐ¾Ðº Ð¸Ð· ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ð¹, Ð¾Ð¿Ð¸ÑÐ°Ð½Ð¸Ð¹ ÐºÐ½Ð¾Ð¿Ð¾Ðº Ð¸
 ÐºÐ°ÑÑÐ¸Ð½Ð¾Ðº. ÐÑÐ¾ ÐºÐ½Ð¾Ð¿ÐºÐ¸ Ð¸ ÐºÐ°ÑÑÐ¸Ð½ÐºÐ¸ Ð±ÑÐ´ÐµÑ
 Ð´Ð°Ð»ÑÑÐµ. ÐÐ»Ñ Ð·Ð°Ð¿ÑÑÐºÐ° Ð±Ð¾ÑÐ° Ð½ÑÐ¶Ð½Ð¾ Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÑ
 ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ `run_bot()` Ð±ÐµÐ· Ð¿Ð°ÑÐ°Ð¼ÐµÑÑÐ¾Ð². ``` python import
-tgbotzero TOKEN = '123123123:tokenFromBotFatherInTelegram' def on_message(msg:
+tgbotzero TOKEN = '123:tokenHereFromBotFatherInTelegram' def on_message(msg:
 str): return "Ð¢Ð²Ð¾Ñ ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ðµ: " + msg run_bot() ``` [echobot]#
 Ð£ÑÑÐ°Ð½Ð¾Ð²ÐºÐ° ÐÐ²ÐµÐ´Ð¸ÑÐµ Ð² ÑÐµÑÐ¼Ð¸Ð½Ð°Ð»Ðµ: ```shell pip install
 tgbotzero --upgrade --user ``` ÐÐ»Ð¸ Ð·Ð°Ð¿ÑÑÑÐ¸ÑÐµ ÑÑÑ
 Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ: ```python import os, sys python = sys.executable user = '--
 user' if 'venv' not in python and 'envs' not in python else '' cmd = f'"
 {python}" -m pip install tgbotzero --upgrade {user}' os.system(cmd) ``` ###
 ÐÐ¾Ñ Ñ ÐºÐ½Ð¾Ð¿ÐºÐ°Ð¼Ð¸: ÐÐ»Ñ ÑÐ¾Ð³Ð¾ ÑÑÐ¾Ð±Ñ Ð´Ð¾Ð±Ð°Ð²Ð¸ÑÑ Ðº
@@ -68,9 +68,15 @@
 Ð´Ð¾Ð±Ð°Ð²Ð»ÐµÐ½Ð¸Ðµ ÑÐµÐºÑÑÐ°. Ð¡Ð¸Ð½ÑÐ°ÐºÑÐ¸Ñ: `img.put_text(text,
 color)`, Ð³Ð´Ðµ`color` â ÑÑÐ¾ RGB-ÐºÐ¾ÑÑÐµÐ¶, Ð½Ð°Ð¿ÑÐ¸Ð¼ÐµÑ, `(255, 0,
 0)`. ÐÐ·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ Ð¼Ð¾Ð¶Ð½Ð¾ Ð¼Ð¾Ð´Ð¸ÑÐ¸ÑÐ¸ÑÐ¾Ð²Ð°ÑÑ Ð´Ð°Ð¶Ðµ
 ÐµÑÐ»Ð¸ Ð¾Ð½Ð¸ Ð¾ÑÐºÑÑÑÑ Ð¸Ð· ÑÐ°Ð¹Ð»Ð°: `Image(image_filename).put_text
 (text, color)` ```python from tgbotzero import * TOKEN = '123:
 tokenHereFromBotFatherInTelegram' def on_message(msg: str): return 'ÐÐ´Ñ
 ÐºÐ°ÑÑÐ¸Ð½ÐºÑ Ñ Ð¿Ð¾Ð´Ð¿Ð¸ÑÑÑ!' def on_image(msg: str, img: Image):
-return img.put_text(msg, (255, 0, 0)) run_bot() ``` [puttext]# [Contributing]
+return img.put_text(msg, (255, 0, 0)) run_bot() ``` [puttext]###
+ÐÐ¾Ð»ÑÑÐµÐ½Ð¸Ðµ chat_id: Ð Ð»ÑÐ±Ð¾Ð¹ ÑÑÐ½ÐºÑÐ¸Ð¸-Ð¾Ð±ÑÐ°Ð±Ð¾ÑÑÐ¸ÐºÑ
+Ð¼Ð¾Ð¶Ð½Ð¾ Ð´Ð¾Ð±Ð°Ð²Ð¸ÑÑ ÐµÑÑ Ð¾Ð´Ð¸Ð½ Ð¿Ð°ÑÐ°Ð¼ÐµÑÑ `chat_id: int`,
+ÐµÑÐ»Ð¸ ÑÐ¾ÑÐµÑÑÑ ÑÐ°Ð·Ð»Ð¸ÑÐ°ÑÑ Ð¿Ð¾Ð»ÑÐ·Ð¾Ð²Ð°ÑÐµÐ»ÐµÐ¹.
+```python from tgbotzero import * TOKEN = '123:
+tokenHereFromBotFatherInTelegram' def on_message(msg: str, chat_id: int):
+return f"Ð¢ÐµÐºÑÑÐ¸Ð¹ chat id: {chat_id}" run_bot() ``` # [Contributing]
 (CONTRIBUTING.md)
```

### Comparing `tgbotzero-0.0.7/docs/buttonbot.png` & `tgbotzero-0.0.9/docs/buttonbot.png`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/docs/commands.png` & `tgbotzero-0.0.9/docs/commands.png`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/docs/echobot.png` & `tgbotzero-0.0.9/docs/echobot.png`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/docs/gallery.png` & `tgbotzero-0.0.9/docs/gallery.png`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/docs/img.png` & `tgbotzero-0.0.9/docs/img.png`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/docs/onstart.png` & `tgbotzero-0.0.9/docs/onstart.png`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/docs/puttext.png` & `tgbotzero-0.0.9/docs/puttext.png`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/setup.py` & `tgbotzero-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/src/tgbotzero/examples/02_bot_with_buttons.py` & `tgbotzero-0.0.9/src/tgbotzero/examples/02_bot_with_buttons.py`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/src/tgbotzero/examples/05_schedule_bot.py` & `tgbotzero-0.0.9/src/tgbotzero/examples/05_schedule_bot.py`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/src/tgbotzero/examples/07_commands.py` & `tgbotzero-0.0.9/src/tgbotzero/examples/07_commands.py`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/src/tgbotzero/examples/cat.png` & `tgbotzero-0.0.9/src/tgbotzero/examples/cat.png`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/src/tgbotzero/examples/dog.png` & `tgbotzero-0.0.9/src/tgbotzero/examples/dog.png`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/src/tgbotzero/utils/botzero.py` & `tgbotzero-0.0.9/src/tgbotzero/utils/botzero.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import os
 import sys
 import atexit
 import traceback
 import types
 import json
 import re
@@ -30,30 +31,40 @@
 
 def set_up_token(bot: telebot.TeleBot, main_module: types.ModuleType):
     token = getattr(main_module, "TOKEN", None)
     if not token or 'BotFather' in token:
         token = os.environ.get('TOKEN', None)
     if not token:
         help()
-        raise ValueError('Необходимо в переменную TOKEN записать токен телеграм-бота. Как-то так: '
+        raise ValueError('Необходимо в переменную TOKEN записать токен телеграм-бота (от BotFather). Как-то так: '
                          'TOKEN = "123123123:abcabcabcabcabcabcabcabcabc"')
     bot.token = token
 
 
 def set_up_on_text_message(bot: telebot.TeleBot, main_module: types.ModuleType):
     on_message = getattr(main_module, "on_message", None)
     if not on_message:
         help()
         raise ValueError('Необходимо определить функцию on_message. Например, так:'
                          'def on_message(msg: str):'
                          '    return "Твоё сообщение: " + msg')
+    signature = inspect.signature(on_message)
+    num_parms = len(signature.parameters)
 
     def on_text_message(message: telebot.types.Message):
+        if num_parms == 0:
+            args = tuple()
+        elif num_parms == 1:
+            args = (message.text,)
+        elif num_parms == 2:
+            args = (message.text, message.chat.id)
+        else:
+            raise ValueError('Функция on_message не должна иметь больше двух параметров')
         try:
-            answer = on_message(message.text)
+            answer = on_message(*args)
         except Exception as e:
             bot.send_message(message.from_user.id, f'Возникла ошибка:\n{traceback.format_exc()}')
             raise
         send_answer(bot, message.from_user.id, answer)
 
     bot.message_handler(content_types=['text'])(on_text_message)
 
@@ -64,37 +75,49 @@
         def on_image_message(message: telebot.types.Message):
             text = ('Необходимо определить функцию on_image. Например, так:'
                     'def on_image(msg: txt, img: Image):'
                     '    return ["Твоё фото", img]')
             bot.send_message(message.from_user.id, text)
             raise ValueError(text)
     else:
+        signature = inspect.signature(on_image)
+        num_parms = len(signature.parameters)
+
         def on_image_message(message: telebot.types.Message):
             try:
                 file_id = message.photo[-1].file_id
                 file_info = bot.get_file(file_id)
                 downloaded_file = bot.download_file(file_info.file_path)
                 image = Image(downloaded_file)
                 _image_manager[image] = file_id
-                answer = on_image(message.caption or '', image)
+                if num_parms == 2:
+                    args = (message.caption or '', image)
+                elif num_parms == 3:
+                    args = (message.caption or '', image, message.chat.id)
+                else:
+                    raise ValueError(f'Функция {on_image.__name__} не должна иметь два или три параметра')
+                answer = on_image(*args)
             except Exception as e:
                 bot.send_message(message.from_user.id, f'Возникла ошибка:\n{traceback.format_exc()}')
                 raise
             send_answer(bot, message.from_user.id, answer)
 
     bot.message_handler(content_types=['photo'])(on_image_message)
 
 
 def set_up_default_handler(bot: telebot.TeleBot, main_module: types.ModuleType):
     bot.message_handler(func=lambda message: True)(handle_all_messages)
 
 
 def print_bot_info(bot: telebot.TeleBot):
-    bot_info = bot.get_me()
-    bot_name = bot_info.username
+    try:
+        bot_info = bot.get_me()
+        bot_name = bot_info.username
+    except telebot.apihelper.ApiTelegramException as e:
+        raise ValueError(f'Кажется, токен {bot.token} неправильный.')
 
     print('Бот ждёт: https://t.me/' + bot_name)
 
 
 @bot.message_handler(regexp="^/")
 def handle_all_commands(message: telebot.types.Message):
     cmd = re.search(r'(?<=\/)[a-zA-Z_]*', message.text).group()
@@ -110,16 +133,27 @@
     raise_exc = None
     if not command_function:
         answer = (f"Необходимо определить функцию {command_function_name}. Например:\n"
                   f"def {command_function_name}(cmd: str):\n"
                   f"    return 'Выполнена команда {cmd}, данные: ' + repr(cmd)\n")
         raise_exc = ValueError(answer)
     else:
+        signature = inspect.signature(command_function)
+        num_parms = len(signature.parameters)
+        if num_parms == 0:
+            args = tuple()
+        elif num_parms == 1:
+            args = (message.text,)
+        elif num_parms == 2:
+            args = (message.text, message.chat.id)
+        else:
+            raise ValueError(f'Функция {command_function.__name__} не должна иметь больше двух параметров')
+
         try:
-            answer = command_function(message.text)
+            answer = command_function(*args)
         except Exception as e:
             answer = f'Возникла ошибка:\n{traceback.format_exc()}'
             raise_exc = e
     send_answer(bot, message.from_user.id, answer)
     if raise_exc:
         raise raise_exc
 
@@ -137,16 +171,27 @@
     raise_exc = None
     if not callback_function:
         answer = (f"Необходимо определить функцию {callback_function_name}. Например:\n"
                   f"def {callback_function_name}(data):\n"
                   f"    return 'Нажата кнопка {name}, данные: ' + repr(data)\n")
         raise_exc = ValueError(answer)
     else:
+        signature = inspect.signature(callback_function)
+        num_parms = len(signature.parameters)
+        if num_parms == 0:
+            args = tuple()
+        elif num_parms == 1:
+            args = (data,)
+        elif num_parms == 2:
+            args = (data, callback_obj.message.chat.id)
+        else:
+            raise ValueError(f'Функция {callback_function.__name__} не должна иметь больше двух параметров')
+
         try:
-            answer = callback_function(data)
+            answer = callback_function(*args)
         except Exception as e:
             answer = f'Возникла ошибка:\n{traceback.format_exc()}'
             raise_exc = e
 
     bot.edit_message_reply_markup(chat_id=callback_obj.message.chat.id,
                                   message_id=callback_obj.message.message_id,
                                   reply_markup=None)
@@ -200,15 +245,15 @@
     print_bot_info(bot)
     bot.infinity_polling()
 
 
 def check_run_bot():
     if already_started:
         return
-    raise ValueError('Необходимо добавить функцию run_bot() в конец кода для запуска бота')
+    raise ValueError('Необходимо добавить вызов функции run_bot() в самый конец кода для запуска бота')
 
 
 if __name__ == '__main__':
     print('Модуль должен быть импортирован:\nfrom tgbotzero import *')
     sys.exit()
 
 atexit.register(check_run_bot)
```

### Comparing `tgbotzero-0.0.7/src/tgbotzero/utils/check_on_button_functions.py` & `tgbotzero-0.0.9/src/tgbotzero/utils/check_on_button_functions.py`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/src/tgbotzero/utils/help.py` & `tgbotzero-0.0.9/src/tgbotzero/utils/help.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     print('''# # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 # Вот пример очень простого бота:
 from tgbotzero import *
 
 # Токен нужно получить у https://t.me/BotFather
-TOKEN = '123:tokenFromBotFather'
+TOKEN = '123:123:tokenHereFromBotFatherInTelegram'
 
 # Функция on_message принимает на вход строку с сообщением 
 # и должна вернуть строку с ответом 
 def on_message(msg: str):
     return "Твоё сообщение: " + msg
 
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
```

### Comparing `tgbotzero-0.0.7/src/tgbotzero/utils/images.py` & `tgbotzero-0.0.9/src/tgbotzero/utils/images.py`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/src/tgbotzero/utils/reply_markup.py` & `tgbotzero-0.0.9/src/tgbotzero/utils/reply_markup.py`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/src/tgbotzero/utils/send_answer.py` & `tgbotzero-0.0.9/src/tgbotzero/utils/send_answer.py`

 * *Files identical despite different names*

### Comparing `tgbotzero-0.0.7/src/tgbotzero.egg-info/PKG-INFO` & `tgbotzero-0.0.9/src/tgbotzero.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgbotzero
-Version: 0.0.7
+Version: 0.0.9
 Summary: A zero-boilerplate simple telegram bots
 Home-page: https://github.com/ShashkovS/tgbotzero
 Author: Sergey Shashkov
 Author-email: sh57@yandex.ru
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -49,15 +49,15 @@
 Токен нужно указать в глобальной переменной TOKEN.
 Для обработки текстовых сообщений нужно создать функцию on_message(msg: str). Функция принимает текст сообщения, и может вернуть либо строку с текстом ответа, либо список из сообщений, описаний кнопок и картинок. Про кнопки и картинки будет дальше.
 Для запуска бота нужно выполнить команду `run_bot()` без параметров.
 
 ``` python
 import tgbotzero
 
-TOKEN = '123123123:tokenFromBotFatherInTelegram'
+TOKEN = '123:tokenHereFromBotFatherInTelegram'
 
 def on_message(msg: str):
     return "Твоё сообщение: " + msg
     
 run_bot()
 ```
 
@@ -196,8 +196,28 @@
 
 run_bot()
 ```
 <img alt="puttext" src="https://github.com/ShashkovS/tgbotzero/blob/main/docs/puttext.png?raw=true" width="323">
 
 
 
+
+### Получение chat_id:
+
+К любой функции-обработчику можно добавить ещё один параметр `chat_id: int`, если хочется различать пользователей.
+
+```python
+from tgbotzero import *
+
+TOKEN = '123:tokenHereFromBotFatherInTelegram'
+
+
+def on_message(msg: str, chat_id: int):
+    return f"Текущий chat id: {chat_id}"
+
+
+run_bot()
+```
+
+
+
 # [Contributing](CONTRIBUTING.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tgbotzero Version: 0.0.7 Summary: A zero-
+Metadata-Version: 2.1 Name: tgbotzero Version: 0.0.9 Summary: A zero-
 boilerplate simple telegram bots Home-page: https://github.com/ShashkovS/
 tgbotzero Author: Sergey Shashkov Author-email: sh57@yandex.ru License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: End Users/Desktop Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -24,15 +24,15 @@
 ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ð¹ Ð½ÑÐ¶Ð½Ð¾ ÑÐ¾Ð·Ð´Ð°ÑÑ ÑÑÐ½ÐºÑÐ¸Ñ on_message(msg:
 str). Ð¤ÑÐ½ÐºÑÐ¸Ñ Ð¿ÑÐ¸Ð½Ð¸Ð¼Ð°ÐµÑ ÑÐµÐºÑÑ ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ñ, Ð¸
 Ð¼Ð¾Ð¶ÐµÑ Ð²ÐµÑÐ½ÑÑÑ Ð»Ð¸Ð±Ð¾ ÑÑÑÐ¾ÐºÑ Ñ ÑÐµÐºÑÑÐ¾Ð¼ Ð¾ÑÐ²ÐµÑÐ°,
 Ð»Ð¸Ð±Ð¾ ÑÐ¿Ð¸ÑÐ¾Ðº Ð¸Ð· ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ð¹, Ð¾Ð¿Ð¸ÑÐ°Ð½Ð¸Ð¹ ÐºÐ½Ð¾Ð¿Ð¾Ðº Ð¸
 ÐºÐ°ÑÑÐ¸Ð½Ð¾Ðº. ÐÑÐ¾ ÐºÐ½Ð¾Ð¿ÐºÐ¸ Ð¸ ÐºÐ°ÑÑÐ¸Ð½ÐºÐ¸ Ð±ÑÐ´ÐµÑ
 Ð´Ð°Ð»ÑÑÐµ. ÐÐ»Ñ Ð·Ð°Ð¿ÑÑÐºÐ° Ð±Ð¾ÑÐ° Ð½ÑÐ¶Ð½Ð¾ Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÑ
 ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ `run_bot()` Ð±ÐµÐ· Ð¿Ð°ÑÐ°Ð¼ÐµÑÑÐ¾Ð². ``` python import
-tgbotzero TOKEN = '123123123:tokenFromBotFatherInTelegram' def on_message(msg:
+tgbotzero TOKEN = '123:tokenHereFromBotFatherInTelegram' def on_message(msg:
 str): return "Ð¢Ð²Ð¾Ñ ÑÐ¾Ð¾Ð±ÑÐµÐ½Ð¸Ðµ: " + msg run_bot() ``` [echobot]#
 Ð£ÑÑÐ°Ð½Ð¾Ð²ÐºÐ° ÐÐ²ÐµÐ´Ð¸ÑÐµ Ð² ÑÐµÑÐ¼Ð¸Ð½Ð°Ð»Ðµ: ```shell pip install
 tgbotzero --upgrade --user ``` ÐÐ»Ð¸ Ð·Ð°Ð¿ÑÑÑÐ¸ÑÐµ ÑÑÑ
 Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ: ```python import os, sys python = sys.executable user = '--
 user' if 'venv' not in python and 'envs' not in python else '' cmd = f'"
 {python}" -m pip install tgbotzero --upgrade {user}' os.system(cmd) ``` ###
 ÐÐ¾Ñ Ñ ÐºÐ½Ð¾Ð¿ÐºÐ°Ð¼Ð¸: ÐÐ»Ñ ÑÐ¾Ð³Ð¾ ÑÑÐ¾Ð±Ñ Ð´Ð¾Ð±Ð°Ð²Ð¸ÑÑ Ðº
@@ -83,9 +83,15 @@
 Ð´Ð¾Ð±Ð°Ð²Ð»ÐµÐ½Ð¸Ðµ ÑÐµÐºÑÑÐ°. Ð¡Ð¸Ð½ÑÐ°ÐºÑÐ¸Ñ: `img.put_text(text,
 color)`, Ð³Ð´Ðµ`color` â ÑÑÐ¾ RGB-ÐºÐ¾ÑÑÐµÐ¶, Ð½Ð°Ð¿ÑÐ¸Ð¼ÐµÑ, `(255, 0,
 0)`. ÐÐ·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ Ð¼Ð¾Ð¶Ð½Ð¾ Ð¼Ð¾Ð´Ð¸ÑÐ¸ÑÐ¸ÑÐ¾Ð²Ð°ÑÑ Ð´Ð°Ð¶Ðµ
 ÐµÑÐ»Ð¸ Ð¾Ð½Ð¸ Ð¾ÑÐºÑÑÑÑ Ð¸Ð· ÑÐ°Ð¹Ð»Ð°: `Image(image_filename).put_text
 (text, color)` ```python from tgbotzero import * TOKEN = '123:
 tokenHereFromBotFatherInTelegram' def on_message(msg: str): return 'ÐÐ´Ñ
 ÐºÐ°ÑÑÐ¸Ð½ÐºÑ Ñ Ð¿Ð¾Ð´Ð¿Ð¸ÑÑÑ!' def on_image(msg: str, img: Image):
-return img.put_text(msg, (255, 0, 0)) run_bot() ``` [puttext]# [Contributing]
+return img.put_text(msg, (255, 0, 0)) run_bot() ``` [puttext]###
+ÐÐ¾Ð»ÑÑÐµÐ½Ð¸Ðµ chat_id: Ð Ð»ÑÐ±Ð¾Ð¹ ÑÑÐ½ÐºÑÐ¸Ð¸-Ð¾Ð±ÑÐ°Ð±Ð¾ÑÑÐ¸ÐºÑ
+Ð¼Ð¾Ð¶Ð½Ð¾ Ð´Ð¾Ð±Ð°Ð²Ð¸ÑÑ ÐµÑÑ Ð¾Ð´Ð¸Ð½ Ð¿Ð°ÑÐ°Ð¼ÐµÑÑ `chat_id: int`,
+ÐµÑÐ»Ð¸ ÑÐ¾ÑÐµÑÑÑ ÑÐ°Ð·Ð»Ð¸ÑÐ°ÑÑ Ð¿Ð¾Ð»ÑÐ·Ð¾Ð²Ð°ÑÐµÐ»ÐµÐ¹.
+```python from tgbotzero import * TOKEN = '123:
+tokenHereFromBotFatherInTelegram' def on_message(msg: str, chat_id: int):
+return f"Ð¢ÐµÐºÑÑÐ¸Ð¹ chat id: {chat_id}" run_bot() ``` # [Contributing]
 (CONTRIBUTING.md)
```

### Comparing `tgbotzero-0.0.7/src/tgbotzero.egg-info/SOURCES.txt` & `tgbotzero-0.0.9/src/tgbotzero.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 src/tgbotzero/examples/05_schedule_bot.py
 src/tgbotzero/examples/06_on_start.py
 src/tgbotzero/examples/07_commands.py
 src/tgbotzero/examples/08_send_image.py
 src/tgbotzero/examples/09_image_gallery.py
 src/tgbotzero/examples/10_on_image.py
 src/tgbotzero/examples/11_add_text_on_image.py
-src/tgbotzero/examples/99_demo.py
+src/tgbotzero/examples/12_chat_id_bot.py
 src/tgbotzero/examples/__init__.py
 src/tgbotzero/examples/cat.png
 src/tgbotzero/examples/dog.png
 src/tgbotzero/utils/__init__.py
 src/tgbotzero/utils/botzero.py
 src/tgbotzero/utils/check_on_button_functions.py
 src/tgbotzero/utils/copy_examples.py
```

### Comparing `tgbotzero-0.0.7/tests/test_copy_examples.py` & `tgbotzero-0.0.9/tests/test_copy_examples.py`

 * *Files identical despite different names*

