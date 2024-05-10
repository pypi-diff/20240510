# Comparing `tmp/crud_repository-0.2.1.tar.gz` & `tmp/crud_repository-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crud_repository-0.2.1.tar", last modified: Wed May  8 08:03:15 2024, max compression
+gzip compressed data, was "crud_repository-0.2.2.tar", last modified: Fri May 10 08:37:31 2024, max compression
```

## Comparing `crud_repository-0.2.1.tar` & `crud_repository-0.2.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:15.205933 crud_repository-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 08:03:05.000000 crud_repository-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-08 08:03:05.000000 crud_repository-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-08 08:03:15.205933 crud_repository-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-08 08:03:05.000000 crud_repository-0.2.1/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-05-08 08:03:05.000000 crud_repository-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:15.201933 crud_repository-0.2.1/crud_repository/
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/__config__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:15.205933 crud_repository-0.2.1/crud_repository/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/db/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/db/idatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:15.205933 crud_repository-0.2.1/crud_repository/db/mariadb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/db/mariadb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/db/mariadb/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:15.205933 crud_repository-0.2.1/crud_repository/db/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/db/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/db/mysql/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:15.205933 crud_repository-0.2.1/crud_repository/db/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/db/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/db/postgres/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:15.205933 crud_repository-0.2.1/crud_repository/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:15.205933 crud_repository-0.2.1/crud_repository/my_logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/my_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/my_logger/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/my_logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/my_logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/my_logger/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:15.205933 crud_repository-0.2.1/crud_repository/repo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-08 08:03:05.000000 crud_repository-0.2.1/crud_repository/repo/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:15.205933 crud_repository-0.2.1/crud_repository.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-08 08:03:15.000000 crud_repository-0.2.1/crud_repository.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-08 08:03:15.000000 crud_repository-0.2.1/crud_repository.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:03:15.000000 crud_repository-0.2.1/crud_repository.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:03:15.000000 crud_repository-0.2.1/crud_repository.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 08:03:15.000000 crud_repository-0.2.1/crud_repository.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 08:03:15.000000 crud_repository-0.2.1/crud_repository.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 08:03:13.000000 crud_repository-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-08 08:03:15.209933 crud_repository-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-08 08:03:05.000000 crud_repository-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.946884 crud_repository-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-10 08:37:21.000000 crud_repository-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-10 08:37:21.000000 crud_repository-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-10 08:37:31.946884 crud_repository-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-10 08:37:21.000000 crud_repository-0.2.2/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16267 2024-05-10 08:37:21.000000 crud_repository-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/__config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/idatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/db/mariadb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/mariadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/mariadb/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/db/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/mysql/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/db/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/db/postgres/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.942885 crud_repository-0.2.2/crud_repository/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.946884 crud_repository-0.2.2/crud_repository/my_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/my_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/my_logger/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/my_logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/my_logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/my_logger/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.946884 crud_repository-0.2.2/crud_repository/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-10 08:37:21.000000 crud_repository-0.2.2/crud_repository/repo/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:37:31.946884 crud_repository-0.2.2/crud_repository.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 08:37:31.000000 crud_repository-0.2.2/crud_repository.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-10 08:37:30.000000 crud_repository-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-10 08:37:31.946884 crud_repository-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-10 08:37:21.000000 crud_repository-0.2.2/setup.py
```

### Comparing `crud_repository-0.2.1/LICENSE` & `crud_repository-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.1/MANIFEST.in` & `crud_repository-0.2.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.1/PKG-INFO` & `crud_repository-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.2.1
+Version: 0.2.2
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
         
@@ -24,15 +24,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/dellius-alexander/CRUDRepository.git
-Keywords: crud-repository,database,model,abstraction
+Keywords: crud-repository,database,model,abstraction,sqlalchemy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -155,20 +155,17 @@
         'password': "adminpassword",
         'host': "127.0.0.1",
         'port': "5432"
     }
     # Create a new database instance
     db = DatabaseFactory.create(db_config)
 
-    # Create a UserRepository instance with the database instance
-    user_repo = UserRepository(db)
-
-    # OR create a generic Repository instance with the 
+    # Create a User Repository instance with the 
     # database instance and the User model
-    #user_repo = Repository(db, User)
+    user_repo = Repository(db, User)
 
     # Create a new user
     user = User(username='Candy', password='password')
 
     # Add the user to the database
     user_repo.create(user)
 ```
```

### Comparing `crud_repository-0.2.1/PYPI.md` & `crud_repository-0.2.2/PYPI.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,20 +106,17 @@
         'password': "adminpassword",
         'host': "127.0.0.1",
         'port': "5432"
     }
     # Create a new database instance
     db = DatabaseFactory.create(db_config)
 
