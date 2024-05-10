# Comparing `tmp/logginger-0.0.4.tar.gz` & `tmp/logginger-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logginger-0.0.4.tar", max compression
+gzip compressed data, was "logginger-0.0.5.tar", max compression
```

## Comparing `logginger-0.0.4.tar` & `logginger-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-05-10 12:51:49.562627 logginger-0.0.4/LICENSE
--rw-r--r--   0        0        0     4107 2024-05-10 12:50:15.987048 logginger-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-05-10 13:43:58.288423 logginger-0.0.4/logginger/__init__.py
--rw-r--r--   0        0        0      134 2024-05-10 16:46:05.449184 logginger-0.0.4/logginger/config.py
--rw-r--r--   0        0        0      333 2024-05-10 15:16:32.900348 logginger-0.0.4/logginger/fmts.py
--rw-r--r--   0        0        0     3289 2024-05-10 16:19:52.578314 logginger-0.0.4/logginger/formatters.py
--rw-r--r--   0        0        0     7674 2024-05-10 16:46:05.452178 logginger-0.0.4/logginger/slack/__init__.py
--rw-r--r--   0        0        0      477 2024-05-10 12:02:14.121035 logginger-0.0.4/logginger/slack/colors.py
--rw-r--r--   0        0        0      229 2024-05-10 13:05:24.360119 logginger-0.0.4/logginger/utils.py
--rw-r--r--   0        0        0     1873 2024-05-10 15:20:31.721410 logginger-0.0.4/logginger/uvicorn/__init__.py
--rw-r--r--   0        0        0      479 2024-05-10 17:08:27.239878 logginger-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 logginger-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 12:51:49.562627 logginger-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4107 2024-05-10 12:50:15.987048 logginger-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 13:43:58.288423 logginger-0.0.5/logginger/__init__.py
+-rw-r--r--   0        0        0      134 2024-05-10 16:46:05.449184 logginger-0.0.5/logginger/config.py
+-rw-r--r--   0        0        0      333 2024-05-10 18:36:00.340204 logginger-0.0.5/logginger/fmts.py
+-rw-r--r--   0        0        0     3015 2024-05-10 18:34:08.416505 logginger-0.0.5/logginger/formatters.py
+-rw-r--r--   0        0        0     7685 2024-05-10 18:01:38.985607 logginger-0.0.5/logginger/slack/__init__.py
+-rw-r--r--   0        0        0      477 2024-05-10 12:02:14.121035 logginger-0.0.5/logginger/slack/colors.py
+-rw-r--r--   0        0        0      229 2024-05-10 13:05:24.360119 logginger-0.0.5/logginger/utils.py
+-rw-r--r--   0        0        0     1873 2024-05-10 15:20:31.721410 logginger-0.0.5/logginger/uvicorn/__init__.py
+-rw-r--r--   0        0        0      479 2024-05-10 18:36:15.405336 logginger-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 logginger-0.0.5/PKG-INFO
```

### Comparing `logginger-0.0.4/LICENSE` & `logginger-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `logginger-0.0.4/README.md` & `logginger-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `logginger-0.0.4/logginger/formatters.py` & `logginger-0.0.5/logginger/formatters.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,29 +65,23 @@
                 record_copy.msg = record_copy.__dict__["color_message"]
                 record_copy.__dict__["message"] = record_copy.getMessage()
         record_copy.__dict__["levelprefix"] = levelname + ":" + seperator
         return super().formatMessage(record_copy)
 
 
 class DefaultFormatter(ColorizedFormatter):
-    def should_use_colors(self) -> bool:
-        return sys.stderr.isatty()  # pragma: no cover
+    pass
 
 
 class NoStacktraceFormatter(ColorizedFormatter):
     """
     By default, the stacktrace will be formatted as part of the message.
     Since we want the stacktrace to be in the attachment of the Slack message,
         we need a custom formatter to leave it out of the message
     """
 
     def formatException(self, ei):
         return None
 
-    def format(self, record: LogRecord):
-        # Work-around for https://bugs.python.org/issue29056
-        saved_exc_text = record.exc_text
+    def formatMessage(self, record: LogRecord) -> str:
         record.exc_text = None
-        try:
-            return super(NoStacktraceFormatter, self).format(record)
-        finally:
-            record.exc_text = saved_exc_text
+        return super().formatMessage(record)
```

### Comparing `logginger-0.0.4/logginger/slack/__init__.py` & `logginger-0.0.5/logginger/slack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     Logging filter to decide when logging to Slack is requested, using
     the `extra` kwargs:
 
         `logger.info("...", extra={'notify_slack': True})`
     """
 
-    def filter(self, record):
+    def filter(self, record: LogRecord):
         return getattr(record, "notify_slack", False)
 
 
 class SlackLogHandler(Handler):
     def __init__(
         self,
         slack_token: Optional[str] = None,
```

### Comparing `logginger-0.0.4/logginger/uvicorn/__init__.py` & `logginger-0.0.5/logginger/uvicorn/__init__.py`

 * *Files identical despite different names*

### Comparing `logginger-0.0.4/PKG-INFO` & `logginger-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logginger
-Version: 0.0.4
+Version: 0.0.5
 Summary: Logginger is a simple logging library that includes tools to extend the logging module.
 Author: Hikmat Samadov
 Author-email: hikmat@cublya.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

