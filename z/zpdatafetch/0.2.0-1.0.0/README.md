# Comparing `tmp/zpdatafetch-0.2.0.tar.gz` & `tmp/zpdatafetch-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpdatafetch-0.2.0.tar", last modified: Fri May 10 15:00:31 2024, max compression
+gzip compressed data, was "zpdatafetch-1.0.0.tar", last modified: Fri May 10 18:36:53 2024, max compression
```

## Comparing `zpdatafetch-0.2.0.tar` & `zpdatafetch-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxr-x   0 doug       (501) staff       (20)        0 2024-05-10 15:00:31.557799 zpdatafetch-0.2.0/
--rw-rw-r--   0 doug       (501) staff       (20)     1068 2024-05-09 11:00:52.000000 zpdatafetch-0.2.0/LICENSE
--rw-r--r--   0 doug       (501) staff       (20)     1356 2024-05-10 15:00:31.557400 zpdatafetch-0.2.0/PKG-INFO
--rw-rw-r--   0 doug       (501) staff       (20)      944 2024-05-10 14:57:23.000000 zpdatafetch-0.2.0/README.md
--rw-rw-r--   0 doug       (501) staff       (20)      701 2024-05-09 12:19:39.000000 zpdatafetch-0.2.0/pyproject.toml
--rw-rw-r--   0 doug       (501) staff       (20)      644 2024-05-10 15:00:31.558490 zpdatafetch-0.2.0/setup.cfg
-drwxrwxr-x   0 doug       (501) staff       (20)        0 2024-05-10 15:00:31.541258 zpdatafetch-0.2.0/src/
-drwxrwxr-x   0 doug       (501) staff       (20)        0 2024-05-10 15:00:31.547752 zpdatafetch-0.2.0/src/zpdatafetch/
--rw-rw-r--   0 doug       (501) staff       (20)      333 2024-05-10 14:55:28.000000 zpdatafetch-0.2.0/src/zpdatafetch/__init__.py
--rw-rw-r--   0 doug       (501) staff       (20)     2181 2024-05-10 14:55:40.000000 zpdatafetch-0.2.0/src/zpdatafetch/config.py
--rwxrwxr-x   0 doug       (501) staff       (20)     2168 2024-05-10 14:55:45.000000 zpdatafetch-0.2.0/src/zpdatafetch/cyclist.py
--rw-rw-r--   0 doug       (501) staff       (20)     2475 2024-05-10 14:55:48.000000 zpdatafetch-0.2.0/src/zpdatafetch/primes.py
--rw-rw-r--   0 doug       (501) staff       (20)     1538 2024-05-10 14:55:52.000000 zpdatafetch-0.2.0/src/zpdatafetch/result.py
--rw-rw-r--   0 doug       (501) staff       (20)     1598 2024-05-10 14:55:55.000000 zpdatafetch-0.2.0/src/zpdatafetch/signup.py
--rw-rw-r--   0 doug       (501) staff       (20)     1517 2024-05-10 14:56:00.000000 zpdatafetch-0.2.0/src/zpdatafetch/team.py
--rwxrwxr-x   0 doug       (501) staff       (20)     3608 2024-05-10 14:56:03.000000 zpdatafetch-0.2.0/src/zpdatafetch/zp.py
-drwxrwxr-x   0 doug       (501) staff       (20)        0 2024-05-10 15:00:31.556357 zpdatafetch-0.2.0/src/zpdatafetch.egg-info/
--rw-r--r--   0 doug       (501) staff       (20)     1356 2024-05-10 15:00:31.000000 zpdatafetch-0.2.0/src/zpdatafetch.egg-info/PKG-INFO
--rw-rw-r--   0 doug       (501) staff       (20)      576 2024-05-10 15:00:31.000000 zpdatafetch-0.2.0/src/zpdatafetch.egg-info/SOURCES.txt
--rw-rw-r--   0 doug       (501) staff       (20)        1 2024-05-10 15:00:31.000000 zpdatafetch-0.2.0/src/zpdatafetch.egg-info/dependency_links.txt
--rw-rw-r--   0 doug       (501) staff       (20)       65 2024-05-10 15:00:31.000000 zpdatafetch-0.2.0/src/zpdatafetch.egg-info/requires.txt
--rw-rw-r--   0 doug       (501) staff       (20)       12 2024-05-10 15:00:31.000000 zpdatafetch-0.2.0/src/zpdatafetch.egg-info/top_level.txt
-drwxrwxr-x   0 doug       (501) staff       (20)        0 2024-05-10 15:00:31.555138 zpdatafetch-0.2.0/test/
--rw-rw-r--   0 doug       (501) staff       (20)      806 2024-05-10 14:56:39.000000 zpdatafetch-0.2.0/test/test_config.py
--rw-rw-r--   0 doug       (501) staff       (20)       56 2024-05-10 09:01:56.000000 zpdatafetch-0.2.0/test/test_cyclist.py
--rw-rw-r--   0 doug       (501) staff       (20)       53 2024-05-10 09:02:40.000000 zpdatafetch-0.2.0/test/test_primes.py
--rw-rw-r--   0 doug       (501) staff       (20)       53 2024-05-10 09:04:34.000000 zpdatafetch-0.2.0/test/test_result.py
--rw-rw-r--   0 doug       (501) staff       (20)       53 2024-05-10 09:04:48.000000 zpdatafetch-0.2.0/test/test_signup.py
--rw-rw-r--   0 doug       (501) staff       (20)       47 2024-05-10 09:03:56.000000 zpdatafetch-0.2.0/test/test_team.py
--rw-rw-r--   0 doug       (501) staff       (20)      751 2024-05-09 14:35:31.000000 zpdatafetch-0.2.0/test/test_zp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:36:53.531396 zpdatafetch-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-10 18:36:53.531396 zpdatafetch-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 18:36:53.531396 zpdatafetch-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:36:53.527397 zpdatafetch-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:36:53.531396 zpdatafetch-1.0.0/src/zpdatafetch/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/src/zpdatafetch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1249 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/src/zpdatafetch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/src/zpdatafetch/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2168 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/src/zpdatafetch/cyclist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/src/zpdatafetch/primes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/src/zpdatafetch/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/src/zpdatafetch/signup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/src/zpdatafetch/team.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3608 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/src/zpdatafetch/zp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:36:53.531396 zpdatafetch-1.0.0/src/zpdatafetch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-10 18:36:53.000000 zpdatafetch-1.0.0/src/zpdatafetch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-10 18:36:53.000000 zpdatafetch-1.0.0/src/zpdatafetch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 18:36:53.000000 zpdatafetch-1.0.0/src/zpdatafetch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 18:36:53.000000 zpdatafetch-1.0.0/src/zpdatafetch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-10 18:36:53.000000 zpdatafetch-1.0.0/src/zpdatafetch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 18:36:53.000000 zpdatafetch-1.0.0/src/zpdatafetch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:36:53.531396 zpdatafetch-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/test/test_cyclist.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/test/test_primes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/test/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/test/test_signup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/test/test_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-10 18:36:38.000000 zpdatafetch-1.0.0/test/test_zp.py
```

### Comparing `zpdatafetch-0.2.0/LICENSE` & `zpdatafetch-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zpdatafetch-0.2.0/setup.cfg` & `zpdatafetch-1.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [metadata]
 name = zpdatafetch
