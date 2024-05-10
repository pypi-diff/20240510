# Comparing `tmp/heimdall_tools-0.1.2.tar.gz` & `tmp/heimdall_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heimdall_tools-0.1.2.tar", last modified: Tue Apr 23 07:53:45 2024, max compression
+gzip compressed data, was "heimdall_tools-0.2.0.tar", last modified: Fri May 10 13:37:39 2024, max compression
```

## Comparing `heimdall_tools-0.1.2.tar` & `heimdall_tools-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-23 07:53:45.421256 heimdall_tools-0.1.2/
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)     1177 2024-04-23 07:53:45.417749 heimdall_tools-0.1.2/PKG-INFO
--rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)      576 2024-04-23 07:53:00.000000 heimdall_tools-0.1.2/README.md
-drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-23 07:53:45.409654 heimdall_tools-0.1.2/heimdall_tools/
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)      121 2024-04-08 13:34:54.000000 heimdall_tools-0.1.2/heimdall_tools/__init__.py
--rwxr-xr-x   0 pediashops  (1000) pediashops  (1000)     2458 2024-04-23 07:52:00.000000 heimdall_tools-0.1.2/heimdall_tools/mysql_client.py
--rwxr-xr-x   0 pediashops  (1000) pediashops  (1000)      806 2024-04-08 11:55:43.000000 heimdall_tools-0.1.2/heimdall_tools/sns.py
--rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)     1208 2024-04-11 13:49:12.000000 heimdall_tools-0.1.2/heimdall_tools/sqs.py
-drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-23 07:53:45.417749 heimdall_tools-0.1.2/heimdall_tools.egg-info/
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)     1177 2024-04-23 07:53:44.000000 heimdall_tools-0.1.2/heimdall_tools.egg-info/PKG-INFO
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)      309 2024-04-23 07:53:45.000000 heimdall_tools-0.1.2/heimdall_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)        1 2024-04-23 07:53:44.000000 heimdall_tools-0.1.2/heimdall_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)       29 2024-04-23 07:53:44.000000 heimdall_tools-0.1.2/heimdall_tools.egg-info/requires.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)       15 2024-04-23 07:53:44.000000 heimdall_tools-0.1.2/heimdall_tools.egg-info/top_level.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)       38 2024-04-23 07:53:45.421256 heimdall_tools-0.1.2/setup.cfg
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)      861 2024-04-23 07:53:35.000000 heimdall_tools-0.1.2/setup.py
+drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-05-10 13:37:39.307482 heimdall_tools-0.2.0/
+-rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)     1119 2024-04-21 16:43:44.000000 heimdall_tools-0.2.0/LICENSE
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)     1041 2024-05-10 13:37:39.307482 heimdall_tools-0.2.0/PKG-INFO
+-rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)      598 2024-04-23 12:30:33.000000 heimdall_tools-0.2.0/README.md
+drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-05-10 13:37:39.270983 heimdall_tools-0.2.0/heimdall_tools/
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)      121 2024-04-08 13:34:54.000000 heimdall_tools-0.2.0/heimdall_tools/__init__.py
+-rwxr-xr-x   0 pediashops  (1000) pediashops  (1000)     2564 2024-04-30 16:25:01.000000 heimdall_tools-0.2.0/heimdall_tools/mysql_client.py
+-rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)      395 2024-05-10 13:34:29.000000 heimdall_tools-0.2.0/heimdall_tools/redis_client.py
+-rwxr-xr-x   0 pediashops  (1000) pediashops  (1000)      806 2024-04-24 12:11:04.000000 heimdall_tools-0.2.0/heimdall_tools/sns.py
+-rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)     1208 2024-04-11 13:49:12.000000 heimdall_tools-0.2.0/heimdall_tools/sqs.py
+drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-05-10 13:37:39.307482 heimdall_tools-0.2.0/heimdall_tools.egg-info/
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)     1041 2024-05-10 13:37:31.000000 heimdall_tools-0.2.0/heimdall_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)      348 2024-05-10 13:37:38.000000 heimdall_tools-0.2.0/heimdall_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)        1 2024-05-10 13:37:31.000000 heimdall_tools-0.2.0/heimdall_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)       12 2024-05-10 13:37:31.000000 heimdall_tools-0.2.0/heimdall_tools.egg-info/requires.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)       15 2024-05-10 13:37:31.000000 heimdall_tools-0.2.0/heimdall_tools.egg-info/top_level.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)       38 2024-05-10 13:37:39.307482 heimdall_tools-0.2.0/setup.cfg
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)      836 2024-05-10 13:36:48.000000 heimdall_tools-0.2.0/setup.py
```

### Comparing `heimdall_tools-0.1.2/PKG-INFO` & `heimdall_tools-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 Metadata-Version: 2.1
 Name: heimdall_tools
