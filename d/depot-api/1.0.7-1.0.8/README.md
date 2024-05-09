# Comparing `tmp/depot_api-1.0.7.tar.gz` & `tmp/depot_api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depot_api-1.0.7.tar", last modified: Tue Apr 30 13:07:27 2024, max compression
+gzip compressed data, was "depot_api-1.0.8.tar", last modified: Thu May  9 23:29:43 2024, max compression
```

## Comparing `depot_api-1.0.7.tar` & `depot_api-1.0.8.tar`

### file list

```diff
@@ -1,53 +1,71 @@
--rw-r--r--   0        0        0     7628 2024-04-30 11:01:54.696567 depot_api-1.0.7/README.md
--rw-r--r--   0        0        0     1579 2024-04-30 11:01:54.720574 depot_api-1.0.7/depot_api/__init__.py
--rw-r--r--   0        0        0       97 2024-04-30 11:01:54.722210 depot_api-1.0.7/depot_api/api/__init__.py
--rw-r--r--   0        0        0   257139 2024-04-30 11:01:54.654214 depot_api-1.0.7/depot_api/api/default_api.py
--rw-r--r--   0        0        0    25761 2024-04-30 11:01:54.727516 depot_api-1.0.7/depot_api/api_client.py
--rw-r--r--   0        0        0      652 2024-04-30 11:01:54.728128 depot_api-1.0.7/depot_api/api_response.py
--rw-r--r--   0        0        0    14735 2024-04-30 11:01:54.719388 depot_api-1.0.7/depot_api/configuration.py
--rw-r--r--   0        0        0     5972 2024-04-30 11:01:54.723817 depot_api-1.0.7/depot_api/exceptions.py
--rw-r--r--   0        0        0     1031 2024-04-30 11:01:54.721577 depot_api-1.0.7/depot_api/models/__init__.py
--rw-r--r--   0        0        0     4826 2024-04-30 11:01:54.502071 depot_api-1.0.7/depot_api/models/client_id.py
--rw-r--r--   0        0        0     4850 2024-04-30 11:01:54.511995 depot_api-1.0.7/depot_api/models/client_secret.py
--rw-r--r--   0        0        0     3049 2024-04-15 14:00:46.761397 depot_api-1.0.7/depot_api/models/cluster.py
--rw-r--r--   0        0        0     2716 2024-04-30 11:01:54.519862 depot_api-1.0.7/depot_api/models/cluster_in.py
--rw-r--r--   0        0        0     4897 2024-04-30 11:01:54.526646 depot_api-1.0.7/depot_api/models/grant_type.py
--rw-r--r--   0        0        0     2978 2024-04-30 11:01:54.535113 depot_api-1.0.7/depot_api/models/http_validation_error.py
--rw-r--r--   0        0        0     4801 2024-04-30 11:01:54.541423 depot_api-1.0.7/depot_api/models/id.py
--rw-r--r--   0        0        0     3427 2024-04-18 08:54:32.098926 depot_api-1.0.7/depot_api/models/job_instance.py
--rw-r--r--   0        0        0     2948 2024-04-30 11:01:54.548015 depot_api-1.0.7/depot_api/models/job_instance_in.py
--rw-r--r--   0        0        0     4838 2024-04-30 09:34:16.126240 depot_api-1.0.7/depot_api/models/private_key.py
--rw-r--r--   0        0        0     3056 2024-04-30 11:01:54.553912 depot_api-1.0.7/depot_api/models/provider.py
--rw-r--r--   0        0        0     4832 2024-04-30 09:34:16.126948 depot_api-1.0.7/depot_api/models/public_key.py
--rw-r--r--   0        0        0     2988 2024-04-18 08:54:32.122496 depot_api-1.0.7/depot_api/models/repository.py
--rw-r--r--   0        0        0     2650 2024-04-30 11:01:54.560586 depot_api-1.0.7/depot_api/models/repository_in.py
--rw-r--r--   0        0        0     4856 2024-04-30 09:34:16.127862 depot_api-1.0.7/depot_api/models/repository_key.py
--rw-r--r--   0        0        0     3199 2024-04-18 08:54:32.125437 depot_api-1.0.7/depot_api/models/repository_out.py
--rw-r--r--   0        0        0     2715 2024-04-30 11:01:54.568091 depot_api-1.0.7/depot_api/models/ssh_key_in.py
--rw-r--r--   0        0        0     3079 2024-04-30 11:01:54.572631 depot_api-1.0.7/depot_api/models/validation_error.py
--rw-r--r--   0        0        0     4901 2024-04-30 11:01:54.576452 depot_api-1.0.7/depot_api/models/validation_error_loc_inner.py
--rw-r--r--   0        0        0        0 2024-04-30 11:01:54.716503 depot_api-1.0.7/depot_api/py.typed
--rw-r--r--   0        0        0     9227 2024-04-30 11:01:54.729580 depot_api-1.0.7/depot_api/rest.py
--rw-r--r--   0        0        0     1919 2024-04-30 13:07:27.717369 depot_api-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-30 11:01:54.724655 depot_api-1.0.7/test/__init__.py
--rw-r--r--   0        0        0     1276 2024-04-18 20:09:02.454188 depot_api-1.0.7/test/test_client_id.py
--rw-r--r--   0        0        0     1324 2024-04-18 20:09:02.466568 depot_api-1.0.7/test/test_client_secret.py
--rw-r--r--   0        0        0     1509 2024-04-15 14:00:46.763230 depot_api-1.0.7/test/test_cluster.py
--rw-r--r--   0        0        0     1685 2024-04-16 05:26:03.952432 depot_api-1.0.7/test/test_cluster_in.py
--rw-r--r--   0        0        0     3543 2024-04-15 14:00:46.839817 depot_api-1.0.7/test/test_default_api.py
--rw-r--r--   0        0        0     1288 2024-04-18 20:09:02.478374 depot_api-1.0.7/test/test_grant_type.py
--rw-r--r--   0        0        0     1698 2024-04-15 14:00:46.769812 depot_api-1.0.7/test/test_http_validation_error.py
--rw-r--r--   0        0        0     1203 2024-04-15 14:00:46.780645 depot_api-1.0.7/test/test_id.py
--rw-r--r--   0        0        0     1663 2024-04-15 14:00:46.785728 depot_api-1.0.7/test/test_job_instance.py
--rw-r--r--   0        0        0     1732 2024-04-18 06:49:32.731307 depot_api-1.0.7/test/test_job_instance_in.py
--rw-r--r--   0        0        0     1300 2024-04-30 09:34:16.145205 depot_api-1.0.7/test/test_private_key.py
--rw-r--r--   0        0        0     1526 2024-04-15 14:00:46.790366 depot_api-1.0.7/test/test_provider.py
--rw-r--r--   0        0        0     1288 2024-04-30 09:34:16.149824 depot_api-1.0.7/test/test_public_key.py
--rw-r--r--   0        0        0     1569 2024-04-15 14:00:46.793463 depot_api-1.0.7/test/test_repository.py
--rw-r--r--   0        0        0     1513 2024-04-30 09:34:16.155031 depot_api-1.0.7/test/test_repository_in.py
--rw-r--r--   0        0        0     1336 2024-04-30 09:34:16.157940 depot_api-1.0.7/test/test_repository_key.py
--rw-r--r--   0        0        0     2371 2024-04-15 14:00:46.796985 depot_api-1.0.7/test/test_repository_out.py
--rw-r--r--   0        0        0     1528 2024-04-30 09:34:16.159968 depot_api-1.0.7/test/test_ssh_key_in.py
--rw-r--r--   0        0        0     1609 2024-04-15 14:00:46.800103 depot_api-1.0.7/test/test_validation_error.py
--rw-r--r--   0        0        0     1458 2024-04-15 14:00:46.802999 depot_api-1.0.7/test/test_validation_error_loc_inner.py
--rw-r--r--   0        0        0     8369 1970-01-01 00:00:00.000000 depot_api-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     8560 2024-05-09 22:33:29.864059 depot_api-1.0.8/README.md
+-rw-r--r--   0        0        0     2056 2024-05-09 22:33:29.883448 depot_api-1.0.8/depot_api/__init__.py
+-rw-r--r--   0        0        0       97 2024-05-09 22:33:29.924536 depot_api-1.0.8/depot_api/api/__init__.py
+-rw-r--r--   0        0        0   288568 2024-05-09 22:33:29.849028 depot_api-1.0.8/depot_api/api/default_api.py
+-rw-r--r--   0        0        0    25761 2024-05-09 22:33:29.934264 depot_api-1.0.8/depot_api/api_client.py
+-rw-r--r--   0        0        0      652 2024-05-09 22:33:29.935022 depot_api-1.0.8/depot_api/api_response.py
+-rw-r--r--   0        0        0    14735 2024-05-09 22:33:29.881487 depot_api-1.0.8/depot_api/configuration.py
+-rw-r--r--   0        0        0     5972 2024-05-09 22:33:29.926247 depot_api-1.0.8/depot_api/exceptions.py
+-rw-r--r--   0        0        0     1508 2024-05-09 22:33:29.921199 depot_api-1.0.8/depot_api/models/__init__.py
+-rw-r--r--   0        0        0     4826 2024-05-09 22:33:29.554031 depot_api-1.0.8/depot_api/models/client_id.py
+-rw-r--r--   0        0        0     4850 2024-05-09 22:33:29.564968 depot_api-1.0.8/depot_api/models/client_secret.py
+-rw-r--r--   0        0        0     3124 2024-05-09 10:12:13.034256 depot_api-1.0.8/depot_api/models/cluster.py
+-rw-r--r--   0        0        0     2716 2024-05-09 22:33:29.573023 depot_api-1.0.8/depot_api/models/cluster_in.py
+-rw-r--r--   0        0        0     2911 2024-05-09 22:33:29.581723 depot_api-1.0.8/depot_api/models/cluster_out.py
+-rw-r--r--   0        0        0     4838 2024-05-09 22:33:29.592102 depot_api-1.0.8/depot_api/models/finished_at.py
+-rw-r--r--   0        0        0     4897 2024-05-09 22:33:29.609131 depot_api-1.0.8/depot_api/models/grant_type.py
+-rw-r--r--   0        0        0     2978 2024-05-09 22:33:29.616546 depot_api-1.0.8/depot_api/models/http_validation_error.py
+-rw-r--r--   0        0        0     4801 2024-05-09 22:33:29.622256 depot_api-1.0.8/depot_api/models/id.py
+-rw-r--r--   0        0        0     2428 2024-05-09 22:33:29.627504 depot_api-1.0.8/depot_api/models/id_out.py
+-rw-r--r--   0        0        0     3427 2024-04-18 08:54:32.098926 depot_api-1.0.8/depot_api/models/job_instance.py
+-rw-r--r--   0        0        0     2925 2024-05-09 22:33:29.633118 depot_api-1.0.8/depot_api/models/job_instance_in.py
+-rw-r--r--   0        0        0     3956 2024-05-09 22:33:29.639411 depot_api-1.0.8/depot_api/models/job_instance_out.py
+-rw-r--r--   0        0        0     2436 2024-05-09 22:33:29.647807 depot_api-1.0.8/depot_api/models/log_out.py
+-rw-r--r--   0        0        0     4838 2024-04-30 09:34:16.126240 depot_api-1.0.8/depot_api/models/private_key.py
+-rw-r--r--   0        0        0     3056 2024-05-09 22:33:29.656910 depot_api-1.0.8/depot_api/models/provider.py
+-rw-r--r--   0        0        0     2960 2024-05-09 22:33:29.662902 depot_api-1.0.8/depot_api/models/provider_out.py
+-rw-r--r--   0        0        0     2843 2024-05-09 22:03:54.487206 depot_api-1.0.8/depot_api/models/provider_type.py
+-rw-r--r--   0        0        0     2617 2024-05-09 22:33:29.667714 depot_api-1.0.8/depot_api/models/provider_type_out.py
+-rw-r--r--   0        0        0     4832 2024-04-30 09:34:16.126948 depot_api-1.0.8/depot_api/models/public_key.py
+-rw-r--r--   0        0        0     2988 2024-04-18 08:54:32.122496 depot_api-1.0.8/depot_api/models/repository.py
+-rw-r--r--   0        0        0     2650 2024-05-09 22:33:29.671843 depot_api-1.0.8/depot_api/models/repository_in.py
+-rw-r--r--   0        0        0     4856 2024-04-30 09:34:16.127862 depot_api-1.0.8/depot_api/models/repository_key.py
+-rw-r--r--   0        0        0     2796 2024-05-09 22:33:29.676717 depot_api-1.0.8/depot_api/models/repository_out.py
+-rw-r--r--   0        0        0     2715 2024-05-09 22:33:29.682062 depot_api-1.0.8/depot_api/models/ssh_key_in.py
+-rw-r--r--   0        0        0     2542 2024-05-09 22:33:29.698358 depot_api-1.0.8/depot_api/models/ssh_key_out.py
+-rw-r--r--   0        0        0     3079 2024-05-09 22:33:29.706307 depot_api-1.0.8/depot_api/models/validation_error.py
+-rw-r--r--   0        0        0     4901 2024-05-09 22:33:29.714172 depot_api-1.0.8/depot_api/models/validation_error_loc_inner.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:33:29.878223 depot_api-1.0.8/depot_api/py.typed
+-rw-r--r--   0        0        0     9227 2024-05-09 22:33:29.936102 depot_api-1.0.8/depot_api/rest.py
+-rw-r--r--   0        0        0     1840 2024-05-09 23:29:43.138905 depot_api-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-09 22:33:29.932532 depot_api-1.0.8/test/__init__.py
+-rw-r--r--   0        0        0     1276 2024-04-18 20:09:02.454188 depot_api-1.0.8/test/test_client_id.py
+-rw-r--r--   0        0        0     1324 2024-04-18 20:09:02.466568 depot_api-1.0.8/test/test_client_secret.py
+-rw-r--r--   0        0        0     1509 2024-04-15 14:00:46.763230 depot_api-1.0.8/test/test_cluster.py
+-rw-r--r--   0        0        0     1685 2024-04-16 05:26:03.952432 depot_api-1.0.8/test/test_cluster_in.py
+-rw-r--r--   0        0        0     1955 2024-05-09 20:02:06.356349 depot_api-1.0.8/test/test_cluster_out.py
+-rw-r--r--   0        0        0     3543 2024-04-15 14:00:46.839817 depot_api-1.0.8/test/test_default_api.py
+-rw-r--r--   0        0        0     1300 2024-05-09 10:06:00.235677 depot_api-1.0.8/test/test_finished_at.py
+-rw-r--r--   0        0        0     1288 2024-04-18 20:09:02.478374 depot_api-1.0.8/test/test_grant_type.py
+-rw-r--r--   0        0        0     1698 2024-04-15 14:00:46.769812 depot_api-1.0.8/test/test_http_validation_error.py
+-rw-r--r--   0        0        0     1203 2024-04-15 14:00:46.780645 depot_api-1.0.8/test/test_id.py
+-rw-r--r--   0        0        0     1289 2024-05-09 10:06:00.259673 depot_api-1.0.8/test/test_id_out.py
+-rw-r--r--   0        0        0     1663 2024-04-15 14:00:46.785728 depot_api-1.0.8/test/test_job_instance.py
+-rw-r--r--   0        0        0     1732 2024-04-18 06:49:32.731307 depot_api-1.0.8/test/test_job_instance_in.py
+-rw-r--r--   0        0        0     1994 2024-05-09 10:06:00.269492 depot_api-1.0.8/test/test_job_instance_out.py
+-rw-r--r--   0        0        0     1303 2024-05-09 10:06:00.274417 depot_api-1.0.8/test/test_log_out.py
+-rw-r--r--   0        0        0     1300 2024-04-30 09:34:16.145205 depot_api-1.0.8/test/test_private_key.py
+-rw-r--r--   0        0        0     1526 2024-04-15 14:00:46.790366 depot_api-1.0.8/test/test_provider.py
+-rw-r--r--   0        0        0     1669 2024-05-09 20:02:06.423275 depot_api-1.0.8/test/test_provider_out.py
+-rw-r--r--   0        0        0     1462 2024-05-09 10:12:13.106855 depot_api-1.0.8/test/test_provider_type.py
+-rw-r--r--   0        0        0     1472 2024-05-09 20:02:06.432253 depot_api-1.0.8/test/test_provider_type_out.py
+-rw-r--r--   0        0        0     1288 2024-04-30 09:34:16.149824 depot_api-1.0.8/test/test_public_key.py
+-rw-r--r--   0        0        0     1569 2024-04-15 14:00:46.793463 depot_api-1.0.8/test/test_repository.py
+-rw-r--r--   0        0        0     1513 2024-04-30 09:34:16.155031 depot_api-1.0.8/test/test_repository_in.py
+-rw-r--r--   0        0        0     1336 2024-04-30 09:34:16.157940 depot_api-1.0.8/test/test_repository_key.py
+-rw-r--r--   0        0        0     2371 2024-04-15 14:00:46.796985 depot_api-1.0.8/test/test_repository_out.py
+-rw-r--r--   0        0        0     1528 2024-04-30 09:34:16.159968 depot_api-1.0.8/test/test_ssh_key_in.py
+-rw-r--r--   0        0        0     1406 2024-05-09 10:06:00.295723 depot_api-1.0.8/test/test_ssh_key_out.py
+-rw-r--r--   0        0        0     1609 2024-04-15 14:00:46.800103 depot_api-1.0.8/test/test_validation_error.py
+-rw-r--r--   0        0        0     1458 2024-04-15 14:00:46.802999 depot_api-1.0.8/test/test_validation_error_loc_inner.py
+-rw-r--r--   0        0        0     9248 1970-01-01 00:00:00.000000 depot_api-1.0.8/PKG-INFO
```

### Comparing `depot_api-1.0.7/README.md` & `depot_api-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -106,35 +106,47 @@
 *DefaultApi* | [**list_job_instances_job_instances_get**](docs/DefaultApi.md#list_job_instances_job_instances_get) | **GET** /job_instances/ | List Job Instances
 *DefaultApi* | [**list_providers_providers_get**](docs/DefaultApi.md#list_providers_providers_get) | **GET** /providers/ | List Providers
 *DefaultApi* | [**list_providers_types_provider_types_get**](docs/DefaultApi.md#list_providers_types_provider_types_get) | **GET** /provider_types/ | List Providers Types
 *DefaultApi* | [**list_repositories_repositories_get**](docs/DefaultApi.md#list_repositories_repositories_get) | **GET** /repositories/ | List Repositories
 *DefaultApi* | [**list_ssh_keys_ssh_keys_get**](docs/DefaultApi.md#list_ssh_keys_ssh_keys_get) | **GET** /ssh_keys/ | List Ssh Keys
 *DefaultApi* | [**login_token_post**](docs/DefaultApi.md#login_token_post) | **POST** /token | Login
 *DefaultApi* | [**read_cluster_clusters_cluster_id_get**](docs/DefaultApi.md#read_cluster_clusters_cluster_id_get) | **GET** /clusters/{cluster_id} | Read Cluster
+*DefaultApi* | [**read_job_instance_by_name_job_instances_by_name_get**](docs/DefaultApi.md#read_job_instance_by_name_job_instances_by_name_get) | **GET** /job_instances/by_name/ | Read Job Instance By Name
 *DefaultApi* | [**read_job_instance_job_instances_job_instance_id_get**](docs/DefaultApi.md#read_job_instance_job_instances_job_instance_id_get) | **GET** /job_instances/{job_instance_id} | Read Job Instance
 *DefaultApi* | [**read_log_logs_job_instance_id_get**](docs/DefaultApi.md#read_log_logs_job_instance_id_get) | **GET** /logs/{job_instance_id} | Read Log
+*DefaultApi* | [**read_provider_by_name_providers_by_name_get**](docs/DefaultApi.md#read_provider_by_name_providers_by_name_get) | **GET** /providers/by_name/ | Read Provider By Name
 *DefaultApi* | [**read_provider_providers_provider_id_get**](docs/DefaultApi.md#read_provider_providers_provider_id_get) | **GET** /providers/{provider_id} | Read Provider
+*DefaultApi* | [**read_provider_type_by_name_provider_types_by_name_get**](docs/DefaultApi.md#read_provider_type_by_name_provider_types_by_name_get) | **GET** /provider_types/by_name | Read Provider Type By Name
 *DefaultApi* | [**read_repository_by_name_repositories_by_name_get**](docs/DefaultApi.md#read_repository_by_name_repositories_by_name_get) | **GET** /repositories/by_name/ | Read Repository By Name
 *DefaultApi* | [**read_ssh_key_by_name_ssh_keys_by_name_get**](docs/DefaultApi.md#read_ssh_key_by_name_ssh_keys_by_name_get) | **GET** /ssh_keys/by_name/ | Read Ssh Key By Name
 *DefaultApi* | [**read_users_me_users_me_get**](docs/DefaultApi.md#read_users_me_users_me_get) | **GET** /users/me | Read Users Me
 *DefaultApi* | [**update_repository_repositories_by_name_patch**](docs/DefaultApi.md#update_repository_repositories_by_name_patch) | **PATCH** /repositories/by_name/ | Update Repository
 
 
 ## Documentation For Models
 
  - [ClientId](docs/ClientId.md)
  - [ClientSecret](docs/ClientSecret.md)
  - [ClusterIn](docs/ClusterIn.md)
+ - [ClusterOut](docs/ClusterOut.md)
+ - [FinishedAt](docs/FinishedAt.md)
  - [GrantType](docs/GrantType.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
  - [Id](docs/Id.md)
+ - [IdOut](docs/IdOut.md)
  - [JobInstanceIn](docs/JobInstanceIn.md)
+ - [JobInstanceOut](docs/JobInstanceOut.md)
+ - [LogOut](docs/LogOut.md)
  - [Provider](docs/Provider.md)
+ - [ProviderOut](docs/ProviderOut.md)
+ - [ProviderTypeOut](docs/ProviderTypeOut.md)
  - [RepositoryIn](docs/RepositoryIn.md)
+ - [RepositoryOut](docs/RepositoryOut.md)
  - [SshKeyIn](docs/SshKeyIn.md)
+ - [SshKeyOut](docs/SshKeyOut.md)
  - [ValidationError](docs/ValidationError.md)
  - [ValidationErrorLocInner](docs/ValidationErrorLocInner.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
```

### Comparing `depot_api-1.0.7/depot_api/api/default_api.py` & `depot_api-1.0.8/depot_api/api/default_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,27 @@
 from typing_extensions import Annotated
 
 from pydantic import StrictInt, StrictStr
 from typing import Optional
 from depot_api.models.client_id import ClientId
 from depot_api.models.client_secret import ClientSecret
 from depot_api.models.cluster_in import ClusterIn
+from depot_api.models.cluster_out import ClusterOut
 from depot_api.models.grant_type import GrantType
+from depot_api.models.id_out import IdOut
 from depot_api.models.job_instance_in import JobInstanceIn
+from depot_api.models.job_instance_out import JobInstanceOut
+from depot_api.models.log_out import LogOut
 from depot_api.models.provider import Provider
+from depot_api.models.provider_out import ProviderOut
+from depot_api.models.provider_type_out import ProviderTypeOut
 from depot_api.models.repository_in import RepositoryIn
+from depot_api.models.repository_out import RepositoryOut
 from depot_api.models.ssh_key_in import SshKeyIn
+from depot_api.models.ssh_key_out import SshKeyOut
 
 from depot_api.api_client import ApiClient, RequestSerialized
 from depot_api.api_response import ApiResponse
 from depot_api.rest import RESTResponseType
 
 
 class DefaultApi:
@@ -57,15 +65,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> IdOut:
         """Create Cluster
 
 
         :param cluster_in: (required)
         :type cluster_in: ClusterIn
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -94,15 +102,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -124,15 +132,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[IdOut]:
         """Create Cluster
 
 
         :param cluster_in: (required)
         :type cluster_in: ClusterIn
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -161,15 +169,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -228,15 +236,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -328,15 +336,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> IdOut:
         """Create Job Instance
 
 
         :param job_instance_in: (required)
         :type job_instance_in: JobInstanceIn
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -365,15 +373,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -395,15 +403,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[IdOut]:
         """Create Job Instance
 
 
         :param job_instance_in: (required)
         :type job_instance_in: JobInstanceIn
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -432,15 +440,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -499,15 +507,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -599,15 +607,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> SshKeyOut:
         """Create Managed Ssh Key
 
 
         :param service: (required)
         :type service: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -636,15 +644,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -666,15 +674,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[SshKeyOut]:
         """Create Managed Ssh Key
 
 
         :param service: (required)
         :type service: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -703,15 +711,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -770,15 +778,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -859,15 +867,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> ProviderOut:
         """Create Provider
 
 
         :param provider: (required)
         :type provider: Provider
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -896,15 +904,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ProviderOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -926,15 +934,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[ProviderOut]:
         """Create Provider
 
 
         :param provider: (required)
         :type provider: Provider
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -963,15 +971,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ProviderOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1030,15 +1038,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ProviderOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -1130,15 +1138,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> RepositoryOut:
         """Create Repository
 
 
         :param repository_in: (required)
         :type repository_in: RepositoryIn
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1167,15 +1175,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "RepositoryOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1197,15 +1205,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[RepositoryOut]:
         """Create Repository
 
 
         :param repository_in: (required)
         :type repository_in: RepositoryIn
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1234,15 +1242,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "RepositoryOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1301,15 +1309,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "RepositoryOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -1401,15 +1409,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> SshKeyOut:
         """Create Ssh Key
 
 
         :param ssh_key_in: (required)
         :type ssh_key_in: SshKeyIn
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1438,15 +1446,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1468,15 +1476,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[SshKeyOut]:
         """Create Ssh Key
 
 
         :param ssh_key_in: (required)
         :type ssh_key_in: SshKeyIn
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1505,15 +1513,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1572,15 +1580,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -1672,15 +1680,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> IdOut:
         """Delete Cluster
 
 
         :param cluster_id: (required)
         :type cluster_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1709,15 +1717,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1739,15 +1747,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[IdOut]:
         """Delete Cluster
 
 
         :param cluster_id: (required)
         :type cluster_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1776,15 +1784,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1843,15 +1851,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -1930,15 +1938,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> IdOut:
         """Delete Job Instance
 
 
         :param job_instance_id: (required)
         :type job_instance_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1967,15 +1975,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1997,15 +2005,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[IdOut]:
         """Delete Job Instance
 
 
         :param job_instance_id: (required)
         :type job_instance_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2034,15 +2042,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -2101,15 +2109,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "IdOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -2188,15 +2196,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> ProviderOut:
         """Delete Provider
 
 
         :param provider_id: (required)
         :type provider_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2225,15 +2233,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ProviderOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -2255,15 +2263,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[ProviderOut]:
         """Delete Provider
 
 
         :param provider_id: (required)
         :type provider_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2292,15 +2300,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ProviderOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -2359,15 +2367,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ProviderOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -2704,15 +2712,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> SshKeyOut:
         """Get Managed Ssh Key
 
 
         :param service: (required)
         :type service: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2741,15 +2749,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -2771,15 +2779,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[SshKeyOut]:
         """Get Managed Ssh Key
 
 
         :param service: (required)
         :type service: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2808,15 +2816,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -2875,15 +2883,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -2963,15 +2971,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> List[ClusterOut]:
         """List Clusters
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2997,15 +3005,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[ClusterOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -3025,15 +3033,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[List[ClusterOut]]:
         """List Clusters
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -3059,15 +3067,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[ClusterOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -3121,15 +3129,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[ClusterOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -3203,15 +3211,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> List[JobInstanceOut]:
         """List Job Instances
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -3237,15 +3245,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[JobInstanceOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -3265,15 +3273,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[List[JobInstanceOut]]:
         """List Job Instances
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -3299,15 +3307,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[JobInstanceOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -3361,15 +3369,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[JobInstanceOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -3443,15 +3451,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> List[ProviderOut]:
         """List Providers
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -3477,15 +3485,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[ProviderOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -3505,15 +3513,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[List[ProviderOut]]:
         """List Providers
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -3539,15 +3547,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[ProviderOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -3601,15 +3609,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[ProviderOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -3683,15 +3691,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> List[ProviderTypeOut]:
         """List Providers Types
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -3717,15 +3725,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[ProviderTypeOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -3745,15 +3753,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[List[ProviderTypeOut]]:
         """List Providers Types
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -3779,15 +3787,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[ProviderTypeOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -3841,15 +3849,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[ProviderTypeOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -3923,15 +3931,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> List[RepositoryOut]:
         """List Repositories
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -3957,15 +3965,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[RepositoryOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -3985,15 +3993,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[List[RepositoryOut]]:
         """List Repositories
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -4019,15 +4027,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[RepositoryOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -4081,15 +4089,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[RepositoryOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -4163,15 +4171,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> List[SshKeyOut]:
         """List Ssh Keys
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -4197,15 +4205,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[SshKeyOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -4225,15 +4233,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[List[SshKeyOut]]:
         """List Ssh Keys
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -4259,15 +4267,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[SshKeyOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -4321,15 +4329,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "List[SshKeyOut]",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -4749,15 +4757,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> ClusterOut:
         """Read Cluster
 
 
         :param cluster_id: (required)
         :type cluster_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -4786,15 +4794,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ClusterOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -4816,15 +4824,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[ClusterOut]:
         """Read Cluster
 
 
         :param cluster_id: (required)
         :type cluster_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -4853,15 +4861,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ClusterOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -4920,15 +4928,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ClusterOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -4992,14 +5000,291 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def read_job_instance_by_name_job_instances_by_name_get(
+        self,
+        repository_url: StrictStr,
+        job_instance_name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> JobInstanceOut:
+        """Read Job Instance By Name
+
+
+        :param repository_url: (required)
+        :type repository_url: str
+        :param job_instance_name: (required)
+        :type job_instance_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_job_instance_by_name_job_instances_by_name_get_serialize(
+            repository_url=repository_url,
+            job_instance_name=job_instance_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "JobInstanceOut",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def read_job_instance_by_name_job_instances_by_name_get_with_http_info(
+        self,
+        repository_url: StrictStr,
+        job_instance_name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[JobInstanceOut]:
+        """Read Job Instance By Name
+
+
+        :param repository_url: (required)
+        :type repository_url: str
+        :param job_instance_name: (required)
+        :type job_instance_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_job_instance_by_name_job_instances_by_name_get_serialize(
+            repository_url=repository_url,
+            job_instance_name=job_instance_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "JobInstanceOut",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def read_job_instance_by_name_job_instances_by_name_get_without_preload_content(
+        self,
+        repository_url: StrictStr,
+        job_instance_name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Read Job Instance By Name
+
+
+        :param repository_url: (required)
+        :type repository_url: str
+        :param job_instance_name: (required)
+        :type job_instance_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_job_instance_by_name_job_instances_by_name_get_serialize(
+            repository_url=repository_url,
+            job_instance_name=job_instance_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "JobInstanceOut",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _read_job_instance_by_name_job_instances_by_name_get_serialize(
+        self,
+        repository_url,
+        job_instance_name,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if repository_url is not None:
+            
+            _query_params.append(('repository_url', repository_url))
+            
+        if job_instance_name is not None:
+            
+            _query_params.append(('job_instance_name', job_instance_name))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/job_instances/by_name/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def read_job_instance_job_instances_job_instance_id_get(
         self,
         job_instance_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -5007,15 +5292,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> JobInstanceOut:
         """Read Job Instance
 
 
         :param job_instance_id: (required)
         :type job_instance_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -5044,15 +5329,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "JobInstanceOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -5074,15 +5359,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[JobInstanceOut]:
         """Read Job Instance
 
 
         :param job_instance_id: (required)
         :type job_instance_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -5111,15 +5396,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "JobInstanceOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -5178,15 +5463,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "JobInstanceOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -5265,15 +5550,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> LogOut:
         """Read Log
 
 
         :param job_instance_id: (required)
         :type job_instance_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -5302,15 +5587,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "LogOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -5332,15 +5617,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[LogOut]:
         """Read Log
 
 
         :param job_instance_id: (required)
         :type job_instance_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -5369,15 +5654,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "LogOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -5436,15 +5721,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "LogOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -5508,14 +5793,274 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def read_provider_by_name_providers_by_name_get(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ProviderOut:
+        """Read Provider By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_provider_by_name_providers_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ProviderOut",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def read_provider_by_name_providers_by_name_get_with_http_info(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[ProviderOut]:
+        """Read Provider By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_provider_by_name_providers_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ProviderOut",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def read_provider_by_name_providers_by_name_get_without_preload_content(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Read Provider By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_provider_by_name_providers_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ProviderOut",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _read_provider_by_name_providers_by_name_get_serialize(
+        self,
+        name,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if name is not None:
+            
+            _query_params.append(('name', name))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/providers/by_name/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def read_provider_providers_provider_id_get(
         self,
         provider_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -5523,15 +6068,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> ProviderOut:
         """Read Provider
 
 
         :param provider_id: (required)
         :type provider_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -5560,15 +6105,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ProviderOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -5590,15 +6135,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[ProviderOut]:
         """Read Provider
 
 
         :param provider_id: (required)
         :type provider_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -5627,15 +6172,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ProviderOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -5694,15 +6239,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "ProviderOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -5766,14 +6311,274 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def read_provider_type_by_name_provider_types_by_name_get(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ProviderTypeOut:
+        """Read Provider Type By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_provider_type_by_name_provider_types_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ProviderTypeOut",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def read_provider_type_by_name_provider_types_by_name_get_with_http_info(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[ProviderTypeOut]:
+        """Read Provider Type By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_provider_type_by_name_provider_types_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ProviderTypeOut",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def read_provider_type_by_name_provider_types_by_name_get_without_preload_content(
+        self,
+        name: StrictStr,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Read Provider Type By Name
+
+
+        :param name: (required)
+        :type name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._read_provider_type_by_name_provider_types_by_name_get_serialize(
+            name=name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ProviderTypeOut",
+            '422': "HTTPValidationError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _read_provider_type_by_name_provider_types_by_name_get_serialize(
+        self,
+        name,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if name is not None:
+            
+            _query_params.append(('name', name))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/provider_types/by_name',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def read_repository_by_name_repositories_by_name_get(
         self,
         name: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -5781,15 +6586,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> RepositoryOut:
         """Read Repository By Name
 
 
         :param name: (required)
         :type name: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -5818,15 +6623,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "RepositoryOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -5848,15 +6653,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[RepositoryOut]:
         """Read Repository By Name
 
 
         :param name: (required)
         :type name: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -5885,15 +6690,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "RepositoryOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -5952,15 +6757,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "RepositoryOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -6041,15 +6846,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> SshKeyOut:
         """Read Ssh Key By Name
 
 
         :param name: (required)
         :type name: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -6078,15 +6883,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -6108,15 +6913,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[SshKeyOut]:
         """Read Ssh Key By Name
 
 
         :param name: (required)
         :type name: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -6145,15 +6950,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -6212,15 +7017,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "SshKeyOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -6542,15 +7347,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
+    ) -> RepositoryOut:
         """Update Repository
 
 
         :param repository_url: (required)
         :type repository_url: str
         :param ssh_key_name: (required)
         :type ssh_key_name: str
@@ -6582,15 +7387,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "RepositoryOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -6613,15 +7418,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
+    ) -> ApiResponse[RepositoryOut]:
         """Update Repository
 
 
         :param repository_url: (required)
         :type repository_url: str
         :param ssh_key_name: (required)
         :type ssh_key_name: str
@@ -6653,15 +7458,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "RepositoryOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -6724,15 +7529,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "RepositoryOut",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `depot_api-1.0.7/depot_api/api_client.py` & `depot_api-1.0.8/depot_api/api_client.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/api_response.py` & `depot_api-1.0.8/depot_api/api_response.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/configuration.py` & `depot_api-1.0.8/depot_api/configuration.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/exceptions.py` & `depot_api-1.0.8/depot_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/client_id.py` & `depot_api-1.0.8/depot_api/models/client_id.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/client_secret.py` & `depot_api-1.0.8/depot_api/models/client_secret.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/cluster.py` & `depot_api-1.0.8/depot_api/models/cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,17 @@
     """
     Cluster
     """ # noqa: E501
     id: Optional[Id] = None
     name: StrictStr
     credentials: StrictStr
     userlogin: StrictStr
+    nodes: List[StrictStr]
     provider_id: Optional[StrictInt] = None
-    __properties: ClassVar[List[str]] = ["id", "name", "credentials", "userlogin", "provider_id"]
+    __properties: ClassVar[List[str]] = ["id", "name", "credentials", "userlogin", "nodes", "provider_id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -88,12 +89,13 @@
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": Id.from_dict(obj["id"]) if obj.get("id") is not None else None,
             "name": obj.get("name"),
             "credentials": obj.get("credentials"),
             "userlogin": obj.get("userlogin"),
+            "nodes": obj.get("nodes"),
             "provider_id": obj.get("provider_id")
         })
         return _obj
```

### Comparing `depot_api-1.0.7/depot_api/models/cluster_in.py` & `depot_api-1.0.8/depot_api/models/cluster_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/grant_type.py` & `depot_api-1.0.8/depot_api/models/grant_type.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/http_validation_error.py` & `depot_api-1.0.8/depot_api/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/id.py` & `depot_api-1.0.8/depot_api/models/id.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/job_instance.py` & `depot_api-1.0.8/depot_api/models/job_instance.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/job_instance_in.py` & `depot_api-1.0.8/depot_api/models/job_instance_in.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
 class JobInstanceIn(BaseModel):
     """
     JobInstanceIn
     """ # noqa: E501
     name: StrictStr
     job_name: StrictStr
     repository_url: StrictStr
     starting_commit: StrictStr
-    cluster_id: StrictInt
+    cluster: StrictStr
     userlogin: StrictStr
-    __properties: ClassVar[List[str]] = ["name", "job_name", "repository_url", "starting_commit", "cluster_id", "userlogin"]
+    __properties: ClassVar[List[str]] = ["name", "job_name", "repository_url", "starting_commit", "cluster", "userlogin"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -85,13 +85,13 @@
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
             "job_name": obj.get("job_name"),
             "repository_url": obj.get("repository_url"),
             "starting_commit": obj.get("starting_commit"),
-            "cluster_id": obj.get("cluster_id"),
+            "cluster": obj.get("cluster"),
             "userlogin": obj.get("userlogin")
         })
         return _obj
```

### Comparing `depot_api-1.0.7/depot_api/models/private_key.py` & `depot_api-1.0.8/depot_api/models/private_key.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/provider.py` & `depot_api-1.0.8/depot_api/models/provider.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/public_key.py` & `depot_api-1.0.8/depot_api/models/public_key.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/repository.py` & `depot_api-1.0.8/depot_api/models/repository.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/repository_in.py` & `depot_api-1.0.8/depot_api/models/repository_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/repository_key.py` & `depot_api-1.0.8/depot_api/models/repository_key.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/repository_out.py` & `depot_api-1.0.8/depot_api/models/ssh_key_in.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,29 +13,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from depot_api.models.job_instance import JobInstance
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RepositoryOut(BaseModel):
+class SshKeyIn(BaseModel):
     """
-    RepositoryOut
+    SshKeyIn
     """ # noqa: E501
-    id: StrictInt
-    url: StrictStr
+    name: StrictStr
     userlogin: StrictStr
-    job_instances: List[JobInstance]
-    __properties: ClassVar[List[str]] = ["id", "url", "userlogin", "job_instances"]
+    public_key: StrictStr
+    private_key: StrictStr
+    __properties: ClassVar[List[str]] = ["name", "userlogin", "public_key", "private_key"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RepositoryOut from a JSON string"""
+        """Create an instance of SshKeyIn from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,34 +67,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in job_instances (list)
-        _items = []
-        if self.job_instances:
-            for _item in self.job_instances:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['job_instances'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RepositoryOut from a dict"""
+        """Create an instance of SshKeyIn from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "url": obj.get("url"),
+            "name": obj.get("name"),
             "userlogin": obj.get("userlogin"),
-            "job_instances": [JobInstance.from_dict(_item) for _item in obj["job_instances"]] if obj.get("job_instances") is not None else None
+            "public_key": obj.get("public_key"),
+            "private_key": obj.get("private_key")
         })
         return _obj
```

### Comparing `depot_api-1.0.7/depot_api/models/ssh_key_in.py` & `depot_api-1.0.8/depot_api/models/provider_type_out.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,28 +13,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SshKeyIn(BaseModel):
+class ProviderTypeOut(BaseModel):
     """
-    SshKeyIn
+    ProviderTypeOut
     """ # noqa: E501
+    id: StrictInt
     name: StrictStr
-    userlogin: StrictStr
-    public_key: StrictStr
-    private_key: StrictStr
-    __properties: ClassVar[List[str]] = ["name", "userlogin", "public_key", "private_key"]
+    module: StrictStr
+    __properties: ClassVar[List[str]] = ["id", "name", "module"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SshKeyIn from a JSON string"""
+        """Create an instance of ProviderTypeOut from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,23 +70,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SshKeyIn from a dict"""
+        """Create an instance of ProviderTypeOut from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
-            "userlogin": obj.get("userlogin"),
-            "public_key": obj.get("public_key"),
-            "private_key": obj.get("private_key")
+            "module": obj.get("module")
         })
         return _obj
```

### Comparing `depot_api-1.0.7/depot_api/models/validation_error.py` & `depot_api-1.0.8/depot_api/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/models/validation_error_loc_inner.py` & `depot_api-1.0.8/depot_api/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/depot_api/rest.py` & `depot_api-1.0.8/depot_api/rest.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/pyproject.toml` & `depot_api-1.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -56,30 +56,29 @@
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 authors = [
     { name = "OpenAPI Generator Community", email = "team@openapitools.org" },
-    { name = "OpenAPI Generator community", email = "team@openapitools.org" },
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 requires-python = "<4.0,>=3.7"
 dependencies = [
     "urllib3>=1.25.3",
     "python-dateutil>=2.8.2",
     "pydantic>=2",
     "typing-extensions>=4.7.1",
     "pydantic >= 2",
     "python-dateutil",
     "typing-extensions >= 4.7.1",
     "urllib3 >= 1.25.3, < 2.1.0",
 ]
 name = "depot-api"
-version = "1.0.7"
+version = "1.0.8"
 description = "Depot API"
 readme = "README.md"
 keywords = [
     "OpenAPI",
     "OpenAPI-Generator",
     "FastAPI",
 ]
```

### Comparing `depot_api-1.0.7/test/test_client_id.py` & `depot_api-1.0.8/test/test_client_id.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_client_secret.py` & `depot_api-1.0.8/test/test_client_secret.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_cluster.py` & `depot_api-1.0.8/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_cluster_in.py` & `depot_api-1.0.8/test/test_cluster_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_default_api.py` & `depot_api-1.0.8/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_grant_type.py` & `depot_api-1.0.8/test/test_grant_type.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_http_validation_error.py` & `depot_api-1.0.8/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_id.py` & `depot_api-1.0.8/test/test_id.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_job_instance.py` & `depot_api-1.0.8/test/test_job_instance.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_job_instance_in.py` & `depot_api-1.0.8/test/test_job_instance_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_private_key.py` & `depot_api-1.0.8/test/test_private_key.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_provider.py` & `depot_api-1.0.8/test/test_provider.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_public_key.py` & `depot_api-1.0.8/test/test_public_key.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_repository.py` & `depot_api-1.0.8/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_repository_in.py` & `depot_api-1.0.8/test/test_repository_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_repository_key.py` & `depot_api-1.0.8/test/test_repository_key.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_repository_out.py` & `depot_api-1.0.8/test/test_repository_out.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_ssh_key_in.py` & `depot_api-1.0.8/test/test_ssh_key_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_validation_error.py` & `depot_api-1.0.8/test/test_validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/test/test_validation_error_loc_inner.py` & `depot_api-1.0.8/test/test_validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.7/PKG-INFO` & `depot_api-1.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: depot-api
-Version: 1.0.7
+Version: 1.0.8
 Summary: Depot API
 Keywords: OpenAPI,OpenAPI-Generator,FastAPI
-Author-Email: OpenAPI Generator Community <team@openapitools.org>, OpenAPI Generator community <team@openapitools.org>, CodeDepot <contact@codedepot.ai>
+Author-Email: OpenAPI Generator Community <team@openapitools.org>, CodeDepot <contact@codedepot.ai>
 License: NoLicense
 Project-URL: Repository, https://github.com/GIT_USER_ID/GIT_REPO_ID
 Project-URL: Homepage, https://codedepot.ai
 Requires-Python: <4.0,>=3.7
 Requires-Dist: urllib3>=1.25.3
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: pydantic>=2
@@ -126,35 +126,47 @@
 *DefaultApi* | [**list_job_instances_job_instances_get**](docs/DefaultApi.md#list_job_instances_job_instances_get) | **GET** /job_instances/ | List Job Instances
 *DefaultApi* | [**list_providers_providers_get**](docs/DefaultApi.md#list_providers_providers_get) | **GET** /providers/ | List Providers
 *DefaultApi* | [**list_providers_types_provider_types_get**](docs/DefaultApi.md#list_providers_types_provider_types_get) | **GET** /provider_types/ | List Providers Types
 *DefaultApi* | [**list_repositories_repositories_get**](docs/DefaultApi.md#list_repositories_repositories_get) | **GET** /repositories/ | List Repositories
 *DefaultApi* | [**list_ssh_keys_ssh_keys_get**](docs/DefaultApi.md#list_ssh_keys_ssh_keys_get) | **GET** /ssh_keys/ | List Ssh Keys
 *DefaultApi* | [**login_token_post**](docs/DefaultApi.md#login_token_post) | **POST** /token | Login
 *DefaultApi* | [**read_cluster_clusters_cluster_id_get**](docs/DefaultApi.md#read_cluster_clusters_cluster_id_get) | **GET** /clusters/{cluster_id} | Read Cluster
+*DefaultApi* | [**read_job_instance_by_name_job_instances_by_name_get**](docs/DefaultApi.md#read_job_instance_by_name_job_instances_by_name_get) | **GET** /job_instances/by_name/ | Read Job Instance By Name
 *DefaultApi* | [**read_job_instance_job_instances_job_instance_id_get**](docs/DefaultApi.md#read_job_instance_job_instances_job_instance_id_get) | **GET** /job_instances/{job_instance_id} | Read Job Instance
 *DefaultApi* | [**read_log_logs_job_instance_id_get**](docs/DefaultApi.md#read_log_logs_job_instance_id_get) | **GET** /logs/{job_instance_id} | Read Log
+*DefaultApi* | [**read_provider_by_name_providers_by_name_get**](docs/DefaultApi.md#read_provider_by_name_providers_by_name_get) | **GET** /providers/by_name/ | Read Provider By Name
 *DefaultApi* | [**read_provider_providers_provider_id_get**](docs/DefaultApi.md#read_provider_providers_provider_id_get) | **GET** /providers/{provider_id} | Read Provider
+*DefaultApi* | [**read_provider_type_by_name_provider_types_by_name_get**](docs/DefaultApi.md#read_provider_type_by_name_provider_types_by_name_get) | **GET** /provider_types/by_name | Read Provider Type By Name
 *DefaultApi* | [**read_repository_by_name_repositories_by_name_get**](docs/DefaultApi.md#read_repository_by_name_repositories_by_name_get) | **GET** /repositories/by_name/ | Read Repository By Name
 *DefaultApi* | [**read_ssh_key_by_name_ssh_keys_by_name_get**](docs/DefaultApi.md#read_ssh_key_by_name_ssh_keys_by_name_get) | **GET** /ssh_keys/by_name/ | Read Ssh Key By Name
 *DefaultApi* | [**read_users_me_users_me_get**](docs/DefaultApi.md#read_users_me_users_me_get) | **GET** /users/me | Read Users Me
 *DefaultApi* | [**update_repository_repositories_by_name_patch**](docs/DefaultApi.md#update_repository_repositories_by_name_patch) | **PATCH** /repositories/by_name/ | Update Repository
 
 
 ## Documentation For Models
 
  - [ClientId](docs/ClientId.md)
  - [ClientSecret](docs/ClientSecret.md)
  - [ClusterIn](docs/ClusterIn.md)
+ - [ClusterOut](docs/ClusterOut.md)
+ - [FinishedAt](docs/FinishedAt.md)
  - [GrantType](docs/GrantType.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
  - [Id](docs/Id.md)
+ - [IdOut](docs/IdOut.md)
  - [JobInstanceIn](docs/JobInstanceIn.md)
+ - [JobInstanceOut](docs/JobInstanceOut.md)
+ - [LogOut](docs/LogOut.md)
  - [Provider](docs/Provider.md)
+ - [ProviderOut](docs/ProviderOut.md)
+ - [ProviderTypeOut](docs/ProviderTypeOut.md)
  - [RepositoryIn](docs/RepositoryIn.md)
+ - [RepositoryOut](docs/RepositoryOut.md)
  - [SshKeyIn](docs/SshKeyIn.md)
+ - [SshKeyOut](docs/SshKeyOut.md)
  - [ValidationError](docs/ValidationError.md)
  - [ValidationErrorLocInner](docs/ValidationErrorLocInner.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
```