-version = 0.2.0
+version = 1.0.0
 url = https://github.com/puckdoug/zpdatafetch
 author = Doug Morris
 author_email = "Doug Morris" <doug@mhost.com>
 description = A package for fetching data from Zwiftpower
 long_description = file: README.md
 long_description_content_type = text/markdown
+license = MIT
 
 [options]
 package_dir = 
 	=src
 packages = find:
 install_requires = 
 	httpx>=0.27.0
```

### Comparing `zpdatafetch-0.2.0/src/zpdatafetch/config.py` & `zpdatafetch-1.0.0/src/zpdatafetch/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 from getpass import getpass
 # ===============================================================================
 
 
 class Config:
   verbose: bool = False
   domain: str = 'zpdatafetch'
-  username: str = None
-  password: str = None
-  keyring: keyring.backend.KeyringBackend
+  username: str = ''
+  password: str = ''
 
   # -----------------------------------------------------------------------------
   def __init__(self):
-    self.keyring = keyring.get_keyring()
+    self.kr = keyring.get_keyring()
 
   #   self.load()
 
   # -----------------------------------------------------------------------------
   def set_keyring(self, kr):
     keyring.set_keyring(kr)
 
@@ -28,29 +27,35 @@
   # -----------------------------------------------------------------------------
   def save(self):
     keyring.set_password(self.domain, 'username', self.username)
     keyring.set_password(self.domain, 'password', self.password)
 
   # -----------------------------------------------------------------------------
   def load(self):
-    self.username = keyring.get_password(self.domain, 'username')
-    self.password = keyring.get_password(self.domain, 'password')
+    u = keyring.get_password(self.domain, 'username')
+    if u:
+      self.username = u
+    p = keyring.get_password(self.domain, 'password')
+    if p:
+      self.password = p
 
   # -----------------------------------------------------------------------------
   def setup(self, username='', password=''):
     if username:
       self.username = username
     else:
       self.username = input('zwiftpower username (for use with zpdatafetch): ')
       keyring.set_password(self.domain, 'username', self.username)
 
     if password:
       self.password = password
     else:
