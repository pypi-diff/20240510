# Comparing `tmp/slpkg-5.0.7.tar.gz` & `tmp/slpkg-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slpkg-5.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "slpkg-5.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `slpkg-5.0.7.tar` & `slpkg-5.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1945 2024-05-07 07:23:19.000000 slpkg-5.0.7/README.md
--rw-r--r--   0        0        0     1693 2024-05-07 07:23:19.000000 slpkg-5.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/binaries/__init__.py
--rw-r--r--   0        0        0     9687 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/binaries/install.py
--rw-r--r--   0        0        0     2284 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/binaries/required.py
--rw-r--r--   0        0        0     1117 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/blacklist.py
--rw-r--r--   0        0        0     7545 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/check_updates.py
--rw-r--r--   0        0        0     1558 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/checks.py
--rw-r--r--   0        0        0     1856 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/checksum.py
--rw-r--r--   0        0        0     4548 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/choose_packages.py
--rw-r--r--   0        0        0      948 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/cleanings.py
--rw-r--r--   0        0        0     5722 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/configs.py
--rw-r--r--   0        0        0     4783 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/dependees.py
--rw-r--r--   0        0        0     2080 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/dialog_box.py
--rw-r--r--   0        0        0     5293 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/dialog_configs.py
--rw-r--r--   0        0        0     4699 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/download_only.py
--rw-r--r--   0        0        0     4283 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/downloader.py
--rw-r--r--   0        0        0      667 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/error_messages.py
--rw-r--r--   0        0        0     2284 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/find_installed.py
--rw-r--r--   0        0        0     1558 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/gpg_verify.py
--rw-r--r--   0        0        0    10625 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/install_data.py
--rw-r--r--   0        0        0     4211 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/load_data.py
--rw-r--r--   0        0        0    29927 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/main.py
--rw-r--r--   0        0        0     6630 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/multi_process.py
--rw-r--r--   0        0        0    12003 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/new_configs.py
--rw-r--r--   0        0        0     3207 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/progress_bar.py
--rw-r--r--   0        0        0     6881 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/remove_packages.py
--rw-r--r--   0        0        0     5389 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/repo_info.py
--rw-r--r--   0        0        0    18095 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/repositories.py
--rw-r--r--   0        0        0        0 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/sbos/__init__.py
--rw-r--r--   0        0        0      858 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/sbos/dependencies.py
--rw-r--r--   0        0        0     5192 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/sbos/sbo_generate.py
--rw-r--r--   0        0        0    13290 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/sbos/slackbuild.py
--rw-r--r--   0        0        0     3684 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/search.py
--rw-r--r--   0        0        0      712 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/toml_errors.py
--rw-r--r--   0        0        0     5185 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/tracking.py
--rw-r--r--   0        0        0     6878 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/update_repositories.py
--rw-r--r--   0        0        0    11475 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/upgrade.py
--rw-r--r--   0        0        0     9832 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/utilities.py
--rw-r--r--   0        0        0        0 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/__init__.py
--rw-r--r--   0        0        0     6757 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/asciibox.py
--rw-r--r--   0        0        0     6696 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/cli_menu.py
--rw-r--r--   0        0        0      690 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/version.py
--rw-r--r--   0        0        0     8072 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/view_package.py
--rw-r--r--   0        0        0     1942 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/view_process.py
--rw-r--r--   0        0        0    12662 2024-05-07 07:23:19.000000 slpkg-5.0.7/slpkg/views/views.py
--rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 slpkg-5.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1945 2024-05-10 20:55:25.000000 slpkg-5.0.8/README.md
+-rw-r--r--   0        0        0     1693 2024-05-10 20:55:25.000000 slpkg-5.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/binaries/__init__.py
+-rw-r--r--   0        0        0     9746 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/binaries/install.py
+-rw-r--r--   0        0        0     2202 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/binaries/required.py
+-rw-r--r--   0        0        0     1117 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/blacklist.py
+-rw-r--r--   0        0        0     7545 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/check_updates.py
+-rw-r--r--   0        0        0     1558 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/checks.py
+-rw-r--r--   0        0        0     1856 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/checksum.py
+-rw-r--r--   0        0        0     4548 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/choose_packages.py
+-rw-r--r--   0        0        0      948 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/cleanings.py
+-rw-r--r--   0        0        0     5637 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/configs.py
+-rw-r--r--   0        0        0     4783 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/dependees.py
+-rw-r--r--   0        0        0     2080 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/dialog_box.py
+-rw-r--r--   0        0        0     5220 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/dialog_configs.py
+-rw-r--r--   0        0        0     4699 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/download_only.py
+-rw-r--r--   0        0        0     4283 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/downloader.py
+-rw-r--r--   0        0        0      667 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/error_messages.py
+-rw-r--r--   0        0        0     2284 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/find_installed.py
+-rw-r--r--   0        0        0     1558 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/gpg_verify.py
+-rw-r--r--   0        0        0    10030 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/install_data.py
+-rw-r--r--   0        0        0     4211 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/load_data.py
+-rw-r--r--   0        0        0    29927 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/main.py
+-rw-r--r--   0        0        0     6630 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/multi_process.py
+-rw-r--r--   0        0        0    12003 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/new_configs.py
+-rw-r--r--   0        0        0     3207 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/progress_bar.py
+-rw-r--r--   0        0        0     6881 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/remove_packages.py
+-rw-r--r--   0        0        0     5389 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/repo_info.py
+-rw-r--r--   0        0        0    17569 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/repositories.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/sbos/__init__.py
+-rw-r--r--   0        0        0     1419 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/sbos/dependencies.py
+-rw-r--r--   0        0        0     5192 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0        0        0    13345 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/sbos/slackbuild.py
+-rw-r--r--   0        0        0     3684 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/search.py
+-rw-r--r--   0        0        0      712 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/toml_errors.py
+-rw-r--r--   0        0        0     5529 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/tracking.py
+-rw-r--r--   0        0        0     6878 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/update_repositories.py
+-rw-r--r--   0        0        0    11373 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/upgrade.py
+-rw-r--r--   0        0        0     9832 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/utilities.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/__init__.py
+-rw-r--r--   0        0        0     6757 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/asciibox.py
+-rw-r--r--   0        0        0     6696 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/cli_menu.py
+-rw-r--r--   0        0        0      690 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/version.py
+-rw-r--r--   0        0        0     8072 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/view_package.py
+-rw-r--r--   0        0        0     1942 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/view_process.py
+-rw-r--r--   0        0        0    13487 2024-05-10 20:55:25.000000 slpkg-5.0.8/slpkg/views/views.py
+-rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 slpkg-5.0.8/PKG-INFO
```

### Comparing `slpkg-5.0.7/README.md` & `slpkg-5.0.8/README.md`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/pyproject.toml` & `slpkg-5.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "slpkg"
-version = "5.0.7"
+version = "5.0.8"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 maintainers = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Package manager utility for Slackware Linux"
```