-    # Create a UserRepository instance with the database instance
-    user_repo = UserRepository(db)
-
-    # OR create a generic Repository instance with the 
+    # Create a User Repository instance with the 
     # database instance and the User model
-    #user_repo = Repository(db, User)
+    user_repo = Repository(db, User)
 
     # Create a new user
     user = User(username='Candy', password='password')
 
     # Add the user to the database
     user_repo.create(user)
 ```
```

### Comparing `crud_repository-0.2.1/README.md` & `crud_repository-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -385,22 +385,14 @@
     def __repr__(self) -> str:
         return (
             f"User(id={self.id!r}, name={self.username!r}, fullname={self.password!r})"
         )
 
 
 # ---------------------------------------------------------
-# Create a UserRepository instance with the database instance
-# ---------------------------------------------------------
-class UserRepository(Repository[User]):
-    def __init__(self, database: IDatabase):
-        super().__init__(database, User)
-
-
-# ---------------------------------------------------------
 # Create a new user
 # ---------------------------------------------------------
 if __name__ == '__main__':
     # Create a new database instance
     db_config = {
         'type': 'postgresql',
         'db_name': 'volunteer',
@@ -408,21 +400,23 @@
         'password': "adminpassword",
         'host': "127.0.0.1",
         'port': "5432"
     }
     # Create a new database instance
     db = DatabaseFactory.create(db_config)
 
-    # Create a UserRepository instance with the database instance
-    user_repo = UserRepository(db)
-
-    # OR create a generic Repository instance with the 
+    # Create a User Repository instance with the 
     # database instance and the User model
-    #user_repo = Repository(db, User)
+    user_repo = Repository(db, User)
 
     # Create a new user
     user = User(username='Candy', password='password')
 
     # Add the user to the database
     user_repo.create(user)
 ```
 ---
+Models:
+  * User: Represents a user entity with attributes id, username, password, email (email.id), address (address.id), role (role.id) last_updated
+  * Address: Represents an address entity with attributes id, street, city, state, zipcode, last_updated
+  * Role: Represents a role entity with attributes id, name, last_updated
+  * Email: Represents an email entity with attributes id, email, last_updated
```

### Comparing `crud_repository-0.2.1/crud_repository/__config__.py` & `crud_repository-0.2.2/crud_repository/__config__.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.1/crud_repository/db/idatabase.py` & `crud_repository-0.2.2/crud_repository/db/idatabase.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.1/crud_repository/db/mariadb/db.py` & `crud_repository-0.2.2/crud_repository/db/mariadb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,9 +56,9 @@
         except OperationalError as e:
             log.debug(f"Error connecting to MySQL database: {e}")
             traceback.print_exc()
             raise e
         except Exception as e:
             log.debug(f"Error initializing MySQL database: {e}")
             traceback.print_exc()
-            sys.exit(1)
+            raise e
```

### Comparing `crud_repository-0.2.1/crud_repository/db/mysql/db.py` & `crud_repository-0.2.2/crud_repository/db/mysql/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,19 +39,20 @@
             url = kwargs.get("url", f"mysql+pymysql://{user}:{password}@{host}:{port}/{db_name}")
             # Create the database if it doesn't exist
             if not database_exists(url):
                 create_database(url)
             # Create the engine and session
             self.engine = create_engine(url)
             self.session = scoped_session(sessionmaker(bind=self.engine))
-            # Add this line to create all tables based on Base class
+            # Create all tables for the specific database type
+            self.engine.echo = True
             Base.metadata.create_all(self.engine)
         except OperationalError as e:
             log.debug(f"Error connecting to MySQL database: {e}")
             traceback.print_exc()
             raise e
         except Exception as e:
             log.debug(f"Error initializing MySQL database: {e}")
             traceback.print_exc()
-            sys.exit(1)
+            raise e
```

### Comparing `crud_repository-0.2.1/crud_repository/db/postgres/db.py` & `crud_repository-0.2.2/crud_repository/db/postgres/db.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 This module provides classes for managing databases.
 """
+import sys
+import traceback
 from sqlalchemy import create_engine, Connection, text
+from sqlalchemy.exc import OperationalError
 from sqlalchemy.orm import scoped_session, sessionmaker
 from sqlalchemy_utils import database_exists, create_database
-
 from crud_repository.db.idatabase import IDatabase
 from crud_repository.model.base import Base
 from crud_repository.my_logger.logger import CustomLogger
 
 log = CustomLogger(__name__).get_logger("DEBUG")
 
 
@@ -21,22 +23,32 @@
     """
 
     def __init__(self, **kwargs):
         """
         Initialize the PostgreSQLDatabase.
         :param kwargs: (dict) The keyword arguments for the PostgreSQL database.
         """
