# Comparing `tmp/mkdocs_addresses-0.3.1.tar.gz` & `tmp/mkdocs_addresses-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_addresses-0.3.1.tar", max compression
+gzip compressed data, was "mkdocs_addresses-0.3.2.tar", max compression
```

## Comparing `mkdocs_addresses-0.3.1.tar` & `mkdocs_addresses-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0   303056 2024-04-07 13:02:30.042002 mkdocs_addresses-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     6870 2024-04-07 13:19:35.416233 mkdocs_addresses-0.3.1/README.md
--rw-r--r--   0        0        0      141 2024-04-07 13:02:30.158005 mkdocs_addresses-0.3.1/mkdocs_addresses/__init__.py
--rw-r--r--   0        0        0       22 2024-04-08 15:15:46.388646 mkdocs_addresses-0.3.1/mkdocs_addresses/__version__.py
--rw-r--r--   0        0        0    12859 2024-04-07 13:02:30.158005 mkdocs_addresses-0.3.1/mkdocs_addresses/addresses_checker.py
--rw-r--r--   0        0        0    35160 2024-04-07 13:02:30.178006 mkdocs_addresses-0.3.1/mkdocs_addresses/addresses_plugin.py
--rw-r--r--   0        0        0     1826 2024-04-07 13:02:30.242007 mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/__init__.py
--rw-r--r--   0        0        0     3851 2024-04-07 13:02:30.278009 mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_base_handler.py
--rw-r--r--   0        0        0     1273 2024-04-07 13:02:30.278009 mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_no_completion_handler.py
--rw-r--r--   0        0        0     4173 2024-04-07 13:02:30.290009 mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_vsc_handlers.py
--rw-r--r--   0        0        0    25225 2024-04-08 15:13:31.968454 mkdocs_addresses-0.3.1/mkdocs_addresses/config_plugin.py
--rw-r--r--   0        0        0     4482 2023-09-21 08:35:25.358662 mkdocs_addresses-0.3.1/mkdocs_addresses/exceptions.py
--rw-r--r--   0        0        0     8074 2024-04-07 13:02:30.298009 mkdocs_addresses-0.3.1/mkdocs_addresses/logger.py
--rw-r--r--   0        0        0        0 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.1/mkdocs_addresses/other_plugins_handling/__init__.py
--rw-r--r--   0        0        0     1663 2024-04-07 13:02:30.310009 mkdocs_addresses-0.3.1/mkdocs_addresses/other_plugins_handling/autorefs.py
--rw-r--r--   0        0        0     1897 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.1/mkdocs_addresses/path_manager.py
--rw-r--r--   0        0        0     5260 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.1/mkdocs_addresses/soup_excluding_codes.py
--rw-r--r--   0        0        0      692 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/__init__.py
--rw-r--r--   0        0        0     1965 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/files_tracker.py
--rw-r--r--   0        0        0    17190 2024-04-08 15:15:46.344645 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/static_handler.py
--rw-r--r--   0        0        0     2525 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py
--rw-r--r--   0        0        0     5805 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_data_pages.py
--rw-r--r--   0        0        0     2228 2023-09-20 13:11:14.914470 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_errors_counter.py
--rw-r--r--   0        0        0     5628 2024-04-07 13:02:30.342010 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_references.py
--rw-r--r--   0        0        0      712 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/types_aliases.py
--rw-r--r--   0        0        0      492 2024-04-07 13:02:30.342010 mkdocs_addresses-0.3.1/mkdocs_addresses/toolbox.py
--rw-r--r--   0        0        0     2013 2024-04-08 15:15:46.340645 mkdocs_addresses-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     8327 1970-01-01 00:00:00.000000 mkdocs_addresses-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0   303056 2024-04-08 15:15:55.544929 mkdocs_addresses-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0     6870 2024-04-08 15:15:55.548929 mkdocs_addresses-0.3.2/README.md
+-rw-r--r--   0        0        0      141 2024-04-07 13:02:30.158005 mkdocs_addresses-0.3.2/mkdocs_addresses/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-10 21:45:55.311317 mkdocs_addresses-0.3.2/mkdocs_addresses/__version__.py
+-rw-r--r--   0        0        0    12859 2024-04-07 13:02:30.158005 mkdocs_addresses-0.3.2/mkdocs_addresses/addresses_checker.py
+-rw-r--r--   0        0        0    35469 2024-05-10 21:31:36.909895 mkdocs_addresses-0.3.2/mkdocs_addresses/addresses_plugin.py
+-rw-r--r--   0        0        0     1826 2024-04-07 13:02:30.242007 mkdocs_addresses-0.3.2/mkdocs_addresses/auto_completion_handler/__init__.py
+-rw-r--r--   0        0        0     3851 2024-04-07 13:02:30.278009 mkdocs_addresses-0.3.2/mkdocs_addresses/auto_completion_handler/_base_handler.py
+-rw-r--r--   0        0        0     1273 2024-04-07 13:02:30.278009 mkdocs_addresses-0.3.2/mkdocs_addresses/auto_completion_handler/_no_completion_handler.py
+-rw-r--r--   0        0        0     4173 2024-04-07 13:02:30.290009 mkdocs_addresses-0.3.2/mkdocs_addresses/auto_completion_handler/_vsc_handlers.py
+-rw-r--r--   0        0        0    25547 2024-05-10 21:31:36.909895 mkdocs_addresses-0.3.2/mkdocs_addresses/config_plugin.py
+-rw-r--r--   0        0        0     4482 2023-09-21 08:35:25.358662 mkdocs_addresses-0.3.2/mkdocs_addresses/exceptions.py
+-rw-r--r--   0        0        0     8074 2024-04-07 13:02:30.298009 mkdocs_addresses-0.3.2/mkdocs_addresses/logger.py
+-rw-r--r--   0        0        0        0 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.2/mkdocs_addresses/other_plugins_handling/__init__.py
+-rw-r--r--   0        0        0     1663 2024-04-07 13:02:30.310009 mkdocs_addresses-0.3.2/mkdocs_addresses/other_plugins_handling/autorefs.py
+-rw-r--r--   0        0        0     1897 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.2/mkdocs_addresses/path_manager.py
+-rw-r--r--   0        0        0     5260 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.2/mkdocs_addresses/soup_excluding_codes.py
+-rw-r--r--   0        0        0      692 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/__init__.py
+-rw-r--r--   0        0        0     1965 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/files_tracker.py
+-rw-r--r--   0        0        0    17190 2024-05-10 21:45:55.263316 mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/static_handler.py
+-rw-r--r--   0        0        0     2525 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py
+-rw-r--r--   0        0        0     5837 2024-05-10 21:31:36.909895 mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/tracker_data_pages.py
+-rw-r--r--   0        0        0     2228 2023-09-20 13:11:14.914470 mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/tracker_errors_counter.py
+-rw-r--r--   0        0        0     5628 2024-04-07 13:02:30.342010 mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/tracker_references.py
+-rw-r--r--   0        0        0      712 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/types_aliases.py
+-rw-r--r--   0        0        0      492 2024-04-07 13:02:30.342010 mkdocs_addresses-0.3.2/mkdocs_addresses/toolbox.py
+-rw-r--r--   0        0        0     2013 2024-05-10 21:45:55.263316 mkdocs_addresses-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8327 1970-01-01 00:00:00.000000 mkdocs_addresses-0.3.2/PKG-INFO
```

### Comparing `mkdocs_addresses-0.3.1/LICENSE.md` & `mkdocs_addresses-0.3.2/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mkdocs-addresses
-0.3.0
+0.3.1
 FreeBSD License
 Copyright (c) 2022 Frédéric Zinelli, All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