### Comparing `slpkg-5.0.7/slpkg/binaries/install.py` & `slpkg-5.0.8/slpkg/binaries/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         self.choose_package_dependencies()
         self.add_dependencies_to_install_order()
         self.clean_the_main_slackbuilds()
         self.add_main_packages_to_install_order()
         self.check_for_skipped()
 
         self.view.install_upgrade_packages(self.packages, self.dependencies, self.mode)
+        self.view.missing_dependencies(self.install_order)
         self.view.question()
 
         start: float = time.time()
         self.view.skipping_packages(self.skipped_packages)
         self.crating_the_package_urls_list()
         self.checksum_binary_packages()
         self.set_progress_message()
```

### Comparing `slpkg-5.0.7/slpkg/binaries/required.py` & `slpkg-5.0.8/slpkg/binaries/required.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,16 +28,14 @@
         self.full_requires: bool = False
         if self.repos.repos_information.is_file():
             info: dict = self.utils.read_json_file(self.repos.repos_information)
             repo_name: str = data[name]['repo']
             if info.get(repo_name):
                 self.full_requires: bool = info[repo_name].get('full_requires', False)
 
-        self.repository_packages: tuple = tuple(self.data.keys())
-
         self.option_for_resolve_off: bool = self.utils.is_option(
             ('-O', '--resolve-off'), flags)
 
     def resolve(self) -> tuple:
         """ Resolve the dependencies.
         """
         dependencies: tuple = ()
