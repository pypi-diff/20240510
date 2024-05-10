# Comparing `tmp/contact-person-profile-csv-imp-local-0.0.6.tar.gz` & `tmp/contact_person_profile_csv_imp_local-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-person-profile-csv-imp-local-0.0.6.tar", last modified: Tue Jan  2 16:39:50 2024, max compression
+gzip compressed data, was "contact_person_profile_csv_imp_local-0.0.7.tar", last modified: Fri May 10 04:47:58 2024, max compression
```

## Comparing `contact-person-profile-csv-imp-local-0.0.6.tar` & `contact_person_profile_csv_imp_local-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:39:50.033275 contact-person-profile-csv-imp-local-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-02 16:39:50.033275 contact-person-profile-csv-imp-local-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-01-02 16:39:14.000000 contact-person-profile-csv-imp-local-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:39:50.033275 contact-person-profile-csv-imp-local-0.0.6/contact_person_profile_csv_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-02 16:39:50.000000 contact-person-profile-csv-imp-local-0.0.6/contact_person_profile_csv_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-02 16:39:50.000000 contact-person-profile-csv-imp-local-0.0.6/contact_person_profile_csv_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 16:39:50.000000 contact-person-profile-csv-imp-local-0.0.6/contact_person_profile_csv_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 16:39:50.000000 contact-person-profile-csv-imp-local-0.0.6/contact_person_profile_csv_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-01-02 16:39:14.000000 contact-person-profile-csv-imp-local-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 16:39:50.033275 contact-person-profile-csv-imp-local-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-01-02 16:39:14.000000 contact-person-profile-csv-imp-local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:58.539374 contact_person_profile_csv_imp_local-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 04:47:58.539374 contact_person_profile_csv_imp_local-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:58.535374 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:58.539374 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    21321 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local/src/CSVToContactPersonProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:58.539374 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 04:47:58.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-10 04:47:58.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:47:58.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-10 04:47:58.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 04:47:58.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:47:58.539374 contact_person_profile_csv_imp_local-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/setup.py
```

### Comparing `contact-person-profile-csv-imp-local-0.0.6/README.md` & `contact_person_profile_csv_imp_local-0.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 # python-package-template
+
 To create local package and remote package layers (not to create GraphQL and REST-API layers)
 
 # directory structure
-Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e. location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br> 
+
+Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e.
+location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br>
 /location_local<br>
 /location_local/get_country_name<br>
 /location_local/get_country_name/src<br>
 /location_local/get_country_name/src/get_country_name.py<br>
 /location_local/get_country_name/tests<br>
 /location_local/get_country_name/tests/test_get_country_name.py<br>
 
 # database Python scripts in /db folder
+
 Please place <table-name>.py in /db<br>
 No need for seperate file for _ml table<br>
 Please delete the example file if not needed<br>
-  
+
 # Create the files to create the database schema, tables, view and populate Meta Data and Test Date
+
 /db/<table-name>.py - CREATE SCHEMA ... CREATE TABLE ... CREATE VIEW ...<br>
 /db/<table-name>_insert.py to create records
 
 # Update the setup.py (i.e.name, version)
- 
+
 # Please create test directory inside the directory of the project i.e. /<project-name>/tests
 
 # Update the serverless.yml in the root directory
+
 provider:
-  stage: play1
-  
+stage: play1
+
 Update the endpoints in serverless.yml
 
 # Working with VS Code
+
 Please make sure you push to the repo launch.json fie that enables to run and debug the code<br>
 
 # Unit-Test
+
 We prefer using pytest and not unittest package<br>
 
 Please create pytest.init in the project directory and not in the root directory
+
 ```
 [pytest]
 markers =
     test: custom mark for tests
 ```
```

### Comparing `contact-person-profile-csv-imp-local-0.0.6/pyproject.toml` & `contact_person_profile_csv_imp_local-0.0.7/pyproject.toml`

 * *Files identical despite different names*

