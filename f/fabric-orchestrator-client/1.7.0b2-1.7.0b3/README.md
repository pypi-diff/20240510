# Comparing `tmp/fabric-orchestrator-client-1.7.0b2.tar.gz` & `tmp/fabric-orchestrator-client-1.7.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-orchestrator-client-1.7.0b2.tar", last modified: Tue May  7 21:30:34 2024, max compression
+gzip compressed data, was "fabric-orchestrator-client-1.7.0b3.tar", last modified: Fri May 10 08:43:09 2024, max compression
```

## Comparing `fabric-orchestrator-client-1.7.0b2.tar` & `fabric-orchestrator-client-1.7.0b3.tar`

### file list

```diff
@@ -1,103 +1,110 @@
--rw-r--r--   0        0        0      793 2024-01-12 03:42:46.101822 fabric-orchestrator-client-1.7.0b2/.gitignore
--rw-r--r--   0        0        0     1030 2024-01-12 03:42:46.102099 fabric-orchestrator-client-1.7.0b2/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2024-04-05 22:19:27.031216 fabric-orchestrator-client-1.7.0b2/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2024-01-12 03:42:46.102462 fabric-orchestrator-client-1.7.0b2/.travis.yml
--rw-r--r--   0        0        0      770 2024-01-12 03:42:46.103447 fabric-orchestrator-client-1.7.0b2/CODEGEN.md
--rw-r--r--   0        0        0     1071 2024-01-12 03:42:46.103789 fabric-orchestrator-client-1.7.0b2/LICENSE
--rw-r--r--   0        0        0       59 2024-01-12 03:42:46.103927 fabric-orchestrator-client-1.7.0b2/MANIFEST.in
--rw-r--r--   0        0        0    10034 2024-04-05 22:21:50.264153 fabric-orchestrator-client-1.7.0b2/README.md
--rw-r--r--   0        0        0      340 2024-01-12 03:42:46.104503 fabric-orchestrator-client-1.7.0b2/docs/Poa.md
--rw-r--r--   0        0        0      557 2024-01-12 03:42:46.104673 fabric-orchestrator-client-1.7.0b2/docs/PoaData.md
--rw-r--r--   0        0        0      376 2024-01-12 03:42:46.104783 fabric-orchestrator-client-1.7.0b2/docs/PoaPost.md
--rw-r--r--   0        0        0      506 2024-01-12 03:42:46.104909 fabric-orchestrator-client-1.7.0b2/docs/PoaPostData.md
--rw-r--r--   0        0        0      344 2024-01-12 03:42:46.105043 fabric-orchestrator-client-1.7.0b2/docs/PoaPostDataKeys.md
--rw-r--r--   0        0        0      347 2024-01-12 03:42:46.105181 fabric-orchestrator-client-1.7.0b2/docs/PoaPostDataVcpuCpuMap.md
--rw-r--r--   0        0        0     6404 2024-01-12 03:42:46.105378 fabric-orchestrator-client-1.7.0b2/docs/PoasApi.md
--rw-r--r--   0        0        0     6399 2024-04-17 02:23:54.719199 fabric-orchestrator-client-1.7.0b2/docs/ResourcesApi.md
--rw-r--r--   0        0        0    21291 2024-04-17 15:13:57.283895 fabric-orchestrator-client-1.7.0b2/docs/SlicesApi.md
--rw-r--r--   0        0        0     4102 2024-01-12 03:42:46.105832 fabric-orchestrator-client-1.7.0b2/docs/SliversApi.md
--rw-r--r--   0        0        0      335 2024-01-12 03:42:46.105947 fabric-orchestrator-client-1.7.0b2/docs/Success.md
--rw-r--r--   0        0        0      352 2024-01-12 03:42:46.106047 fabric-orchestrator-client-1.7.0b2/docs/Version.md
--rw-r--r--   0        0        0       24 2024-04-17 15:18:33.120939 fabric-orchestrator-client-1.7.0b2/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2024-01-12 03:42:46.106357 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0    23598 2024-05-07 21:26:43.695878 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/orchestrator_proxy.py
--rw-r--r--   0        0        0     3649 2024-01-12 03:42:46.106764 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/__init__.py
--rw-r--r--   0        0        0      468 2024-01-12 03:42:46.106916 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/__init__.py
--rw-r--r--   0        0        0    13557 2024-01-12 03:42:46.107141 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/poas_api.py
--rw-r--r--   0        0        0    12556 2024-04-17 02:23:07.530313 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/resources_api.py
--rw-r--r--   0        0        0    45209 2024-04-17 15:16:58.826551 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/slices_api.py
--rw-r--r--   0        0        0     9260 2024-01-12 03:42:46.107691 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
--rw-r--r--   0        0        0     3748 2024-01-12 03:42:46.107811 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25272 2024-01-12 03:42:46.107971 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api_client.py
--rw-r--r--   0        0        0     8240 2024-01-12 03:42:46.108170 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/configuration.py
--rw-r--r--   0        0        0     3070 2024-04-05 22:28:49.311561 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     3427 2024-01-12 03:42:46.108447 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa.py
--rw-r--r--   0        0        0     6654 2024-01-12 03:42:46.108554 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_data.py
--rw-r--r--   0        0        0     4057 2024-01-12 03:42:46.108900 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post.py
--rw-r--r--   0        0        0     4505 2024-01-12 03:42:46.109052 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
--rw-r--r--   0        0        0     3804 2024-01-12 03:42:46.109164 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py
--rw-r--r--   0        0        0     3813 2024-01-12 03:42:46.109262 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     3055 2024-01-12 03:42:46.109386 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/resource.py
--rw-r--r--   0        0        0     3420 2024-01-12 03:42:46.109491 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/resources.py
--rw-r--r--   0        0        0     9914 2024-04-05 22:29:14.527230 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slice.py
--rw-r--r--   0        0        0     3444 2024-01-12 03:42:46.109991 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slice_details.py
--rw-r--r--   0        0        0     3412 2024-01-12 03:42:46.110167 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slices.py
--rw-r--r--   0        0        0     3951 2024-01-12 03:42:46.110282 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slices_post.py
--rw-r--r--   0        0        0    12331 2024-04-05 22:29:46.008920 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/sliver.py
--rw-r--r--   0        0        0     3422 2024-01-12 03:42:46.110560 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slivers.py
--rw-r--r--   0        0        0     4999 2024-01-12 03:42:46.110692 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3832 2024-01-12 03:42:46.110803 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     6211 2024-01-12 03:42:46.110942 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     4253 2024-01-12 03:42:46.111050 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3163 2024-01-12 03:42:46.111145 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5771 2024-01-12 03:42:46.111249 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5063 2024-01-12 03:42:46.111344 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3870 2024-01-12 03:42:46.111451 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     4994 2024-01-12 03:42:46.111569 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3831 2024-01-12 03:42:46.111663 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4971 2024-01-12 03:42:46.111759 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3819 2024-01-12 03:42:46.111853 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5224 2024-01-12 03:42:46.111956 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3963 2024-01-12 03:42:46.112233 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3413 2024-01-12 03:42:46.112337 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/version.py
--rw-r--r--   0        0        0     3882 2024-01-12 03:42:46.112446 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    12985 2024-04-05 22:30:18.293171 fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2024-01-12 03:42:46.112753 fabric-orchestrator-client-1.7.0b2/git_push.sh
--rw-r--r--   0        0        0     1024 2024-04-05 22:18:00.458232 fabric-orchestrator-client-1.7.0b2/pyproject.toml
--rw-r--r--   0        0        0       16 2024-01-12 03:42:46.112995 fabric-orchestrator-client-1.7.0b2/test/__init__.py
--rw-r--r--   0        0        0      809 2024-01-12 03:42:46.113118 fabric-orchestrator-client-1.7.0b2/test/test_poa.py
--rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113207 fabric-orchestrator-client-1.7.0b2/test/test_poa_data.py
--rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113308 fabric-orchestrator-client-1.7.0b2/test/test_poa_post.py
--rw-r--r--   0        0        0      877 2024-01-12 03:42:46.113402 fabric-orchestrator-client-1.7.0b2/test/test_poa_post_data.py
--rw-r--r--   0        0        0      963 2024-01-12 03:42:46.113498 fabric-orchestrator-client-1.7.0b2/test/test_poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     1157 2024-01-12 03:42:46.113583 fabric-orchestrator-client-1.7.0b2/test/test_poas_api.py
--rw-r--r--   0        0        0      896 2024-01-12 03:42:46.113672 fabric-orchestrator-client-1.7.0b2/test/test_resource.py
--rw-r--r--   0        0        0      950 2024-01-12 03:42:46.113770 fabric-orchestrator-client-1.7.0b2/test/test_resources.py
--rw-r--r--   0        0        0     1206 2024-01-12 03:42:46.113870 fabric-orchestrator-client-1.7.0b2/test/test_resources_api.py
--rw-r--r--   0        0        0      872 2024-01-12 03:42:46.113959 fabric-orchestrator-client-1.7.0b2/test/test_slice.py
--rw-r--r--   0        0        0      930 2024-01-12 03:42:46.114058 fabric-orchestrator-client-1.7.0b2/test/test_slice_details.py
--rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114249 fabric-orchestrator-client-1.7.0b2/test/test_slices.py
--rw-r--r--   0        0        0     2165 2024-01-12 03:42:46.114383 fabric-orchestrator-client-1.7.0b2/test/test_slices_api.py
--rw-r--r--   0        0        0      867 2024-01-12 03:42:46.114477 fabric-orchestrator-client-1.7.0b2/test/test_slices_post.py
--rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114575 fabric-orchestrator-client-1.7.0b2/test/test_sliver.py
--rw-r--r--   0        0        0      888 2024-01-12 03:42:46.114670 fabric-orchestrator-client-1.7.0b2/test/test_slivers.py
--rw-r--r--   0        0        0      974 2024-01-12 03:42:46.114770 fabric-orchestrator-client-1.7.0b2/test/test_slivers_api.py
--rw-r--r--   0        0        0      998 2024-01-12 03:42:46.114861 fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1032 2024-01-12 03:42:46.114968 fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      996 2024-01-12 03:42:46.115068 fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_paginated.py
--rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115159 fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      988 2024-01-12 03:42:46.115251 fabric-orchestrator-client-1.7.0b2/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1038 2024-01-12 03:42:46.115351 fabric-orchestrator-client-1.7.0b2/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0     1002 2024-01-12 03:42:46.115454 fabric-orchestrator-client-1.7.0b2/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1052 2024-01-12 03:42:46.115553 fabric-orchestrator-client-1.7.0b2/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      978 2024-01-12 03:42:46.115643 fabric-orchestrator-client-1.7.0b2/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1028 2024-01-12 03:42:46.115743 fabric-orchestrator-client-1.7.0b2/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115834 fabric-orchestrator-client-1.7.0b2/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1022 2024-01-12 03:42:46.115939 fabric-orchestrator-client-1.7.0b2/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1062 2024-01-12 03:42:46.116047 fabric-orchestrator-client-1.7.0b2/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1112 2024-01-12 03:42:46.116160 fabric-orchestrator-client-1.7.0b2/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      888 2024-01-12 03:42:46.116255 fabric-orchestrator-client-1.7.0b2/test/test_version.py
--rw-r--r--   0        0        0      814 2024-01-12 03:42:46.116365 fabric-orchestrator-client-1.7.0b2/test/test_version_api.py
--rw-r--r--   0        0        0      922 2024-01-12 03:42:46.116524 fabric-orchestrator-client-1.7.0b2/test/test_version_data.py
--rw-r--r--   0        0        0      143 2024-01-12 03:42:46.116674 fabric-orchestrator-client-1.7.0b2/tox.ini
--rw-r--r--   0        0        0    10985 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.7.0b2/PKG-INFO
+-rw-r--r--   0        0        0      793 2024-01-12 03:42:46.101822 fabric-orchestrator-client-1.7.0b3/.gitignore
+-rw-r--r--   0        0        0     1030 2024-01-12 03:42:46.102099 fabric-orchestrator-client-1.7.0b3/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2024-04-05 22:19:27.031216 fabric-orchestrator-client-1.7.0b3/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2024-01-12 03:42:46.102462 fabric-orchestrator-client-1.7.0b3/.travis.yml
+-rw-r--r--   0        0        0      770 2024-01-12 03:42:46.103447 fabric-orchestrator-client-1.7.0b3/CODEGEN.md
+-rw-r--r--   0        0        0     1071 2024-01-12 03:42:46.103789 fabric-orchestrator-client-1.7.0b3/LICENSE
+-rw-r--r--   0        0        0       59 2024-01-12 03:42:46.103927 fabric-orchestrator-client-1.7.0b3/MANIFEST.in
+-rw-r--r--   0        0        0    10034 2024-04-05 22:21:50.264153 fabric-orchestrator-client-1.7.0b3/README.md
+-rw-r--r--   0        0        0      332 2024-05-10 08:06:45.794386 fabric-orchestrator-client-1.7.0b3/docs/Metrics.md
+-rw-r--r--   0        0        0     1704 2024-05-10 08:06:45.794972 fabric-orchestrator-client-1.7.0b3/docs/MetricsApi.md
+-rw-r--r--   0        0        0      340 2024-01-12 03:42:46.104503 fabric-orchestrator-client-1.7.0b3/docs/Poa.md
+-rw-r--r--   0        0        0      557 2024-01-12 03:42:46.104673 fabric-orchestrator-client-1.7.0b3/docs/PoaData.md
+-rw-r--r--   0        0        0      376 2024-01-12 03:42:46.104783 fabric-orchestrator-client-1.7.0b3/docs/PoaPost.md
+-rw-r--r--   0        0        0      506 2024-01-12 03:42:46.104909 fabric-orchestrator-client-1.7.0b3/docs/PoaPostData.md
+-rw-r--r--   0        0        0      344 2024-01-12 03:42:46.105043 fabric-orchestrator-client-1.7.0b3/docs/PoaPostDataKeys.md
+-rw-r--r--   0        0        0      347 2024-01-12 03:42:46.105181 fabric-orchestrator-client-1.7.0b3/docs/PoaPostDataVcpuCpuMap.md
+-rw-r--r--   0        0        0     6404 2024-01-12 03:42:46.105378 fabric-orchestrator-client-1.7.0b3/docs/PoasApi.md
+-rw-r--r--   0        0        0     6399 2024-04-17 02:23:54.719199 fabric-orchestrator-client-1.7.0b3/docs/ResourcesApi.md
+-rw-r--r--   0        0        0    21291 2024-04-17 15:13:57.283895 fabric-orchestrator-client-1.7.0b3/docs/SlicesApi.md
+-rw-r--r--   0        0        0     4102 2024-01-12 03:42:46.105832 fabric-orchestrator-client-1.7.0b3/docs/SliversApi.md
+-rw-r--r--   0        0        0      335 2024-01-12 03:42:46.105947 fabric-orchestrator-client-1.7.0b3/docs/Success.md
+-rw-r--r--   0        0        0      352 2024-01-12 03:42:46.106047 fabric-orchestrator-client-1.7.0b3/docs/Version.md
+-rw-r--r--   0        0        0     6148 2024-05-10 08:08:19.553614 fabric-orchestrator-client-1.7.0b3/fabric_cf/.DS_Store
+-rw-r--r--   0        0        0       24 2024-05-10 08:21:40.332775 fabric-orchestrator-client-1.7.0b3/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-12 03:42:46.106357 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0    24373 2024-05-10 08:42:11.302019 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/orchestrator_proxy.py
+-rw-r--r--   0        0        0     3799 2024-05-10 08:09:51.937758 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/__init__.py
+-rw-r--r--   0        0        0      545 2024-05-10 08:09:51.932097 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0     4445 2024-05-10 08:21:30.675181 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/metrics_api.py
+-rw-r--r--   0        0        0    13557 2024-01-12 03:42:46.107141 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/poas_api.py
+-rw-r--r--   0        0        0    12556 2024-04-17 02:23:07.530313 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/resources_api.py
+-rw-r--r--   0        0        0    45209 2024-04-17 15:16:58.826551 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/slices_api.py
+-rw-r--r--   0        0        0     9260 2024-01-12 03:42:46.107691 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
+-rw-r--r--   0        0        0     3748 2024-01-12 03:42:46.107811 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25272 2024-01-12 03:42:46.107971 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8240 2024-01-12 03:42:46.108170 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/configuration.py
+-rw-r--r--   0        0        0     3070 2024-04-05 22:28:49.311561 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     3459 2024-05-10 08:12:50.816882 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/metrics.py
+-rw-r--r--   0        0        0     3369 2024-05-10 08:13:24.762105 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa.py
+-rw-r--r--   0        0        0     6654 2024-01-12 03:42:46.108554 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa_data.py
+-rw-r--r--   0        0        0     4057 2024-01-12 03:42:46.108900 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post.py
+-rw-r--r--   0        0        0     4505 2024-01-12 03:42:46.109052 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
+-rw-r--r--   0        0        0     3804 2024-01-12 03:42:46.109164 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py
+-rw-r--r--   0        0        0     3813 2024-01-12 03:42:46.109262 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     3055 2024-01-12 03:42:46.109386 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/resource.py
+-rw-r--r--   0        0        0     3420 2024-01-12 03:42:46.109491 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/resources.py
+-rw-r--r--   0        0        0     9914 2024-04-05 22:29:14.527230 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/slice.py
+-rw-r--r--   0        0        0     3435 2024-05-10 08:14:02.157712 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/slice_details.py
+-rw-r--r--   0        0        0     3412 2024-01-12 03:42:46.110167 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/slices.py
+-rw-r--r--   0        0        0     3951 2024-01-12 03:42:46.110282 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/slices_post.py
+-rw-r--r--   0        0        0    12331 2024-04-05 22:29:46.008920 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/sliver.py
+-rw-r--r--   0        0        0     3422 2024-01-12 03:42:46.110560 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/slivers.py
+-rw-r--r--   0        0        0     4999 2024-01-12 03:42:46.110692 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3832 2024-01-12 03:42:46.110803 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     6211 2024-01-12 03:42:46.110942 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4253 2024-01-12 03:42:46.111050 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3163 2024-01-12 03:42:46.111145 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5771 2024-01-12 03:42:46.111249 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5063 2024-01-12 03:42:46.111344 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3870 2024-01-12 03:42:46.111451 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     4994 2024-01-12 03:42:46.111569 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3831 2024-01-12 03:42:46.111663 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4971 2024-01-12 03:42:46.111759 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3819 2024-01-12 03:42:46.111853 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5224 2024-01-12 03:42:46.111956 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3963 2024-01-12 03:42:46.112233 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3413 2024-01-12 03:42:46.112337 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3882 2024-01-12 03:42:46.112446 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    12985 2024-04-05 22:30:18.293171 fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2024-01-12 03:42:46.112753 fabric-orchestrator-client-1.7.0b3/git_push.sh
+-rw-r--r--   0        0        0     1024 2024-04-05 22:18:00.458232 fabric-orchestrator-client-1.7.0b3/pyproject.toml
+-rw-r--r--   0        0        0       16 2024-01-12 03:42:46.112995 fabric-orchestrator-client-1.7.0b3/test/__init__.py
+-rw-r--r--   0        0        0      841 2024-05-10 08:06:33.139490 fabric-orchestrator-client-1.7.0b3/test/test_metrics.py
+-rw-r--r--   0        0        0      835 2024-05-10 08:06:33.140705 fabric-orchestrator-client-1.7.0b3/test/test_metrics_api.py
+-rw-r--r--   0        0        0      809 2024-01-12 03:42:46.113118 fabric-orchestrator-client-1.7.0b3/test/test_poa.py
+-rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113207 fabric-orchestrator-client-1.7.0b3/test/test_poa_data.py
+-rw-r--r--   0        0        0      843 2024-01-12 03:42:46.113308 fabric-orchestrator-client-1.7.0b3/test/test_poa_post.py
+-rw-r--r--   0        0        0      877 2024-01-12 03:42:46.113402 fabric-orchestrator-client-1.7.0b3/test/test_poa_post_data.py
+-rw-r--r--   0        0        0      963 2024-01-12 03:42:46.113498 fabric-orchestrator-client-1.7.0b3/test/test_poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     1157 2024-01-12 03:42:46.113583 fabric-orchestrator-client-1.7.0b3/test/test_poas_api.py
+-rw-r--r--   0        0        0      896 2024-01-12 03:42:46.113672 fabric-orchestrator-client-1.7.0b3/test/test_resource.py
+-rw-r--r--   0        0        0      950 2024-01-12 03:42:46.113770 fabric-orchestrator-client-1.7.0b3/test/test_resources.py
+-rw-r--r--   0        0        0     1206 2024-01-12 03:42:46.113870 fabric-orchestrator-client-1.7.0b3/test/test_resources_api.py
+-rw-r--r--   0        0        0      872 2024-01-12 03:42:46.113959 fabric-orchestrator-client-1.7.0b3/test/test_slice.py
+-rw-r--r--   0        0        0      930 2024-01-12 03:42:46.114058 fabric-orchestrator-client-1.7.0b3/test/test_slice_details.py
+-rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114249 fabric-orchestrator-client-1.7.0b3/test/test_slices.py
+-rw-r--r--   0        0        0     2165 2024-01-12 03:42:46.114383 fabric-orchestrator-client-1.7.0b3/test/test_slices_api.py
+-rw-r--r--   0        0        0      867 2024-01-12 03:42:46.114477 fabric-orchestrator-client-1.7.0b3/test/test_slices_post.py
+-rw-r--r--   0        0        0      880 2024-01-12 03:42:46.114575 fabric-orchestrator-client-1.7.0b3/test/test_sliver.py
+-rw-r--r--   0        0        0      888 2024-01-12 03:42:46.114670 fabric-orchestrator-client-1.7.0b3/test/test_slivers.py
+-rw-r--r--   0        0        0      974 2024-01-12 03:42:46.114770 fabric-orchestrator-client-1.7.0b3/test/test_slivers_api.py
+-rw-r--r--   0        0        0      998 2024-01-12 03:42:46.114861 fabric-orchestrator-client-1.7.0b3/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1032 2024-01-12 03:42:46.114968 fabric-orchestrator-client-1.7.0b3/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      996 2024-01-12 03:42:46.115068 fabric-orchestrator-client-1.7.0b3/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115159 fabric-orchestrator-client-1.7.0b3/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      988 2024-01-12 03:42:46.115251 fabric-orchestrator-client-1.7.0b3/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1038 2024-01-12 03:42:46.115351 fabric-orchestrator-client-1.7.0b3/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0     1002 2024-01-12 03:42:46.115454 fabric-orchestrator-client-1.7.0b3/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1052 2024-01-12 03:42:46.115553 fabric-orchestrator-client-1.7.0b3/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      978 2024-01-12 03:42:46.115643 fabric-orchestrator-client-1.7.0b3/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1028 2024-01-12 03:42:46.115743 fabric-orchestrator-client-1.7.0b3/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      972 2024-01-12 03:42:46.115834 fabric-orchestrator-client-1.7.0b3/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1022 2024-01-12 03:42:46.115939 fabric-orchestrator-client-1.7.0b3/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1062 2024-01-12 03:42:46.116047 fabric-orchestrator-client-1.7.0b3/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1112 2024-01-12 03:42:46.116160 fabric-orchestrator-client-1.7.0b3/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      888 2024-01-12 03:42:46.116255 fabric-orchestrator-client-1.7.0b3/test/test_version.py
+-rw-r--r--   0        0        0      814 2024-01-12 03:42:46.116365 fabric-orchestrator-client-1.7.0b3/test/test_version_api.py
+-rw-r--r--   0        0        0      922 2024-01-12 03:42:46.116524 fabric-orchestrator-client-1.7.0b3/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2024-01-12 03:42:46.116674 fabric-orchestrator-client-1.7.0b3/tox.ini
+-rw-r--r--   0        0        0    10985 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.7.0b3/PKG-INFO
```

### Comparing `fabric-orchestrator-client-1.7.0b2/.gitignore` & `fabric-orchestrator-client-1.7.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/.swagger-codegen-ignore` & `fabric-orchestrator-client-1.7.0b3/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/CODEGEN.md` & `fabric-orchestrator-client-1.7.0b3/CODEGEN.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/LICENSE` & `fabric-orchestrator-client-1.7.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/README.md` & `fabric-orchestrator-client-1.7.0b3/README.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/docs/PoaData.md` & `fabric-orchestrator-client-1.7.0b3/docs/PoaData.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/docs/PoasApi.md` & `fabric-orchestrator-client-1.7.0b3/docs/PoasApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/docs/ResourcesApi.md` & `fabric-orchestrator-client-1.7.0b3/docs/ResourcesApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/docs/SlicesApi.md` & `fabric-orchestrator-client-1.7.0b3/docs/SlicesApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/docs/SliversApi.md` & `fabric-orchestrator-client-1.7.0b3/docs/SliversApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/orchestrator_proxy.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/orchestrator_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
             #configuration.verify_ssl = False
             configuration.host = f"https://{orchestrator_host}/"
             api_instance = swagger_client.ApiClient(configuration)
             self.slices_api = swagger_client.SlicesApi(api_client=api_instance)
             self.slivers_api = swagger_client.SliversApi(api_client=api_instance)
             self.resources_api = swagger_client.ResourcesApi(api_client=api_instance)
             self.poas_api = swagger_client.PoasApi(api_client=api_instance)