@@ -63,8 +61,8 @@
 
         Args:
             requires (list): List of requires.
 
         Returns:
             list: List of packages name.
         """
-        return [req for req in requires if req in self.repository_packages]
+        return [req for req in requires if req in self.data]
```

### Comparing `slpkg-5.0.7/slpkg/blacklist.py` & `slpkg-5.0.8/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/check_updates.py` & `slpkg-5.0.8/slpkg/check_updates.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/checks.py` & `slpkg-5.0.8/slpkg/checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/checksum.py` & `slpkg-5.0.8/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/choose_packages.py` & `slpkg-5.0.8/slpkg/choose_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/cleanings.py` & `slpkg-5.0.8/slpkg/cleanings.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/configs.py` & `slpkg-5.0.8/slpkg/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,15 @@
     reinstall: str = 'upgradepkg --reinstall'
     removepkg: str = 'removepkg'
     colors: bool = True
     makeflags: str = '-j4'
     gpg_verification: bool = False
     checksum_md5: bool = True
     dialog: bool = True
-    new_packages: bool = False
-    removed_packages: bool = False
+    view_missing_deps: bool = True
     downloader: str = 'wget'
     wget_options: str = '--c -q --progress=bar:force:noscroll --show-progress'
     curl_options: str = ''
     lftp_get_options: str = '-c get -e'
     lftp_mirror_options: str = '-c mirror --parallel=100 --only-newer --delete'
     ascii_characters: bool = True
     ask_question: bool = True
@@ -87,16 +86,15 @@
             reinstall: str = config['reinstall']
             removepkg: str = config['removepkg']
             colors: bool = config['colors']
             makeflags: str = config['makeflags']
             gpg_verification: bool = config['gpg_verification']
             checksum_md5: bool = config['checksum_md5']
             dialog: bool = config['dialog']
-            new_packages: bool = config['new_packages']
-            removed_packages: bool = config['removed_packages']
+            view_missing_deps: bool = config['view_missing_deps']
             downloader: str = config['downloader']
             wget_options: str = config['wget_options']
             curl_options: str = config['curl_options']
             lftp_get_options: str = config['lftp_get_options']
             lftp_mirror_options: str = config['lftp_mirror_options']
             ascii_characters: bool = config['ascii_characters']
             file_list_suffix: str = config['file_list_suffix']
```

### Comparing `slpkg-5.0.7/slpkg/dependees.py` & `slpkg-5.0.8/slpkg/dependees.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/dialog_box.py` & `slpkg-5.0.8/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/dialog_configs.py` & `slpkg-5.0.8/slpkg/dialog_configs.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,29 +78,28 @@
 
     def check_configs(self, tags: list) -> bool:
         """ Check for true of false values.
         """
         keys: list = [
             'COLORS',
             'DIALOG',
+            'VIEW_MISSING_DEPS',
             'SILENT_MODE',
             'ASCII_CHARACTERS',
             'ASK_QUESTION',
             'KERNEL_VERSION',
             'PARALLEL_DOWNLOADS',
             'PROGRESS_BAR',
             'SPINNING_BAR',
             'CASE_INSENSITIVE',
             'PROCESS_LOG',
             'URLLIB_RETRIES',
             'URLLIB_REDIRECT',
             'GPG_VERIFICATION',
-            'CHECKSUM_MD5',
-            'NEW_PACKAGES',
-            'REMOVED_PACKAGES'
+            'CHECKSUM_MD5'
         ]
         values: list = ['true', 'false']
 
         for key, value in zip(self.configs['configs'].keys(), tags):
 
             if key in keys and value not in values:
                 self.dialogbox.msgbox(f"\nError: Value for '{key}', it must be 'true' or 'false.'\n",
@@ -132,28 +131,27 @@
                     if line.lstrip().startswith(f'{key} ='):
                         line = f'  {key} = "{value}"\n'
 
                     if line.lstrip().startswith(
 
                             ('COLORS =',
                              'DIALOG =',
+                             'VIEW_MISSING_DEPS =',
                              'SILENT_MODE =',
                              'ASCII_CHARACTERS =',
                              'ASK_QUESTION =',
                              'KERNEL_VERSION =',
                              'PARALLEL_DOWNLOADS =',
                              'MAXIMUM_PARALLEL = ',
                              'PROGRESS_BAR =',
                              'SPINNING_BAR =',
                              'CASE_SENSITIVE =',
                              'PROCESS_LOG =',
                              'URLLIB_RETRIES =',
                              'URLLIB_REDIRECT =',
                              'URLLIB_TIMEOUT =',
                              'GPG_VERIFICATION =',
-                             'CHECKSUM_MD5 =',
-                             'NEW_PACKAGES =',
-                             'REMOVED_PACKAGES =')
+                             'CHECKSUM_MD5 =')
                     ):
                         line: str = line.replace('"', '')
 
                 patch_toml.write(line)
```

### Comparing `slpkg-5.0.7/slpkg/download_only.py` & `slpkg-5.0.8/slpkg/download_only.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/downloader.py` & `slpkg-5.0.8/slpkg/downloader.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/error_messages.py` & `slpkg-5.0.8/slpkg/error_messages.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/find_installed.py` & `slpkg-5.0.8/slpkg/find_installed.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/gpg_verify.py` & `slpkg-5.0.8/slpkg/gpg_verify.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/install_data.py` & `slpkg-5.0.8/slpkg/install_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,20 +55,18 @@
 
         Args:
             repo (str): repository name.
 
         No Longer Returned:
             None.
         """
