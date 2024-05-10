# Comparing `tmp/django-cache-pydantic-0.0.4.tar.gz` & `tmp/django_cache_pydantic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cache-pydantic-0.0.4.tar", last modified: Fri Mar 15 15:08:26 2024, max compression
+gzip compressed data, was "django_cache_pydantic-0.1.0.tar", last modified: Fri May 10 09:27:38 2024, max compression
```

## Comparing `django-cache-pydantic-0.0.4.tar` & `django_cache_pydantic-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-03-15 15:08:26.271091 django-cache-pydantic-0.0.4/
--rw-rw-r--   0 druid     (1000) druid     (1000)       86 2024-03-15 12:54:46.000000 django-cache-pydantic-0.0.4/CHANGELOG.rst
--rw-rw-r--   0 druid     (1000) druid     (1000)     1090 2024-03-14 12:36:31.000000 django-cache-pydantic-0.0.4/LICENSE
--rw-rw-r--   0 druid     (1000) druid     (1000)      115 2024-03-08 22:52:06.000000 django-cache-pydantic-0.0.4/MANIFEST.in
--rw-r--r--   0 druid     (1000) druid     (1000)     4699 2024-03-15 15:08:26.267091 django-cache-pydantic-0.0.4/PKG-INFO
--rw-rw-r--   0 druid     (1000) druid     (1000)     3264 2024-03-15 14:52:49.000000 django-cache-pydantic-0.0.4/README.rst
--rw-rw-r--   0 druid     (1000) druid     (1000)     2015 2024-03-15 15:08:11.000000 django-cache-pydantic-0.0.4/pyproject.toml
--rw-rw-r--   0 druid     (1000) druid     (1000)       38 2024-03-15 15:08:26.271091 django-cache-pydantic-0.0.4/setup.cfg
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-03-15 15:08:26.263091 django-cache-pydantic-0.0.4/src/
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-03-15 15:08:26.267091 django-cache-pydantic-0.0.4/src/django_cache_pydantic/
--rw-rw-r--   0 druid     (1000) druid     (1000)       38 2024-03-09 15:08:25.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic/__init__.py
--rw-rw-r--   0 druid     (1000) druid     (1000)      191 2024-03-15 14:24:29.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic/apps.py
--rw-rw-r--   0 druid     (1000) druid     (1000)     2019 2024-03-15 15:08:11.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic/base.py
--rw-rw-r--   0 druid     (1000) druid     (1000)      525 2024-03-15 14:24:29.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic/conf.py
--rw-rw-r--   0 druid     (1000) druid     (1000)       83 2024-03-09 11:16:25.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic/defaults.py
--rw-rw-r--   0 druid     (1000) druid     (1000)     1626 2024-03-09 15:08:25.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic/manager.py
--rw-rw-r--   0 druid     (1000) druid     (1000)     1588 2024-03-15 14:24:29.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic/options.py
--rw-rw-r--   0 druid     (1000) druid     (1000)        0 2024-03-08 22:52:06.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic/py.typed
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-03-15 15:08:26.267091 django-cache-pydantic-0.0.4/src/django_cache_pydantic.egg-info/
--rw-r--r--   0 druid     (1000) druid     (1000)     4699 2024-03-15 15:08:26.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic.egg-info/PKG-INFO
--rw-rw-r--   0 druid     (1000) druid     (1000)      590 2024-03-15 15:08:26.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic.egg-info/SOURCES.txt
--rw-rw-r--   0 druid     (1000) druid     (1000)        1 2024-03-15 15:08:26.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic.egg-info/dependency_links.txt
--rw-rw-r--   0 druid     (1000) druid     (1000)       26 2024-03-15 15:08:26.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic.egg-info/requires.txt
--rw-rw-r--   0 druid     (1000) druid     (1000)       22 2024-03-15 15:08:26.000000 django-cache-pydantic-0.0.4/src/django_cache_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-05-10 09:27:38.928264 django_cache_pydantic-0.1.0/
+-rw-rw-r--   0 druid     (1000) druid     (1000)      208 2024-05-10 09:26:36.000000 django_cache_pydantic-0.1.0/CHANGELOG.rst
+-rw-rw-r--   0 druid     (1000) druid     (1000)     1090 2024-03-14 12:36:31.000000 django_cache_pydantic-0.1.0/LICENSE
+-rw-rw-r--   0 druid     (1000) druid     (1000)      115 2024-03-08 22:52:06.000000 django_cache_pydantic-0.1.0/MANIFEST.in
+-rw-r--r--   0 druid     (1000) druid     (1000)     4736 2024-05-10 09:27:38.928264 django_cache_pydantic-0.1.0/PKG-INFO
+-rw-rw-r--   0 druid     (1000) druid     (1000)     3301 2024-05-10 09:26:36.000000 django_cache_pydantic-0.1.0/README.rst
+-rw-rw-r--   0 druid     (1000) druid     (1000)     2015 2024-05-10 09:26:36.000000 django_cache_pydantic-0.1.0/pyproject.toml
+-rw-rw-r--   0 druid     (1000) druid     (1000)       38 2024-05-10 09:27:38.928264 django_cache_pydantic-0.1.0/setup.cfg
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-05-10 09:27:38.924265 django_cache_pydantic-0.1.0/src/
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-05-10 09:27:38.928264 django_cache_pydantic-0.1.0/src/django_cache_pydantic/
+-rw-rw-r--   0 druid     (1000) druid     (1000)       38 2024-03-09 15:08:25.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic/__init__.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)      191 2024-03-15 14:24:29.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic/apps.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)     2453 2024-05-10 09:26:36.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic/base.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)      525 2024-03-15 14:24:29.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic/conf.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)       83 2024-03-09 11:16:25.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic/defaults.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)     1991 2024-05-10 09:26:36.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic/manager.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)     1588 2024-03-15 14:24:29.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic/options.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)        0 2024-03-08 22:52:06.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic/py.typed
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-05-10 09:27:38.928264 django_cache_pydantic-0.1.0/src/django_cache_pydantic.egg-info/
+-rw-r--r--   0 druid     (1000) druid     (1000)     4736 2024-05-10 09:27:38.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 druid     (1000) druid     (1000)      590 2024-05-10 09:27:38.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 druid     (1000) druid     (1000)        1 2024-05-10 09:27:38.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 druid     (1000) druid     (1000)       26 2024-05-10 09:27:38.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 druid     (1000) druid     (1000)       22 2024-05-10 09:27:38.000000 django_cache_pydantic-0.1.0/src/django_cache_pydantic.egg-info/top_level.txt
```

### Comparing `django-cache-pydantic-0.0.4/LICENSE` & `django_cache_pydantic-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cache-pydantic-0.0.4/PKG-INFO` & `django_cache_pydantic-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cache-pydantic
-Version: 0.0.4
+Version: 0.1.0
 Summary: Django application to integrate pydantic models into django cache with an orm interface.
 Author-email: Ali Abharya <abharya.dev@gmail.com>
 Maintainer-email: Ali Abharya <abharya.dev@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/bindruid/django-cache-pydantic/blob/master/CHANGELOG.rst
 Project-URL: Repository, https://github.com/bindruid/django-cache-pydantic
 Keywords: cache,django,pydantic,orm
