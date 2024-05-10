# Comparing `tmp/carmen_cloud_client-1.0.3.tar.gz` & `tmp/carmen_cloud_client-1.1.0.tar.gz`

## Comparing `carmen_cloud_client-1.0.3.tar` & `carmen_cloud_client-1.1.0.tar`

### file list

```diff
@@ -1,60 +1,82 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/.dockerignore
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/.editorconfig
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/.env.example
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/DEVELOPMENT.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/Dockerfile
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/generate-response.sh
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/requirements-dev.txt
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/requirements.txt
--rwxr-xr-x   0        0        0      303 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/update-openapi-spec.sh
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/assets/transport/response.schema.json
--rw-r--r--   0        0        0    35039 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/assets/vehicle/response.schema.json
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/__init__.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/errors.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/__init__.py
--rw-r--r--   0        0        0    53584 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa01.jpg
--rw-r--r--   0        0        0    50105 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa02.jpg
--rw-r--r--   0        0        0    50896 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa03.jpg
--rw-r--r--   0        0        0   174381 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa20.jpg
--rw-r--r--   0        0        0   407461 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra01.jpg
--rw-r--r--   0        0        0   464913 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra02.jpg
--rw-r--r--   0        0        0   444103 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra03.jpg
--rw-r--r--   0        0        0   290590 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra20.jpg
--rw-r--r--   0        0        0    58721 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis01.jpg
--rw-r--r--   0        0        0    55968 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis02.jpg
--rw-r--r--   0        0        0    54027 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis03.jpg
--rw-r--r--   0        0        0    51029 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis20.jpg
--rw-r--r--   0        0        0   591726 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu01.jpg
--rw-r--r--   0        0        0   631603 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu02.jpg
--rw-r--r--   0        0        0   591726 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu03.jpg
--rw-r--r--   0        0        0   322324 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu20.jpg
--rwxr-xr-x   0        0        0  1310563 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/iso01.jpg
--rwxr-xr-x   0        0        0  1303972 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/iso02.jpg
--rwxr-xr-x   0        0        0   568572 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/iso20.jpg
--rw-r--r--   0        0        0     8457 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/test_client.py
--rw-r--r--   0        0        0    18554 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic01.jpg
--rw-r--r--   0        0        0    18263 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic02.jpg
--rw-r--r--   0        0        0    18360 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic03.jpg
--rw-r--r--   0        0        0   134606 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic20.jpg
--rwxr-xr-x   0        0        0   111561 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/usdot01.jpg
--rwxr-xr-x   0        0        0   117809 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/usdot20.jpg
--rw-r--r--   0        0        0    62487 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/adr-test.jpg
--rwxr-xr-x   0        0        0   221278 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/many_plates_hun.jpg
--rw-r--r--   0        0        0   287526 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/test.jpg
--rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/test_client.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/transport/__init__.py
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/transport/client.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/transport/options.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/transport/response.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/__init__.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/client.py
--rw-r--r--   0        0        0    21298 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/options.py
--rw-r--r--   0        0        0    19472 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/response.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/LICENSE
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/README.md
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/.dockerignore
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/.editorconfig
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/.env.example
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/DEVELOPMENT.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/Dockerfile
+-rwxr-xr-x   0        0        0     1675 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/generate-response.sh
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/requirements-dev.txt
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/requirements.txt
+-rwxr-xr-x   0        0        0     1827 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/update-openapi-spec.sh
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/assets/storage-and-hook/APIStorageStatusRequest.schema.json
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/assets/storage-and-hook/CreateHookRequest.schema.json
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/assets/storage-and-hook/EventsResponse.schema.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/assets/storage-and-hook/Hook.schema.json
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/assets/storage-and-hook/Hooks.schema.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/assets/storage-and-hook/OKResponse.schema.json
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/assets/storage-and-hook/StorageStatusResponse.schema.json
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/assets/storage-and-hook/UpdateHookRequest.schema.json
+-rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/assets/transport/response.schema.json
+-rw-r--r--   0        0        0    35039 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/assets/vehicle/response.schema.json
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/__init__.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/errors.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/models.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/utils.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/storage_and_hook/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/storage_and_hook/api_storage_status_request.py
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/storage_and_hook/client.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/storage_and_hook/create_hook_request.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/storage_and_hook/events_response.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/storage_and_hook/hook.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/storage_and_hook/ok_response.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/storage_and_hook/options.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/storage_and_hook/storage_status_response.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/storage_and_hook/update_hook_request.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/__init__.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/storage_and_hook/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/storage_and_hook/test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/__init__.py
+-rw-r--r--   0        0        0    53584 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/accr_usa01.jpg
+-rw-r--r--   0        0        0    50105 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/accr_usa02.jpg
+-rw-r--r--   0        0        0    50896 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/accr_usa03.jpg
+-rw-r--r--   0        0        0   174381 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/accr_usa20.jpg
+-rw-r--r--   0        0        0   407461 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/bra01.jpg
+-rw-r--r--   0        0        0   464913 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/bra02.jpg
+-rw-r--r--   0        0        0   444103 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/bra03.jpg
+-rw-r--r--   0        0        0   290590 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/bra20.jpg
+-rw-r--r--   0        0        0    58721 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/chassis01.jpg
+-rw-r--r--   0        0        0    55968 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/chassis02.jpg
+-rw-r--r--   0        0        0    54027 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/chassis03.jpg
+-rw-r--r--   0        0        0    51029 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/chassis20.jpg
+-rw-r--r--   0        0        0   591726 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/ilu01.jpg
+-rw-r--r--   0        0        0   631603 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/ilu02.jpg
+-rw-r--r--   0        0        0   591726 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/ilu03.jpg
+-rw-r--r--   0        0        0   322324 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/ilu20.jpg
+-rwxr-xr-x   0        0        0  1310563 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/iso01.jpg
+-rwxr-xr-x   0        0        0  1303972 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/iso02.jpg
+-rwxr-xr-x   0        0        0   568572 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/iso20.jpg
+-rw-r--r--   0        0        0     8457 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/test_client.py
+-rw-r--r--   0        0        0    18554 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/uic01.jpg
+-rw-r--r--   0        0        0    18263 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/uic02.jpg
+-rw-r--r--   0        0        0    18360 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/uic03.jpg
+-rw-r--r--   0        0        0   134606 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/uic20.jpg
+-rwxr-xr-x   0        0        0   111561 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/usdot01.jpg
+-rwxr-xr-x   0        0        0   117809 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/usdot20.jpg
+-rw-r--r--   0        0        0    62487 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/vehicle/adr-test.jpg
+-rwxr-xr-x   0        0        0   221278 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/vehicle/many_plates_hun.jpg
+-rw-r--r--   0        0        0   287526 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/vehicle/test.jpg
+-rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/test/vehicle/test_client.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/transport/__init__.py
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/transport/client.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/transport/options.py
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/transport/response.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/vehicle/__init__.py
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/vehicle/client.py
+-rw-r--r--   0        0        0    21190 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/vehicle/options.py
+-rw-r--r--   0        0        0    19472 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/carmen_cloud_client/vehicle/response.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/README.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 carmen_cloud_client-1.1.0/PKG-INFO
```

