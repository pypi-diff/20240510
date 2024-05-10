# Comparing `tmp/phones_local-0.0.19.tar.gz` & `tmp/phones_local-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.19.tar", last modified: Thu May  9 07:25:56 2024, max compression
+gzip compressed data, was "phones_local-0.0.20.tar", last modified: Fri May 10 02:19:53 2024, max compression
```

## Comparing `phones_local-0.0.19.tar` & `phones_local-0.0.20.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:25:56.277891 phones_local-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-09 07:25:56.277891 phones_local-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-09 07:25:28.000000 phones_local-0.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:25:56.273891 phones_local-0.0.19/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:25:56.277891 phones_local-0.0.19/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:25:28.000000 phones_local-0.0.19/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-09 07:25:28.000000 phones_local-0.0.19/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-09 07:25:28.000000 phones_local-0.0.19/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:25:56.277891 phones_local-0.0.19/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-09 07:25:56.000000 phones_local-0.0.19/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-09 07:25:56.000000 phones_local-0.0.19/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:25:56.000000 phones_local-0.0.19/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-09 07:25:56.000000 phones_local-0.0.19/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 07:25:56.000000 phones_local-0.0.19/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-09 07:25:28.000000 phones_local-0.0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:25:56.277891 phones_local-0.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-09 07:25:28.000000 phones_local-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:19:53.289062 phones_local-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 02:19:53.289062 phones_local-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-10 02:19:28.000000 phones_local-0.0.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:19:53.285062 phones_local-0.0.20/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:19:53.289062 phones_local-0.0.20/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:19:28.000000 phones_local-0.0.20/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-10 02:19:28.000000 phones_local-0.0.20/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-10 02:19:28.000000 phones_local-0.0.20/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:19:53.289062 phones_local-0.0.20/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 02:19:53.000000 phones_local-0.0.20/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-10 02:19:53.000000 phones_local-0.0.20/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 02:19:53.000000 phones_local-0.0.20/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 02:19:53.000000 phones_local-0.0.20/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 02:19:53.000000 phones_local-0.0.20/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-10 02:19:28.000000 phones_local-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 02:19:53.289062 phones_local-0.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 02:19:28.000000 phones_local-0.0.20/setup.py
```

### Comparing `phones_local-0.0.19/PKG-INFO` & `phones_local-0.0.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.19
+Version: 0.0.20
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.19/README.md` & `phones_local-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.19/phones_local/src/phone_local_constans.py` & `phones_local-0.0.20/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.19/phones_local/src/phones_local.py` & `phones_local-0.0.20/phones_local/src/phones_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from database_mysql_local.generic_mapping import GenericMapping
 from logger_local.LoggerLocal import Logger
 from phonenumbers import (NumberParseException, PhoneNumberFormat,
                           format_number, parse)
+from user_context_remote.user_context import UserContext
 
 from .phone_local_constans import code_object_init
 
 logger = Logger.create_logger(object=code_object_init)