-        db_name = kwargs.get("db_name", None)
-        user = kwargs.get("user", None)
-        password = kwargs.get("password", None)
-        host = kwargs.get("host", None)
-        port = kwargs.get("port", None)
-        url = kwargs.get("url", f"postgresql+psycopg2://{user}:{password}@{host}:{port}/{db_name}")
-        # Create the database if it doesn't exist
-        if not database_exists(url):
-            create_database(url)
-        # Create the engine and session
-        self.engine = create_engine(url)
-        self.session = scoped_session(sessionmaker(bind=self.engine))
-        Base.metadata.create_all(self.engine)
-
+        try:
+            db_name = kwargs.get("db_name", None)
+            user = kwargs.get("user", None)
+            password = kwargs.get("password", None)
+            host = kwargs.get("host", None)
+            port = kwargs.get("port", None)
+            url = kwargs.get("url", f"postgresql+psycopg2://{user}:{password}@{host}:{port}/{db_name}")
+            # Create the database if it doesn't exist
+            if not database_exists(url):
+                create_database(url)
+            # Create the engine and session
+            self.engine = create_engine(url)
+            self.session = scoped_session(sessionmaker(bind=self.engine))
+            # Create all tables for the specific database type
+            self.engine.echo = True
+            Base.metadata.create_all(self.engine)
+        except OperationalError as e:
+            log.debug(f"Error connecting to MySQL database: {e}")
+            traceback.print_exc()
+            raise e
+        except Exception as e:
+            log.debug(f"Error initializing MySQL database: {e}")
+            traceback.print_exc()
+            raise e
```

### Comparing `crud_repository-0.2.1/crud_repository/my_logger/formatters.py` & `crud_repository-0.2.2/crud_repository/my_logger/formatters.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.1/crud_repository/my_logger/handlers.py` & `crud_repository-0.2.2/crud_repository/my_logger/handlers.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.1/crud_repository/my_logger/logger.py` & `crud_repository-0.2.2/crud_repository/my_logger/logger.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.1/crud_repository/my_logger/monitor.py` & `crud_repository-0.2.2/crud_repository/my_logger/monitor.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.1/crud_repository/repo/repository.py` & `crud_repository-0.2.2/crud_repository/repo/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from abc import ABC, abstractmethod
-from typing import Generic, TypeVar
+from typing import Generic, TypeVar, Type
 import sqlalchemy
 from sqlalchemy.exc import SQLAlchemyError
 from crud_repository.db.idatabase import IDatabase
 from crud_repository.model.base import Base
 from crud_repository.my_logger.logger import CustomLogger
 
 log = CustomLogger(__name__).get_logger("DEBUG")
@@ -29,15 +29,15 @@
     @abstractmethod
     def delete(self, entity) -> None:
         pass
 
 
 # ---------------------------------------------------------
 class Repository(IRepository[T]):
-    def __init__(self, database: IDatabase, model: type[T]):
+    def __init__(self, database: IDatabase, model: Type[T]):
         self.database = database
         self.model = model
 
     def create(self, entity: T) -> T:
         session = self.database.get_scoped_session()
         try:
             session.add(entity)
```

### Comparing `crud_repository-0.2.1/crud_repository.egg-info/PKG-INFO` & `crud_repository-0.2.2/crud_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.2.1
+Version: 0.2.2
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
         
@@ -24,15 +24,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/dellius-alexander/CRUDRepository.git
-Keywords: crud-repository,database,model,abstraction
+Keywords: crud-repository,database,model,abstraction,sqlalchemy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -155,20 +155,17 @@
         'password': "adminpassword",
         'host': "127.0.0.1",
         'port': "5432"
     }
     # Create a new database instance
     db = DatabaseFactory.create(db_config)
 
-    # Create a UserRepository instance with the database instance
-    user_repo = UserRepository(db)
-
-    # OR create a generic Repository instance with the 
+    # Create a User Repository instance with the 
     # database instance and the User model
-    #user_repo = Repository(db, User)
+    user_repo = Repository(db, User)
 
     # Create a new user
     user = User(username='Candy', password='password')
 
     # Add the user to the database
     user_repo.create(user)
 ```
```

### Comparing `crud_repository-0.2.1/crud_repository.egg-info/SOURCES.txt` & `crud_repository-0.2.2/crud_repository.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crud_repository-0.2.1/pyproject.toml` & `crud_repository-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crud_repository"
-version = "0.2.1"
+version = "0.2.2"
 description = "The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases."
 authors = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"},
   {email = "info@hyfisolutions.com"},
 ]
 maintainers = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"}
 ]
 readme = {file = "PYPI.md", content-type = "text/markdown"}
-keywords = ["crud-repository", "database", "model", "abstraction"]
+keywords = ["crud-repository", "database", "model", "abstraction", "sqlalchemy"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `crud_repository-0.2.1/setup.py` & `crud_repository-0.2.2/setup.py`

 * *Files identical despite different names*