### Comparing `carmen_cloud_client-1.0.3/Dockerfile` & `carmen_cloud_client-1.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/requirements-dev.txt` & `carmen_cloud_client-1.1.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/.github/workflows/ci.yml` & `carmen_cloud_client-1.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/assets/transport/response.schema.json` & `carmen_cloud_client-1.1.0/assets/transport/response.schema.json`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/assets/vehicle/response.schema.json` & `carmen_cloud_client-1.1.0/assets/vehicle/response.schema.json`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/errors.py` & `carmen_cloud_client-1.1.0/carmen_cloud_client/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,36 @@
         message (str): The error message.
 
     Attributes:
         name (str): The name of the exception.
     """
     def __init__(self, message):
         super().__init__(message)
-        self.name = "TransportAPIConfigError"
+        self.name = "CarmenAPIConfigError"
 
 class InvalidImageError(Exception):
     """
     Exception raised when the provided image is invalid.
 
     Args:
         message (str): The error message.
 
     Attributes:
         name (str): The name of the exception.
     """
     def __init__(self, message):
         super().__init__(message)
         self.name = "InvalidImageError"
+
+class CarmenAPIError(Exception):
+    """
+    Exception raised when an API call fails after the configured number of retries.
+
+    Args:
+        message (str): The error message.
+
+    Attributes:
+        name (str): The name of the exception.
+    """
+    def __init__(self, message):
+        super().__init__(message)
+        self.name = "CarmenAPIError"
```

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa01.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/accr_usa01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa02.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/accr_usa02.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa03.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/accr_usa03.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa20.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/accr_usa20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra01.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/bra01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra02.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/bra02.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra03.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/bra03.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra20.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/bra20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis01.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/chassis01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis02.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/chassis02.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis03.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/chassis03.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis20.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/chassis20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu01.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/ilu01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu02.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/ilu02.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu03.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/ilu03.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu20.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/ilu20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/iso01.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/iso01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/iso02.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/iso02.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/iso20.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/iso20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/test_client.py` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/test_client.py`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic01.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/uic01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic02.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/uic02.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic03.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/uic03.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic20.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/uic20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/usdot01.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/usdot01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/usdot20.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/transport/usdot20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/adr-test.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/vehicle/adr-test.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/many_plates_hun.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/vehicle/many_plates_hun.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/test.jpg` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/vehicle/test.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/test_client.py` & `carmen_cloud_client-1.1.0/carmen_cloud_client/test/vehicle/test_client.py`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/transport/client.py` & `carmen_cloud_client-1.1.0/carmen_cloud_client/transport/client.py`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/transport/options.py` & `carmen_cloud_client-1.1.0/carmen_cloud_client/transport/options.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import Optional
 from enum import Enum
+from ..models import CloudServiceRegion
 
 class CodeType(Enum):
     """
     The type of code to read.
     """
     ISO = "iso"
     TRUCK = "truck"
@@ -15,15 +16,15 @@
 class TransportAPIOptions:
     """
     Options for configuring the TransportAPI client.
     """
     api_key: str
     type: CodeType
     endpoint: Optional[str] = None
-    cloud_service_region: Optional[str] = None
+    cloud_service_region: Optional[CloudServiceRegion] = None
     disable_iso_code: Optional[bool] = False
     disable_checksum_check: Optional[bool] = False
     enable_full_us_accr_code: Optional[bool] = False
     disable_image_resizing: Optional[bool] = False
     enable_wide_range_analysis: Optional[bool] = False
     max_reads: Optional[int] = 1
     retry_count: Optional[int] = 2
```

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/transport/response.py` & `carmen_cloud_client-1.1.0/carmen_cloud_client/transport/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  response.schema.json
-#   timestamp: 2024-04-26T11:06:14+00:00
+#   timestamp: 2024-05-10T13:30:44+00:00
 
 from __future__ import annotations
 
 from typing import List, Optional
 
 from pydantic import BaseModel, Field, conint
```

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/client.py` & `carmen_cloud_client-1.1.0/carmen_cloud_client/vehicle/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from typing import List, Union
 from io import BytesIO
 from requests.exceptions import RetryError
 from urllib.parse import urljoin
-from carmen_cloud_client.errors import CarmenAPIConfigError, InvalidImageError
+from carmen_cloud_client.errors import CarmenAPIConfigError, CarmenAPIError, InvalidImageError
 from .options import VehicleAPIOptions, CloudServiceRegion
 from .response import VehicleApiResponse
 
 class VehicleAPIClient:
     supported_api_version: str = "1.4.1"
 
     def __init__(self, options: VehicleAPIOptions):
@@ -33,15 +33,15 @@
         session.mount("https://", adapter)
 
         response = None
         try:
             response = session.post(self.api_url, headers=headers, data=form_data)
             response.raise_for_status()
         except RetryError as e:
-            raise CarmenAPIConfigError(f"Failed to send request after {self.options.retry_count} retries: {e}")
+            raise CarmenAPIError(f"Failed to send request after {self.options.retry_count} retries: {e}")
 
         return VehicleApiResponse.parse_obj(response.json())
 
     def get_image_bytes(self, image_data_or_path: Union[str, bytes, BytesIO]) -> Union[bytes, BytesIO]:
         if isinstance(image_data_or_path, bytes) or isinstance(image_data_or_path, BytesIO):
             return image_data_or_path
         elif isinstance(image_data_or_path, str) and os.path.exists(image_data_or_path):
```

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/options.py` & `carmen_cloud_client-1.1.0/carmen_cloud_client/vehicle/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from typing import Optional, Tuple
 from enum import Enum
 from ..errors import CarmenAPIConfigError
+from ..models import CloudServiceRegion
 
 @dataclass(frozen=True)
 class SelectedServices:
     """
     Specifies the recognition services to call on the input image. At least one
     service must be selected.
 
