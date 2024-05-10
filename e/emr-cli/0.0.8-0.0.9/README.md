# Comparing `tmp/emr_cli-0.0.8.tar.gz` & `tmp/emr_cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emr_cli-0.0.8.tar", max compression
+gzip compressed data, was "emr_cli-0.0.9.tar", max compression
```

## Comparing `emr_cli-0.0.8.tar` & `emr_cli-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10173 2023-04-06 23:53:41.013939 emr_cli-0.0.8/LICENSE
--rw-r--r--   0        0        0     4755 2023-04-06 23:53:41.013939 emr_cli-0.0.8/README.md
--rw-r--r--   0        0        0      593 2023-04-06 23:53:59.558425 emr_cli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      976 2023-04-06 23:53:41.013939 emr_cli-0.0.8/src/emr_cli/config.py
--rw-r--r--   0        0        0     1286 2023-04-06 23:53:41.013939 emr_cli-0.0.8/src/emr_cli/deployments/__init__.py
--rw-r--r--   0        0        0     5650 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/deployments/emr_ec2.py
--rw-r--r--   0        0        0    10964 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/deployments/emr_serverless.py
--rw-r--r--   0        0        0     6940 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/emr_cli.py
--rw-r--r--   0        0        0     1564 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/packaging/detector.py
--rw-r--r--   0        0        0     1905 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/packaging/python_files_project.py
--rw-r--r--   0        0        0     3877 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/packaging/python_poetry_project.py
--rw-r--r--   0        0        0     3704 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/packaging/python_project.py
--rw-r--r--   0        0        0      856 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/packaging/simple_project.py
--rw-r--r--   0        0        0     1101 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/templates/poetry/README.md
--rw-r--r--   0        0        0      413 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/templates/poetry/pyproject.toml
--rw-r--r--   0        0        0        6 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/templates/pyspark/.dockerignore
--rw-r--r--   0        0        0       12 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/templates/pyspark/.gitignore
--rw-r--r--   0        0        0     2680 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/templates/pyspark/Dockerfile
--rw-r--r--   0        0        0      458 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/templates/pyspark/entrypoint.py
--rw-r--r--   0        0        0     3369 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/templates/pyspark/jobs/extreme_weather.py
--rw-r--r--   0        0        0      175 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/templates/pyspark/pyproject.toml
--rw-r--r--   0        0        0     2619 2023-04-06 23:53:41.017939 emr_cli-0.0.8/src/emr_cli/utils/__init__.py
--rw-r--r--   0        0        0     5543 1970-01-01 00:00:00.000000 emr_cli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-05-09 17:30:22.086017 emr_cli-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4755 2023-05-09 17:30:22.086017 emr_cli-0.0.9/README.md
+-rw-r--r--   0        0        0      593 2023-05-09 17:30:48.158147 emr_cli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      976 2023-05-09 17:30:22.086017 emr_cli-0.0.9/src/emr_cli/config.py
+-rw-r--r--   0        0        0     1286 2023-05-09 17:30:22.086017 emr_cli-0.0.9/src/emr_cli/deployments/__init__.py
+-rw-r--r--   0        0        0     5329 2023-05-09 17:30:22.086017 emr_cli-0.0.9/src/emr_cli/deployments/emr_ec2.py
+-rw-r--r--   0        0        0    11322 2023-05-09 17:30:22.086017 emr_cli-0.0.9/src/emr_cli/deployments/emr_serverless.py
+-rw-r--r--   0        0        0     7046 2023-05-09 17:30:22.086017 emr_cli-0.0.9/src/emr_cli/emr_cli.py
+-rw-r--r--   0        0        0     1564 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/packaging/detector.py
+-rw-r--r--   0        0        0     1905 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/packaging/python_files_project.py
+-rw-r--r--   0        0        0     3877 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/packaging/python_poetry_project.py
+-rw-r--r--   0        0        0     3704 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/packaging/python_project.py
+-rw-r--r--   0        0        0      856 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/packaging/simple_project.py
+-rw-r--r--   0        0        0     1101 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/templates/poetry/README.md
+-rw-r--r--   0        0        0      413 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/templates/poetry/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/templates/pyspark/.dockerignore
+-rw-r--r--   0        0        0       12 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/templates/pyspark/.gitignore
+-rw-r--r--   0        0        0     2680 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/templates/pyspark/Dockerfile
+-rw-r--r--   0        0        0      458 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/templates/pyspark/entrypoint.py
+-rw-r--r--   0        0        0     3369 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/templates/pyspark/jobs/extreme_weather.py
+-rw-r--r--   0        0        0      175 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/templates/pyspark/pyproject.toml
+-rw-r--r--   0        0        0     2983 2023-05-09 17:30:22.090017 emr_cli-0.0.9/src/emr_cli/utils/__init__.py
+-rw-r--r--   0        0        0     5543 1970-01-01 00:00:00.000000 emr_cli-0.0.9/PKG-INFO
```

### Comparing `emr_cli-0.0.8/LICENSE` & `emr_cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/README.md` & `emr_cli-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/pyproject.toml` & `emr_cli-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emr-cli"
-version = "v0.0.8"
+version = "v0.0.9"
 description = "A command-line interface for packaging, deploying, and running your EMR Serverless Spark jobs."
 authors = ["Amazon EMR <emr-developer-advocates@amazon.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `emr_cli-0.0.8/src/emr_cli/config.py` & `emr_cli-0.0.9/src/emr_cli/config.py`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/src/emr_cli/deployments/__init__.py` & `emr_cli-0.0.9/src/emr_cli/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/src/emr_cli/deployments/emr_ec2.py` & `emr_cli-0.0.9/src/emr_cli/deployments/emr_ec2.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from os.path import join
 from typing import List, Optional
 
 import boto3
 from botocore.exceptions import ClientError, WaiterError
 from emr_cli.deployments.emr_serverless import DeploymentPackage
-from emr_cli.utils import console_log, parse_bucket_uri
+from emr_cli.utils import console_log, parse_bucket_uri, print_s3_gz
 
 LOG_WAITER_DELAY_SEC = 30
 
 
 class EMREC2:
     def __init__(
         self, cluster_id: str, deployment_package: DeploymentPackage, region: str = ""
@@ -96,15 +96,15 @@
 
         if show_logs:
             # We need to validate s3-logging is enabled and fetch the location of the logs
             try:
                 logs_location = self._fetch_log_location()
                 stdout_location = self._wait_for_logs(step_id, logs_location, 30 * 60)
                 console_log(f"stdout for {step_id}\n{'-'*36}")
-                self._print_logs(stdout_location)
+                print_s3_gz(self.s3_client, stdout_location)
                 if job_failed:
                     sys.exit(1)
             except RuntimeError as e:
                 console_log(f"ERR: {e}")
                 sys.exit(1)
             except WaiterError as e:
                 console_log(f"ERR: While waiting for logs to appear: {e}")
@@ -136,16 +136,7 @@
             Key=key,
             WaiterConfig={
                 "Delay": LOG_WAITER_DELAY_SEC,
                 "MaxAttempts": timeout_secs / LOG_WAITER_DELAY_SEC,
             },
         )
         return object_name
-
-    def _print_logs(self, s3_uri: str):
-        """
-        Downloads and decompresses a gzip file from S3 and prints the logs to stdout.
-        """
-        bucket, key = parse_bucket_uri(s3_uri)
-        gz = self.s3_client.get_object(Bucket=bucket, Key=key)
-        with gzip.open(gz["Body"]) as data:
-            print(data.read().decode())
```

### Comparing `emr_cli-0.0.8/src/emr_cli/deployments/emr_serverless.py` & `emr_cli-0.0.9/src/emr_cli/deployments/emr_serverless.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import abc
 import json
 import os
 import sys
 import zipfile
+from os.path import join
 from time import sleep
 from typing import List, Optional
 
 import boto3
-
 from emr_cli.deployments import SparkParams
-from emr_cli.utils import console_log, find_files, mkdir
+from emr_cli.utils import console_log, find_files, mkdir, print_s3_gz
 
 
 class DeploymentPackage(metaclass=abc.ABCMeta):
     def __init__(
         self, entry_point_path: str = "entrypoint.py", s3_target_uri: str = ""
     ) -> None:
         self.entry_point_path = entry_point_path
@@ -206,35 +206,33 @@
         job_role: str,
         deployment_package: DeploymentPackage,
         region: str = "",
     ) -> None:
         self.application_id = application_id
         self.job_role = job_role
         self.dp = deployment_package