-        print()
         self.view_process.message(f'Updating the database for {repo}')
 
         data: dict = {}
         cache: list = []
-        names: list = []
         sbo_tags: list = [
             'SLACKBUILD NAME:',
             'SLACKBUILD LOCATION:',
             'SLACKBUILD FILES:',
             'SLACKBUILD VERSION:',
             'SLACKBUILD DOWNLOAD:',
             'SLACKBUILD DOWNLOAD_x86_64:',
@@ -78,40 +76,35 @@
             'SLACKBUILD SHORT DESCRIPTION:'
         ]
 
         slackbuilds_txt: list = Path(self.repos.repositories[repo]['path'],
                                      self.repos.repositories[repo]['slackbuilds_txt']).read_text(
             encoding='utf-8').splitlines()
 
-        for line in slackbuilds_txt:
-            if line.startswith(sbo_tags[0]):
-                names.append(line.replace(sbo_tags[0], '').strip())
-
         for i, line in enumerate(slackbuilds_txt, 1):
             for tag in sbo_tags:
                 if line.startswith(tag):
                     line = line.replace(tag, '').strip()
                     cache.append(line)
 
             if (i % 11) == 0:
                 build: str = ''
                 name: str = cache[0]
                 version: str = cache[3]
                 location: str = cache[1].split('/')[1]
-                requires: list = [item for item in cache[8].split() if item in names]
 
                 data[name] = {
                     'location': location,
                     'files': cache[2].split(),
                     'version': version,
                     'download': cache[4].split(),
                     'download64': cache[5].split(),
                     'md5sum': cache[6].split(),
                     'md5sum64': cache[7].split(),
-                    'requires': requires,
+                    'requires': cache[8].replace('%README%', '').split(),
                     'description': cache[9]
                 }
 
                 arch: str = self.os_arch
                 sbo_file: Path = Path(self.repos.repositories[repo]['path'], location, name, f'{name}.SlackBuild')
                 if sbo_file.is_file():
                     slackbuild = sbo_file.read_text(encoding='utf-8').splitlines()
@@ -158,15 +151,14 @@
             mirror: str = self.repos.repositories[repo]['mirror_changelog']
 
         checksums_dict: dict = {}
         data: dict = {}
         build: str = ''
         arch: str = ''
         requires: list = []
-        names: list = []
         full_requires: bool = False
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
@@ -176,20 +168,14 @@
                                    self.repos.repositories[repo]['packages_txt'])
         path_checksums: Path = Path(self.repos.repositories[repo]['path'],
                                     self.repos.repositories[repo]['checksums_md5'])
         packages_txt: list = self.utils.read_text_file(path_packages)
 
         checksums_md5: list = self.utils.read_text_file(path_checksums)
 
-        for line in packages_txt:
-            if line.startswith(pkg_tag[0]):
-                package: str = line.replace(pkg_tag[0], '').strip()
-                name: str = self.utils.split_package(package)['name']
-                names.append(name)
-
         for line in checksums_md5:
             line = line.strip()
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
@@ -228,17 +214,17 @@
                     deps: list = []
                     for req in required.split(','):
                         dep = req.split('|')
                         if len(dep) > 1:
                             deps.append(dep[1])
                         else:
                             deps.extend(dep)
-                    requires: list = [item for item in list(set(deps)) if item in names]
+                    requires: list = list(set(deps))
                 else:
