# Comparing `tmp/ntdrt-1.8.0.tar.gz` & `tmp/ntdrt-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ntdrt-1.8.0.tar", last modified: Fri Apr  9 07:11:10 2021, max compression
+gzip compressed data, was "dist\ntdrt-1.9.0.tar", last modified: Sun Apr 11 07:33:18 2021, max compression
```

## Comparing `ntdrt-1.8.0.tar` & `ntdrt-1.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-04-09 07:11:10.000000 ntdrt-1.8.0/
-drwxrwxrwx   0        0        0        0 2021-04-09 07:11:10.000000 ntdrt-1.8.0/ntdrt/
--rw-rw-rw-   0        0        0     9597 2020-09-05 16:09:24.000000 ntdrt-1.8.0/ntdrt/log.py
--rw-rw-rw-   0        0        0     6074 2021-02-24 20:24:26.000000 ntdrt-1.8.0/ntdrt/process.py
--rw-rw-rw-   0        0        0     2634 2021-04-09 07:06:43.000000 ntdrt-1.8.0/ntdrt/threads.py
--rw-rw-rw-   0        0        0        0 2019-09-20 09:43:54.000000 ntdrt-1.8.0/ntdrt/__init__.py
--rw-rw-rw-   0        0        0       23 2021-04-09 07:11:07.000000 ntdrt-1.8.0/ntdrt/__version__.py
-drwxrwxrwx   0        0        0        0 2021-04-09 07:11:10.000000 ntdrt-1.8.0/ntdrt.egg-info/
--rw-rw-rw-   0        0        0        1 2021-04-09 07:11:09.000000 ntdrt-1.8.0/ntdrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-02-24 19:04:47.000000 ntdrt-1.8.0/ntdrt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      261 2021-04-09 07:11:09.000000 ntdrt-1.8.0/ntdrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2021-04-09 07:11:10.000000 ntdrt-1.8.0/ntdrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2021-04-09 07:11:09.000000 ntdrt-1.8.0/ntdrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      261 2021-04-09 07:11:10.000000 ntdrt-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0       12 2021-04-09 07:09:28.000000 ntdrt-1.8.0/README.md
--rw-rw-rw-   0        0        0       42 2021-04-09 07:11:10.000000 ntdrt-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0      562 2021-02-24 20:06:13.000000 ntdrt-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-04-11 07:33:18.000000 ntdrt-1.9.0/
+drwxrwxrwx   0        0        0        0 2021-04-11 07:33:18.000000 ntdrt-1.9.0/ntdrt/
+-rw-rw-rw-   0        0        0    10023 2021-04-11 07:32:13.000000 ntdrt-1.9.0/ntdrt/log.py
+-rw-rw-rw-   0        0        0     6074 2021-02-24 20:24:26.000000 ntdrt-1.9.0/ntdrt/process.py
+-rw-rw-rw-   0        0        0     2634 2021-04-09 07:06:43.000000 ntdrt-1.9.0/ntdrt/threads.py
+-rw-rw-rw-   0        0        0        0 2019-09-20 09:43:54.000000 ntdrt-1.9.0/ntdrt/__init__.py
+-rw-rw-rw-   0        0        0       23 2021-04-11 07:33:16.000000 ntdrt-1.9.0/ntdrt/__version__.py
+drwxrwxrwx   0        0        0        0 2021-04-11 07:33:18.000000 ntdrt-1.9.0/ntdrt.egg-info/
+-rw-rw-rw-   0        0        0        1 2021-04-11 07:33:18.000000 ntdrt-1.9.0/ntdrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-02-24 19:04:47.000000 ntdrt-1.9.0/ntdrt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      261 2021-04-11 07:33:18.000000 ntdrt-1.9.0/ntdrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2021-04-11 07:33:18.000000 ntdrt-1.9.0/ntdrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        6 2021-04-11 07:33:18.000000 ntdrt-1.9.0/ntdrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      261 2021-04-11 07:33:18.000000 ntdrt-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2021-04-09 07:09:28.000000 ntdrt-1.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2021-04-11 07:33:18.000000 ntdrt-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      562 2021-02-24 20:06:13.000000 ntdrt-1.9.0/setup.py
```

### Comparing `ntdrt-1.8.0/ntdrt/log.py` & `ntdrt-1.9.0/ntdrt/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,16 +136,20 @@
         self.max_level = exclusive_maximum
 
     def filter(self, record):
         return 1 if record.levelno < self.max_level else 0
 
 
 class BufferingSMTPHandler(logging.Handler):
+    ENCRYPTION_STARTTLS = "starttls"
+    ENCRYPTION_TLS = "tls"
+
     credentials = None
-    secure = False
+    encryption = None
+    secure = False  # = starttls backward compatibility
     timeout = 5.0
 
     timer = None
     buffer = None
     last_flush = 0
     flush_timeouts = None
     flush_timeout_current = 0
@@ -226,19 +230,26 @@
 
         content = []
         for record in self.buffer:
             content.append(self.format(record))
         message.set_content("\n".join(content))
 
         host, port = self.get_host_port()
-        smtp = smtplib.SMTP(host, port, timeout=self.timeout)
 
-        if self.secure:
-            smtp.starttls()
-            smtp.ehlo()
+        if self.encryption == self.ENCRYPTION_TLS:
+            if port is None:
+                port = smtplib.SMTP_SSL_PORT
+            smtp = smtplib.SMTP_SSL(host, port, timeout=self.timeout)
+        else:
+            if port is None:
+                port = smtplib.SMTP_PORT
+            smtp = smtplib.SMTP(host, port, timeout=self.timeout)
+
+            if self.encryption == self.ENCRYPTION_STARTTLS or self.secure:
+                smtp.starttls()
 
         username, password = self.get_credentials()
         if username is not None:
             smtp.login(username, password)
 
         smtp.send_message(message)
         smtp.quit()
@@ -248,15 +259,15 @@
         if isinstance(recipients, str):
             recipients = [recipients]
         return recipients
 
     def get_host_port(self):
         if isinstance(self.host, (list, tuple)):
             return self.host
-        return self.host, smtplib.SMTP_PORT
+        return self.host, None
 
     def get_credentials(self):
         if isinstance(self.credentials, (list, tuple)):
             return self.credentials
         elif self.credentials is not None:
             raise Exception("unsupported credentials format: " + str(type(self.credentials)))
         return None, None
```

### Comparing `ntdrt-1.8.0/ntdrt/process.py` & `ntdrt-1.9.0/ntdrt/process.py`

 * *Files identical despite different names*

### Comparing `ntdrt-1.8.0/ntdrt/threads.py` & `ntdrt-1.9.0/ntdrt/threads.py`

 * *Files identical despite different names*

### Comparing `ntdrt-1.8.0/setup.py` & `ntdrt-1.9.0/setup.py`

 * *Files identical despite different names*