@@ -38,16 +38,16 @@
 Django Cache Pydantic is a minimal wrapper around django cache framework which allows you
 to create pydantic instances directly inside your django project cache and retrieve them
 using a similar interface like django orm.
 
 Status
 ------
 
-.. image:: https://github.com/bindruid/django-cache-pydantic/workflows/Test/badge.svg?branch=master
-   :target: https://github.com/bindruid/django-cache-pydantic/actions
+.. image:: https://img.shields.io/github/actions/workflow/status/bindruid/django-cache-pydantic/test.yml.svg?branch=master
+   :target: https://github.com/bindruid/django-cache-pydantic/actions?workflow=Test
 
 .. image:: https://img.shields.io/pypi/v/django-cache-pydantic.svg
    :target: https://pypi.python.org/pypi/django-cache-pydantic
 
 .. image:: https://img.shields.io/pypi/pyversions/django-cache-pydantic.svg
    :target: https://pypi.org/project/django-cache-pydantic
```

### Comparing `django-cache-pydantic-0.0.4/README.rst` & `django_cache_pydantic-0.1.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 Django Cache Pydantic is a minimal wrapper around django cache framework which allows you
 to create pydantic instances directly inside your django project cache and retrieve them
 using a similar interface like django orm.
 
 Status
 ------
 
-.. image:: https://github.com/bindruid/django-cache-pydantic/workflows/Test/badge.svg?branch=master
-   :target: https://github.com/bindruid/django-cache-pydantic/actions
+.. image:: https://img.shields.io/github/actions/workflow/status/bindruid/django-cache-pydantic/test.yml.svg?branch=master
+   :target: https://github.com/bindruid/django-cache-pydantic/actions?workflow=Test
 
 .. image:: https://img.shields.io/pypi/v/django-cache-pydantic.svg
    :target: https://pypi.python.org/pypi/django-cache-pydantic
 
 .. image:: https://img.shields.io/pypi/pyversions/django-cache-pydantic.svg
    :target: https://pypi.org/project/django-cache-pydantic
```

### Comparing `django-cache-pydantic-0.0.4/pyproject.toml` & `django_cache_pydantic-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools",
 ]
 
 [project]
 name = "django-cache-pydantic"
-version = "0.0.4"
+version = "0.1.0"
 description = "Django application to integrate pydantic models into django cache with an orm interface."
 keywords = [
   "cache",
   "django",
   "pydantic",
   "orm",
 ]