-                    requires: list = [item for item in required.split(',') if item in names]
+                    requires: list = required.split(',')
 
             if line.startswith(pkg_tag[5]):
                 package_description = line.replace(pkg_tag[5], '').strip()
                 cache.append(package_description)
 
             if len(cache) == 9:
                 data[cache[0]] = {
```

### Comparing `slpkg-5.0.7/slpkg/load_data.py` & `slpkg-5.0.8/slpkg/load_data.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/main.py` & `slpkg-5.0.8/slpkg/main.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/multi_process.py` & `slpkg-5.0.8/slpkg/multi_process.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/new_configs.py` & `slpkg-5.0.8/slpkg/new_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/progress_bar.py` & `slpkg-5.0.8/slpkg/progress_bar.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/remove_packages.py` & `slpkg-5.0.8/slpkg/remove_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/repo_info.py` & `slpkg-5.0.8/slpkg/repo_info.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/repositories.py` & `slpkg-5.0.8/slpkg/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     utils = Utilities()
 
     repositories_toml_file: Path = Path(Configs.etc_path, 'repositories.toml')
     repositories_path: Path = Path(Configs.lib_path, 'repos')
 
     repos_config = {}
     repositories = {}
-    repos_toml = {}  # type: ignore[var-annotated]
+    repos_toml = {}
 
     data_json: str = 'data.json'
     repos_information: Path = Path(repositories_path, 'repos_information.json')
     default_repository: str = 'sbo'
 
     slackbuilds_txt: str = 'SLACKBUILDS.TXT'
     packages_txt: str = 'PACKAGES.TXT'
@@ -118,20 +118,14 @@
 
     conraid_repo: bool = False
     conraid_repo_name: str = 'conraid'
     conraid_repo_path: Path = Path(repositories_path, conraid_repo_name)
     conraid_repo_mirror: str = ''
     conraid_repo_tag: str = 'cf'
 
-    slackdce_repo: bool = False
-    slackdce_repo_name: str = 'slackdce'
-    slackdce_repo_path: Path = Path(repositories_path, slackdce_repo_name)
-    slackdce_repo_mirror: str = ''
-    slackdce_repo_tag: str = 'dce'
-
     slackonly_repo: bool = False
     slackonly_repo_name: str = 'slackonly'
     slackonly_repo_path: Path = Path(repositories_path, slackonly_repo_name)
     slackonly_repo_mirror: str = ''
     slackonly_repo_tag: str = 'slonly'
 
     salix_repo: bool = False
@@ -167,15 +161,18 @@
     try:
         if repositories_toml_file.is_file():
             with open(repositories_toml_file, 'rb') as repo:
                 repos_config = tomli.load(repo)
 
             repos_config = utils.convert_dict_keys_to_lower(repos_config)
 
-            default_repository: str = repos_config['default']['repo'].lower()
+            default_repository: str = repos_config['default']['repository'].lower()
+
+            new_packages = repos_config['new_packages']['repositories']
+            remove_packages = repos_config['remove_packages']['repositories']
 
             sbo_repo: bool = repos_config['sbo']['enable']
             sbo_repo_mirror: str = repos_config['sbo']['mirror']
 
             ponce_repo: bool = repos_config['ponce']['enable']
             ponce_repo_mirror: str = repos_config['ponce']['mirror']
 
@@ -217,17 +214,14 @@
 
             csb_repo: bool = repos_config['csb']['enable']
             csb_repo_mirror: str = repos_config['csb']['mirror']
 
             conraid_repo: bool = repos_config['conraid']['enable']
             conraid_repo_mirror: str = repos_config['conraid']['mirror']
 
-            slackdce_repo: bool = repos_config['slackdce']['enable']
-            slackdce_repo_mirror: str = repos_config['slackdce']['mirror']
-
             slackonly_repo: bool = repos_config['slackonly']['enable']
             slackonly_repo_mirror: str = repos_config['slackonly']['mirror']
 
             salix_repo: bool = repos_config['salix']['enable']
             salix_repo_mirror: str = repos_config['salix']['mirror']
 
             salix_extra_repo: bool = repos_config['salix_extra']['enable']
@@ -362,24 +356,14 @@
             'mirror_packages': conraid_repo_mirror,
             'mirror_changelog': conraid_repo_mirror,
             'packages_txt': packages_txt,
             'checksums_md5': checksums_md5,
             'changelog_txt': changelog_txt,
             'repo_tag': conraid_repo_tag},
 
-        slackdce_repo_name: {
-            'enable': slackdce_repo,
-            'path': slackdce_repo_path,
-            'mirror_packages': slackdce_repo_mirror,
-            'mirror_changelog': slackdce_repo_mirror,
-            'packages_txt': packages_txt,
-            'checksums_md5': checksums_md5,
-            'changelog_txt': changelog_txt,
-            'repo_tag': slackdce_repo_tag},
-
         slackonly_repo_name: {
             'enable': slackonly_repo,
             'path': slackonly_repo_path,
             'mirror_packages': slackonly_repo_mirror,
             'mirror_changelog': slackonly_repo_mirror,
             'packages_txt': packages_txt,
             'checksums_md5': checksums_md5,
@@ -437,15 +421,17 @@
             'repo_tag': pprkut_repo_tag}
     }
 
     all_repos = list(repos_config.keys())
     defaults_repos = list(repositories.keys())
 
     diff_repos = list(set(all_repos) - set(defaults_repos))