@@ -280,22 +281,14 @@
     SouthAmerica = SouthAmerica
     CentralAsia = CentralAsia
     EastAsia = EastAsia
     SouthAsia = SouthAsia
     MiddleEast = MiddleEast
     AustraliaAndOceania = AustraliaAndOceania
 
-class CloudServiceRegion(Enum):
-    """
-    The cloud service region to use for the request.
-    """
-    AUTO = "AUTO"
-    EU = "EU"
-    US = "US"
-
 @dataclass
 class VehicleAPIOptions:
     """
     An object containing configuration options for the Vehicle API client.
 
     Attributes
     ----------
```

### Comparing `carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/response.py` & `carmen_cloud_client-1.1.0/carmen_cloud_client/vehicle/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  response.schema.json
-#   timestamp: 2024-04-26T11:06:15+00:00
+#   timestamp: 2024-05-10T13:30:45+00:00
 
 from __future__ import annotations
 
 from typing import List, Optional
 
 from pydantic import BaseModel, Field, conint
```

### Comparing `carmen_cloud_client-1.0.3/LICENSE` & `carmen_cloud_client-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.3/pyproject.toml` & `carmen_cloud_client-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "carmen_cloud_client"
-version = "1.0.3"
+version = "1.1.0"
 authors = [
   { name="Botond BALÁZS", email="botond.balazs@arip.hu" },
 ]
 description = "Python client for Carmen Cloud by Adaptive Recognition. Efficiently read license plates, recognize vehicle details, and process container, railway wagon, and US DOT codes."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `carmen_cloud_client-1.0.3/PKG-INFO` & `carmen_cloud_client-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.3
-Name: carmen_cloud_client
-Version: 1.0.3
-Summary: Python client for Carmen Cloud by Adaptive Recognition. Efficiently read license plates, recognize vehicle details, and process container, railway wagon, and US DOT codes.
-Project-URL: Homepage, https://github.com/adaptiverecognition/python-carmen-cloud-client
-Project-URL: Bug Tracker, https://github.com/adaptiverecognition/python-carmen-cloud-client/issues
-Author-email: Botond BALÁZS <botond.balazs@arip.hu>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: pydantic>=1.10.9
-Requires-Dist: requests-toolbelt>=1.0.0
-Requires-Dist: requests>=2.31.0
-Requires-Dist: urllib3>=2.0.3
-Description-Content-Type: text/markdown
-
 # Carmen Cloud Client by Adaptive Recognition
 
 Python client for [Carmen Cloud](https://carmencloud.com/) by [Adaptive Recognition](https://adaptiverecognition.com/). This unified library provides you with access to both the **Vehicle API** and the **Transportation & Cargo API**.
 
 ## Supported API Versions
 
 - Vehicle API: v1.4.1
@@ -64,10 +46,70 @@
 )
 client = TransportAPIClient(options)
 
 response = client.send("./container.jpg")
 print(response)
 ```
 
+### 📦 Storage & Hook API
+
+```python
+from carmen_cloud_client import (
+    APIName,
+    CreateHookRequest,
+    EventFilters,
+    StorageAndHookAPIClient,
+    StorageAndHookAPIOptions,
+    StorageStatusRequest,
+    UpdateHookRequest,
+)
+
+options = StorageAndHookAPIOptions(
+    api_key="<YOUR_API_KEY>",
+    cloud_service_region="EU"
+)
+client = StorageAndHookAPIClient(options)
+
+# List Events
+filters = EventFilters(limit=5)
+events = client.get_events(APIName.Vehicle, filters)
+print("events:", events)
+
+# Get Storage Status
+status = client.get_storage_status()
+print("status:", status)
+
+# Update Storage Status
+apis = StorageStatusRequest(vehicle=True, transport=False)
+updated_status = client.update_storage_status(apis)
+print('updatedStatus:', updated_status)
+
+# Create Hook
+hook = CreateHookRequest(
+    hookUrl='http://request-logger.botond.online',
+    apis=Apis(vehicle=True, transport=False)
+)
+created_hook = client.create_hook(hook)
+print('createdHook:', created_hook)
+
+# List Hooks
+hooks = client.get_hooks()
+print('hooks:', hooks)
+
+# Get Hook
+hook = client.get_hook('https://your-domain.com/your-hook-path')
+print('hook:', hook)
+
+# Update Hook
+updated_hook = client.update_hook(
+    'https://your-domain.com/your-hook-path',
+    UpdateHookRequest(vehicle=True, transport=True)
+)
+print('updatedHook:', updated_hook)
+
+# Delete Hook
+client.delete_hook('https://your-domain.com/your-hook-path')
+```
+
 ## 🔧 Development
 
 For more information about developing and contributing to this project, see [DEVELOPMENT.md](DEVELOPMENT.md).
```

