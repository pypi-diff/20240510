# Comparing `tmp/mrkutil-1.3.3.tar.gz` & `tmp/mrkutil-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrkutil-1.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mrkutil-1.3.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mrkutil-1.3.3.tar` & `mrkutil-1.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       91 2024-04-10 18:38:36.896155 mrkutil-1.3.3/.flake8
--rw-r--r--   0        0        0     1800 2024-04-10 13:44:48.196615 mrkutil-1.3.3/.gitignore
--rw-r--r--   0        0        0      366 2024-04-10 18:38:32.560123 mrkutil-1.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2024-04-10 13:44:48.196615 mrkutil-1.3.3/LICENSE
--rw-r--r--   0        0        0     3057 2024-04-11 06:14:47.021960 mrkutil-1.3.3/README.md
--rw-r--r--   0        0        0      113 2024-05-07 05:20:50.197943 mrkutil-1.3.3/mrkutil/__init__.py
--rw-r--r--   0        0        0       72 2024-04-10 13:44:48.196615 mrkutil-1.3.3/mrkutil/base/__init__.py
--rw-r--r--   0        0        0     1748 2024-04-10 19:00:33.746768 mrkutil-1.3.3/mrkutil/base/base_handler.py
--rw-r--r--   0        0        0       94 2024-04-29 09:23:03.607864 mrkutil-1.3.3/mrkutil/cache/__init__.py
--rw-r--r--   0        0        0     5269 2024-05-07 05:21:12.746133 mrkutil-1.3.3/mrkutil/cache/base_redis.py
--rw-r--r--   0        0        0      262 2024-04-24 12:44:29.700772 mrkutil-1.3.3/mrkutil/communication/__init__.py
--rw-r--r--   0        0        0     1462 2024-04-24 11:50:42.829911 mrkutil-1.3.3/mrkutil/communication/call_service.py
--rw-r--r--   0        0        0     3162 2024-04-24 14:31:17.548693 mrkutil-1.3.3/mrkutil/communication/listen.py
--rw-r--r--   0        0        0     1375 2024-04-24 12:37:29.267696 mrkutil-1.3.3/mrkutil/communication/trigger_service.py
--rw-r--r--   0        0        0      154 2024-04-10 13:44:48.196615 mrkutil-1.3.3/mrkutil/logging/__init__.py
--rw-r--r--   0        0        0     2681 2024-04-10 19:05:36.249709 mrkutil-1.3.3/mrkutil/logging/logging_config.py
--rw-r--r--   0        0        0     1831 2024-04-10 19:05:53.713880 mrkutil-1.3.3/mrkutil/logging/logging_formatter.py
--rw-r--r--   0        0        0      143 2024-04-10 13:44:48.196615 mrkutil-1.3.3/mrkutil/pagination/__init__.py
--rw-r--r--   0        0        0      805 2024-04-10 19:06:55.098484 mrkutil-1.3.3/mrkutil/pagination/dependency.py
--rw-r--r--   0        0        0     1692 2024-04-10 19:12:12.205642 mrkutil-1.3.3/mrkutil/pagination/mongoengine.py
--rw-r--r--   0        0        0     2552 2024-04-10 19:12:07.341593 mrkutil-1.3.3/mrkutil/pagination/sqlalchemy.py
--rw-r--r--   0        0        0       77 2024-04-10 18:53:14.101683 mrkutil-1.3.3/mrkutil/responses/__init__.py
--rw-r--r--   0        0        0     3225 2024-04-12 08:51:40.055110 mrkutil-1.3.3/mrkutil/responses/response_helper.py
--rw-r--r--   0        0        0      256 2024-04-10 18:53:21.969785 mrkutil-1.3.3/mrkutil/utilities.py
--rw-r--r--   0        0        0      822 2024-04-24 12:36:34.647032 mrkutil-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mrkutil-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-04-10 18:38:36.896155 mrkutil-1.3.5/.flake8
+-rw-r--r--   0        0        0     1800 2024-04-10 13:44:48.196615 mrkutil-1.3.5/.gitignore
+-rw-r--r--   0        0        0      366 2024-04-10 18:38:32.560123 mrkutil-1.3.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2024-04-10 13:44:48.196615 mrkutil-1.3.5/LICENSE
+-rw-r--r--   0        0        0     3057 2024-04-11 06:14:47.021960 mrkutil-1.3.5/README.md
+-rw-r--r--   0        0        0      113 2024-05-09 17:18:57.797812 mrkutil-1.3.5/mrkutil/__init__.py
+-rw-r--r--   0        0        0       72 2024-04-10 13:44:48.196615 mrkutil-1.3.5/mrkutil/base/__init__.py
+-rw-r--r--   0        0        0     1748 2024-04-10 19:00:33.746768 mrkutil-1.3.5/mrkutil/base/base_handler.py
+-rw-r--r--   0        0        0       94 2024-04-29 09:23:03.607864 mrkutil-1.3.5/mrkutil/cache/__init__.py
+-rw-r--r--   0        0        0     5269 2024-05-07 05:21:12.746133 mrkutil-1.3.5/mrkutil/cache/base_redis.py
+-rw-r--r--   0        0        0      262 2024-04-24 12:44:29.700772 mrkutil-1.3.5/mrkutil/communication/__init__.py
+-rw-r--r--   0        0        0     1462 2024-04-24 11:50:42.829911 mrkutil-1.3.5/mrkutil/communication/call_service.py
+-rw-r--r--   0        0        0     3162 2024-04-24 14:31:17.548693 mrkutil-1.3.5/mrkutil/communication/listen.py
+-rw-r--r--   0        0        0     1375 2024-04-24 12:37:29.267696 mrkutil-1.3.5/mrkutil/communication/trigger_service.py
+-rw-r--r--   0        0        0      154 2024-04-10 13:44:48.196615 mrkutil-1.3.5/mrkutil/logging/__init__.py
+-rw-r--r--   0        0        0     2681 2024-04-10 19:05:36.249709 mrkutil-1.3.5/mrkutil/logging/logging_config.py
+-rw-r--r--   0        0        0     1831 2024-04-10 19:05:53.713880 mrkutil-1.3.5/mrkutil/logging/logging_formatter.py
+-rw-r--r--   0        0        0       82 2024-05-09 15:50:48.203270 mrkutil-1.3.5/mrkutil/pagination/__init__.py
+-rw-r--r--   0        0        0      805 2024-04-10 19:06:55.098484 mrkutil-1.3.5/mrkutil/pagination/dependency.py
+-rw-r--r--   0        0        0     1692 2024-04-10 19:12:12.205642 mrkutil-1.3.5/mrkutil/pagination/mongoengine.py
+-rw-r--r--   0        0        0     3051 2024-05-09 17:18:46.497731 mrkutil-1.3.5/mrkutil/pagination/sqlalchemy.py
+-rw-r--r--   0        0        0       77 2024-04-10 18:53:14.101683 mrkutil-1.3.5/mrkutil/responses/__init__.py
+-rw-r--r--   0        0        0     3225 2024-04-12 08:51:40.055110 mrkutil-1.3.5/mrkutil/responses/response_helper.py
+-rw-r--r--   0        0        0      256 2024-04-10 18:53:21.969785 mrkutil-1.3.5/mrkutil/utilities.py
+-rw-r--r--   0        0        0      822 2024-04-24 12:36:34.647032 mrkutil-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mrkutil-1.3.5/PKG-INFO
```

### Comparing `mrkutil-1.3.3/.gitignore` & `mrkutil-1.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/LICENSE` & `mrkutil-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/README.md` & `mrkutil-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/mrkutil/base/base_handler.py` & `mrkutil-1.3.5/mrkutil/base/base_handler.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/mrkutil/cache/base_redis.py` & `mrkutil-1.3.5/mrkutil/cache/base_redis.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/mrkutil/communication/call_service.py` & `mrkutil-1.3.5/mrkutil/communication/call_service.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/mrkutil/communication/listen.py` & `mrkutil-1.3.5/mrkutil/communication/listen.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/mrkutil/communication/trigger_service.py` & `mrkutil-1.3.5/mrkutil/communication/trigger_service.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/mrkutil/logging/logging_config.py` & `mrkutil-1.3.5/mrkutil/logging/logging_config.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/mrkutil/logging/logging_formatter.py` & `mrkutil-1.3.5/mrkutil/logging/logging_formatter.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/mrkutil/pagination/dependency.py` & `mrkutil-1.3.5/mrkutil/pagination/dependency.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/mrkutil/pagination/mongoengine.py` & `mrkutil-1.3.5/mrkutil/pagination/mongoengine.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/mrkutil/pagination/sqlalchemy.py` & `mrkutil-1.3.5/mrkutil/pagination/sqlalchemy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,42 @@
+from typing import Optional
+from sqlalchemy import select, func, desc, Select, inspect, asc
+from sqlalchemy.orm import Session
+
+
 def paginate(
-    query,
+    query: Select,
+    session: Session,
+    recurse: bool = True,
     page_number: int = None,
     page_size: int = None,
     direction: str = None,
     sort_by: str = None,
 ):
     """Apply pagination to a SQLAlchemy query object.
+    :param query:
+        SQLAlchemy Select object.
+    :param session:
+        SQLAlchemy Session object.
     :param page_number:
         Page to be returned (starts and defaults to 1).
     :param page_size:
         Maximum number of results to be returned in the page (defaults
         to the total results).
     :param direction:
         Direction of ordering, asc or desc
     :param sort_by:
         Column for sorting
     :returns:
-        A dict with items(sqlalchemy objects converted to dict),
+        A dict with items (SQLAlchemy objects converted to dict),
         page number, desired page size, total number of results
     Basic usage::
-        object = paginate(query, 1, 10, "asc", "email")
+        object = paginate(select([User]), session, 1, 10, "asc", "email")
     """