+        self.s3_client = boto3.client("s3")
         if region:
             self.client = boto3.client("emr-serverless", region_name=region)
         else:
             # Note that boto3 uses AWS_DEFAULT_REGION, not AWS_REGION
             # We may want to add an extra check here for the latter.
             self.client = boto3.client("emr-serverless")
 
     def run_job(
         self,
         job_name: str,
         job_args: Optional[List[str]] = None,
         spark_submit_opts: Optional[str] = None,
         wait: bool = True,
         show_logs: bool = False,
+        s3_logs_uri: Optional[str] = None,
     ):
-        if show_logs:
-            raise RuntimeError(
-                "--show-stdout is not compatible with EMR Serverless (yet).\n"
-                + "Please 👍 this GitHub issue to voice your support: "
-                + "https://github.com/awslabs/amazon-emr-cli/issues/11"
-            )
+        if show_logs and not s3_logs_uri:
+            raise RuntimeError("--show-stdout requires --s3-logs-uri to be set.")
 
         jobDriver = {
             "sparkSubmit": {
                 "entryPoint": self.dp.entrypoint_uri(),
             }
         }
         spark_submit_parameters = self.dp.spark_submit_parameters().params_for(
@@ -248,57 +246,70 @@
 
         if spark_submit_parameters:
             jobDriver["sparkSubmit"]["sparkSubmitParameters"] = spark_submit_parameters
 
         if job_args:
             jobDriver["sparkSubmit"]["entryPointArguments"] = job_args  # type: ignore
 
+        config_overrides = {}
+        if s3_logs_uri:
+            config_overrides = {
+                "monitoringConfiguration": {
+                    "s3MonitoringConfiguration": {"logUri": s3_logs_uri}
+                }
+            }
+
         response = self.client.start_job_run(
             applicationId=self.application_id,
             executionRoleArn=self.job_role,
             name=job_name,
             jobDriver=jobDriver,
-            # configurationOverrides={
-            #     "monitoringConfiguration": {
-            #         "s3MonitoringConfiguration": {
-            #             "logUri": "s3://<BUCKET>/logs/"
-            #         }
-            #     }
-            # },
+            configurationOverrides=config_overrides,
         )
         job_run_id = response.get("jobRunId")
 
         console_log(f"Job submitted to EMR Serverless (Job Run ID: {job_run_id})")
-        if wait:
-            console_log("Waiting for job to complete...")
+        if not wait and not show_logs:
+            return job_run_id
 
+        console_log("Waiting for job to complete...")
         job_done = False
         job_state = "SUBMITTED"
         jr_response = {}
-        while wait and not job_done:
+        while not job_done:
             jr_response = self.get_job_run(job_run_id)
             new_state = jr_response.get("state")
             if new_state != job_state:
                 console_log(f"Job state is now: {new_state}")
                 job_state = new_state
             job_done = new_state in [
                 "SUCCESS",
                 "FAILED",
                 "CANCELLING",
                 "CANCELLED",
             ]
             sleep(2)
 
-        if wait:
-            if jr_response.get("state") != "SUCCESS":
-                console_log(
-                    f"EMR Serverless job failed: {jr_response.get('stateDetails')}"
-                )
-                sys.exit(1)
-            console_log("Job completed successfully!")
+        if show_logs:
+            console_log(f"stdout for {job_run_id}\n{'-'*38}")
+            log_location = join(
+                f"{s3_logs_uri}",
+                "applications",
+                self.application_id,
+                "jobs",
+                job_run_id,
+                "SPARK_DRIVER",
+                "stdout.gz",
+            )
+            print_s3_gz(self.s3_client, log_location)
+
+        if jr_response.get("state") != "SUCCESS":
+            console_log(f"EMR Serverless job failed: {jr_response.get('stateDetails')}")
+            sys.exit(1)
+        console_log("Job completed successfully!")
 
         return job_run_id
 
     def get_job_run(self, job_run_id: str) -> dict:
         response = self.client.get_job_run(
             applicationId=self.application_id, jobRunId=job_run_id
         )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `emr_cli-0.0.8/src/emr_cli/emr_cli.py` & `emr_cli-0.0.9/src/emr_cli/emr_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
     "--entry-point",
     type=click.Path(exists=True, dir_okay=False, allow_dash=False),
     help="Python or Jar file for the main entrypoint",
 )
 @click.option("--job-role", help="IAM Role ARN to use for the job execution")
 @click.option("--wait", default=False, is_flag=True, help="Wait for job to finish")
 @click.option("--s3-code-uri", help="Where to copy/run code artifacts to/from")
+@click.option("--s3-logs-uri", help="Where to send EMR Serverless logs to")
 @click.option("--job-name", help="The name of the job", default="emr-cli job")
 @click.option(
     "--job-args",
     help="Comma-delimited string of arguments to be passed to Spark job",
     default=None,
 )
 @click.option(
@@ -183,14 +184,15 @@
     project,
     application_id,
     cluster_id,
     entry_point,
     job_role,
     wait,
     s3_code_uri,
+    s3_logs_uri,
     job_name,
     job_args,
     spark_submit_opts,
     build,
     show_stdout,
 ):
     """
@@ -220,15 +222,15 @@
             raise click.BadArgumentUsage(
                 "--entry-point and --job-role are required if --application-id is used."
             )
 
         if job_args:
             job_args = job_args.split(",")
         emrs = EMRServerless(application_id, job_role, p)
-        emrs.run_job(job_name, job_args, spark_submit_opts, wait, show_stdout)
+        emrs.run_job(job_name, job_args, spark_submit_opts, wait, show_stdout, s3_logs_uri)
 
     # cluster_id indicates EMR on EC2 job
     if cluster_id is not None:
         if job_args:
             job_args = job_args.split(",")
         emr = EMREC2(cluster_id, p)
         emr.run_job(job_name, job_args, wait, show_stdout)
```

### Comparing `emr_cli-0.0.8/src/emr_cli/packaging/detector.py` & `emr_cli-0.0.9/src/emr_cli/packaging/detector.py`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/src/emr_cli/packaging/python_files_project.py` & `emr_cli-0.0.9/src/emr_cli/packaging/python_files_project.py`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/src/emr_cli/packaging/python_poetry_project.py` & `emr_cli-0.0.9/src/emr_cli/packaging/python_poetry_project.py`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/src/emr_cli/packaging/python_project.py` & `emr_cli-0.0.9/src/emr_cli/packaging/python_project.py`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/src/emr_cli/packaging/simple_project.py` & `emr_cli-0.0.9/src/emr_cli/packaging/simple_project.py`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/src/emr_cli/templates/poetry/README.md` & `emr_cli-0.0.9/src/emr_cli/templates/poetry/README.md`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/src/emr_cli/templates/pyspark/Dockerfile` & `emr_cli-0.0.9/src/emr_cli/templates/pyspark/Dockerfile`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/src/emr_cli/templates/pyspark/jobs/extreme_weather.py` & `emr_cli-0.0.9/src/emr_cli/templates/pyspark/jobs/extreme_weather.py`

 * *Files identical despite different names*

### Comparing `emr_cli-0.0.8/src/emr_cli/utils/__init__.py` & `emr_cli-0.0.9/src/emr_cli/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import gzip
 import os
 import re
 import sys
 from calendar import c
 from pathlib import Path
 from shutil import copyfile, copytree, ignore_patterns
 from typing import List
 from urllib.parse import urlparse
 
+import boto3
+
 
 def console_log(message):
     print(f"[emr-cli]: {message}")
 
 
 def find_files(directory, excluded_dirs=[], search=None) -> List[str]:
     files = []
@@ -84,7 +87,17 @@
         console_log(f"ERR: Target `{name}` not found in Dockerfile.")
         console_log(
             "ERR: Try creating a new dockerfile with the `emr init --dockerfile .` command."
         )
         sys.exit(1)
 
     return False
+
+
+def print_s3_gz(client: boto3.session.Session.client, s3_uri: str):
+    """
+    Downloads and decompresses a gzip file from S3 and prints the logs to stdout.
+    """
+    bucket, key = parse_bucket_uri(s3_uri)
+    gz = client.get_object(Bucket=bucket, Key=key)
+    with gzip.open(gz["Body"]) as data:
+        print(data.read().decode())
```

### Comparing `emr_cli-0.0.8/PKG-INFO` & `emr_cli-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emr-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: A command-line interface for packaging, deploying, and running your EMR Serverless Spark jobs.
 License: Apache-2.0
 Author: Amazon EMR
 Author-email: emr-developer-advocates@amazon.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

