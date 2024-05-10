# Comparing `tmp/remindmail-2024.4.29.2.tar.gz` & `tmp/remindmail-2024.5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2024.4.29.2.tar", last modified: Tue Apr 30 05:22:58 2024, max compression
+gzip compressed data, was "remindmail-2024.5.9.1.tar", last modified: Fri May 10 05:34:15 2024, max compression
```

## Comparing `remindmail-2024.4.29.2.tar` & `remindmail-2024.5.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 05:22:58.073754 remindmail-2024.4.29.2/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.29.2/LICENSE.md
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-30 05:22:58.073754 remindmail-2024.4.29.2/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6239 2024-04-16 03:57:58.000000 remindmail-2024.4.29.2/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.29.2/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-30 05:22:58.073754 remindmail-2024.4.29.2/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 05:22:58.069754 remindmail-2024.4.29.2/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 05:22:58.073754 remindmail-2024.4.29.2/src/remind/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.29.2/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2927 2024-04-21 19:03:57.000000 remindmail-2024.4.29.2/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 23:49:35.000000 remindmail-2024.4.29.2/src/remind/error_handler.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11832 2024-04-30 05:19:56.000000 remindmail-2024.4.29.2/src/remind/query_manager.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    10846 2024-04-28 18:42:11.000000 remindmail-2024.4.29.2/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    24388 2024-04-28 19:22:42.000000 remindmail-2024.4.29.2/src/remind/reminder_confirmation.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    18650 2024-04-21 19:03:57.000000 remindmail-2024.4.29.2/src/remind/reminder_manager.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 05:22:58.073754 remindmail-2024.4.29.2/src/remindmail.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-30 05:22:58.000000 remindmail-2024.4.29.2/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-30 05:22:58.000000 remindmail-2024.4.29.2/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-30 05:22:58.000000 remindmail-2024.4.29.2/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-30 05:22:58.000000 remindmail-2024.4.29.2/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-30 05:22:58.000000 remindmail-2024.4.29.2/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-10 05:34:15.751940 remindmail-2024.5.9.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.5.9.1/LICENSE.md
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6599 2024-05-10 05:34:15.751940 remindmail-2024.5.9.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6239 2024-04-16 03:57:58.000000 remindmail-2024.5.9.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.5.9.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-05-10 05:34:15.751940 remindmail-2024.5.9.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-10 05:34:15.747940 remindmail-2024.5.9.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-10 05:34:15.751940 remindmail-2024.5.9.1/src/remind/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.5.9.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2927 2024-04-21 19:03:57.000000 remindmail-2024.5.9.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 23:49:35.000000 remindmail-2024.5.9.1/src/remind/error_handler.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11832 2024-04-30 05:19:56.000000 remindmail-2024.5.9.1/src/remind/query_manager.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    10812 2024-05-10 05:33:22.000000 remindmail-2024.5.9.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    24388 2024-04-28 19:22:42.000000 remindmail-2024.5.9.1/src/remind/reminder_confirmation.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    18788 2024-05-10 05:33:56.000000 remindmail-2024.5.9.1/src/remind/reminder_manager.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-10 05:34:15.751940 remindmail-2024.5.9.1/src/remindmail.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6599 2024-05-10 05:34:15.000000 remindmail-2024.5.9.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-05-10 05:34:15.000000 remindmail-2024.5.9.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-05-10 05:34:15.000000 remindmail-2024.5.9.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-05-10 05:34:15.000000 remindmail-2024.5.9.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-05-10 05:34:15.000000 remindmail-2024.5.9.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2024.4.29.2/LICENSE.md` & `remindmail-2024.5.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.29.2/PKG-INFO` & `remindmail-2024.5.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.29.2
+Version: 2024.5.9.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `remindmail-2024.4.29.2/README.md` & `remindmail-2024.5.9.1/README.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.29.2/setup.cfg` & `remindmail-2024.5.9.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2024.04.29.2
+version = 2024.05.09.1
 author = Tyler Woodfin
 author_email = feedback-remindmail@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2024.4.29.2/src/remind/__main__.py` & `remindmail-2024.5.9.1/src/remind/__main__.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.29.2/src/remind/error_handler.py` & `remindmail-2024.5.9.1/src/remind/error_handler.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.29.2/src/remind/query_manager.py` & `remindmail-2024.5.9.1/src/remind/query_manager.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.29.2/src/remind/reminder.py` & `remindmail-2024.5.9.1/src/remind/reminder.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,25 +71,25 @@
         title (str): The title or main content of the reminder.
         notes (str): Additional notes associated with the reminder.
         cabinet (Cabinet): instance of Cabinet, a file management tool
         mail (Mail): The instance in which to send reminders as emails
         path_remind_file: The path from ReminderManager in which to access remind.md
     """
     def __init__(self,
-                 key: ReminderKeyType,
+                 key,
                  value: Optional[str],
                  frequency: Optional[int],
                  offset: int,
                  modifiers: str,
                  title: str,
                  notes: Optional[str],
                  cabinet: Cabinet,
                  mail: Mail,
                  path_remind_file: str | None):
-        self.key: ReminderKeyType = key
+        self.key = key
         self.value: Optional[str] = value
         self.frequency: int = frequency or 0
         self.offset: int = offset
         self.modifiers: str = modifiers
         self.title: str = title
         self.notes: Optional[str] = notes
         self.should_send_today: Optional[bool] = False
```