-    total_results = query.count()
+    total_results = session.scalar(select(func.count()).select_from(query.subquery()))
 
     query = _sort_by(query, direction, sort_by)
 
     query = _limit(query, page_size)
 
     # cast to int if params are str
     if isinstance(page_number, str):
@@ -39,51 +50,55 @@
 
     query = _offset(query, page_number, page_size)
 
     # Page number defaults to 1
     if page_number is None:
         page_number = 1
 
+    results = session.scalars(query).all()
+
     return {
-        "items": [k._asdict() for k in query.all()],
+        "items": [k.to_dict(recurse=recurse) for k in results],
         "page": page_number,
         "size": page_size,
         "total": total_results,
     }
 
 
-def _limit(query, page_size):
+def _limit(query: Select, page_size: Optional[int]) -> Select:
     if page_size is not None:
         if page_size < 0:
             raise Exception("Page size should not be negative: {}".format(page_size))
 
         query = query.limit(page_size)
 
     return query
 
 
-def _offset(query, page_number, page_size):
+def _offset(
+    query: Select, page_number: Optional[int], page_size: Optional[int]
+) -> Select:
     if page_number is not None:
         if page_number < 1:
             raise Exception("Page number should be positive: {}".format(page_number))
 
         query = query.offset((page_number - 1) * page_size)
 
     return query
 
 