```

### Comparing `django-cache-pydantic-0.0.4/src/django_cache_pydantic/base.py` & `django_cache_pydantic-0.1.0/src/django_cache_pydantic/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,34 +32,46 @@
         if cache_class is not None and type(cache_class) is not type:
             raise TypeError('CacheMeta should be a class and not of type %s' % type(cache_class))
         new_cache_class = CacheMetaOptions(cls, cache_class).define_options_class()
         setattr(cls, '_cache_meta', new_cache_class)
 
     def __init__(self, /, **data):
         super().__init__(**data)
-        internal_id = uuid4().hex
-        setattr(self, '_id', internal_id)
+        _internal_id = uuid4().hex
+        setattr(self, '_internal_id', _internal_id)
 
     @computed_field
     def id(self) -> str:
         """
         Computed property for generating the composite ID.
 
         :return: str: The composite ID.
         """
-        internal_id = self._id
-        cache_key = internal_id
         pk_field = getattr(self.CacheMeta, 'primary_key_field', None)
-        if pk_field is not None:
-            cache_key = str(getattr(self, pk_field))
-        return cache_key
+        return getattr(self, pk_field) if pk_field is not None else self._internal_id
+
+    def _get_composite_id(self) -> str:
+        """
+        Returns composite ID composed of class name and internal id.
+        :return: str: The composite ID.
+        """
+        return f'{self.__class__.__name__.lower()}__{self.id}'
 
     @computed_field
     def pk(self) -> str:
         return self.id
 
     def save(self):
         """
         Saves the instance in the cache with a specified time-to-live (ttl).
         """
         cache = self._cache_meta.cache_backend
-        cache.set(self.pk, self, self._cache_meta.ttl)
+        composite_id = self._get_composite_id()
+        cache.set(composite_id, self, self._cache_meta.ttl)
+
+    def delete(self):
+        """
+        Delete the instance from the cache.
+        """
+        cache = self._cache_meta.cache_backend
+        composite_id = self._get_composite_id()
+        cache.delete(composite_id)
```

### Comparing `django-cache-pydantic-0.0.4/src/django_cache_pydantic/conf.py` & `django_cache_pydantic-0.1.0/src/django_cache_pydantic/conf.py`

 * *Files identical despite different names*

### Comparing `django-cache-pydantic-0.0.4/src/django_cache_pydantic/manager.py` & `django_cache_pydantic-0.1.0/src/django_cache_pydantic/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,25 @@
 
     def get(self, pk):
         """
         Retrieve a model instance from the cache based on the primary key.
         """
 
         cache = self.cache_meta_class.cache_backend
-        return cache.get(pk)
+        composite_id = f'{self.model_class.__name__.lower()}__{pk}'
+        return cache.get(composite_id)
+
+    def delete(self, pk):
+        """
+        Delete a model instance from the cache based on the primary key.
+        """
+
+        cache = self.cache_meta_class.cache_backend
+        composite_id = f'{self.model_class.__name__.lower()}__{pk}'
+        return cache.delete(composite_id)
 
 
 class CacheManager:
     """
     Descriptor class allowing to access objects manager from class not instances.
     """
```

### Comparing `django-cache-pydantic-0.0.4/src/django_cache_pydantic/options.py` & `django_cache_pydantic-0.1.0/src/django_cache_pydantic/options.py`

 * *Files identical despite different names*

### Comparing `django-cache-pydantic-0.0.4/src/django_cache_pydantic.egg-info/PKG-INFO` & `django_cache_pydantic-0.1.0/src/django_cache_pydantic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cache-pydantic
-Version: 0.0.4
+Version: 0.1.0
 Summary: Django application to integrate pydantic models into django cache with an orm interface.
 Author-email: Ali Abharya <abharya.dev@gmail.com>
 Maintainer-email: Ali Abharya <abharya.dev@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/bindruid/django-cache-pydantic/blob/master/CHANGELOG.rst
 Project-URL: Repository, https://github.com/bindruid/django-cache-pydantic
 Keywords: cache,django,pydantic,orm
@@ -38,16 +38,16 @@
 Django Cache Pydantic is a minimal wrapper around django cache framework which allows you
 to create pydantic instances directly inside your django project cache and retrieve them
 using a similar interface like django orm.
 
 Status
 ------
 
-.. image:: https://github.com/bindruid/django-cache-pydantic/workflows/Test/badge.svg?branch=master
-   :target: https://github.com/bindruid/django-cache-pydantic/actions
+.. image:: https://img.shields.io/github/actions/workflow/status/bindruid/django-cache-pydantic/test.yml.svg?branch=master
+   :target: https://github.com/bindruid/django-cache-pydantic/actions?workflow=Test
 
 .. image:: https://img.shields.io/pypi/v/django-cache-pydantic.svg
    :target: https://pypi.python.org/pypi/django-cache-pydantic
 
 .. image:: https://img.shields.io/pypi/pyversions/django-cache-pydantic.svg
    :target: https://pypi.org/project/django-cache-pydantic
```

### Comparing `django-cache-pydantic-0.0.4/src/django_cache_pydantic.egg-info/SOURCES.txt` & `django_cache_pydantic-0.1.0/src/django_cache_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