### Comparing `remindmail-2024.4.29.2/src/remind/reminder_confirmation.py` & `remindmail-2024.5.9.1/src/remind/reminder_confirmation.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.29.2/src/remind/reminder_manager.py` & `remindmail-2024.5.9.1/src/remind/reminder_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import re
 import os
 import subprocess
 import sys
 import glob
 import readline
-from datetime import date, timedelta
+from datetime import date, timedelta, datetime
 from typing import List, Optional
 from rich.console import Console
 from remind.reminder import ReminderKeyType
 from cabinet import Cabinet, Mail
 from . import reminder, error_handler
 
 def complete_file_input(text, state):
@@ -132,15 +132,14 @@
                         r"thu(rsday)?|"
                         r"fri(day)?|"
                         r"sat(urday)?)$"
                     )
 
                     match = re.match(pattern_any_reminder, stripped_line)
                     if match:
-                        reminder_key: ReminderKeyType
                         details, reminder_modifiers, title = match.groups()
                         details = details.lower()
 
                         details = details.split(",")
 
                         # get reminder type
                         try:
@@ -303,23 +302,28 @@
                 self.console.print(r.title, style="bold green")
                 print(r.notes)
 
     def show_reminders_for_days(self, limit: int = 8) -> None:
         """
         Displays reminders scheduled for the upcoming <limit> days.
 
-        This method calculates the dates for the next <limit> days, starting from tomorrow,
-        and checks each day for scheduled reminders. For each day, it prints the date
+        This method calculates the dates for the next <limit> days, starting from tomorrow
+        (today if between midnight and 4am),
+        and it checks each day for scheduled reminders. For each day, it prints the date
         and any corresponding reminders. If there are no reminders for a specific day,
         it indicates so. Reminders with specific modifiers change the display style
         to highlight their importance or category.
         """
 
+        current_time = datetime.now().time()
+        start_day_offset = 0 if current_time.hour < 4 else 1
+
         # Prepare the next 7 days
-        dates = [date.today() + timedelta(days=i) for i in range(1, limit)]
+        dates = [date.today() + timedelta(days=i) for i in range(
+            start_day_offset, limit)]
 
         # Parse reminders file if necessary
         if not self.parsed_reminders:
             self.parse_reminders_file()
 
         # Iterate through each upcoming day
         for day in dates:
```

### Comparing `remindmail-2024.4.29.2/src/remindmail.egg-info/PKG-INFO` & `remindmail-2024.5.9.1/src/remindmail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.29.2
+Version: 2024.5.9.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