-    diff_repos.remove('default')
+    items_to_remove = ('default', 'new_packages', 'remove_packages')
+    for item in items_to_remove:
+        diff_repos.remove(item)
 
     if diff_repos:
         for repo, data in repos_config.items():
 
             if repo in diff_repos:
                 mirror_packages: str = data.get('mirror', '')
                 mirror_changelog: str = mirror_packages
```

### Comparing `slpkg-5.0.7/slpkg/sbos/dependencies.py` & `slpkg-5.0.8/slpkg/sbos/dependencies.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 
 from slpkg.utilities import Utilities
 
 
-def resolve_requires(data: dict, name: str, flags: list) -> tuple:
-    """ Resolve dependencies.
+class Requires:
+    """ Creates a tuple of dependencies with
+    the right order to install. """
+    __slots__ = (
+        'data', 'name', 'flags', 'utils', 'option_for_resolve_off'
+    )
+
+    def __init__(self, data: dict, name: str, flags: list):
+        self.data: dict = data
+        self.name: str = name
+        self.utils = Utilities()
+
+        self.option_for_resolve_off: bool = self.utils.is_option(
+            ('-O', '--resolve-off'), flags)
+
+    def resolve(self) -> tuple:
+        """ Resolve the dependencies. """
+        dependencies: tuple = ()
 
-    Args:
-        data (dict): Repository data.
-        name (str): Slackbuild name.
-        flags (list): List of options.
-
-    Returns:
-        tuple: Description
-    """
-    dependencies: tuple = tuple()
-    utils = Utilities()
-
-    if not utils.is_option(('-O', '--resolve-off'), flags):
-        requires: list[str] = data[name]['requires']
-        for require in requires:
-
-            sub_requires: list[str] = data[require]['requires']
-            for sub in sub_requires:
-                if sub not in requires:
+        if not self.option_for_resolve_off:
+            requires: list[str] = self.remove_deps(self.data[self.name]['requires'])
+
+            for require in requires:
+                sub_requires: list[str] = self.remove_deps(self.data[require]['requires'])
+
+                for sub in sub_requires:
                     requires.append(sub)
 
-        requires.reverse()
-        dependencies: tuple = tuple(dict.fromkeys(requires))
+            requires.reverse()
+            dependencies: tuple = tuple(dict.fromkeys(requires))
+
+        return dependencies
 
-    return dependencies
+    def remove_deps(self, requires: list) -> list:
+        """Remove requirements that not in the repository.
+        Args:
+            requires (list): List of requires.
+
+        Returns:
+            list: List of packages name.
+        """
+        return [req for req in requires if req in self.data]
```

### Comparing `slpkg-5.0.7/slpkg/sbos/sbo_generate.py` & `slpkg-5.0.8/slpkg/sbos/sbo_generate.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/sbos/slackbuild.py` & `slpkg-5.0.8/slpkg/sbos/slackbuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from slpkg.gpg_verify import GPGVerify
 from slpkg.error_messages import Errors
 from slpkg.downloader import Downloader
 from slpkg.views.asciibox import AsciiBox
 from slpkg.repositories import Repositories
 from slpkg.multi_process import MultiProcess
 from slpkg.views.view_process import ViewProcess
-from slpkg.sbos.dependencies import resolve_requires
+from slpkg.sbos.dependencies import Requires
 
 
 class Slackbuilds(Configs):  # pylint: disable=[R0902,R0904]
 
     """
     Download build and install the SlackBuilds.
     """
@@ -78,15 +78,18 @@
         self.view_process.message('Resolving dependencies')
         self.creating_dependencies_list()
         self.choose_package_dependencies()
         self.add_dependencies_to_install_order()
         self.clean_the_main_slackbuilds()
         self.add_main_packages_to_install_order()
         self.check_for_skipped()
+
         self.view_slackbuilds_before_build()
+        self.view.missing_dependencies(self.install_order)
+        self.view.question()
 
         start: float = time.time()
         self.view.skipping_packages(self.skipped_packages)
         self.prepare_slackbuilds_for_build()
         self.download_the_sources()
         self.set_progress_message()
         self.build_and_install_the_slackbuilds()
@@ -94,15 +97,15 @@
 
         self.utils.finished_time(elapsed_time)
 
     def creating_dependencies_list(self) -> None:
         """ Creates the package dependencies list.
         """
         for slackbuild in self.slackbuilds:
-            dependencies: tuple = resolve_requires(self.data, slackbuild, self.flags)
+            dependencies: tuple = Requires(self.data, slackbuild, self.flags).resolve()
 
             for dependency in dependencies:
                 self.dependencies.append(dependency)
 
         self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
 
     def add_dependencies_to_install_order(self) -> None:
