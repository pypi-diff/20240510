# Comparing `tmp/bigfunctions-0.1.tar.gz` & `tmp/bigfunctions-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigfunctions-0.1.tar", last modified: Wed Jan 24 17:11:21 2024, max compression
+gzip compressed data, was "bigfunctions-0.2.tar", last modified: Fri May 10 16:37:56 2024, max compression
```

## Comparing `bigfunctions-0.1.tar` & `bigfunctions-0.2.tar`

### file list

```diff
@@ -1,32 +1,45 @@
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-01-24 17:11:21.500810 bigfunctions-0.1/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2023-11-08 21:20:23.000000 bigfunctions-0.1/LICENSE
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9227 2024-01-24 17:11:21.499810 bigfunctions-0.1/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     8460 2024-01-19 20:34:23.000000 bigfunctions-0.1/README.md
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-01-24 17:11:21.468808 bigfunctions-0.1/bigfun/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2023-11-08 21:20:23.000000 bigfunctions-0.1/bigfun/__init__.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     5679 2024-01-19 20:34:23.000000 bigfunctions-0.1/bigfun/cli.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     5373 2024-01-19 20:34:23.000000 bigfunctions-0.1/bigfun/deploy.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     3733 2024-01-19 20:34:23.000000 bigfunctions-0.1/bigfun/generate_doc.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      844 2023-12-01 17:33:50.000000 bigfunctions-0.1/bigfun/load_table.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-01-24 17:11:21.495810 bigfunctions-0.1/bigfun/templates/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1086 2023-11-08 21:20:23.000000 bigfunctions-0.1/bigfun/templates/Dockerfile
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     8781 2023-12-01 16:35:59.000000 bigfunctions-0.1/bigfun/templates/bigfunctions.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     3784 2024-01-19 20:34:23.000000 bigfunctions-0.1/bigfun/templates/bookmarklet.js
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6358 2024-01-19 20:34:23.000000 bigfunctions-0.1/bigfun/templates/bookmarklet_doc.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4186 2023-12-01 16:35:59.000000 bigfunctions-0.1/bigfun/templates/data.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      458 2023-11-08 21:20:23.000000 bigfunctions-0.1/bigfun/templates/function_js.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7616 2024-01-19 20:34:23.000000 bigfunctions-0.1/bigfun/templates/function_py.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      298 2023-11-08 21:20:23.000000 bigfunctions-0.1/bigfun/templates/function_py.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      314 2023-11-08 21:20:23.000000 bigfunctions-0.1/bigfun/templates/function_sql.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      287 2023-11-08 21:20:23.000000 bigfunctions-0.1/bigfun/templates/procedure.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      249 2023-11-08 21:20:23.000000 bigfunctions-0.1/bigfun/templates/table_function.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    11711 2024-01-19 20:36:08.000000 bigfunctions-0.1/bigfun/utils.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-01-24 17:11:21.498810 bigfunctions-0.1/bigfunctions.egg-info/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9227 2024-01-24 17:11:21.000000 bigfunctions-0.1/bigfunctions.egg-info/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      707 2024-01-24 17:11:21.000000 bigfunctions-0.1/bigfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-01-24 17:11:21.000000 bigfunctions-0.1/bigfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       42 2024-01-24 17:11:21.000000 bigfunctions-0.1/bigfunctions.egg-info/entry_points.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      158 2024-01-24 17:11:21.000000 bigfunctions-0.1/bigfunctions.egg-info/requires.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        7 2024-01-24 17:11:21.000000 bigfunctions-0.1/bigfunctions.egg-info/top_level.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-01-24 17:11:21.500810 bigfunctions-0.1/setup.cfg
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1195 2024-01-24 17:08:59.000000 bigfunctions-0.1/setup.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.658268 bigfunctions-0.2/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2023-11-08 21:20:23.000000 bigfunctions-0.2/LICENSE
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-10 16:37:56.657268 bigfunctions-0.2/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9097 2024-02-22 22:16:20.000000 bigfunctions-0.2/README.md
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.645267 bigfunctions-0.2/bigfun/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2023-11-08 21:20:23.000000 bigfunctions-0.2/bigfun/__init__.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9876 2024-05-10 13:07:40.000000 bigfunctions-0.2/bigfun/bigfunctions.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7860 2024-05-10 13:28:21.000000 bigfunctions-0.2/bigfun/cli.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      844 2023-12-01 17:33:50.000000 bigfunctions-0.2/bigfun/load_table.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.649267 bigfunctions-0.2/bigfun/templates/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1086 2023-11-08 21:20:23.000000 bigfunctions-0.2/bigfun/templates/Dockerfile
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    11320 2024-05-10 12:31:51.000000 bigfunctions-0.2/bigfun/templates/bigfunction.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     3784 2024-01-19 20:34:23.000000 bigfunctions-0.2/bigfun/templates/bookmarklet.js
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1618 2024-05-10 09:49:39.000000 bigfunctions-0.2/bigfun/templates/categories.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1958 2024-03-01 20:43:46.000000 bigfunctions-0.2/bigfun/templates/categories.yaml
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4164 2024-01-24 23:20:01.000000 bigfunctions-0.2/bigfun/templates/data.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      554 2024-02-23 19:54:09.000000 bigfunctions-0.2/bigfun/templates/function_js.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7724 2024-02-23 21:48:51.000000 bigfunctions-0.2/bigfun/templates/function_py.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      316 2024-02-23 19:48:03.000000 bigfunctions-0.2/bigfun/templates/function_py.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      212 2024-02-23 21:42:39.000000 bigfunctions-0.2/bigfun/templates/function_py_test.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      410 2024-02-23 19:54:09.000000 bigfunctions-0.2/bigfun/templates/function_sql.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      251 2024-02-23 22:59:01.000000 bigfunctions-0.2/bigfun/templates/function_sql_test.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      702 2024-02-23 19:54:09.000000 bigfunctions-0.2/bigfun/templates/procedure.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      717 2024-02-23 22:23:06.000000 bigfunctions-0.2/bigfun/templates/procedure_test.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      345 2024-02-23 19:54:09.000000 bigfunctions-0.2/bigfun/templates/table_function.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    13249 2024-02-28 09:48:29.000000 bigfunctions-0.2/bigfun/utils.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.649267 bigfunctions-0.2/bigfun/website/
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.654268 bigfunctions-0.2/bigfun/website/assets/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1714 2023-11-29 13:48:58.000000 bigfunctions-0.2/bigfun/website/assets/GitHub-Mark-32px.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)  1353755 2024-01-19 20:34:23.000000 bigfunctions-0.2/bigfun/website/assets/bookmarklet_usage.gif
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    23806 2023-11-29 13:48:58.000000 bigfunctions-0.2/bigfun/website/assets/logo.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    73519 2023-11-29 13:48:58.000000 bigfunctions-0.2/bigfun/website/assets/logo_and_name.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    49771 2023-11-29 13:48:58.000000 bigfunctions-0.2/bigfun/website/assets/logo_and_name_wo_supercharge.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      888 2024-05-10 16:32:26.000000 bigfunctions-0.2/bigfun/website/mkdocs.yml
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.655268 bigfunctions-0.2/bigfun/website/theme_overrides/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6185 2024-05-10 12:11:21.000000 bigfunctions-0.2/bigfun/website/theme_overrides/main.html
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-10 16:37:56.657268 bigfunctions-0.2/bigfunctions.egg-info/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1109 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       42 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/entry_points.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      130 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/requires.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        7 2024-05-10 16:37:56.000000 bigfunctions-0.2/bigfunctions.egg-info/top_level.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-10 16:37:56.658268 bigfunctions-0.2/setup.cfg
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1329 2024-05-10 16:29:21.000000 bigfunctions-0.2/setup.py
```

### Comparing `bigfunctions-0.1/LICENSE` & `bigfunctions-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.1/PKG-INFO` & `bigfunctions-0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: bigfunctions
-Version: 0.1
+Version: 0.2
 Summary: Supercharge BigQuery with BigFunctions
-Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.1.tar.gz
+Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.2.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-bigquery_connection
 Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml
 Requires-Dist: jinja2
 Requires-Dist: mkdocs-material
-Requires-Dist: mkdocs-awesome-pages-plugin
 Requires-Dist: click
 Requires-Dist: click-help-colors
 
 
 <p align="center">
   <img class="hero-image" src="https://user-images.githubusercontent.com/111615732/186508787-6af04ed0-4750-4c49-926a-eacfd4a3dfbb.png" alt="logo_and_name" style="width: 100%; max-width: 600px">
 </p>
@@ -116,47 +115,59 @@
 
 ## 💥 5. `bigfun` CLI
 
 `bigfun` CLI (command-line-interface) facilitates BigFunctions development, test, deployment, documentation and monitoring.
 
 ### 5.1 Install `bigfun` 🛠️
 
-Clone the repo and from the repo directory run:
 
 ``` sh
-virtualenv venv
-. venv/bin/activate
-pip install --editable .
+pip install bigfunctions
 ```
 
 ### 5.2 Use `bigfun` 🔥
 
 ``` sh
 $ bigfun --help
 Usage: bigfun [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --help  Show this message and exit.
 
 Commands:
-  deploy  Deploy BIGFUNCTION
-  doc     Generate, serve and publish documentation
-  test    Test BIGFUNCTION
+  deploy      Deploy BIGFUNCTION
+  docs        Generate, serve and publish documentation
+  get         Download BIGFUNCTION yaml file from unytics/bigfunctions...
+  test        Test BIGFUNCTION
 ```
 
 
+### 5.3 Create you first function 👷
 