```

### Comparing `mkdocs_addresses-0.3.1/README.md` & `mkdocs_addresses-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/addresses_checker.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/addresses_checker.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/addresses_plugin.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/addresses_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,22 @@
         }
         plugin.update({
             "references": dict(self.global_handler.references.id_to_data),
         })
         return f'{ self.__class__.__name__ }:\n{ json.dumps(plugin, indent=4) }'
 
 
+    def is_to_skip(self, some:str) -> bool:
+        """
+        Return True of the given input matches some of the exclusion rules :
+            - black_list_pattern
+            - ignored_identifiers_or_addresses
+        """
+        return some in self.ignored_identifiers_or_addresses or bool(self.black_list_pattern.match(some))
+
 
 
     #-------------------------------------------------------------------
     #                           Plugin Events
     #-------------------------------------------------------------------
 
 
@@ -738,22 +746,23 @@
             (let mkdocs build the urls for those, according to the user's settings)
         """
         self.log(LogMessages.setup_non_md_files)
 
         for file in files:
             cwd_path = self.uni_docs_dir / file.src_path
             uri = file.src_uri
+
             is_md = uri.endswith('.md')
-            is_builtin = (
+            is_builtin = is_md or (
                 uri.startswith('assets/javascripts/')
                 or uri.startswith('assets/stylesheets/')
                 or uri == 'assets/images/favicon.png'       # mkdocs default config
             )
-            is_to_skip = self.black_list_pattern.match(str(cwd_path))
-            if not is_builtin and not is_md and not is_to_skip:
+            is_to_skip = is_builtin or self.is_to_skip(str(cwd_path))
+            if not is_to_skip:
                 self.add_file_infos(cwd_path, file)
 
 
 
 
     @StaticHandler.other_files_cached_with(
         cwd_path_arg_extractor_other_files,
```

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/__init__.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/auto_completion_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_base_handler.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/auto_completion_handler/_base_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_no_completion_handler.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/auto_completion_handler/_no_completion_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/auto_completion_handler/_vsc_handlers.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/auto_completion_handler/_vsc_handlers.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/config_plugin.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/config_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
     Regex string: all addresses or identifiers that will
     [`re.match`](https://docs.python.org/3/library/re.html#re.match){: target=_blank } with it will be ignored.
 
     This allows to register absolute addresses, external links, or any other unusual scenarios you could
     think of, so that errors are not raised by the plugin when handling them.
     """
 
+    black_listed_patterns: List[str] = []
+    """
+    Alternative to black_list_pattern, to get simpler declarations. Both will be merge with OR.
+    """
+
 
     dump_action: str = 'normal'
     """
     The plugin normally dumps information about all the available references  on each serve
     (either as a file of code snippets, or as a text file. See
     [`dump_snippets_file`][mkdocs_addresses.config_plugin.PluginOptions.dump_snippets_file]
     option). The `dump_action` may change that behavior:
@@ -443,14 +448,16 @@
 
     inclusions = C.ListOfItems(C.Type(str), default=PluginOptions.inclusions)
 
     # inclusions_with_root = C.Type(bool, default=PluginOptions.inclusions_with_root)
 
     black_list_pattern = C.Type(str, default=PluginOptions.black_list_pattern)
 
+    black_listed_patterns = C.ListOfItems(C.Type(str), default=PluginOptions.black_listed_patterns)
+
     more_verbose = C.Type(bool, default=PluginOptions.more_verbose)
 
     plugin_off = C.Type(bool, default=PluginOptions.plugin_off)
 
     strict_anchor_check = C.Type(bool, default=PluginOptions.strict_anchor_check)
 
     # LEGACY:
@@ -473,46 +480,48 @@
 
     def validate_and_process(self, config:MkDocsConfig):
         """ Performs the basic, then extras validations on each property, and also apply the
             post conversions to the data structures that need it.
             Add on the fly the needed fields from the mkdocs config.
         """
         # Enforce no unexpected option name (because this is boring AF...)
-        # Enforce no unexpected option name (because this is boring AF...)
         if 'plugins' in config and 'mkdocs-addresses' in config.plugins:
             settings = set(config.plugins['mkdocs-addresses'].config)
             base_settings = set(dir(config.plugins['mkdocs-addresses'].__class__.mro()[1]))
             user_settings = settings - base_settings
         else:
             # when testing in mkdocs-addresses, the plugin isn't in the yml file (must change
             # that: see use of entry-points in pyodide-mkdocs-theme):
             user_settings = set(self.user_configs[-1])
 
-        nope          = user_settings - CONFIG_ANNOTATIONS
+        nope = user_settings - CONFIG_ANNOTATIONS
         if nope:
             nope    = ''.join( '\n   '+key for key in sorted(nope))
             options = ''.join( '\n   '+key for key in sorted(CONFIG_ANNOTATIONS))
             raise AddresserConfigError(
                 f"Unexpected option(s) name(s):{ nope }\n\n Available options are:{options}"
             )
 
         # Extract completion handler class, handling use_vsc, ide and dump_snippets_file defaults
         # (no validation):
         completion_class = validate_config_and_get_auto_completion_handler(self)
 
 
-        # Perform "post" conversions:       (yeah, "post"... lol...)
-        #----------------------------
+        # Perform "~~post"~~" PRE-conversions:       (yeah, "post"... lol...)
+        #-------------------------------------
 
         maybe_abs = path_manager.to_os(config['docs_dir'])
         self.uni_docs_dir = maybe_abs.absolute().relative_to(Path.cwd())
 
         for prop in 'docs_dir  use_directory_urls'.split():
             setattr(self, prop, config[prop])
 
+        self.black_list_pattern = "|".join(
+            [self.black_list_pattern] + self.black_listed_patterns
+        ).strip('|')
 
         post_conversions: Tuple[Callable[[str],Any], str] = [
             (re.compile, 'imgs_extension_pattern  black_list_pattern'),
             (set,        'ignored_identifiers_or_addresses  ignored_classes verify_only  inclusions'),
         ]
         for conversion,props in post_conversions:
             for prop in props.split():
```

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/exceptions.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/exceptions.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/logger.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/logger.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/other_plugins_handling/autorefs.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/other_plugins_handling/autorefs.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/path_manager.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/path_manager.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/soup_excluding_codes.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/soup_excluding_codes.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/__init__.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/files_tracker.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/files_tracker.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/static_handler.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/static_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_data_pages.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/tracker_data_pages.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,20 +85,20 @@
             logic if needed.
         """
         cwd_path   = self.format_source(source)
         known_srcs = self.id_to_sources[identifier]
 
         if self.UNIQUE_SRC and known_srcs:
             there = next(iter(known_srcs))
-            info  = "" if id_declared_as is None else f"(found written as { id_declared_as !r})"
+            info  = "" if id_declared_as is None else f"(found written as \033[31m{ id_declared_as !r}\033[34m)"
             raise DuplicateIdentifierError(
                 f"{ identifier !r} is already used.\n"
                 f"  - Attempt to add it to references\n"        # this line is used in the tests: do not modify
                 f"  - Adding from file { cwd_path }{ info }\n"
-                f"  - Already registered with file {there}\n"
+                f"  - Already registered with file \033[35m{there}\033[34m\n"
             )
 
         known_srcs.add(cwd_path)
         self.source_to_ids[cwd_path].add(identifier)
 
         return cwd_path
```

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_errors_counter.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/tracker_errors_counter.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/tracker_references.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/tracker_references.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/mkdocs_addresses/static_handler/types_aliases.py` & `mkdocs_addresses-0.3.2/mkdocs_addresses/static_handler/types_aliases.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.3.1/pyproject.toml` & `mkdocs_addresses-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-addresses"
-version = "0.3.1"
+version = "0.3.2"
 description = "Mkdocs automatic paths/addresses building - auto-completion support (VSC)"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/frederic-zinelli/mkdocs-addresses"
 homepage = "http://frederic-zinelli.gitlab.io/mkdocs-addresses/"
 exclude = ["mkdocs_addresses/_test_data_extraction.py"]
 keywords = [
```

### Comparing `mkdocs_addresses-0.3.1/PKG-INFO` & `mkdocs_addresses-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-addresses
-Version: 0.3.1
+Version: 0.3.2
 Summary: Mkdocs automatic paths/addresses building - auto-completion support (VSC)
 Home-page: http://frederic-zinelli.gitlab.io/mkdocs-addresses/
 Keywords: mkdocs,mkdocs-plugin,links,autocompletion
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Plugins
```