@@ -138,16 +141,14 @@
         """ View packages before build.
         """
         if self.mode == 'build':
             self.view.build_packages(self.slackbuilds, self.dependencies)
         else:
             self.view.install_upgrade_packages(self.slackbuilds, self.dependencies, self.mode)
 
-        self.view.question()
-
     def prepare_slackbuilds_for_build(self) -> None:
         """ Prepare slackbuilds for build.
         """
         if self.install_order:
             self.view_process.message('Prepare sources for downloading')
             for sbo in self.install_order:
                 build_path: Path = Path(self.build_path, sbo)
@@ -258,15 +259,15 @@
 
         Args:
             name (str): Slackbuild name.
         """
         deps: dict = {}
         deps_logs: dict = {}
         installed_requires: list = []
-        requires: tuple = resolve_requires(self.data, name, self.flags)
+        requires: tuple = Requires(self.data, name, self.flags).resolve()
         # Verify for installation.
         for req in requires:
             if self.utils.is_package_installed(req):
                 installed_requires.append(req)
 
         deps[name] = installed_requires
         if self.deps_log_file.is_file():
```

### Comparing `slpkg-5.0.7/slpkg/search.py` & `slpkg-5.0.8/slpkg/search.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/toml_errors.py` & `slpkg-5.0.8/slpkg/toml_errors.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/tracking.py` & `slpkg-5.0.8/slpkg/tracking.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.views.asciibox import AsciiBox
 from slpkg.repositories import Repositories
-from slpkg.sbos.dependencies import resolve_requires
+from slpkg.sbos.dependencies import Requires
 from slpkg.binaries.required import Required
 
 
 class Tracking(Configs):  # pylint: disable=[R0902]
 
     """
     Tracking of the package dependencies.
@@ -27,15 +27,15 @@
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.llc: str = self.ascii.lower_left_corner
         self.hl: str = self.ascii.horizontal_line
         self.package_version: str = ''
         self.package_dependency_version: str = ''
-        self.package_requires: tuple = ()
+        self.package_requires: list = []
         self.package_line: str = ''
         self.require_line: str = ''
         self.count_requires: int = 0
         self.require_length: int = 0
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ('-p', '--pkg-version'), flags)
@@ -100,18 +100,23 @@
 
     def set_the_package_require_line(self, require: str) -> None:
         """ Sets the requires.
 
         Args:
             require (str): Require name.
         """
-        self.require_line: str = f'{self.cyan}{require}{self.endc}'
+        color: str = self.cyan
+        if require not in self.data:
+            color: str = self.red
+
+        self.require_line: str = f'{color}{require}{self.endc}'
+
         if self.option_for_pkg_version:
             self.set_package_dependency_version(require)