-      self.password = getpass('zwiftpower password (for use with zpdatafetch): ')
+      self.password = getpass(
+        'zwiftpower password (for use with zpdatafetch): '
+      )
       keyring.set_password(self.domain, 'password', self.password)
 
   # -----------------------------------------------------------------------------
   def dump(self):
     print(f'username: {self.username}')
     print(f'password: {self.password}')
```

### Comparing `zpdatafetch-0.2.0/src/zpdatafetch/cyclist.py` & `zpdatafetch-1.0.0/src/zpdatafetch/cyclist.py`

 * *Files identical despite different names*

### Comparing `zpdatafetch-0.2.0/src/zpdatafetch/primes.py` & `zpdatafetch-1.0.0/src/zpdatafetch/primes.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,16 +42,18 @@
       for cat in self._cat:
         if cat not in p[race]:
           p[race][cat] = {}
         for primetype in self._type:
           url = f'{self._url_base}{self._url_race_id}{race}{self._url_category}{cat}{self._url_primetype}{primetype}&_={ts}'
           res = zp.fetch_json(url)
           if self.verbose:
-            if len(res['data']) == 0:
-              print('No Results')
+            if 'data' not in res:
+              print(f'No Results for {primetype} in pen {cat}')
+            elif len(res['data']) == 0:
+              print(f'No Results for {primetype} in pen {cat}')
             else:
               print(f'Results found for {primetype} in pen {cat}')
           p[race][cat][primetype] = res
           ts = ts + 1
 
     self.raw = p
```

### Comparing `zpdatafetch-0.2.0/src/zpdatafetch/result.py` & `zpdatafetch-1.0.0/src/zpdatafetch/result.py`

 * *Files identical despite different names*

### Comparing `zpdatafetch-0.2.0/src/zpdatafetch/signup.py` & `zpdatafetch-1.0.0/src/zpdatafetch/signup.py`

 * *Files identical despite different names*

### Comparing `zpdatafetch-0.2.0/src/zpdatafetch/team.py` & `zpdatafetch-1.0.0/src/zpdatafetch/team.py`

 * *Files identical despite different names*

### Comparing `zpdatafetch-0.2.0/src/zpdatafetch/zp.py` & `zpdatafetch-1.0.0/src/zpdatafetch/zp.py`

 * *Files identical despite different names*

### Comparing `zpdatafetch-0.2.0/src/zpdatafetch.egg-info/SOURCES.txt` & `zpdatafetch-1.0.0/src/zpdatafetch.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/zpdatafetch/__init__.py
+src/zpdatafetch/cli.py
 src/zpdatafetch/config.py
 src/zpdatafetch/cyclist.py
 src/zpdatafetch/primes.py
 src/zpdatafetch/result.py
 src/zpdatafetch/signup.py
 src/zpdatafetch/team.py
 src/zpdatafetch/zp.py
 src/zpdatafetch.egg-info/PKG-INFO
 src/zpdatafetch.egg-info/SOURCES.txt
 src/zpdatafetch.egg-info/dependency_links.txt
+src/zpdatafetch.egg-info/entry_points.txt
 src/zpdatafetch.egg-info/requires.txt
 src/zpdatafetch.egg-info/top_level.txt
 test/test_config.py
 test/test_cyclist.py
 test/test_primes.py
 test/test_result.py
 test/test_signup.py
```

### Comparing `zpdatafetch-0.2.0/test/test_config.py` & `zpdatafetch-1.0.0/test/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 
 def test_setup(config):
   assert config is not None
 
 
 def test_setup_has_no_default_creds(config):
-  assert config.username is None
-  assert config.password is None
+  assert config.username is ''
+  assert config.password is ''
 
 
 def test_domain_can_be_changed(config):
   config.domain = 'test-zpdatafetch'
   assert config.domain == 'test-zpdatafetch'
 
 
 def test_load_config_has_no_creds_before_set(config):
   config.domain = 'test-zpdatafetch'
   config.load()
-  assert config.username is None
-  assert config.password is None
+  assert config.username is ''
+  assert config.password is ''
 
 
 def test_after_load_config_has_creds(config):
   tuser = 'test_username'
   tpass = 'test_password'
   config.set_keyring(PlaintextKeyring())
   config.domain = 'test-zpdatafetch'
```

### Comparing `zpdatafetch-0.2.0/test/test_zp.py` & `zpdatafetch-1.0.0/test/test_zp.py`

 * *Files identical despite different names*