-def _sort_by(query, direction, sort_by):
+def _sort_by(query: Select, direction: Optional[str], sort_by: Optional[str]) -> Select:
     """
-    If None is passed to sqlalchemy order_by, it will do default sorting
-    This way we are allowing sorting by ascending/descending without a specified
-    sort by parameter
+    Sorts query by a specific column in ascending or descending order,
+    after verifying that the column exists.
     """
-    # check if sort by exists in columns otherwise default it to None
-    if sort_by not in query.statement.columns.keys():
-        sort_by = None
-    if direction == "desc":
-        from sqlalchemy import desc
+    if sort_by:
+        columns = [column.key for column in inspect(query).c]
+        if sort_by not in columns:
+            sort_by = None
 
+    if sort_by and direction == "desc":
         query = query.order_by(desc(sort_by))
-    else:
-        query = query.order_by(sort_by)
+    elif sort_by and direction == "asc":
+        query = query.order_by(asc(sort_by))
+
     return query
```

### Comparing `mrkutil-1.3.3/mrkutil/responses/response_helper.py` & `mrkutil-1.3.5/mrkutil/responses/response_helper.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/pyproject.toml` & `mrkutil-1.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.3/PKG-INFO` & `mrkutil-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrkutil
-Version: 1.3.3
+Version: 1.3.5
 Summary: Python package containing common functions for python service based architecture.
 Author-email: Nebojsa Mrkic <mrkic.nebojsa@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: RabbitMQPubSub>=1.1.1
 Requires-Dist: redis>=4.3 ; extra == "extras"
 Requires-Dist: sqlalchemy>=1.4 ; extra == "extras"
```