-            self.require_line: str = (f'{self.cyan}{require:<{self.require_length}}{self.endc}'
+            self.require_line: str = (f'{color}{require:<{self.require_length}}{self.endc}'
                                       f'{self.package_dependency_version}')
 
     def set_package_dependency_version(self, require: str) -> None:
         """ Sets the dependency version.
 
         Args:
             require (str): Description
@@ -132,19 +137,26 @@
 
     def set_package_requires(self, package: str) -> None:
         """ Sets for the package require.
 
         Args:
             package (str): Package name.
         """
+
         if self.repository not in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
-            self.package_requires: tuple = Required(self.data, package, self.flags).resolve()
+            self.package_requires: list = list(Required(self.data, package, self.flags).resolve())
         else:
-            self.package_requires: tuple = resolve_requires(self.data, package, self.flags)
+            self.package_requires: list = list(Requires(self.data, package, self.flags).resolve())
+
         if self.package_requires:
+            if self.view_missing_deps:
+                requires: list = self.data[package]['requires']
+                for req in requires:
+                    if req not in self.data:
+                        self.package_requires.append(req)
             self.require_length: int = max(len(name) for name in self.package_requires)
 
     def view_summary_of_tracking(self, package: str) -> None:
         """ Prints the summary.
 
         Args:
             package (str): Package name.
```

### Comparing `slpkg-5.0.7/slpkg/update_repositories.py` & `slpkg-5.0.8/slpkg/update_repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/upgrade.py` & `slpkg-5.0.8/slpkg/upgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,19 +81,19 @@
         self.load_installed_packages(self.repository)
 
         for inst in self.installed_packages:
             name: str = self.utils.split_package(inst.name)['name']
             if self.is_package_upgradeable(inst.name):
                 yield name
 
-            if self.repository == self.repos.slack_repo_name and self.removed_packages:
+            if self.repository in self.repos.remove_packages:
                 if name not in self.data.keys():
                     yield name + '_Removed.'
 
-        if self.repository == self.repos.slack_repo_name and self.new_packages:
+        if self.repository in self.repos.new_packages:
             for name in self.data.keys():
                 # if not self.utils.is_package_installed(name):
                 if name not in self.installed_names:
                     yield name
 
     def is_package_upgradeable(self, installed: str) -> bool:  # pylint: disable=[R0911]
         """Returns True for upgradeable packages.
@@ -186,15 +186,15 @@
                             'inst_build': inst_build,
                             'repo_version': repo_version,
                             'repo_build': repo_build,
                             'repo': repo,
                             'type': 'upgrade'
                         }
 
-                if repo == self.repos.slack_repo_name and self.removed_packages:
+                if repo in self.repos.remove_packages:
                     tag: str = self.utils.split_package(installed.name)['tag']
                     if not tag and name not in data.keys():
                         self.id += 1
                         self.sum_removed += 1
                         inst_version: str = self.utils.split_package(installed.name)['version']
                         inst_build: str = self.utils.split_package(installed.name)['build']
 
@@ -204,15 +204,15 @@
                             'inst_build': inst_build,
                             'repo_version': '',
                             'repo_build': '',
                             'repo': repo,
                             'type': 'remove'
                         }
 
-            if repo == self.repos.slack_repo_name and self.new_packages:
+            if repo in self.repos.new_packages:
                 for name in data.keys():
                     # if not self.utils.is_package_installed(name):
                     if name not in self.installed_names:
                         self.id += 1
                         self.sum_added += 1
                         repo_version: str = data[name]['version']
                         repo_build: str = data[name]['build']
```

### Comparing `slpkg-5.0.7/slpkg/utilities.py` & `slpkg-5.0.8/slpkg/utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/views/asciibox.py` & `slpkg-5.0.8/slpkg/views/asciibox.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/views/cli_menu.py` & `slpkg-5.0.8/slpkg/views/cli_menu.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/views/version.py` & `slpkg-5.0.8/slpkg/views/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 
 class Version:  # pylint: disable=[R0903]
     """ Print the version. """
 
     def __init__(self):
-        self.version: str = "5.0.7"
+        self.version: str = "5.0.8"
         self.license: str = 'GNU General Public License v3 (GPLv3)'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
         self.email: str = 'dslackw@gmail.com'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-5.0.7/slpkg/views/view_package.py` & `slpkg-5.0.8/slpkg/views/view_package.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/views/view_process.py` & `slpkg-5.0.8/slpkg/views/view_process.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.7/slpkg/views/views.py` & `slpkg-5.0.8/slpkg/views/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -327,14 +327,31 @@
             print('Packages skipped by the user:\n')
             for name in packages:
                 failed: str = f'{self.red}{self.ascii.skipped}{self.endc}'
                 print(f"\r{'':>2}{self.bred}{self.ascii.bullet}{self.endc} "
                       f"{self.data[name]['package']} {failed}{' ' * 17}")
             print()
 
+    def missing_dependencies(self, packages: list) -> None:
+        """ View for missing dependencies.
+        """
+        if self.view_missing_deps:
+            missing_deps: dict = {}
+            for package in packages:
+                requires: list = self.data[package]['requires']
+                for req in requires:
+                    if req not in self.data:
+                        missing_deps[package] = [req for req in requires if req not in self.data]
+            if missing_deps:
+                print('\nPackages with missing dependencies:')
+                for pkg, deps in missing_deps.items():
+                    if deps and deps != ['']:
+                        print(f"> {self.cyan}{pkg}{self.endc}: Requires "
+                              f"({len(deps)}) -> {self.red}{', '.join(deps)}{self.endc}")
+
     def question(self, message: str = 'Do you want to continue?') -> None:
         """ View a question.
 
         Args:
             message (str, optional): Message of question.
 
         Raises:
```

### Comparing `slpkg-5.0.7/PKG-INFO` & `slpkg-5.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 5.0.7
+Version: 5.0.8
 Summary: Package manager utility for Slackware Linux
 Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Maintainer-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: slpkg Version: 5.0.7 Summary: Package manager
+Metadata-Version: 2.1 Name: slpkg Version: 5.0.8 Summary: Package manager
 utility for Slackware Linux Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis
 gmail.com> Maintainer-email: Dimitris Zlatanidis
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Environment :: Console
 Classifier: Operating System :: POSIX Classifier: Operating System :: POSIX ::
```