+            self.metrics_api = swagger_client.MetricsApi(api_client=api_instance)
 
     def __set_tokens(self, *, token: str):
         """
         Set tokens
         @param token token
         """
         # Set the tokens
@@ -552,8 +553,24 @@
             elif sliver_id is not None:
                 poa_data = self.poas_api.poas_get(sliver_id=sliver_id, limit=limit, offset=offset)
             else:
                 raise Exception("Invalid Arguments")
 
             return Status.OK, poa_data.data if poa_data.data is not None else None
         except Exception as e:
-            return Status.FAILURE, e
+            return Status.FAILURE, e
+
+    def get_metrics_overview(self, *, token: str = None,
+                             excluded_projects: List[str] = None) -> Tuple[Status, Union[Exception, list]]:
+        """
+        Modify a slice
+        @param token fabric token
+        @param excluded_projects list of project ids to exclude
+        @return Tuple containing Status and Exception/Json containing poa info created
+        """
+        try:
+            # Set the tokens
+            self.__set_tokens(token=token)
+            result = self.metrics_api.metrics_overview_get(excluded_projects=excluded_projects)
+            return Status.OK, result.results
+        except Exception as e:
+            return Status.FAILURE, e
```

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/__init__.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,25 @@
     Contact: kthare10@unc.edu
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
+from fabric_cf.orchestrator.swagger_client.api.metrics_api import MetricsApi
 from fabric_cf.orchestrator.swagger_client.api.poas_api import PoasApi
 from fabric_cf.orchestrator.swagger_client.api.resources_api import ResourcesApi
 from fabric_cf.orchestrator.swagger_client.api.slices_api import SlicesApi
 from fabric_cf.orchestrator.swagger_client.api.slivers_api import SliversApi
 from fabric_cf.orchestrator.swagger_client.api.version_api import VersionApi
 # import ApiClient
 from fabric_cf.orchestrator.swagger_client.api_client import ApiClient
 from fabric_cf.orchestrator.swagger_client.configuration import Configuration
 # import models into sdk package
+from fabric_cf.orchestrator.swagger_client.models.metrics import Metrics
 from fabric_cf.orchestrator.swagger_client.models.poa import Poa
 from fabric_cf.orchestrator.swagger_client.models.poa_data import PoaData
 from fabric_cf.orchestrator.swagger_client.models.poa_post import PoaPost
 from fabric_cf.orchestrator.swagger_client.models.poa_post_data import PoaPostData
 from fabric_cf.orchestrator.swagger_client.models.poa_post_data_keys import PoaPostDataKeys
 from fabric_cf.orchestrator.swagger_client.models.poa_post_data_vcpu_cpu_map import PoaPostDataVcpuCpuMap
 from fabric_cf.orchestrator.swagger_client.models.resource import Resource
```

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/poas_api.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/poas_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/resources_api.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/slices_api.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api/version_api.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/api_client.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/configuration.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/__init__.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     def __init__(self, data=None, *args, **kwargs):  # noqa: E501
         """Poa - a model defined in Swagger"""  # noqa: E501
         Status200OkSingle.__init__(self, *args, **kwargs)
         self._data = None
         self.discriminator = None
         if data is not None:
             self.data = data