-### 5.3 Deploy you first function 👨‍💻
+Functions are defined as yaml files under `bigfunctions` folder. To create your first function locally, the easiest is to download an existing yaml file of unytics/bigfunctions Github repo. 
+
+For instance to download `is_email_valid.yaml` into bigfunctions folder, do:
+
+```sh
+bigfun get is_email_valid
+```
+
+You can then update the file to suit your needs.
+
+
+
+
+### 5.4 Deploy you first function 👨‍💻
 
 > 1. Make sure the `gcloud` command is [installed on your computer](https://cloud.google.com/sdk/docs/install)
 > 2. Activate the application-default account with `gcloud auth application-default login`. A browser window should open, and you should be prompted to log into your Google account. Once you've done that, `bigfun` will use your oauth'd credentials to connect to BigQuery through BigQuery python client!
 > 3. Get or create a `DATASET` where you have permission to edit data and where the function will be deployed.
 > 4. The `DATASET` must belong to a `PROJECT` in which you have permission to run BigQuery queries.
 
-You now can deploy `is_email_valid` function with:
+You now can deploy the function `is_email_valid` defined in `bigfunctions/is_email_valid.yaml` yaml file by running:
 
 ```sh
 bigfun deploy is_email_valid
 ```
 
 > The first time you run this command it will ask for `PROJECT` and `DATASET`.
 >
@@ -168,22 +179,22 @@
 ```sql
 select PROJECT.DATASET.is_email_valid('paul.marcombes@unytics.io')
 ```
 
 <br>
 
 
-### 5.4 Deploy you first javascript function which depends on *npm packages* 👽
+### 5.5 Deploy you first javascript function which depends on *npm packages* 👽
 
 *To deploy a **javascript** function* which depends on **npm packages** there are additional requirements *in addition to the ones above*.
 
 > 1. You will need to install each *npm package* on your machine and bundle it into one file. For that, you need to [install *nodejs*](https://nodejs.org/en/download/).
-> 2. The bundled js file will be uploaded into a cloud storage bucket in which you must have write access. The bucket name is asked when you run `bigfun deploy`. Users of your functions must have read access to the bucket.
+> 2. The bundled js file will be uploaded into a cloud storage bucket in which you must have write access. The bucket name must be provided in `config.yaml` file in a variable named `bucket_js_dependencies`. Users of your functions must have read access to the bucket.
 
-You now can deploy `render_template` function with:
+You now can deploy the function `render_template` defined in `bigfunctions/render_template.yaml` yaml file by running:
 
 ```sh
 bigfun deploy render_template
 ```
 
 Test it with 👀:
 
@@ -191,25 +202,25 @@
 select PROJECT.DATASET.render_template('Hello {{ user }}', json '{"user": "James"}')
 ```
 
 
 <br>
 
 
-### 5.5 Deploy you first *remote* function ⚡️
+### 5.6 Deploy you first *remote* function ⚡️
 
 *To deploy a **remote** function* (e.g. python function), there are additional requirements *in addition to the ones of **Deploy you first function** section*.
 
 > 1. A *Cloud Run* service will be deployed to host the code ([as seen here](https://cloud.google.com/bigquery/docs/reference/standard-sql/remote-functions)). So you must have [permissions to deploy a *Cloud Run* service](https://cloud.google.com/run/docs/deploying-source-code#permissions_required_to_deploy) in your project `PROJECT`.
 > 2. `gcloud` CLI will be used directly to deploy the service (using `gcloud run deploy`). Then, make sure you are logged in with `gcloud` by calling: `gcloud auth login`. A browser window should also open, and you should be prompted to log into your Google account. WARNING: you read correctly: you have to authenticate twice. Once for bigquery python client (to deploy any function including remote as seen above.) and once now to use `gcloud` (to deploy a *Cloud Run* service).
 > 3. A *BigQuery Remote Connection* will be created to link BigQuery with the *Cloud Run* service. You then should have permissions to create a remote connection. *[BigQuery Connection Admin](https://cloud.google.com/bigquery/docs/access-control#bigquery.connectionAdmin)* or *[BigQuery Admin](https://cloud.google.com/bigquery/docs/access-control#bigquery.admin)* roles have these permissions.
 > 4. A service account will be automatically created by Google along with the *BigQuery Remote Connection*. BigQuery will use this service account of the remote connection to invoke the *Cloud Run* service. You then must have the permission to authorize this service account to invoke the *Cloud Run* service. This permission is provided in the role *[roles/run.admin](https://cloud.google.com/run/docs/reference/iam/roles)*
 
 
-You now can deploy `faker` function with:
+You now can deploy the function `faker` defined in `bigfunctions/faker.yaml` yaml file by running:
 
 ```sh
 bigfun deploy faker
 ```
 
 Test it with 👀:
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: bigfunctions Version: 0.1 Summary: Supercharge
+Metadata-Version: 2.1 Name: bigfunctions Version: 0.2 Summary: Supercharge
 BigQuery with BigFunctions Download-URL: https://github.com/unytics/
-bigfunctions/archive/refs/tags/v0.1.tar.gz Author: Unytics Author-email:
+bigfunctions/archive/refs/tags/v0.2.tar.gz Author: Unytics Author-email:
 paul.marcombes@unytics.io Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
+:: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: google-cloud-bigquery Requires-
 Dist: google-cloud-bigquery_connection Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml Requires-Dist: jinja2 Requires-Dist: mkdocs-material
-Requires-Dist: mkdocs-awesome-pages-plugin Requires-Dist: click Requires-Dist:
-click-help-colors
+Requires-Dist: click Requires-Dist: click-help-colors
                                 [logo_and_name]
                              Supercharge BBiiggQQuueerryy
                                with BBiiggFFuunnccttiioonnss
 
                            UUppggrraaddee yyoouurr ddaattaa iimmppaacctt
                    with 100+ ready-to-use BigQuery Functions
                        (+ build a catalog of functions)
@@ -51,47 +50,55 @@
 **_h_e_r_e**.
 ## ð 4. Deploy BigFunctions in your GCP project You can also deploy any
 bigfunction in your project! To deploy *my_bigfunction* defined in
 *bigfunctions/my_bigfunction.yaml* file, simply call: ``` sh bigfun deploy
 my_bigfunction ``` Details about `bigfun` command line are given below.
 ## ð¥ 5. `bigfun` CLI `bigfun` CLI (command-line-interface) facilitates
 BigFunctions development, test, deployment, documentation and monitoring. ###
-5.1 Install `bigfun` ð ï¸ Clone the repo and from the repo directory run:
-``` sh virtualenv venv . venv/bin/activate pip install --editable . ``` ### 5.2
-Use `bigfun` ð¥ ``` sh $ bigfun --help Usage: bigfun [OPTIONS] COMMAND
-[ARGS]... Options: --help Show this message and exit. Commands: deploy Deploy
-BIGFUNCTION doc Generate, serve and publish documentation test Test BIGFUNCTION
-``` ### 5.3 Deploy you first function ð¨âð» > 1. Make sure the `gcloud`
-command is [installed on your computer](https://cloud.google.com/sdk/docs/
-install) > 2. Activate the application-default account with `gcloud auth
-application-default login`. A browser window should open, and you should be
-prompted to log into your Google account. Once you've done that, `bigfun` will
-use your oauth'd credentials to connect to BigQuery through BigQuery python
-client! > 3. Get or create a `DATASET` where you have permission to edit data
-and where the function will be deployed. > 4. The `DATASET` must belong to a
-`PROJECT` in which you have permission to run BigQuery queries. You now can
-deploy `is_email_valid` function with: ```sh bigfun deploy is_email_valid ``` >
-The first time you run this command it will ask for `PROJECT` and `DATASET`. >
-> Your inputs will be written to `config.yaml` file in current directory so
-that you won't be asked again (unless you delete the entries in `config.yaml`).
-You can also override this config at deploy time: `bigfun deploy is_email_valid
---project=PROJECT --dataset=DATASET`. Test it with ð: ```sql select
+5.1 Install `bigfun` ð ï¸ ``` sh pip install bigfunctions ``` ### 5.2 Use
+`bigfun` ð¥ ``` sh $ bigfun --help Usage: bigfun [OPTIONS] COMMAND [ARGS]...
+Options: --help Show this message and exit. Commands: deploy Deploy BIGFUNCTION
+docs Generate, serve and publish documentation get Download BIGFUNCTION yaml
+file from unytics/bigfunctions... test Test BIGFUNCTION ``` ### 5.3 Create you
+first function ð· Functions are defined as yaml files under `bigfunctions`
+folder. To create your first function locally, the easiest is to download an
+existing yaml file of unytics/bigfunctions Github repo. For instance to
+download `is_email_valid.yaml` into bigfunctions folder, do: ```sh bigfun get
+is_email_valid ``` You can then update the file to suit your needs. ### 5.4
+Deploy you first function ð¨âð» > 1. Make sure the `gcloud` command is
+[installed on your computer](https://cloud.google.com/sdk/docs/install) > 2.
+Activate the application-default account with `gcloud auth application-default
+login`. A browser window should open, and you should be prompted to log into
+your Google account. Once you've done that, `bigfun` will use your oauth'd
+credentials to connect to BigQuery through BigQuery python client! > 3. Get or
+create a `DATASET` where you have permission to edit data and where the
+function will be deployed. > 4. The `DATASET` must belong to a `PROJECT` in
+which you have permission to run BigQuery queries. You now can deploy the
+function `is_email_valid` defined in `bigfunctions/is_email_valid.yaml` yaml
+file by running: ```sh bigfun deploy is_email_valid ``` > The first time you
+run this command it will ask for `PROJECT` and `DATASET`. > > Your inputs will
+be written to `config.yaml` file in current directory so that you won't be
+asked again (unless you delete the entries in `config.yaml`). You can also
+override this config at deploy time: `bigfun deploy is_email_valid --
+project=PROJECT --dataset=DATASET`. Test it with ð: ```sql select
 PROJECT.DATASET.is_email_valid('paul.marcombes@unytics.io') ```
-### 5.4 Deploy you first javascript function which depends on *npm packages*
+### 5.5 Deploy you first javascript function which depends on *npm packages*
 ð½ *To deploy a **javascript** function* which depends on **npm packages**
 there are additional requirements *in addition to the ones above*. > 1. You
 will need to install each *npm package* on your machine and bundle it into one
 file. For that, you need to [install *nodejs*](https://nodejs.org/en/download/
 ). > 2. The bundled js file will be uploaded into a cloud storage bucket in
-which you must have write access. The bucket name is asked when you run `bigfun
-deploy`. Users of your functions must have read access to the bucket. You now
-can deploy `render_template` function with: ```sh bigfun deploy render_template
-``` Test it with ð: ```sql select PROJECT.DATASET.render_template('Hello {
-{ user }}', json '{"user": "James"}') ```
-### 5.5 Deploy you first *remote* function â¡ï¸ *To deploy a **remote**
+which you must have write access. The bucket name must be provided in
+`config.yaml` file in a variable named `bucket_js_dependencies`. Users of your
+functions must have read access to the bucket. You now can deploy the function
+`render_template` defined in `bigfunctions/render_template.yaml` yaml file by
+running: ```sh bigfun deploy render_template ``` Test it with ð: ```sql
+select PROJECT.DATASET.render_template('Hello {{ user }}', json '{"user":
+"James"}') ```
+### 5.6 Deploy you first *remote* function â¡ï¸ *To deploy a **remote**
 function* (e.g. python function), there are additional requirements *in
 addition to the ones of **Deploy you first function** section*. > 1. A *Cloud
 Run* service will be deployed to host the code ([as seen here](https://
 cloud.google.com/bigquery/docs/reference/standard-sql/remote-functions)). So
 you must have [permissions to deploy a *Cloud Run* service](https://
 cloud.google.com/run/docs/deploying-source-code#permissions_required_to_deploy)
 in your project `PROJECT`. > 2. `gcloud` CLI will be used directly to deploy
@@ -107,16 +114,17 @@
 control#bigquery.connectionAdmin)* or *[BigQuery Admin](https://
 cloud.google.com/bigquery/docs/access-control#bigquery.admin)* roles have these
 permissions. > 4. A service account will be automatically created by Google
 along with the *BigQuery Remote Connection*. BigQuery will use this service
 account of the remote connection to invoke the *Cloud Run* service. You then
 must have the permission to authorize this service account to invoke the *Cloud
 Run* service. This permission is provided in the role *[roles/run.admin](https:
-//cloud.google.com/run/docs/reference/iam/roles)* You now can deploy `faker`
-function with: ```sh bigfun deploy faker ``` Test it with ð: ```sql select
+//cloud.google.com/run/docs/reference/iam/roles)* You now can deploy the
+function `faker` defined in `bigfunctions/faker.yaml` yaml file by running:
+```sh bigfun deploy faker ``` Test it with ð: ```sql select
 PROJECT.DATASET.faker("name", "it_IT") ```
 ## ð 6. Contribute BigFunctions is fully open-source. Any contribution is
 more than welcome ð¤! - Add a â­ on the repo to show your support - [Join
 our Slack](https://join.slack.com/t/unytics/shared_invite/zt-1gbv491mu-
 cs03EJbQ1fsHdQMcFN7E1Q) and talk with us - Suggest a new function [here](https:
 //github.com/unytics/bigfunctions/issues/new?assignees=&labels=new-
 bigfunction&projects=&template=0_new_bigfunction.yaml&title=%5Bnew%5D%3A+%60function_name%28argument1%2C+argument2%29%60)
```

### Comparing `bigfunctions-0.1/README.md` & `bigfunctions-0.2/bigfunctions.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: bigfunctions
+Version: 0.2
+Summary: Supercharge BigQuery with BigFunctions
+Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.2.tar.gz
+Author: Unytics
+Author-email: paul.marcombes@unytics.io
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: google-cloud-bigquery
+Requires-Dist: google-cloud-bigquery_connection
+Requires-Dist: google-cloud-storage
+Requires-Dist: pyyaml
+Requires-Dist: jinja2
+Requires-Dist: mkdocs-material
+Requires-Dist: click
+Requires-Dist: click-help-colors
+
 
 <p align="center">
   <img class="hero-image" src="https://user-images.githubusercontent.com/111615732/186508787-6af04ed0-4750-4c49-926a-eacfd4a3dfbb.png" alt="logo_and_name" style="width: 100%; max-width: 600px">
 </p>
 
 <p align="center">
     Supercharge <em>BigQuery</em><br>with <em>BigFunctions</em><br><br>
@@ -93,47 +115,59 @@
 
 ## 💥 5. `bigfun` CLI
 
 `bigfun` CLI (command-line-interface) facilitates BigFunctions development, test, deployment, documentation and monitoring.
 
 ### 5.1 Install `bigfun` 🛠️
 
-Clone the repo and from the repo directory run:
 
 ``` sh
-virtualenv venv
-. venv/bin/activate
-pip install --editable .
+pip install bigfunctions
 ```
 
 ### 5.2 Use `bigfun` 🔥
 
 ``` sh
 $ bigfun --help
 Usage: bigfun [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --help  Show this message and exit.
 
 Commands:
-  deploy  Deploy BIGFUNCTION
-  doc     Generate, serve and publish documentation
-  test    Test BIGFUNCTION
+  deploy      Deploy BIGFUNCTION
+  docs        Generate, serve and publish documentation
+  get         Download BIGFUNCTION yaml file from unytics/bigfunctions...
+  test        Test BIGFUNCTION
+```
+
+
+### 5.3 Create you first function 👷
+
+Functions are defined as yaml files under `bigfunctions` folder. To create your first function locally, the easiest is to download an existing yaml file of unytics/bigfunctions Github repo. 
+
+For instance to download `is_email_valid.yaml` into bigfunctions folder, do:
+
+```sh
+bigfun get is_email_valid
 ```
 
+You can then update the file to suit your needs.
+
+
 
 
-### 5.3 Deploy you first function 👨‍💻
+### 5.4 Deploy you first function 👨‍💻
 
 > 1. Make sure the `gcloud` command is [installed on your computer](https://cloud.google.com/sdk/docs/install)
 > 2. Activate the application-default account with `gcloud auth application-default login`. A browser window should open, and you should be prompted to log into your Google account. Once you've done that, `bigfun` will use your oauth'd credentials to connect to BigQuery through BigQuery python client!
 > 3. Get or create a `DATASET` where you have permission to edit data and where the function will be deployed.
 > 4. The `DATASET` must belong to a `PROJECT` in which you have permission to run BigQuery queries.
 
-You now can deploy `is_email_valid` function with:
+You now can deploy the function `is_email_valid` defined in `bigfunctions/is_email_valid.yaml` yaml file by running:
 
 ```sh
 bigfun deploy is_email_valid
 ```
 
 > The first time you run this command it will ask for `PROJECT` and `DATASET`.
 >
@@ -145,22 +179,22 @@
 ```sql
 select PROJECT.DATASET.is_email_valid('paul.marcombes@unytics.io')
 ```
 
 <br>
 
 
-### 5.4 Deploy you first javascript function which depends on *npm packages* 👽
+### 5.5 Deploy you first javascript function which depends on *npm packages* 👽
 
 *To deploy a **javascript** function* which depends on **npm packages** there are additional requirements *in addition to the ones above*.
 
 > 1. You will need to install each *npm package* on your machine and bundle it into one file. For that, you need to [install *nodejs*](https://nodejs.org/en/download/).
-> 2. The bundled js file will be uploaded into a cloud storage bucket in which you must have write access. The bucket name is asked when you run `bigfun deploy`. Users of your functions must have read access to the bucket.
+> 2. The bundled js file will be uploaded into a cloud storage bucket in which you must have write access. The bucket name must be provided in `config.yaml` file in a variable named `bucket_js_dependencies`. Users of your functions must have read access to the bucket.
 
-You now can deploy `render_template` function with:
+You now can deploy the function `render_template` defined in `bigfunctions/render_template.yaml` yaml file by running:
 
 ```sh
 bigfun deploy render_template
 ```
 
 Test it with 👀:
 
@@ -168,25 +202,25 @@
 select PROJECT.DATASET.render_template('Hello {{ user }}', json '{"user": "James"}')
 ```
 
 
 <br>
 
 
-### 5.5 Deploy you first *remote* function ⚡️
+### 5.6 Deploy you first *remote* function ⚡️
 
 *To deploy a **remote** function* (e.g. python function), there are additional requirements *in addition to the ones of **Deploy you first function** section*.
 
 > 1. A *Cloud Run* service will be deployed to host the code ([as seen here](https://cloud.google.com/bigquery/docs/reference/standard-sql/remote-functions)). So you must have [permissions to deploy a *Cloud Run* service](https://cloud.google.com/run/docs/deploying-source-code#permissions_required_to_deploy) in your project `PROJECT`.
 > 2. `gcloud` CLI will be used directly to deploy the service (using `gcloud run deploy`). Then, make sure you are logged in with `gcloud` by calling: `gcloud auth login`. A browser window should also open, and you should be prompted to log into your Google account. WARNING: you read correctly: you have to authenticate twice. Once for bigquery python client (to deploy any function including remote as seen above.) and once now to use `gcloud` (to deploy a *Cloud Run* service).
 > 3. A *BigQuery Remote Connection* will be created to link BigQuery with the *Cloud Run* service. You then should have permissions to create a remote connection. *[BigQuery Connection Admin](https://cloud.google.com/bigquery/docs/access-control#bigquery.connectionAdmin)* or *[BigQuery Admin](https://cloud.google.com/bigquery/docs/access-control#bigquery.admin)* roles have these permissions.
 > 4. A service account will be automatically created by Google along with the *BigQuery Remote Connection*. BigQuery will use this service account of the remote connection to invoke the *Cloud Run* service. You then must have the permission to authorize this service account to invoke the *Cloud Run* service. This permission is provided in the role *[roles/run.admin](https://cloud.google.com/run/docs/reference/iam/roles)*
 
 
-You now can deploy `faker` function with:
+You now can deploy the function `faker` defined in `bigfunctions/faker.yaml` yaml file by running:
 
 ```sh
 bigfun deploy faker
 ```
 
 Test it with 👀:
```

#### html2text {}

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1 Name: bigfunctions Version: 0.2 Summary: Supercharge
+BigQuery with BigFunctions Download-URL: https://github.com/unytics/
+bigfunctions/archive/refs/tags/v0.2.tar.gz Author: Unytics Author-email:
+paul.marcombes@unytics.io Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: google-cloud-bigquery Requires-
+Dist: google-cloud-bigquery_connection Requires-Dist: google-cloud-storage
+Requires-Dist: pyyaml Requires-Dist: jinja2 Requires-Dist: mkdocs-material
+Requires-Dist: click Requires-Dist: click-help-colors
                                 [logo_and_name]
                              Supercharge BBiiggQQuueerryy
                                with BBiiggFFuunnccttiioonnss
 
                            UUppggrraaddee yyoouurr ddaattaa iimmppaacctt
                    with 100+ ready-to-use BigQuery Functions
                        (+ build a catalog of functions)
@@ -40,47 +50,55 @@
 **_h_e_r_e**.
 ## ð 4. Deploy BigFunctions in your GCP project You can also deploy any
 bigfunction in your project! To deploy *my_bigfunction* defined in
 *bigfunctions/my_bigfunction.yaml* file, simply call: ``` sh bigfun deploy
 my_bigfunction ``` Details about `bigfun` command line are given below.
 ## ð¥ 5. `bigfun` CLI `bigfun` CLI (command-line-interface) facilitates
 BigFunctions development, test, deployment, documentation and monitoring. ###
-5.1 Install `bigfun` ð ï¸ Clone the repo and from the repo directory run:
-``` sh virtualenv venv . venv/bin/activate pip install --editable . ``` ### 5.2
-Use `bigfun` ð¥ ``` sh $ bigfun --help Usage: bigfun [OPTIONS] COMMAND
-[ARGS]... Options: --help Show this message and exit. Commands: deploy Deploy
-BIGFUNCTION doc Generate, serve and publish documentation test Test BIGFUNCTION
-``` ### 5.3 Deploy you first function ð¨âð» > 1. Make sure the `gcloud`
-command is [installed on your computer](https://cloud.google.com/sdk/docs/
-install) > 2. Activate the application-default account with `gcloud auth
-application-default login`. A browser window should open, and you should be
-prompted to log into your Google account. Once you've done that, `bigfun` will
-use your oauth'd credentials to connect to BigQuery through BigQuery python
-client! > 3. Get or create a `DATASET` where you have permission to edit data
-and where the function will be deployed. > 4. The `DATASET` must belong to a
-`PROJECT` in which you have permission to run BigQuery queries. You now can
-deploy `is_email_valid` function with: ```sh bigfun deploy is_email_valid ``` >
-The first time you run this command it will ask for `PROJECT` and `DATASET`. >
-> Your inputs will be written to `config.yaml` file in current directory so
-that you won't be asked again (unless you delete the entries in `config.yaml`).
-You can also override this config at deploy time: `bigfun deploy is_email_valid
---project=PROJECT --dataset=DATASET`. Test it with ð: ```sql select
+5.1 Install `bigfun` ð ï¸ ``` sh pip install bigfunctions ``` ### 5.2 Use
+`bigfun` ð¥ ``` sh $ bigfun --help Usage: bigfun [OPTIONS] COMMAND [ARGS]...
+Options: --help Show this message and exit. Commands: deploy Deploy BIGFUNCTION
+docs Generate, serve and publish documentation get Download BIGFUNCTION yaml
+file from unytics/bigfunctions... test Test BIGFUNCTION ``` ### 5.3 Create you
+first function ð· Functions are defined as yaml files under `bigfunctions`
+folder. To create your first function locally, the easiest is to download an
+existing yaml file of unytics/bigfunctions Github repo. For instance to
+download `is_email_valid.yaml` into bigfunctions folder, do: ```sh bigfun get
+is_email_valid ``` You can then update the file to suit your needs. ### 5.4
+Deploy you first function ð¨âð» > 1. Make sure the `gcloud` command is
+[installed on your computer](https://cloud.google.com/sdk/docs/install) > 2.
+Activate the application-default account with `gcloud auth application-default
+login`. A browser window should open, and you should be prompted to log into
+your Google account. Once you've done that, `bigfun` will use your oauth'd
+credentials to connect to BigQuery through BigQuery python client! > 3. Get or
+create a `DATASET` where you have permission to edit data and where the
+function will be deployed. > 4. The `DATASET` must belong to a `PROJECT` in
+which you have permission to run BigQuery queries. You now can deploy the
+function `is_email_valid` defined in `bigfunctions/is_email_valid.yaml` yaml
+file by running: ```sh bigfun deploy is_email_valid ``` > The first time you
+run this command it will ask for `PROJECT` and `DATASET`. > > Your inputs will
+be written to `config.yaml` file in current directory so that you won't be
+asked again (unless you delete the entries in `config.yaml`). You can also
+override this config at deploy time: `bigfun deploy is_email_valid --
+project=PROJECT --dataset=DATASET`. Test it with ð: ```sql select
 PROJECT.DATASET.is_email_valid('paul.marcombes@unytics.io') ```
-### 5.4 Deploy you first javascript function which depends on *npm packages*
+### 5.5 Deploy you first javascript function which depends on *npm packages*
 ð½ *To deploy a **javascript** function* which depends on **npm packages**
 there are additional requirements *in addition to the ones above*. > 1. You
 will need to install each *npm package* on your machine and bundle it into one
 file. For that, you need to [install *nodejs*](https://nodejs.org/en/download/
 ). > 2. The bundled js file will be uploaded into a cloud storage bucket in
-which you must have write access. The bucket name is asked when you run `bigfun
-deploy`. Users of your functions must have read access to the bucket. You now
-can deploy `render_template` function with: ```sh bigfun deploy render_template
-``` Test it with ð: ```sql select PROJECT.DATASET.render_template('Hello {
-{ user }}', json '{"user": "James"}') ```
-### 5.5 Deploy you first *remote* function â¡ï¸ *To deploy a **remote**
+which you must have write access. The bucket name must be provided in
+`config.yaml` file in a variable named `bucket_js_dependencies`. Users of your
+functions must have read access to the bucket. You now can deploy the function
+`render_template` defined in `bigfunctions/render_template.yaml` yaml file by
+running: ```sh bigfun deploy render_template ``` Test it with ð: ```sql
+select PROJECT.DATASET.render_template('Hello {{ user }}', json '{"user":
+"James"}') ```
+### 5.6 Deploy you first *remote* function â¡ï¸ *To deploy a **remote**
 function* (e.g. python function), there are additional requirements *in
 addition to the ones of **Deploy you first function** section*. > 1. A *Cloud
 Run* service will be deployed to host the code ([as seen here](https://
 cloud.google.com/bigquery/docs/reference/standard-sql/remote-functions)). So
 you must have [permissions to deploy a *Cloud Run* service](https://
 cloud.google.com/run/docs/deploying-source-code#permissions_required_to_deploy)
 in your project `PROJECT`. > 2. `gcloud` CLI will be used directly to deploy
@@ -96,16 +114,17 @@
 control#bigquery.connectionAdmin)* or *[BigQuery Admin](https://
 cloud.google.com/bigquery/docs/access-control#bigquery.admin)* roles have these
 permissions. > 4. A service account will be automatically created by Google
 along with the *BigQuery Remote Connection*. BigQuery will use this service
 account of the remote connection to invoke the *Cloud Run* service. You then
 must have the permission to authorize this service account to invoke the *Cloud
 Run* service. This permission is provided in the role *[roles/run.admin](https:
-//cloud.google.com/run/docs/reference/iam/roles)* You now can deploy `faker`
-function with: ```sh bigfun deploy faker ``` Test it with ð: ```sql select
+//cloud.google.com/run/docs/reference/iam/roles)* You now can deploy the
+function `faker` defined in `bigfunctions/faker.yaml` yaml file by running:
+```sh bigfun deploy faker ``` Test it with ð: ```sql select
 PROJECT.DATASET.faker("name", "it_IT") ```
 ## ð 6. Contribute BigFunctions is fully open-source. Any contribution is
 more than welcome ð¤! - Add a â­ on the repo to show your support - [Join
 our Slack](https://join.slack.com/t/unytics/shared_invite/zt-1gbv491mu-
 cs03EJbQ1fsHdQMcFN7E1Q) and talk with us - Suggest a new function [here](https:
 //github.com/unytics/bigfunctions/issues/new?assignees=&labels=new-
 bigfunction&projects=&template=0_new_bigfunction.yaml&title=%5Bnew%5D%3A+%60function_name%28argument1%2C+argument2%29%60)
```

### Comparing `bigfunctions-0.1/bigfun/cli.py` & `bigfunctions-0.2/bigfun/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,142 @@
 import os
+import shutil
 import multiprocessing
 
 import yaml
 import click
 from click_help_colors import HelpColorsGroup
 from watchdog.observers import Observer
 from watchdog.events import RegexMatchingEventHandler
 
+from . import bigfunctions as bf
+from . import utils
 
 
 
-BIGFUNCTIONS_FOLDER = 'bigfunctions'
 TABLES_FOLDER = 'data'
+THIS_FOLDER = os.path.dirname(os.path.realpath(__file__)).replace('\\', '/')
+WEBSITE_CONFIG_FOLDER = THIS_FOLDER + '/website'
 CONFIG_FILENAME = 'config.yaml'
 CONFIG = {}
 if os.path.exists(CONFIG_FILENAME):
     CONFIG = yaml.safe_load(open(CONFIG_FILENAME, encoding='utf-8').read()) or {}
 
 
 def get_config_value(name):
     if name in CONFIG:
         return CONFIG[name]
 
     text, default = {
         'project':                   ("Default GCP project where to deploy bigfunctions", None),
-        'dataset':                   ("Default dataset where to deploy bigfunctions", "bigfunctions"),  # eu,us,asia_east1,asia_east2,asia_northeast1,asia_northeast2,asia_northeast3,asia_south1,asia_southeast1,australia_southeast1,europe_north1,europe_west1,europe_west2,europe_west3,europe_west4,europe_west6,northamerica_northeast1,southamerica_east1,us_central1,us_east1,us_east4,us_west1,us_west2
-        'bucket_js_dependencies':    ("Default bucket where to upload npm packages used by js functions", f"{CONFIG['project']}_bigfunctions_js_dependencies" if 'project' in CONFIG else None),
-        'quota_management_backend': ("Backend used for quota management (none or datastore)(if you choose datastore, additionnal intallation steps are required)(if you choose none: only `max_rows_per_query` quota will be checked)", 'none'),
-        'quota_contact': ("Contact which appears when user receives a Quota Error", 'paul.marcombes@unytics.io'),
+        'dataset':                   ("Default dataset where to deploy bigfunctions", None),  # eu,us,asia_east1,asia_east2,asia_northeast1,asia_northeast2,asia_northeast3,asia_south1,asia_southeast1,australia_southeast1,europe_north1,europe_west1,europe_west2,europe_west3,europe_west4,europe_west6,northamerica_northeast1,southamerica_east1,us_central1,us_east1,us_east4,us_west1,us_west2
+        'project_for_tests':         ("Default GCP project where to deploy bigfunctions for TESTING purposes", None),
+        'dataset_for_tests':         ("Default dataset where to deploy bigfunctions for TESTING purposes", None),  # eu,us,asia_east1,asia_east2,asia_northeast1,asia_northeast2,asia_northeast3,asia_south1,asia_southeast1,australia_southeast1,europe_north1,europe_west1,europe_west2,europe_west3,europe_west4,europe_west6,northamerica_northeast1,southamerica_east1,us_central1,us_east1,us_east4,us_west1,us_west2
     }[name]
     CONFIG[name] = click.prompt(text, default=default)
     with open(CONFIG_FILENAME, 'w', encoding='utf-8') as outfile:
         yaml.dump(CONFIG, outfile, default_flow_style=False)
     return CONFIG[name]
 
 
+def generate_doc(project, dataset):
+    os.makedirs('docs', exist_ok=True)
+
+    if not os.path.isfile('README.md'):
+        print('INFO: CREATING A README.md FILE IN CURRENT DIRECTORY WHICH WILL BE THE ROOT CONTENT OF THE WEBSITE')
+        open('README.md', 'w', encoding='utf-8').write('# Hello from README!')
+
+    if not os.path.isfile('mkdocs.yml'):
+        print('INFO: CREATING mkdocs.yml FILE in CURRENT DIRECTORY. It is the configuration file of the website...')
+        shutil.copyfile(WEBSITE_CONFIG_FOLDER + '/mkdocs.yml', 'mkdocs.yml')
+
+    if not os.path.isdir('docs/assets'):
+        print('INFO: COPYING assets FOLDER into docs FOLDER...')
+        shutil.copytree(WEBSITE_CONFIG_FOLDER + '/assets', 'docs/assets')
+
+    if not os.path.isdir('docs/theme_overrides'):
+        print('INFO: COPYING theme_overrides FOLDER into docs FOLDER...')
+        shutil.copytree(WEBSITE_CONFIG_FOLDER + '/theme_overrides', 'docs/theme_overrides')
+
+    shutil.copyfile('README.md', 'docs/README.md')
+    if os.path.isfile('CONTRIBUTING.md'):
+        shutil.copyfile('CONTRIBUTING.md', 'docs/CONTRIBUTING.md')
+
+    bf.generate_doc(project, dataset)
+
+    for image in [f for f in os.listdir('bigfunctions') if f.endswith('.png')]:
+        shutil.copy(f'bigfunctions/{image}', f'docs/bigfunctions/{image}')
+
+
 @click.group(
     cls=HelpColorsGroup,
     help_headers_color='yellow',
     help_options_color='cyan'
 )
 def cli():
     pass
 
 
 @cli.command()
 @click.argument('bigfunction')
+def get(bigfunction):
+    '''
+    Download BIGFUNCTION yaml file from unytics/bigfunctions github repo
+    '''
+    if not os.path.isdir('bigfunctions'):
+        os.makedirs('bigfunctions')
+    url = f'https://raw.githubusercontent.com/unytics/bigfunctions/main/bigfunctions/{bigfunction}.yaml'
+    utils.download(url, f'bigfunctions/{bigfunction}.yaml')
+
+
+
+
+@cli.command()
+@click.argument('bigfunction')
+def test(bigfunction):
+    '''
+    Test BIGFUNCTION
+    '''
+    project = get_config_value('project_for_tests')
+    dataset = get_config_value('dataset_for_tests')
+    bigfunction = bf.BigFunction(bigfunction, project=project, dataset=dataset)
+    bigfunction.test()
+
+
+@cli.command()
+@click.argument('bigfunction')
 @click.option('--project', help='Google Cloud project where the function will be deployed')
 @click.option('--dataset', help='BigQuery dataset name where the function will be deployed')
 def deploy(bigfunction, project, dataset):
     '''
     Deploy BIGFUNCTION
 
     Deploy the function defined in `bigfunctions/{BIGFUNCTION}.yaml` file. If BIGFUNCTION = 'ALL' then all bigfunctions contained in bigfunctions folder are deployed.
     '''
-    from .deploy import deploy as deploy_bigfunction
     project = project or get_config_value('project')
     dataset = dataset or get_config_value('dataset')
     datasets = [dataset.strip() for dataset in dataset.split(',')]
     bigfunctions = [bigfunction.strip() for bigfunction in bigfunction.split(',')]
     if bigfunction == 'ALL':
-        bigfunctions = [f.replace('.yaml', '') for f in os.listdir(BIGFUNCTIONS_FOLDER)]
+        bigfunctions = bf.list_bigfunctions()
 
-    bucket = get_config_value('bucket_js_dependencies')
-    cloud_run_options = CONFIG.get('cloud_run', {})
-
-    quotas = {
-        'backend': get_config_value('quota_management_backend'),
-        'contact': get_config_value('quota_contact'),
-    }
-
-    for bigfunction in bigfunctions:
-        assert bigfunction in bigfunctions, f'Could not find "{bigfunction}" in "{BIGFUNCTIONS_FOLDER}" folder'
-        dataset = datasets[0]
-        deploy_bigfunction(bigfunction, project, dataset, quotas, bucket, cloud_run_options)
+    for name in bigfunctions:
+        bigfunction = bf.BigFunction(name, project=project, dataset=datasets[0])
+        bigfunction.deploy()
         if len(datasets) > 1:
             with multiprocessing.Pool(processes=8) as pool:
-                pool.starmap(
-                    deploy_bigfunction,
-                    [[bigfunction, project, dataset, quotas, bucket, cloud_run_options] for dataset in datasets[1:]]
+                pool.map(
+                    BigFunction.deploy,
+                    [
+                        bf.BigFunction(name, project=project, dataset=dataset)
+                        for dataset in datasets[1:]
+                    ]
                 )
 
 
-@cli.command()
-@click.argument('bigfunction')
-def test(bigfunction):
-    '''
-    Test BIGFUNCTION
-    '''
-    # [TODO] make some tests
-
 
 @cli.command()
 @click.argument('table')
 @click.option('--project', help='Google Cloud project where the table is created')
 @click.option('--dataset', help='BigQuery dataset name where the table is created')
 def load_table(table, project, dataset):
     '''
@@ -119,32 +162,43 @@
 @cli.group()
 def docs():
     '''
     Generate, serve and publish documentation
     '''
     pass
 
+
 @docs.command()
-def generate():
+@click.option('--project', help='Google Cloud project where the table is created')
+@click.option('--dataset', help='BigQuery dataset name where the table is created')
+def generate(project, dataset):
     '''
     Generate markdown files for documentation from yaml bigfunctions files
     '''
-    from .generate_doc import generate_doc
-    generate_doc()
+    project = project or get_config_value('project')
+    dataset = dataset or get_config_value('dataset')
+    generate_doc(project, dataset)
+    os.system('mkdocs build')
+
 
 
 @docs.command()
-def serve():
+@click.option('--project', help='Google Cloud project where the table is created')
+@click.option('--dataset', help='BigQuery dataset name where the table is created')
+def serve(project, dataset):
     '''
     Serve docs locally on http://localhost:8000
     '''
-    from .generate_doc import generate_doc
+    project = project or get_config_value('project')
+    dataset = dataset or get_config_value('dataset')
+    generate_doc(project, dataset)
+
     class EventHandler(RegexMatchingEventHandler):
         def on_any_event(self, event):
             print(f'File {event.src_path} {event.event_type} --> generating README files...')
-            generate_doc()
-    event_handler = EventHandler(regexes=[r'.*\.yaml'])
-    observer = Observer()
-    observer.schedule(event_handler, BIGFUNCTIONS_FOLDER, recursive=True)
-    observer.start()
-    generate_doc()
-    os.system('mkdocs serve --config-file site/mkdocs.yml')
+            generate_doc(project, dataset)
+    # event_handler = EventHandler(regexes=[r'.*\.yaml'])
+    # observer = Observer()
+    # observer.schedule(event_handler, BIGFUNCTIONS_FOLDER, recursive=True)
+    # observer.start()
+    # bf.generate_doc(project, dataset)
+    os.system('mkdocs serve')
```

### Comparing `bigfunctions-0.1/bigfun/load_table.py` & `bigfunctions-0.2/bigfun/load_table.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.1/bigfun/templates/Dockerfile` & `bigfunctions-0.2/bigfun/templates/Dockerfile`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.1/bigfun/templates/bookmarklet.js` & `bigfunctions-0.2/bigfun/templates/bookmarklet.js`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.1/bigfun/templates/data.md` & `bigfunctions-0.2/bigfun/templates/data.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 !!! note ""
 
     **✅ The following public tables** are
 
     - deployed in `bigfunctions` GCP project in 39 datasets for all of the 39 BigQuery regions.
     - They are public, so they can be read by anyone under the eventual license given in the description of the table.
-    - For any question or difficulties, please read [Getting Started](/bigfunctions/).
-    - If you prefer to create the tables in your own project, read [Getting Started](/bigfunctions/).
+    - For any question or difficulties, please read [Getting Started](../).
+    - If you prefer to create the tables in your own project, read [Getting Started](../).
     - Found a bug? Please raise an issue [here](https://github.com/unytics/bigfunctions/issues/new/choose)
 
 ??? info "All BigFunctions Datasets >"
 
     | Region | Dataset |
     |--------|---------|
     | `EU` | `bigfunctions.eu` |
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 --- title: "Tables" description: "Catalog of open-source Tables" --- !!! note
 "" **â The following public tables** are - deployed in `bigfunctions` GCP
 project in 39 datasets for all of the 39 BigQuery regions. - They are public,
 so they can be read by anyone under the eventual license given in the
 description of the table. - For any question or difficulties, please read
-[Getting Started](/bigfunctions/). - If you prefer to create the tables in your
-own project, read [Getting Started](/bigfunctions/). - Found a bug? Please
-raise an issue [here](https://github.com/unytics/bigfunctions/issues/new/
-choose) ??? info "All BigFunctions Datasets >" | Region | Dataset | |--------|-
---------| | `EU` | `bigfunctions.eu` | | `US` | `bigfunctions.us` | | `asia-
-east1` | `bigfunctions.asia_east1` | | `asia-east2` | `bigfunctions.asia_east2`
-| | `asia-northeast1` | `bigfunctions.asia_northeast1` | | `asia-northeast2` |
+[Getting Started](../). - If you prefer to create the tables in your own
+project, read [Getting Started](../). - Found a bug? Please raise an issue
+[here](https://github.com/unytics/bigfunctions/issues/new/choose) ??? info "All
+BigFunctions Datasets >" | Region | Dataset | |--------|---------| | `EU` |
+`bigfunctions.eu` | | `US` | `bigfunctions.us` | | `asia-east1` |
+`bigfunctions.asia_east1` | | `asia-east2` | `bigfunctions.asia_east2` | |
+`asia-northeast1` | `bigfunctions.asia_northeast1` | | `asia-northeast2` |
 `bigfunctions.asia_northeast2` | | `asia-northeast3` |
 `bigfunctions.asia_northeast3` | | `asia-south1` | `bigfunctions.asia_south1` |
 | `asia-south2` | `bigfunctions.asia_south2` | | `asia-southeast1` |
 `bigfunctions.asia_southeast1` | | `asia-southeast2` |
 `bigfunctions.asia_southeast2` | | `australia-southeast1` |
 `bigfunctions.australia_southeast1` | | `australia-southeast2` |
 `bigfunctions.australia_southeast2` | | `europe-central2` |
```

### Comparing `bigfunctions-0.1/bigfun/templates/function_py.py` & `bigfunctions-0.2/bigfun/templates/function_py.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 error_reporter = google.cloud.error_reporting.Client()
 app = Flask(__name__)
 
 
 CACHE = {}
+CURRENT_LOCATION = '{{ cloud_run_location }}'
 
 QUOTAS = {{ quotas }}
 
 
 _, PROJECT = google.auth.default()
 
 
@@ -32,27 +33,24 @@
 
 
 class QuotaException(Exception):
     pass
 
 
 
-class SimpleQuotaManager:
+class Logger:
 
     def __init__(self, data):
-        self.created_at = datetime.datetime.utcnow()
         self.created_time = time.time()
         self.user = data['sessionUser']
         self.row_count = len(data['calls'])
         self.request_id = data['requestId']
         self.caller = data['caller']
-        self.date = self.created_at.strftime("%Y-%m-%d")
-        self.user_bigfunction_date = f'{self.user}/{{ name }}/{self.date}'
 
-    def save_log(self, **kwargs):
+    def log(self, **kwargs):
         duration = 1000 * (time.time() - self.created_time)
         status = kwargs['status']
         message = {
             **{
                 "severity": 'INFO',
                 'message': f"{status.upper()}: {{ name }} from {self.user} with {self.row_count} rows (elasped {duration} ms)",
                 "bigfunction": '{{ name }}',
@@ -62,25 +60,38 @@
                 "caller": self.caller,
                 'elapsed_ms': duration,
             },
             **kwargs,
         }
         print(json.dumps(message))
 
+
+class BaseQuotaManager:
+
+    def __init__(self, data):
+        self.row_count = len(data['calls'])
+
     def check_quotas(self):
-        if QUOTAS.get('max_rows_per_query') and self.row_count > QUOTAS['max_rows_per_query']:
+        if 'max_rows_per_query' in QUOTAS and (self.row_count > QUOTAS['max_rows_per_query']):
             raise QuotaException(f"It only accepts {QUOTAS['max_rows_per_query']} rows per query and you called it now on {self.row_count} rows or more.")
 
 
-class DatastoreQuotaManager(SimpleQuotaManager):
+class DatastoreQuotaManager(BaseQuotaManager):
 
     kind = 'bigfunction_call'
 
     _datastore = None
 
+    def __init__(self, data):
+        super().__init__(data)
+        self.created_at = datetime.datetime.utcnow()
+        self.user = data['sessionUser']
+        today = self.created_at.strftime("%Y-%m-%d")
+        self.user_bigfunction_date = f'{self.user}/{{ name }}/{today}'
+
     @property
     def datastore(self):
         if self._datastore is None:
             import google.cloud.datastore
             self._datastore = google.cloud.datastore.Client()
         return self._datastore
 
@@ -107,24 +118,25 @@
             'timestamp': self.created_at,
             'user_bigfunction_date': self.user_bigfunction_date,
             "row_count": self.row_count,
         })
         self.datastore.put(entity)
 
     def check_quotas(self):
-        if 'max_rows_per_query' in QUOTAS and (self.row_count > QUOTAS['max_rows_per_query']):
-            raise QuotaException(f"It only accepts {QUOTAS['max_rows_per_query']} rows per query and you called it now on {self.row_count} rows or more.")
-
+        super().check_quotas()
         if 'max_rows_per_user_per_day' in QUOTAS:
             today_row_count_for_this_bigfunction = self.get_today_row_count_for_this_bigfunction()
             if today_row_count_for_this_bigfunction + self.row_count > QUOTAS['max_rows_per_user_per_day']:
                 raise QuotaException(f"It only accepts {QUOTAS['max_rows_per_user_per_day']} rows per day per user and you called it today for {today_row_count_for_this_bigfunction + self.row_count} rows.")
             self.save_usage()
 
 
+QuotaManager = DatastoreQuotaManager if QUOTAS.get('backend') == 'datastore' else BaseQuotaManager
+
+
 class SecretManager:
 
     secret_manager = None
     secrets = {}
 
     def get(self, name):
         if name in self.secrets:
@@ -147,59 +159,57 @@
 
 
 {{ init_code }}
 
 {% if code_process_rows_as_batch %}
 
 def compute_all_rows(rows):
-    {{ code|replace('\n', '\n    ') }}
+    {{ code | replace('\n', '\n    ') | replace('{BIGFUNCTIONS_DATASET}',  '`' +  project + '`.`' + dataset + '`' ) }}
 
 {% else %}
 
 def compute_one_row(args):
     {% for argument in arguments %}{{ argument.name }}, {% endfor %} = args
-    {{ code|replace('\n', '\n    ') }}
+    {{ code | replace('\n', '\n    ') | replace('{BIGFUNCTIONS_DATASET}',  '`' +  project + '`.`' + dataset + '`' ) }}
 
 {% endif %}
 
 
 @app.route("/", methods=['POST'])
 def handle():
     try:
         data = request.get_json()
-        rows = data['calls']
-        if QUOTAS['backend'] == 'datastore':
-            quota_manager = DatastoreQuotaManager(data)
-        else:
-            quota_manager = SimpleQuotaManager(data)
+        logger = Logger(data)
+        logger.log(status='started')
+        quota_manager = QuotaManager(data)
         quota_manager.check_quotas()
-        quota_manager.save_log(status='started')
+        rows = data['calls']
         {% if code_process_rows_as_batch %}
         replies = compute_all_rows(rows)
         {% else %}
         replies = [compute_one_row(row) for row in rows]
         {% endif %}
         response = jsonify( { "replies" :  replies} )
-        quota_manager.save_log(status='success')
+        logger.log(status='success')
         return response
     except QuotaException as e:
         error_message = e.args[0]
-        quota_manager.save_log(status='quota_error', status_info=error_message)
+        logger.log(status='quota_error', status_info=error_message)
         return jsonify({
             'errorMessage': f'''
                 Thanks for using BigFunctions!
                 The use of this function `{{ name }}` is limited by quotas.
                 {error_message}.
                 To remove this limit, you can ask for quotas increase to `{QUOTAS['contact']}` or deploy the function in your own project.
                 Details are here: https://github.com/unytics/bigfunctions
                 If you need help, please reach out to the slack: https://join.slack.com/t/bigfunctions/shared_invite/zt-1gbv491mu-cs03EJbQ1fsHdQMcFN7E1Q
             '''.replace('\n', ' ').replace('  ', ' ').replace('  ', ' '),
         }), 400
     except AssertionError as e:
         error_message = e.args[0]
-        quota_manager.save_log(status='assertion_error', status_info=error_message)
+        logger.log(status='assertion_error', status_info=error_message)
         return jsonify({'errorMessage': error_message}), 400
     except Exception as e:
-        error_reporter.report_exception(google.cloud.error_reporting.build_flask_context(request))
         error_message = (str(e) + ' --- ' + traceback.format_exc())[:1000]
-        quota_manager.save_log(status='error', status_info=error_message)
+        logger.log(status='error', status_info=error_message)
+        error_reporter.report_exception(google.cloud.error_reporting.build_flask_context(request))
         return jsonify({'errorMessage': f"{type(e).__name__}: {str(e)}"}), 400
```

### Comparing `bigfunctions-0.1/bigfun/utils.py` & `bigfunctions-0.2/bigfun/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import tempfile
 import shutil
 import os
 import sys
 import subprocess
 import math
+import urllib.request
+
 
 import google.api_core.exceptions
 import google.auth.exceptions
 import google.cloud.bigquery
 import google.cloud.bigquery_connection_v1
 import google.cloud.storage
 import google.iam.v1.policy_pb2
 import click
 
 
+
 def print_color(msg):
     click.echo(click.style(msg, fg="cyan"))
 
 
 def print_success(msg):
     click.echo(click.style(f"SUCCESS: {msg}", fg="green"))
 
@@ -37,14 +40,28 @@
 def handle_error(msg, details=""):
     click.echo(click.style(f"ERROR: {msg}", fg="red"))
     if details:
         click.echo(click.style(f"ERROR_DETAILS: {details}", fg="red"))
     sys.exit()
 
 
+def merge_dict(a: dict, b: dict, path=[]):
+    for key in b:
+        if key in a:
+            if isinstance(a[key], dict) and isinstance(b[key], dict):
+                merge_dict(a[key], b[key], path + [str(key)])
+            elif type(a[key]) != type(b[key]):
+                raise Exception('Conflict at ' + '.'.join(path + [str(key)]) + ': key is in both dicts but type is different')
+            else:
+                a[key] = b[key]
+        else:
+            a[key] = b[key]
+    return a
+
+
 def exec(command):
     print_command(command)
     try:
         return subprocess.check_output(command, shell=True).decode().strip()
     except subprocess.CalledProcessError as e:
         handle_error("See error above. " + e.output.decode(errors="ignore").strip())
 
@@ -62,14 +79,25 @@
     numbered_lines = [
         str(index + starting_index).zfill(nb_zeroes) + ": " + line
         for index, line in enumerate(lines)
     ]
     return "\n".join(numbered_lines)
 
 
+def dataset_access_entry2user(access_entry):
+    if access_entry.entity_id == 'allAuthenticatedUsers':
+        return 'allAuthenticatedUsers'
+    entity_type = 'user'
+    if access_entry.entity_id.endswith('gserviceaccount.com'):
+        entity_type = 'serviceAccount'
+    elif access_entry.entity_type == 'groupByEmail':
+        entity_type = 'group'
+    return f'{entity_type}:{access_entry.entity_id}'
+
+
 class BigQuery:
     def __init__(self, project):
         self.project = project
         self._client = None
         self._bq_connection_client = None
 
     @property
@@ -95,17 +123,23 @@
                     "Google Cloud Application-Default-Credentials are not set. Authenticate with `gcloud auth application-default login` and retry"
                 )
         return self._bq_connection_client
 
     def get_dataset(self, dataset):
         print_info("Getting dataset")
         try:
-            return self.client.get_dataset(dataset.replace("`", ""))
+            dataset = self.client.get_dataset(dataset.replace("`", ""))
         except google.api_core.exceptions.NotFound as e:
             handle_error("Not Found", e.message)
+        dataset.users = [
+            dataset_access_entry2user(access_entry)
+            for access_entry in dataset.access_entries
+            if access_entry.entity_id not in ['projectOwners', 'projectWriters', 'projectReaders']
+        ]
+        return dataset
 
     def query(self, query):
         try:
             return self.client.query(query).result()
         except google.api_core.exceptions.Forbidden as e:
             handle_error("Access Denied", e.message)
         except (
@@ -218,14 +252,16 @@
 class CloudRun:
     def __init__(self, service, project, region):
         self.service = service
         self.project = project
         self.region = region
 
     def exec(self, command, options=None):
+        if shutil.which('gcloud') is None:
+            handle_error('`gcloud` is not installed while needed to deploy a Remote Function.')
         command += " " + self.service
         options = options or {}
         options["region"] = self.region
         options["project"] = self.project
         options_str = "".join([f" --{name} {value}" for name, value in options.items()])
         command += options_str
         return exec(command)
@@ -244,20 +280,20 @@
                 "ingress": "internal",
             },
             **{k.replace("_", "-"): v for k, v in options.items()},
         }
         if self.service in os.environ:
             # This service image has already been built, let's use it
             options["image"] = os.environ[self.service]
-            return self.exec("gcloud beta run deploy", options=options)
+            return self.exec("gcloud run deploy", options=options)
 
         options["source"] = source_folder
-        result = self.exec("gcloud beta run deploy", options=options)
+        result = self.exec("gcloud run deploy", options=options)
         os.environ[self.service] = self.exec(
-            "gcloud beta run services describe", options={"format": '"value(image)"'}
+            "gcloud run services describe", options={"format": '"value(image)"'}
         )
         return result
 
     @property
     def url(self):
         print_info(f"Get Cloud Run url of service `{self.service}`")
         return self.exec(
@@ -289,15 +325,15 @@
         handle_error(
             f"expecting npm package with a version formatted as `package_name@x.x.x` but got: {npm_package}"
         )
 
     name, version = npm_package.split("@")
     package_path = f"./node_modules/{name}"
     if "/" in name:
-        name, _ = name.split("/")
+        name, _ = name.split("/", 1)
     js_entrypoint_variable = name.replace("-", "_")
 
     print_info(
         f"Installing {name}@{version} npm package and webpack in tmp folder {destination_folder}"
     )
     command = (
         f"cd {destination_folder} && npm install webpack webpack-cli {name}@{version}"
@@ -318,7 +354,14 @@
             # This npm package has already been built and uploaded, let's use it
             return storage_filename
         print_info(f"Starting to build and upload npm package {npm_package}")
         build_npm_package(npm_package, output_filename, folder)
         Storage(project).upload(f"{folder}/{output_filename}", storage_filename)
         os.environ[storage_filename] = "uploaded"
         return storage_filename
+
+
+def download(url, destination_filename):
+    try:
+        urllib.request.urlretrieve(url, destination_filename)
+    except Exception as e:
+        handle_error(f'Could not download file at url `{url}`. Reason: {e}')
```

### Comparing `bigfunctions-0.1/bigfunctions.egg-info/PKG-INFO` & `bigfunctions-0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: bigfunctions
-Version: 0.1
-Summary: Supercharge BigQuery with BigFunctions
-Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.1.tar.gz
-Author: Unytics
-Author-email: paul.marcombes@unytics.io
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: google-cloud-bigquery
-Requires-Dist: google-cloud-bigquery_connection
-Requires-Dist: google-cloud-storage
-Requires-Dist: pyyaml
-Requires-Dist: jinja2
-Requires-Dist: mkdocs-material
-Requires-Dist: mkdocs-awesome-pages-plugin
-Requires-Dist: click
-Requires-Dist: click-help-colors
-
 
 <p align="center">
   <img class="hero-image" src="https://user-images.githubusercontent.com/111615732/186508787-6af04ed0-4750-4c49-926a-eacfd4a3dfbb.png" alt="logo_and_name" style="width: 100%; max-width: 600px">
 </p>
 
 <p align="center">
     Supercharge <em>BigQuery</em><br>with <em>BigFunctions</em><br><br>
@@ -116,47 +93,59 @@
 
 ## 💥 5. `bigfun` CLI
 
 `bigfun` CLI (command-line-interface) facilitates BigFunctions development, test, deployment, documentation and monitoring.
 
 ### 5.1 Install `bigfun` 🛠️
 
-Clone the repo and from the repo directory run:
 
 ``` sh
-virtualenv venv
-. venv/bin/activate
-pip install --editable .
+pip install bigfunctions
 ```
 
 ### 5.2 Use `bigfun` 🔥
 
 ``` sh
 $ bigfun --help
 Usage: bigfun [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --help  Show this message and exit.
 
 Commands:
-  deploy  Deploy BIGFUNCTION
-  doc     Generate, serve and publish documentation
-  test    Test BIGFUNCTION
+  deploy      Deploy BIGFUNCTION
+  docs        Generate, serve and publish documentation
+  get         Download BIGFUNCTION yaml file from unytics/bigfunctions...
+  test        Test BIGFUNCTION
+```
+
+
+### 5.3 Create you first function 👷
+
+Functions are defined as yaml files under `bigfunctions` folder. To create your first function locally, the easiest is to download an existing yaml file of unytics/bigfunctions Github repo. 
+
+For instance to download `is_email_valid.yaml` into bigfunctions folder, do:
+
+```sh
+bigfun get is_email_valid
 ```
 
+You can then update the file to suit your needs.
+
+
 
 
-### 5.3 Deploy you first function 👨‍💻
+### 5.4 Deploy you first function 👨‍💻
 
 > 1. Make sure the `gcloud` command is [installed on your computer](https://cloud.google.com/sdk/docs/install)
 > 2. Activate the application-default account with `gcloud auth application-default login`. A browser window should open, and you should be prompted to log into your Google account. Once you've done that, `bigfun` will use your oauth'd credentials to connect to BigQuery through BigQuery python client!
 > 3. Get or create a `DATASET` where you have permission to edit data and where the function will be deployed.
 > 4. The `DATASET` must belong to a `PROJECT` in which you have permission to run BigQuery queries.
 
-You now can deploy `is_email_valid` function with:
+You now can deploy the function `is_email_valid` defined in `bigfunctions/is_email_valid.yaml` yaml file by running:
 
 ```sh
 bigfun deploy is_email_valid
 ```
 
 > The first time you run this command it will ask for `PROJECT` and `DATASET`.
 >
@@ -168,22 +157,22 @@
 ```sql
 select PROJECT.DATASET.is_email_valid('paul.marcombes@unytics.io')
 ```
 
 <br>
 
 
-### 5.4 Deploy you first javascript function which depends on *npm packages* 👽
+### 5.5 Deploy you first javascript function which depends on *npm packages* 👽
 
 *To deploy a **javascript** function* which depends on **npm packages** there are additional requirements *in addition to the ones above*.
 
 > 1. You will need to install each *npm package* on your machine and bundle it into one file. For that, you need to [install *nodejs*](https://nodejs.org/en/download/).
-> 2. The bundled js file will be uploaded into a cloud storage bucket in which you must have write access. The bucket name is asked when you run `bigfun deploy`. Users of your functions must have read access to the bucket.
+> 2. The bundled js file will be uploaded into a cloud storage bucket in which you must have write access. The bucket name must be provided in `config.yaml` file in a variable named `bucket_js_dependencies`. Users of your functions must have read access to the bucket.
 
-You now can deploy `render_template` function with:
+You now can deploy the function `render_template` defined in `bigfunctions/render_template.yaml` yaml file by running:
 
 ```sh
 bigfun deploy render_template
 ```
 
 Test it with 👀:
 
@@ -191,25 +180,25 @@
 select PROJECT.DATASET.render_template('Hello {{ user }}', json '{"user": "James"}')
 ```
 
 
 <br>
 
 
-### 5.5 Deploy you first *remote* function ⚡️
+### 5.6 Deploy you first *remote* function ⚡️
 
 *To deploy a **remote** function* (e.g. python function), there are additional requirements *in addition to the ones of **Deploy you first function** section*.
 
 > 1. A *Cloud Run* service will be deployed to host the code ([as seen here](https://cloud.google.com/bigquery/docs/reference/standard-sql/remote-functions)). So you must have [permissions to deploy a *Cloud Run* service](https://cloud.google.com/run/docs/deploying-source-code#permissions_required_to_deploy) in your project `PROJECT`.
 > 2. `gcloud` CLI will be used directly to deploy the service (using `gcloud run deploy`). Then, make sure you are logged in with `gcloud` by calling: `gcloud auth login`. A browser window should also open, and you should be prompted to log into your Google account. WARNING: you read correctly: you have to authenticate twice. Once for bigquery python client (to deploy any function including remote as seen above.) and once now to use `gcloud` (to deploy a *Cloud Run* service).
 > 3. A *BigQuery Remote Connection* will be created to link BigQuery with the *Cloud Run* service. You then should have permissions to create a remote connection. *[BigQuery Connection Admin](https://cloud.google.com/bigquery/docs/access-control#bigquery.connectionAdmin)* or *[BigQuery Admin](https://cloud.google.com/bigquery/docs/access-control#bigquery.admin)* roles have these permissions.
 > 4. A service account will be automatically created by Google along with the *BigQuery Remote Connection*. BigQuery will use this service account of the remote connection to invoke the *Cloud Run* service. You then must have the permission to authorize this service account to invoke the *Cloud Run* service. This permission is provided in the role *[roles/run.admin](https://cloud.google.com/run/docs/reference/iam/roles)*
 
 
-You now can deploy `faker` function with:
+You now can deploy the function `faker` defined in `bigfunctions/faker.yaml` yaml file by running:
 
 ```sh
 bigfun deploy faker
 ```
 
 Test it with 👀:
```

#### html2text {}

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1 Name: bigfunctions Version: 0.1 Summary: Supercharge
-BigQuery with BigFunctions Download-URL: https://github.com/unytics/
-bigfunctions/archive/refs/tags/v0.1.tar.gz Author: Unytics Author-email:
-paul.marcombes@unytics.io Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: google-cloud-bigquery Requires-
-Dist: google-cloud-bigquery_connection Requires-Dist: google-cloud-storage
-Requires-Dist: pyyaml Requires-Dist: jinja2 Requires-Dist: mkdocs-material
-Requires-Dist: mkdocs-awesome-pages-plugin Requires-Dist: click Requires-Dist:
-click-help-colors
                                 [logo_and_name]
                              Supercharge BBiiggQQuueerryy
                                with BBiiggFFuunnccttiioonnss
 
                            UUppggrraaddee yyoouurr ddaattaa iimmppaacctt
                    with 100+ ready-to-use BigQuery Functions
                        (+ build a catalog of functions)
@@ -51,47 +40,55 @@
 **_h_e_r_e**.
 ## ð 4. Deploy BigFunctions in your GCP project You can also deploy any
 bigfunction in your project! To deploy *my_bigfunction* defined in
 *bigfunctions/my_bigfunction.yaml* file, simply call: ``` sh bigfun deploy
 my_bigfunction ``` Details about `bigfun` command line are given below.
 ## ð¥ 5. `bigfun` CLI `bigfun` CLI (command-line-interface) facilitates
 BigFunctions development, test, deployment, documentation and monitoring. ###
-5.1 Install `bigfun` ð ï¸ Clone the repo and from the repo directory run:
-``` sh virtualenv venv . venv/bin/activate pip install --editable . ``` ### 5.2
-Use `bigfun` ð¥ ``` sh $ bigfun --help Usage: bigfun [OPTIONS] COMMAND
-[ARGS]... Options: --help Show this message and exit. Commands: deploy Deploy
-BIGFUNCTION doc Generate, serve and publish documentation test Test BIGFUNCTION
-``` ### 5.3 Deploy you first function ð¨âð» > 1. Make sure the `gcloud`
-command is [installed on your computer](https://cloud.google.com/sdk/docs/
-install) > 2. Activate the application-default account with `gcloud auth
-application-default login`. A browser window should open, and you should be
-prompted to log into your Google account. Once you've done that, `bigfun` will
-use your oauth'd credentials to connect to BigQuery through BigQuery python
-client! > 3. Get or create a `DATASET` where you have permission to edit data
-and where the function will be deployed. > 4. The `DATASET` must belong to a
-`PROJECT` in which you have permission to run BigQuery queries. You now can
-deploy `is_email_valid` function with: ```sh bigfun deploy is_email_valid ``` >
-The first time you run this command it will ask for `PROJECT` and `DATASET`. >
-> Your inputs will be written to `config.yaml` file in current directory so
-that you won't be asked again (unless you delete the entries in `config.yaml`).
-You can also override this config at deploy time: `bigfun deploy is_email_valid
---project=PROJECT --dataset=DATASET`. Test it with ð: ```sql select
+5.1 Install `bigfun` ð ï¸ ``` sh pip install bigfunctions ``` ### 5.2 Use
+`bigfun` ð¥ ``` sh $ bigfun --help Usage: bigfun [OPTIONS] COMMAND [ARGS]...
+Options: --help Show this message and exit. Commands: deploy Deploy BIGFUNCTION
+docs Generate, serve and publish documentation get Download BIGFUNCTION yaml
+file from unytics/bigfunctions... test Test BIGFUNCTION ``` ### 5.3 Create you
+first function ð· Functions are defined as yaml files under `bigfunctions`
+folder. To create your first function locally, the easiest is to download an
+existing yaml file of unytics/bigfunctions Github repo. For instance to
+download `is_email_valid.yaml` into bigfunctions folder, do: ```sh bigfun get
+is_email_valid ``` You can then update the file to suit your needs. ### 5.4
+Deploy you first function ð¨âð» > 1. Make sure the `gcloud` command is
+[installed on your computer](https://cloud.google.com/sdk/docs/install) > 2.
+Activate the application-default account with `gcloud auth application-default
+login`. A browser window should open, and you should be prompted to log into
+your Google account. Once you've done that, `bigfun` will use your oauth'd
+credentials to connect to BigQuery through BigQuery python client! > 3. Get or
+create a `DATASET` where you have permission to edit data and where the
+function will be deployed. > 4. The `DATASET` must belong to a `PROJECT` in
+which you have permission to run BigQuery queries. You now can deploy the
+function `is_email_valid` defined in `bigfunctions/is_email_valid.yaml` yaml
+file by running: ```sh bigfun deploy is_email_valid ``` > The first time you
+run this command it will ask for `PROJECT` and `DATASET`. > > Your inputs will
+be written to `config.yaml` file in current directory so that you won't be
+asked again (unless you delete the entries in `config.yaml`). You can also
+override this config at deploy time: `bigfun deploy is_email_valid --
+project=PROJECT --dataset=DATASET`. Test it with ð: ```sql select
 PROJECT.DATASET.is_email_valid('paul.marcombes@unytics.io') ```
-### 5.4 Deploy you first javascript function which depends on *npm packages*
+### 5.5 Deploy you first javascript function which depends on *npm packages*
 ð½ *To deploy a **javascript** function* which depends on **npm packages**
 there are additional requirements *in addition to the ones above*. > 1. You
 will need to install each *npm package* on your machine and bundle it into one
 file. For that, you need to [install *nodejs*](https://nodejs.org/en/download/
 ). > 2. The bundled js file will be uploaded into a cloud storage bucket in
-which you must have write access. The bucket name is asked when you run `bigfun
-deploy`. Users of your functions must have read access to the bucket. You now
-can deploy `render_template` function with: ```sh bigfun deploy render_template
-``` Test it with ð: ```sql select PROJECT.DATASET.render_template('Hello {
-{ user }}', json '{"user": "James"}') ```
-### 5.5 Deploy you first *remote* function â¡ï¸ *To deploy a **remote**
+which you must have write access. The bucket name must be provided in
+`config.yaml` file in a variable named `bucket_js_dependencies`. Users of your
+functions must have read access to the bucket. You now can deploy the function
+`render_template` defined in `bigfunctions/render_template.yaml` yaml file by
+running: ```sh bigfun deploy render_template ``` Test it with ð: ```sql
+select PROJECT.DATASET.render_template('Hello {{ user }}', json '{"user":
+"James"}') ```
+### 5.6 Deploy you first *remote* function â¡ï¸ *To deploy a **remote**
 function* (e.g. python function), there are additional requirements *in
 addition to the ones of **Deploy you first function** section*. > 1. A *Cloud
 Run* service will be deployed to host the code ([as seen here](https://
 cloud.google.com/bigquery/docs/reference/standard-sql/remote-functions)). So
 you must have [permissions to deploy a *Cloud Run* service](https://
 cloud.google.com/run/docs/deploying-source-code#permissions_required_to_deploy)
 in your project `PROJECT`. > 2. `gcloud` CLI will be used directly to deploy
@@ -107,16 +104,17 @@
 control#bigquery.connectionAdmin)* or *[BigQuery Admin](https://
 cloud.google.com/bigquery/docs/access-control#bigquery.admin)* roles have these
 permissions. > 4. A service account will be automatically created by Google
 along with the *BigQuery Remote Connection*. BigQuery will use this service
 account of the remote connection to invoke the *Cloud Run* service. You then
 must have the permission to authorize this service account to invoke the *Cloud
 Run* service. This permission is provided in the role *[roles/run.admin](https:
-//cloud.google.com/run/docs/reference/iam/roles)* You now can deploy `faker`
-function with: ```sh bigfun deploy faker ``` Test it with ð: ```sql select
+//cloud.google.com/run/docs/reference/iam/roles)* You now can deploy the
+function `faker` defined in `bigfunctions/faker.yaml` yaml file by running:
+```sh bigfun deploy faker ``` Test it with ð: ```sql select
 PROJECT.DATASET.faker("name", "it_IT") ```
 ## ð 6. Contribute BigFunctions is fully open-source. Any contribution is
 more than welcome ð¤! - Add a â­ on the repo to show your support - [Join
 our Slack](https://join.slack.com/t/unytics/shared_invite/zt-1gbv491mu-
 cs03EJbQ1fsHdQMcFN7E1Q) and talk with us - Suggest a new function [here](https:
 //github.com/unytics/bigfunctions/issues/new?assignees=&labels=new-
 bigfunction&projects=&template=0_new_bigfunction.yaml&title=%5Bnew%5D%3A+%60function_name%28argument1%2C+argument2%29%60)
```

### Comparing `bigfunctions-0.1/setup.py` & `bigfunctions-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,27 @@
+import os
 import setuptools
 
 
-VERSION = '0.1'
+VERSION = '0.2'
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
+extra_files = [
+    os.path.join(root, f)
+    for root, dirs, filenames in os.walk('bigfun')
+    for f in filenames
+    if (
+        not f.endswith('.py')
+        and not '__pycache__' in root
+    )
+]
+
 
 setuptools.setup(
     name='bigfunctions',
     packages=['bigfun'],
     version=VERSION,
     author='Unytics',
     author_email='paul.marcombes@unytics.io',
@@ -19,25 +30,23 @@
     long_description_content_type='text/markdown',
     download_url=f'https://github.com/unytics/bigfunctions/archive/refs/tags/v{VERSION}.tar.gz',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.9',
-    package_data={'': ['*', 'templates/*']},
-    include_package_data=True,
+    python_requires='>=3.10',
+    package_data={'': extra_files},
     install_requires=[
         'google-cloud-bigquery',
         'google-cloud-bigquery_connection',
         'google-cloud-storage',
         'pyyaml',
         'jinja2',
         'mkdocs-material',
-        'mkdocs-awesome-pages-plugin',
         'click',
         'click-help-colors',
     ],
     entry_points={
         'console_scripts': [
             'bigfun = bigfun.cli:cli',
         ],
```