-Version: 0.1.2
+Version: 0.2.0
 Summary: Custom package including all modules required for my application
 Home-page: https://github.com/your_username/your_package
 Author: Robin Thomas
 Author-email: robin@clockhash.com
 License: MIT
-Description: # Heimdall Tools
-        
-        This is a custom package created to use different modules in a single place.
-        The wrapper methods are designed in a way to produce the best results to the application.
-        This helps in code reusability and to improve the performance of application
-        
-        # Create or modify package
-        
-        i. Add the new module in heimdall_tools folder
-        ii. Modify setup.py 
-            ..* add dependices
-        iii. Create the update package file
-        python setup.py sdist 
-        iv. Upload to pypi using twine
-        twine upload dist/*
-        
-        #  how to install package
-        
-        pip install [--upgrade] heimdall_tools
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Heimdall Tools
+
+This is a custom package created to use different modules in a single place.
+The wrapper methods are designed in a way to produce the best results to the application.
+This helps in code reusability and to improve the performance of application
+
+# Create or modify package
+
+i. Add the new module in heimdall_tools folder
+
+ii. Modify setup.py 
+
+    ..* add dependencies
+
+iii. Create the update package file
+
+    python setup.py sdist
+
+iv. Upload to pypi using twine
+s
+    twine upload dist/*
+
+#  How to install package
+
+pip install [--upgrade] heimdall_tools
```

### Comparing `heimdall_tools-0.1.2/README.md` & `heimdall_tools-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 This is a custom package created to use different modules in a single place.
 The wrapper methods are designed in a way to produce the best results to the application.
 This helps in code reusability and to improve the performance of application
 
 # Create or modify package
 
 i. Add the new module in heimdall_tools folder
+
 ii. Modify setup.py 
-    ..* add dependices
+
+    ..* add dependencies
+
 iii. Create the update package file
-python setup.py sdist 
+
+    python setup.py sdist
+
 iv. Upload to pypi using twine
-twine upload dist/*
+s
+    twine upload dist/*
 
-#  how to install package
+#  How to install package
 
 pip install [--upgrade] heimdall_tools
```

### Comparing `heimdall_tools-0.1.2/heimdall_tools/mysql_client.py` & `heimdall_tools-0.2.0/heimdall_tools/mysql_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#TODO Replace this with SQLAlchemy ORM
+
 import mysql.connector
 from typing import List, Tuple
 
 """""
 @dataclass
 class mysql:
     username: String
@@ -35,28 +37,29 @@
         #self.connection.commit()
 
     def db_read_result(self) -> List[Tuple]:
         result = self.cursor.fetchall()
         print(f'Read Result {result}')
         return result
 
+    #TODO change type_id to type_name for better readability
     def db_read_sensor_id_from_heimdall_memory(self, customer_name, site_name, building_name, floor_position, type_id, sensor_name) -> int:
         query =  """
         SELECT sensors.sensor_id
         FROM sensors
         JOIN floors ON sensors.floor_id = floors.floor_id
         JOIN buildings ON floors.building_id = buildings.building_id
         JOIN sites ON buildings.site_id = sites.site_id
         JOIN customers ON sites.customer_id = customers.customer_id
         JOIN sensor_type ON sensors.type_id = sensor_type.type_id
         WHERE customers.customer_name = %s
         AND sites.site_name = %s
         AND buildings.building_name = %s
         AND floors.floor_position = %s
-        AND sensor_type.type_id = %s
+        AND sensor_type.type_name = %s
         AND sensors.sensor_name = %s
         """
         # Execute the query
         self.cursor.execute(query, (customer_name, site_name, building_name, floor_position, type_id, sensor_name))
         result = self.cursor.fetchone()
         if result:
             print(f"MYSQL LOGS: Result --> {result}")
```

### Comparing `heimdall_tools-0.1.2/heimdall_tools/sns.py` & `heimdall_tools-0.2.0/heimdall_tools/sns.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This is an AWS SNS module. The processed MQTT messages will be sent to SNS topic by other services.
 # There will be an different subscribers to SNS to queue/notify the messages for further processing.
 # In the architecture, an HTTP endpoint shall read data from SQS for further processing in most of the cases.
 
 import json
 import boto3
 
-def post_to_sns_topic(region, arn, key, value, topic):
+def post_to_sns_topic(region, arn, topic, key, value):
     sns_client = boto3.client('sns', region_name = region)  # Replace 'your_region' with your AWS region
 
     message = {
         "key": key,
         "value" : value,
         "topic" : topic
     }
```

### Comparing `heimdall_tools-0.1.2/heimdall_tools/sqs.py` & `heimdall_tools-0.2.0/heimdall_tools/sqs.py`

 * *Files identical despite different names*

### Comparing `heimdall_tools-0.1.2/heimdall_tools.egg-info/PKG-INFO` & `heimdall_tools-0.2.0/heimdall_tools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 Metadata-Version: 2.1
 Name: heimdall-tools
-Version: 0.1.2
+Version: 0.2.0
 Summary: Custom package including all modules required for my application
 Home-page: https://github.com/your_username/your_package
 Author: Robin Thomas
 Author-email: robin@clockhash.com
 License: MIT
-Description: # Heimdall Tools
-        
-        This is a custom package created to use different modules in a single place.
-        The wrapper methods are designed in a way to produce the best results to the application.
-        This helps in code reusability and to improve the performance of application
-        
-        # Create or modify package
-        
-        i. Add the new module in heimdall_tools folder
-        ii. Modify setup.py 
-            ..* add dependices
-        iii. Create the update package file
-        python setup.py sdist 
-        iv. Upload to pypi using twine
-        twine upload dist/*
-        
-        #  how to install package
-        
-        pip install [--upgrade] heimdall_tools
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Heimdall Tools
+
+This is a custom package created to use different modules in a single place.
+The wrapper methods are designed in a way to produce the best results to the application.
+This helps in code reusability and to improve the performance of application
+
+# Create or modify package
+
+i. Add the new module in heimdall_tools folder
+
+ii. Modify setup.py 
+
+    ..* add dependencies
+
+iii. Create the update package file
+
+    python setup.py sdist
+
+iv. Upload to pypi using twine
+s
+    twine upload dist/*
+
+#  How to install package
+
+pip install [--upgrade] heimdall_tools
```

### Comparing `heimdall_tools-0.1.2/setup.py` & `heimdall_tools-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 from setuptools import setup, find_packages
 
 packs= find_packages()
 print(packs)
 
 setup(
     name='heimdall_tools',
-    version='0.1.2',
+    version='0.2.0',
     packages=find_packages(),
-    #packages=['heimdall_tools'],
     install_requires=[
-        'boto3',
-        'mysql-connector-python',
+        'boto3', #sqs, sns
+        'redis' # redis_client.py
         # Add any other dependencies here
     ],
     author='Robin Thomas',
     author_email='robin@clockhash.com',
     description='Custom package including all modules required for my application',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