-        Status200OkSingle.__init__(self, *args, **kwargs)
 
     @property
     def data(self):
         """Gets the data of this Poa.  # noqa: E501
 
 
         :return: The data of this Poa.  # noqa: E501
```

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_data.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/resource.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/resources.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slice.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slice_details.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/slice_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,20 +38,19 @@
         'data': 'data'
     }
     if hasattr(Status200OkSingle, "attribute_map"):
         attribute_map.update(Status200OkSingle.attribute_map)
 
     def __init__(self, data=None, *args, **kwargs):  # noqa: E501
         """SliceDetails - a model defined in Swagger"""  # noqa: E501
+        Status200OkSingle.__init__(self, *args, **kwargs)
         self._data = None
         self.discriminator = None
         if data is not None:
             self.data = data
-        Status200OkSingle.__init__(self, *args, **kwargs)
-        
 
     @property
     def data(self):
         """Gets the data of this SliceDetails.  # noqa: E501
 
 
         :return: The data of this SliceDetails.  # noqa: E501
```

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slices.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slices_post.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/sliver.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/slivers.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/version.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/models/version_data.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/fabric_cf/orchestrator/swagger_client/rest.py` & `fabric-orchestrator-client-1.7.0b3/fabric_cf/orchestrator/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/git_push.sh` & `fabric-orchestrator-client-1.7.0b3/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/pyproject.toml` & `fabric-orchestrator-client-1.7.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_poa.py` & `fabric-orchestrator-client-1.7.0b3/test/test_poa.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_poa_data.py` & `fabric-orchestrator-client-1.7.0b3/test/test_poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_poa_post.py` & `fabric-orchestrator-client-1.7.0b3/test/test_poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_poa_post_data.py` & `fabric-orchestrator-client-1.7.0b3/test/test_poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.7.0b3/test/test_poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_poas_api.py` & `fabric-orchestrator-client-1.7.0b3/test/test_poas_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_resource.py` & `fabric-orchestrator-client-1.7.0b3/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_resources.py` & `fabric-orchestrator-client-1.7.0b3/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_resources_api.py` & `fabric-orchestrator-client-1.7.0b3/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_slice.py` & `fabric-orchestrator-client-1.7.0b3/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_slice_details.py` & `fabric-orchestrator-client-1.7.0b3/test/test_slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_slices.py` & `fabric-orchestrator-client-1.7.0b3/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_slices_api.py` & `fabric-orchestrator-client-1.7.0b3/test/test_slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_slices_post.py` & `fabric-orchestrator-client-1.7.0b3/test/test_slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_sliver.py` & `fabric-orchestrator-client-1.7.0b3/test/test_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_slivers.py` & `fabric-orchestrator-client-1.7.0b3/test/test_slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_slivers_api.py` & `fabric-orchestrator-client-1.7.0b3/test/test_slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_no_content.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_paginated.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status200_ok_single.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status400_bad_request.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status400_bad_request_errors.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status401_unauthorized.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status403_forbidden.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status403_forbidden_errors.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status404_not_found.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status404_not_found_errors.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status500_internal_server_error.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.7.0b3/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_version.py` & `fabric-orchestrator-client-1.7.0b3/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_version_api.py` & `fabric-orchestrator-client-1.7.0b3/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/test/test_version_data.py` & `fabric-orchestrator-client-1.7.0b3/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.7.0b2/PKG-INFO` & `fabric-orchestrator-client-1.7.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-orchestrator-client
-Version: 1.7.0b2
+Version: 1.7.0b3
 Summary: Fabric Orchestrator API
 Keywords: Swagger,Fabric Orchestrator API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