+user_context = UserContext()
 
 
 class PhonesLocal(GenericMapping):
     def __init__(self) -> None:
         super().__init__(default_schema_name="phone",
                          default_table_name="phone_table",
                          default_view_table_name="phone_view",
@@ -63,38 +65,38 @@
             "full_number_normalized": "+972549338666"
         }
         """
         try:
             parsed_number = parse(original_number, region)
             international_code = parsed_number.country_code
             full_number_normalized = format_number(parsed_number, PhoneNumberFormat.E164)
+            # parsed_number example: original_number='0687473298' -> PhoneNumber(country_code=972, national_number=687473298, extension=None, italian_leading_zero=None, number_of_leading_zeros=None, country_code_source=0, preferred_domestic_carrier_code=None)
             number_info = {
                 "international_code": international_code,
                 "full_number_normalized": full_number_normalized,
                 "extension": parsed_number.extension,
             }
             return number_info
         except NumberParseException as e:
-            logger.error(f"Invalid phone number: {original_number}.", object=e)
+            logger.exception(f"Invalid phone number: {original_number}.", object=e)
             raise e
 
-    def get_country_iso_code(self, details: dict) -> str:
-        contact_id = details.get('contact_id')
-        profile_id = details.get('profile_id')
-        location_id = details.get('location_id')
-        country_id = details.get('country_id')
+    def get_country_iso_code(self) -> str:
+        contact_id = None  # user_context.get_effective_contact_id()
+        profile_id = user_context.get_effective_profile_id()
+        location_id = None  # user_context.get_effective_location_id()
+        country_id = None  # user_context.get_effective_country_id()
 
         if not country_id:  # get country_id from location_id
             if not location_id:  # get location_id from contact_id or profile_id
                 if contact_id and not profile_id:  # get profile_id from contact_id
                     profile_id = self.select_one_value_by_id(
                         schema_name="contact_profile",
                         view_table_name='contact_profile_view', select_clause_value='profile_id',
                         id_column_name='contact_id', id_column_value=contact_id)
-                    details['profile_id'] = profile_id
                 assert profile_id, "profile_id is required for getting location_id"
                 location_id = self.select_one_value_by_id(
                     schema_name="location_profile",
                     view_table_name='location_profile_view', select_clause_value='location_id',
                     id_column_name='profile_id', id_column_value=profile_id)
 
             assert location_id, "location_id is required for getting country_id"
@@ -106,50 +108,46 @@
             schema_name="country", view_table_name='country_ml_view', select_clause_value='iso',
             id_column_name='country_id', id_column_value=country_id)
         return country_iso_code
 
     # TODO: Is it really necessary to access the database for location?
     # I think it's possible to get the normalized phone number and the international code
     # from original_phone_number
-    def process_phone(self, original_phone_number: str, country_iso_code: str = None, details: dict = None) -> dict:
+    def process_phone(self, original_phone_number: str, country_iso_code: str = None, contact_id: int = None) -> dict:
         """
         Process phone number and return normalized phone number.
         :param original_phone_number: Original phone number.
         :param country_iso_code: Country ISO code.
-        :param details: Dictionary with the details of the phone number
-                (at least one of: country_id, location_id, profile_id, contact_id).
+        :param contact_id: Contact id.
         :return: Dictionary with the normalized phone number and the international code.
         """
-        details = details or {}
-        assert country_iso_code or details, "country_iso_code or details is required"
         logger.start(object={'original_phone_number': original_phone_number})
-        country_iso_code = country_iso_code or self.get_country_iso_code(details)
+        country_iso_code = country_iso_code or self.get_country_iso_code()
         normalized_phone_number = self.normalize_phone_number(
             original_number=original_phone_number, region=country_iso_code)
         phone_data = {
             'number_original': original_phone_number,
             'international_code': normalized_phone_number['international_code'],
             'full_number_normalized': normalized_phone_number['full_number_normalized'],
             'local_number_normalized': int(str(normalized_phone_number['full_number_normalized'])
                                            .replace(str(normalized_phone_number['international_code']), '')),
             'created_user_id': logger.user_context.get_effective_user_id(),
         }
         phone_id = self.insert(data_json=phone_data)
 
         # link phone to profile
-        profile_id = details.get('profile_id')
+        profile_id = user_context.get_effective_profile_id()
         if profile_id:
             phone_profile_id = self.insert_mapping(
                 schema_name='phone_profile',
                 entity_name1='phone', entity_name2='profile', entity_id1=phone_id, entity_id2=profile_id)
         else:
             phone_profile_id = None
 
         # link phone to contact
-        contact_id = details.get('contact_id')
         if contact_id:
             contact_phone_id = self.insert_mapping(
                 schema_name='contact_phone', entity_name1='contact', entity_name2='phone',
                 entity_id1=contact_id, entity_id2=phone_id)
         else:
             contact_phone_id = None
```

### Comparing `phones_local-0.0.19/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.20/phones_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.19
+Version: 0.0.20
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.19/pyproject.toml` & `phones_local-0.0.20/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.19/setup.py` & `phones_local-0.0.20/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.19',  # https://pypi.org/project/phones-local/
+    version='0.0.20',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

