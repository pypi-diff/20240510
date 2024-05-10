# Comparing `tmp/comwatt-0.5.0.tar.gz` & `tmp/comwatt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comwatt-0.5.0.tar", last modified: Wed May  8 16:31:49 2024, max compression
+gzip compressed data, was "comwatt-0.6.0.tar", last modified: Fri May 10 06:21:15 2024, max compression
```

## Comparing `comwatt-0.5.0.tar` & `comwatt-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:31:49.223131 comwatt-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-08 16:31:45.000000 comwatt-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 16:31:49.223131 comwatt-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 16:31:45.000000 comwatt-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:31:49.219131 comwatt-0.5.0/comwatt/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-05-08 16:31:45.000000 comwatt-0.5.0/comwatt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:31:49.223131 comwatt-0.5.0/comwatt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 16:31:49.000000 comwatt-0.5.0/comwatt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-08 16:31:49.000000 comwatt-0.5.0/comwatt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:31:49.000000 comwatt-0.5.0/comwatt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 16:31:49.000000 comwatt-0.5.0/comwatt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 16:31:49.000000 comwatt-0.5.0/comwatt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 16:31:45.000000 comwatt-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:31:49.223131 comwatt-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 16:31:45.000000 comwatt-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:21:15.837944 comwatt-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-10 06:21:06.000000 comwatt-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 06:21:15.837944 comwatt-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-10 06:21:06.000000 comwatt-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:21:15.837944 comwatt-0.6.0/comwatt/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5338 2024-05-10 06:21:06.000000 comwatt-0.6.0/comwatt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:21:15.837944 comwatt-0.6.0/comwatt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 06:21:15.000000 comwatt-0.6.0/comwatt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-10 06:21:15.000000 comwatt-0.6.0/comwatt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:21:15.000000 comwatt-0.6.0/comwatt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 06:21:15.000000 comwatt-0.6.0/comwatt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 06:21:15.000000 comwatt-0.6.0/comwatt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-10 06:21:06.000000 comwatt-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:21:15.837944 comwatt-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 06:21:06.000000 comwatt-0.6.0/setup.py
```

### Comparing `comwatt-0.5.0/LICENSE` & `comwatt-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comwatt-0.5.0/comwatt/__init__.py` & `comwatt-0.6.0/comwatt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,19 +67,14 @@
         self.email = email
         self.password = password
 
         self.login()
 
         self.last_refresh_time = 0
 
-    # def wait_element_by_name(self, name):
-    #     try:
-    #         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.NAME, name))
-    #     except:
-
     def login(self):
 
         # Get the login page
         super().get('https://energy.comwatt.com/#/login/')
 
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.NAME, 'email'))
 
@@ -103,28 +98,26 @@
         # Wait home page
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'css-3kduam'))
 
         m = re.match("https://energy.comwatt.com/#/sites/([abcdef0123456789]+)/home", self.current_url)
         
         self.default_site = m.group(1)
 
-
     def get(self, url, title=None):
         
         # First try
         super().get(url)
 
         # Back to login page -> retry logins
         if self.current_url == URL_LOGIN:
             self.login()
 
             # Second try
             super().get(url)
 
-
     def meter(self, site=None):
 
         if not site:
             site = self.default_site
 
         self.get('https://energy.comwatt.com/#/sites/%s/meter/' % site)
         WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'css-3kduam'))
@@ -132,15 +125,14 @@
         elem = self.find_element(By.CLASS_NAME, 'css-3kduam')
 
         data = elem.text
         assert data[-1] == "%"
         assert data[:-1].isdigit()
         return int(data[:-1])
 
-
     def refresh(self, site=None):
 
         if not site:
             site = self.default_site
 
         self.zones = []
 
@@ -186,15 +178,14 @@
                     
                     if unit == "kW":
                         value *= 1000
 
                     device.initialized = True
                     device.value_instant = value
 
-
     def get_devices(self, device_type):
 
         now = time.time()
 
         if self.last_refresh_time + 1 < now:
             self.refresh()
             self.last_refresh_time = now
@@ -203,7 +194,11 @@
 
         for zone in self.zones:
             for device in zone.devices:
                 if device.type == device_type:
                     list_devices.append(device)
 
         return list_devices
+
+    def __del__(self):
+        # Close all browser windows
+        self.quit()
```

