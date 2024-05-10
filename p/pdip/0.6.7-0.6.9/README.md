# Comparing `tmp/pdip-0.6.7.tar.gz` & `tmp/pdip-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdip-0.6.7.tar", last modified: Fri May  3 01:18:38 2024, max compression
+gzip compressed data, was "pdip-0.6.9.tar", last modified: Fri May 10 08:09:23 2024, max compression
```

## Comparing `pdip-0.6.7.tar` & `pdip-0.6.9.tar`

### file list

```diff
@@ -1,576 +1,576 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.267182 pdip-0.6.7/
--rw-rw-rw-   0        0        0     1097 2024-03-22 10:41:08.000000 pdip-0.6.7/LICENSE
--rw-rw-rw-   0        0        0     1525 2024-05-03 01:18:38.267182 pdip-0.6.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:33.923395 pdip-0.6.7/pdip/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:33.986460 pdip-0.6.7/pdip/api/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:33.996461 pdip-0.6.7/pdip/api/app/
--rw-rw-rw-   0        0        0       48 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/app/__init__.py
--rw-rw-rw-   0        0        0     1941 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/app/flask_app_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.033496 pdip-0.6.7/pdip/api/base/
--rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/base/__init__.py
--rw-rw-rw-   0        0        0     3736 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/api/base/controller_base.py
--rw-rw-rw-   0        0        0     4506 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/base/endpoint_base.py
--rw-rw-rw-   0        0        0     8789 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/base/endpoint_wrapper.py
--rw-rw-rw-   0        0        0      172 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/base/resource_base.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.047494 pdip-0.6.7/pdip/api/converter/
--rw-rw-rw-   0        0        0       49 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/converter/__init__.py
--rw-rw-rw-   0        0        0     3284 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/converter/request_converter.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.063541 pdip-0.6.7/pdip/api/decorators/
--rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/decorators/__init__.py
--rw-rw-rw-   0        0        0      240 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/decorators/controller_base.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.089139 pdip-0.6.7/pdip/api/handlers/
--rw-rw-rw-   0        0        0       88 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/handlers/__init__.py
--rw-rw-rw-   0        0        0     3755 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/handlers/error_handlers.py
--rw-rw-rw-   0        0        0     1515 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/handlers/request_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.113137 pdip-0.6.7/pdip/api/request_parameter/
--rw-rw-rw-   0        0        0       97 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/request_parameter/__init__.py
--rw-rw-rw-   0        0        0      124 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/request_parameter/order_by_parameter.py
--rw-rw-rw-   0        0        0      129 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/request_parameter/paging_parameter.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.141135 pdip-0.6.7/pdip/api/specifications/
--rw-rw-rw-   0        0        0      113 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/specifications/__init__.py
--rw-rw-rw-   0        0        0     1492 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/specifications/order_by_specification.py
--rw-rw-rw-   0        0        0     1252 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/api/specifications/paging_specification.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.158182 pdip-0.6.7/pdip/base/
--rw-rw-rw-   0        0        0       22 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/base/__init__.py
--rw-rw-rw-   0        0        0     1677 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/base/pdi.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.177776 pdip-0.6.7/pdip/configuration/
--rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/__init__.py
--rw-rw-rw-   0        0        0     5293 2024-05-02 23:21:00.000000 pdip-0.6.7/pdip/configuration/config_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.186776 pdip-0.6.7/pdip/configuration/models/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.200776 pdip-0.6.7/pdip/configuration/models/api/
--rw-rw-rw-   0        0        0       35 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/models/api/__init__.py
--rw-rw-rw-   0        0        0      334 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/models/api/api_config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.215774 pdip-0.6.7/pdip/configuration/models/application/
--rw-rw-rw-   0        0        0       51 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/models/application/__init__.py
--rw-rw-rw-   0        0        0      271 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/models/application/application_config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.229772 pdip-0.6.7/pdip/configuration/models/aps/
--rw-rw-rw-   0        0        0       35 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/models/aps/__init__.py
--rw-rw-rw-   0        0        0      380 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/models/aps/aps_config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.245770 pdip-0.6.7/pdip/configuration/models/base/
--rw-rw-rw-   0        0        0      236 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/configuration/models/base/__init__.py
--rw-rw-rw-   0        0        0       87 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/models/base/base_config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.261817 pdip-0.6.7/pdip/configuration/models/database/
--rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/models/database/__init__.py
--rw-rw-rw-   0        0        0      450 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/models/database/database_config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.286417 pdip-0.6.7/pdip/configuration/services/
--rw-rw-rw-   0        0        0       99 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/services/__init__.py
--rw-rw-rw-   0        0        0      482 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/services/config_parameter_base.py
--rw-rw-rw-   0        0        0     1051 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/configuration/services/config_service.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.364458 pdip-0.6.7/pdip/cqrs/
--rw-rw-rw-   0        0        0      301 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/__init__.py
--rw-rw-rw-   0        0        0      162 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/command_query_base.py
--rw-rw-rw-   0        0        0      331 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/command_query_handler_base.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.405167 pdip-0.6.7/pdip/cqrs/decorators/
--rw-rw-rw-   0        0        0      117 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/decorators/__init__.py
--rw-rw-rw-   0        0        0      861 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/decorators/cls_to_dict.py
--rw-rw-rw-   0        0        0      277 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/cqrs/decorators/dto_class.py
--rw-rw-rw-   0        0        0      281 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/cqrs/decorators/request_class.py
--rw-rw-rw-   0        0        0      282 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/cqrs/decorators/response_class.py
--rw-rw-rw-   0        0        0     1586 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/dispatcher.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.421165 pdip-0.6.7/pdip/cqrs/generator/
--rw-rw-rw-   0        0        0       66 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.462210 pdip-0.6.7/pdip/cqrs/generator/domain/
--rw-rw-rw-   0        0        0      187 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/generator/domain/__init__.py
--rw-rw-rw-   0        0        0      126 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/generator/domain/dao_generate_config.py
--rw-rw-rw-   0        0        0      241 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/generator/domain/generate_config.py
--rw-rw-rw-   0        0        0      167 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/generator/domain/generator.py
--rw-rw-rw-   0        0        0      198 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/generator/domain/query_generate_config.py
--rw-rw-rw-   0        0        0    12142 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/generator/query_generator.py
--rw-rw-rw-   0        0        0      223 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/icommand.py
--rw-rw-rw-   0        0        0      361 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/icommand_handler.py
--rw-rw-rw-   0        0        0      221 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/iquery.py
--rw-rw-rw-   0        0        0      354 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cqrs/iquery_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.478809 pdip-0.6.7/pdip/cryptography/
--rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cryptography/__init__.py
--rw-rw-rw-   0        0        0     1058 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/cryptography/crypto_service.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.486808 pdip-0.6.7/pdip/data/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.499808 pdip-0.6.7/pdip/data/base/
--rw-rw-rw-   0        0        0       62 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/data/base/__init__.py
--rw-rw-rw-   0        0        0     2757 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/data/base/database_session_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.517807 pdip-0.6.7/pdip/data/decorators/
--rw-rw-rw-   0        0        0       53 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/data/decorators/__init__.py
--rw-rw-rw-   0        0        0      633 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/data/decorators/transaction_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.544764 pdip-0.6.7/pdip/data/domain/
--rw-rw-rw-   0        0        0       65 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/data/domain/__init__.py
--rw-rw-rw-   0        0        0     1208 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/data/domain/entity.py
--rw-rw-rw-   0        0        0      908 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/data/domain/entity_base.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.561785 pdip-0.6.7/pdip/data/domain/types/
--rw-rw-rw-   0        0        0     1154 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/data/domain/types/GUID.py
--rw-rw-rw-   0        0        0       22 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/data/domain/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.590473 pdip-0.6.7/pdip/data/repository/
--rw-rw-rw-   0        0        0       89 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/data/repository/__init__.py
--rw-rw-rw-   0        0        0     2997 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/data/repository/repository.py
--rw-rw-rw-   0        0        0     2031 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/data/repository/repository_provider.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.635746 pdip-0.6.7/pdip/data/seed/
--rw-rw-rw-   0        0        0       61 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/data/seed/__init__.py
--rw-rw-rw-   0        0        0      115 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/data/seed/seed.py
--rw-rw-rw-   0        0        0     1478 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/data/seed/seed_runner.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.664403 pdip-0.6.7/pdip/delivery/
--rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/delivery/__init__.py
--rw-rw-rw-   0        0        0     4042 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/delivery/email_provider.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.682571 pdip-0.6.7/pdip/dependency/
--rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/dependency/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.698267 pdip-0.6.7/pdip/dependency/container/
--rw-rw-rw-   0        0        0       55 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/dependency/container/__init__.py
--rw-rw-rw-   0        0        0      945 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/dependency/container/dependency_container.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.713387 pdip-0.6.7/pdip/dependency/provider/
--rw-rw-rw-   0        0        0       47 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/dependency/provider/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.729696 pdip-0.6.7/pdip/dependency/provider/api/
--rw-rw-rw-   0        0        0       39 2024-05-02 23:21:00.000000 pdip-0.6.7/pdip/dependency/provider/api/__init__.py
--rw-rw-rw-   0        0        0     4257 2024-05-03 00:13:59.000000 pdip-0.6.7/pdip/dependency/provider/api/api_provider.py
--rw-rw-rw-   0        0        0     6728 2024-05-02 23:21:00.000000 pdip-0.6.7/pdip/dependency/provider/service_provider.py
--rw-rw-rw-   0        0        0      159 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/dependency/scopes.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.783141 pdip-0.6.7/pdip/exceptions/
--rw-rw-rw-   0        0        0      268 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/exceptions/__init__.py
--rw-rw-rw-   0        0        0       58 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/exceptions/incompatible_adapter_exception.py
--rw-rw-rw-   0        0        0      148 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/exceptions/not_supported_feature_exception.py
--rw-rw-rw-   0        0        0       50 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/exceptions/operational_exception.py
--rw-rw-rw-   0        0        0       52 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/exceptions/required_class_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.805564 pdip-0.6.7/pdip/html/
--rw-rw-rw-   0        0        0       68 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/html/__init__.py
--rw-rw-rw-   0        0        0     9512 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/html/html_template_service.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.823018 pdip-0.6.7/pdip/integrator/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.842615 pdip-0.6.7/pdip/integrator/base/
--rw-rw-rw-   0        0        0       36 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/base/__init__.py
--rw-rw-rw-   0        0        0     2233 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/base/integrator.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.853027 pdip-0.6.7/pdip/integrator/connection/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.873909 pdip-0.6.7/pdip/integrator/connection/base/
--rw-rw-rw-   0        0        0      128 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/base/__init__.py
--rw-rw-rw-   0        0        0      668 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/base/connection_source_adapter.py
--rw-rw-rw-   0        0        0      576 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/base/connection_target_adapter.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.880915 pdip-0.6.7/pdip/integrator/connection/domain/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.887241 pdip-0.6.7/pdip/integrator/connection/domain/authentication/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/authentication/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.902609 pdip-0.6.7/pdip/integrator/connection/domain/authentication/basic/
--rw-rw-rw-   0        0        0       76 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/authentication/basic/__init__.py
--rw-rw-rw-   0        0        0      137 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/authentication/basic/connection_basic_authentication.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.920684 pdip-0.6.7/pdip/integrator/connection/domain/authentication/kerberos/
--rw-rw-rw-   0        0        0       61 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/authentication/kerberos/__init__.py
--rw-rw-rw-   0        0        0      218 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/authentication/kerberos/kerberos_authentication.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.935684 pdip-0.6.7/pdip/integrator/connection/domain/authentication/mechanism/
--rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/authentication/mechanism/__init__.py
--rw-rw-rw-   0        0        0      144 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/authentication/mechanism/mechanism_types.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.951300 pdip-0.6.7/pdip/integrator/connection/domain/authentication/type/
--rw-rw-rw-   0        0        0       55 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/authentication/type/__init__.py
--rw-rw-rw-   0        0        0      134 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/authentication/type/authentication_types.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.968304 pdip-0.6.7/pdip/integrator/connection/domain/base/
--rw-rw-rw-   0        0        0       42 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/base/__init__.py
--rw-rw-rw-   0        0        0      263 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/base/column.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.991286 pdip-0.6.7/pdip/integrator/connection/domain/enums/
--rw-rw-rw-   0        0        0       92 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/enums/__init__.py
--rw-rw-rw-   0        0        0      154 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/enums/connection_types.py
--rw-rw-rw-   0        0        0      233 2024-05-02 23:21:00.000000 pdip-0.6.7/pdip/integrator/connection/domain/enums/connector_types.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:34.997789 pdip-0.6.7/pdip/integrator/connection/domain/server/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/server/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.009038 pdip-0.6.7/pdip/integrator/connection/domain/server/base/
--rw-rw-rw-   0        0        0       49 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/server/base/__init__.py
--rw-rw-rw-   0        0        0      120 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/server/base/connection_server.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.026037 pdip-0.6.7/pdip/integrator/connection/domain/task/
--rw-rw-rw-   0        0        0       44 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/task/__init__.py
--rw-rw-rw-   0        0        0      406 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/task/data_queue_task.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.032036 pdip-0.6.7/pdip/integrator/connection/domain/types/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.037577 pdip-0.6.7/pdip/integrator/connection/domain/types/bigdata/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/bigdata/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.048571 pdip-0.6.7/pdip/integrator/connection/domain/types/bigdata/base/
--rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/bigdata/base/__init__.py
--rw-rw-rw-   0        0        0      337 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/bigdata/base/big_data.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.055572 pdip-0.6.7/pdip/integrator/connection/domain/types/bigdata/configuration/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/bigdata/configuration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.067578 pdip-0.6.7/pdip/integrator/connection/domain/types/bigdata/configuration/base/
--rw-rw-rw-   0        0        0       79 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/bigdata/configuration/base/__init__.py
--rw-rw-rw-   0        0        0      902 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/bigdata/configuration/base/big_data_connection_configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.080099 pdip-0.6.7/pdip/integrator/connection/domain/types/inmemory/
--rw-rw-rw-   0        0        0       81 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/inmemory/__init__.py
--rw-rw-rw-   0        0        0      346 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/inmemory/in_memory_connection_configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.087108 pdip-0.6.7/pdip/integrator/connection/domain/types/sql/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.099405 pdip-0.6.7/pdip/integrator/connection/domain/types/sql/base/
--rw-rw-rw-   0        0        0       36 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/sql/base/__init__.py
--rw-rw-rw-   0        0        0      325 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/sql/base/sql.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.107686 pdip-0.6.7/pdip/integrator/connection/domain/types/sql/configuration/
--rw-rw-rw-   0        0        0        2 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/sql/configuration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.120686 pdip-0.6.7/pdip/integrator/connection/domain/types/sql/configuration/base/
--rw-rw-rw-   0        0        0       70 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/sql/configuration/base/__init__.py
--rw-rw-rw-   0        0        0      855 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/sql/configuration/base/sql_connection_configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.127683 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.139648 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/base/
--rw-rw-rw-   0        0        0       51 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/base/__init__.py
--rw-rw-rw-   0        0        0      314 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/base/web_service.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.147660 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/configuration/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/configuration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.163912 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/configuration/base/
--rw-rw-rw-   0        0        0       85 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/configuration/base/__init__.py
--rw-rw-rw-   0        0        0      572 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/configuration/base/web_service_connection_configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.180525 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/configuration/soap/
--rw-rw-rw-   0        0        0       51 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/configuration/soap/__init__.py
--rw-rw-rw-   0        0        0       99 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/configuration/soap/soap_configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.206330 pdip-0.6.7/pdip/integrator/connection/factories/
--rw-rw-rw-   0        0        0      158 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/factories/__init__.py
--rw-rw-rw-   0        0        0     3095 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/factories/connection_source_adapter_factory.py
--rw-rw-rw-   0        0        0     3466 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/factories/connection_target_adapter_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.213328 pdip-0.6.7/pdip/integrator/connection/types/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.220352 pdip-0.6.7/pdip/integrator/connection/types/bigdata/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.226352 pdip-0.6.7/pdip/integrator/connection/types/bigdata/adapters/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.238350 pdip-0.6.7/pdip/integrator/connection/types/bigdata/adapters/source/
--rw-rw-rw-   0        0        0       59 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/adapters/source/__init__.py
--rw-rw-rw-   0        0        0     4642 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/adapters/source/big_data_source_adapter.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.251890 pdip-0.6.7/pdip/integrator/connection/types/bigdata/adapters/target/
--rw-rw-rw-   0        0        0       59 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/adapters/target/__init__.py
--rw-rw-rw-   0        0        0     4589 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/adapters/target/big_data_target_adapter.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.307614 pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/
--rw-rw-rw-   0        0        0      282 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/__init__.py
--rw-rw-rw-   0        0        0      458 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/big_data_connector.py
--rw-rw-rw-   0        0        0     9560 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/big_data_context.py
--rw-rw-rw-   0        0        0     2014 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/big_data_dialect.py
--rw-rw-rw-   0        0        0     1842 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/big_data_iterator.py
--rw-rw-rw-   0        0        0     1450 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/big_data_policy.py
--rw-rw-rw-   0        0        0     2238 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/big_data_provider.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.315605 pdip-0.6.7/pdip/integrator/connection/types/bigdata/connectors/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.328606 pdip-0.6.7/pdip/integrator/connection/types/bigdata/connectors/impala/
--rw-rw-rw-   0        0        0       47 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/connectors/impala/__init__.py
--rw-rw-rw-   0        0        0     3597 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/connectors/impala/impala_connector.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.336604 pdip-0.6.7/pdip/integrator/connection/types/bigdata/dialects/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.370582 pdip-0.6.7/pdip/integrator/connection/types/bigdata/dialects/impala/
--rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/dialects/impala/__init__.py
--rw-rw-rw-   0        0        0     5185 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/bigdata/dialects/impala/impala_dialect.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.391015 pdip-0.6.7/pdip/integrator/connection/types/file/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/file/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.412012 pdip-0.6.7/pdip/integrator/connection/types/file/adapters/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/file/adapters/__init__.py
--rw-rw-rw-   0        0        0     8832 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/file/adapters/file_adapter.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.458757 pdip-0.6.7/pdip/integrator/connection/types/file/base/
--rw-rw-rw-   0        0        0      123 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/file/base/__init__.py
--rw-rw-rw-   0        0        0     1061 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/file/base/file_connector.py
--rw-rw-rw-   0        0        0     3837 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/file/base/file_context.py
--rw-rw-rw-   0        0        0     1938 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/file/base/file_provider.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.467004 pdip-0.6.7/pdip/integrator/connection/types/file/connectors/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/file/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.484526 pdip-0.6.7/pdip/integrator/connection/types/file/connectors/csv/
--rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/file/connectors/csv/__init__.py
--rw-rw-rw-   0        0        0     3384 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/file/connectors/csv/csv_connector.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.493526 pdip-0.6.7/pdip/integrator/connection/types/inmemory/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/inmemory/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.539414 pdip-0.6.7/pdip/integrator/connection/types/inmemory/base/
--rw-rw-rw-   0        0        0      196 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/inmemory/base/__init__.py
--rw-rw-rw-   0        0        0     1273 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/inmemory/base/in_memory_connector.py
--rw-rw-rw-   0        0        0     4465 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/inmemory/base/in_memory_context.py
--rw-rw-rw-   0        0        0     1056 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/inmemory/base/in_memory_policy.py
--rw-rw-rw-   0        0        0     1361 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/inmemory/base/in_memory_provider.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.547412 pdip-0.6.7/pdip/integrator/connection/types/inmemory/connectors/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/inmemory/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.563689 pdip-0.6.7/pdip/integrator/connection/types/inmemory/connectors/sqlite/
--rw-rw-rw-   0        0        0       48 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/inmemory/connectors/sqlite/__init__.py
--rw-rw-rw-   0        0        0     1523 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/inmemory/connectors/sqlite/sq_lite_connector.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.573413 pdip-0.6.7/pdip/integrator/connection/types/queue/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.588006 pdip-0.6.7/pdip/integrator/connection/types/queue/adapters/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/queue/adapters/__init__.py
--rw-rw-rw-   0        0        0     4288 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/queue/adapters/queue_adapter.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.624373 pdip-0.6.7/pdip/integrator/connection/types/queue/base/
--rw-rw-rw-   0        0        0      129 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/queue/base/__init__.py
--rw-rw-rw-   0        0        0     1094 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/queue/base/queue_connector.py
--rw-rw-rw-   0        0        0     2257 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/queue/base/queue_context.py
--rw-rw-rw-   0        0        0     2016 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/queue/base/queue_provider.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.640913 pdip-0.6.7/pdip/integrator/connection/types/queue/connectors/
--rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/queue/connectors/__init__.py
--rw-rw-rw-   0        0        0     6970 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/queue/connectors/kafka_connector.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.649173 pdip-0.6.7/pdip/integrator/connection/types/sql/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.657148 pdip-0.6.7/pdip/integrator/connection/types/sql/adapters/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.674843 pdip-0.6.7/pdip/integrator/connection/types/sql/adapters/source/
--rw-rw-rw-   0        0        0       50 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/adapters/source/__init__.py
--rw-rw-rw-   0        0        0     3820 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/adapters/source/sql_source_adapter.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.689869 pdip-0.6.7/pdip/integrator/connection/types/sql/adapters/target/
--rw-rw-rw-   0        0        0       50 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/adapters/target/__init__.py
--rw-rw-rw-   0        0        0     3672 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/adapters/target/sql_target_adapter.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.752572 pdip-0.6.7/pdip/integrator/connection/types/sql/base/
--rw-rw-rw-   0        0        0      228 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/base/__init__.py
--rw-rw-rw-   0        0        0      478 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/base/sql_connector.py
--rw-rw-rw-   0        0        0     9467 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/base/sql_context.py
--rw-rw-rw-   0        0        0     2014 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/base/sql_dialect.py
--rw-rw-rw-   0        0        0     1797 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/base/sql_iterator.py
--rw-rw-rw-   0        0        0     2188 2024-05-02 23:21:00.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/base/sql_policy.py
--rw-rw-rw-   0        0        0     4383 2024-05-02 23:21:00.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/base/sql_provider.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.761868 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.778317 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/clickhouse/
--rw-rw-rw-   0        0        0       55 2024-05-02 23:21:00.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/clickhouse/__init__.py
--rw-rw-rw-   0        0        0     3357 2024-05-02 23:21:00.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/clickhouse/clickhouse_connector.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.796477 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/mssql/
--rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/mssql/__init__.py
--rw-rw-rw-   0        0        0     3340 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/mssql/mssql_connector.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.814702 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/mysql/
--rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/mysql/__init__.py
--rw-rw-rw-   0        0        0     2113 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/mysql/mysql_connector.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.833497 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/oracle/
--rw-rw-rw-   0        0        0       47 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/oracle/__init__.py
--rw-rw-rw-   0        0        0     2640 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/oracle/oracle_connector.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.853899 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/postgresql/
--rw-rw-rw-   0        0        0       55 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/postgresql/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/postgresql/postgresql_connector.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.865686 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.891385 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/clickhouse/
--rw-rw-rw-   0        0        0       51 2024-05-02 23:21:00.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/clickhouse/__init__.py
--rw-rw-rw-   0        0        0     5224 2024-05-02 23:21:00.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/clickhouse/clickhouse_dialect.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.920960 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/mssql/
--rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/mssql/__init__.py
--rw-rw-rw-   0        0        0     5467 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/mssql/mssql_dialect.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.946152 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/mysql/
--rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/mysql/__init__.py
--rw-rw-rw-   0        0        0     5129 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/mysql/mysql_dialect.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.968287 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/oracle/
--rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/oracle/__init__.py
--rw-rw-rw-   0        0        0     5434 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/oracle/oracle_dialect.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:35.989692 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/postgresql/
--rw-rw-rw-   0        0        0       51 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/postgresql/__init__.py
--rw-rw-rw-   0        0        0     5225 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/postgresql/postgresql_dialect.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.000688 pdip-0.6.7/pdip/integrator/connection/types/webservice/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.008690 pdip-0.6.7/pdip/integrator/connection/types/webservice/adapters/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.026116 pdip-0.6.7/pdip/integrator/connection/types/webservice/adapters/source/
--rw-rw-rw-   0        0        0       65 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/adapters/source/__init__.py
--rw-rw-rw-   0        0        0     1079 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/adapters/source/web_service_source_adapter.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.046049 pdip-0.6.7/pdip/integrator/connection/types/webservice/adapters/target/
--rw-rw-rw-   0        0        0       65 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/adapters/target/__init__.py
--rw-rw-rw-   0        0        0     3434 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/adapters/target/web_service_target_adapter.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.093263 pdip-0.6.7/pdip/integrator/connection/types/webservice/base/
--rw-rw-rw-   0        0        0      212 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/base/__init__.py
--rw-rw-rw-   0        0        0      540 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/base/web_service_connector.py
--rw-rw-rw-   0        0        0     1779 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/base/web_service_context.py
--rw-rw-rw-   0        0        0     1061 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/base/web_service_policy.py
--rw-rw-rw-   0        0        0     1991 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/base/web_service_provider.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.102293 pdip-0.6.7/pdip/integrator/connection/types/webservice/connectors/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.121456 pdip-0.6.7/pdip/integrator/connection/types/webservice/connectors/soap/
--rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/connectors/soap/__init__.py
--rw-rw-rw-   0        0        0     2122 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/connection/types/webservice/connectors/soap/soap_connector.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.131456 pdip-0.6.7/pdip/integrator/domain/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.158532 pdip-0.6.7/pdip/integrator/domain/enums/
--rw-rw-rw-   0        0        0       39 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/domain/enums/__init__.py
--rw-rw-rw-   0        0        0      437 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/domain/enums/events.py
--rw-rw-rw-   0        0        0      120 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/domain/enums/status_types.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.168036 pdip-0.6.7/pdip/integrator/event/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/event/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.204739 pdip-0.6.7/pdip/integrator/event/base/
--rw-rw-rw-   0        0        0      216 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/event/base/__init__.py
--rw-rw-rw-   0        0        0     3100 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/event/base/default_integrator_event_manager.py
--rw-rw-rw-   0        0        0     1250 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/event/base/integrator_event_manager.py
--rw-rw-rw-   0        0        0     1029 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/event/base/integrator_event_manager_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.213643 pdip-0.6.7/pdip/integrator/execution/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/execution/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.221156 pdip-0.6.7/pdip/integrator/execution/base/
--rw-rw-rw-   0        0        0        2 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/execution/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.237156 pdip-0.6.7/pdip/integrator/execution/domain/
--rw-rw-rw-   0        0        0      284 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/execution/domain/__init__.py
--rw-rw-rw-   0        0        0     1080 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/execution/domain/execution.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.245628 pdip-0.6.7/pdip/integrator/initializer/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:36.260645 pdip-0.6.7/pdip/integrator/initializer/base/
--rw-rw-rw-   0        0        0       38 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/base/__init__.py
--rw-rw-rw-   0        0        0       60 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/base/initializer.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.274751 pdip-0.6.7/pdip/integrator/initializer/execution/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.310307 pdip-0.6.7/pdip/integrator/initializer/execution/base/
--rw-rw-rw-   0        0        0      129 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/base/__init__.py
--rw-rw-rw-   0        0        0     1457 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/base/default_execution_initializer.py
--rw-rw-rw-   0        0        0      386 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/base/execution_initializer.py
--rw-rw-rw-   0        0        0     1013 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/base/execution_initializer_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.346168 pdip-0.6.7/pdip/integrator/initializer/execution/integration/
--rw-rw-rw-   0        0        0      327 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/integration/__init__.py
--rw-rw-rw-   0        0        0      533 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/integration/default_operation_integration_execution_initializer.py
--rw-rw-rw-   0        0        0      331 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer.py
--rw-rw-rw-   0        0        0     1217 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.388555 pdip-0.6.7/pdip/integrator/initializer/execution/operation/
--rw-rw-rw-   0        0        0      258 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/operation/__init__.py
--rw-rw-rw-   0        0        0      431 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/operation/default_operation_execution_initializer.py
--rw-rw-rw-   0        0        0      275 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/operation/operation_execution_initializer.py
--rw-rw-rw-   0        0        0     1127 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/execution/operation/operation_execution_initializer_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.426037 pdip-0.6.7/pdip/integrator/initializer/integrator/
--rw-rw-rw-   0        0        0      207 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/integrator/__init__.py
--rw-rw-rw-   0        0        0     3286 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/integrator/default_integrator_initializer.py
--rw-rw-rw-   0        0        0      469 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/integrator/integrator_initializer.py
--rw-rw-rw-   0        0        0     1019 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/initializer/integrator/integrator_initializer_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.434342 pdip-0.6.7/pdip/integrator/integration/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.450958 pdip-0.6.7/pdip/integrator/integration/base/
--rw-rw-rw-   0        0        0       57 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/base/__init__.py
--rw-rw-rw-   0        0        0     3845 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/base/integration_execution.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.459348 pdip-0.6.7/pdip/integrator/integration/domain/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.475219 pdip-0.6.7/pdip/integrator/integration/domain/base/
--rw-rw-rw-   0        0        0       94 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/domain/base/__init__.py
--rw-rw-rw-   0        0        0     1031 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/domain/base/integration.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.489942 pdip-0.6.7/pdip/integrator/integration/domain/enums/
--rw-rw-rw-   0        0        0       49 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/domain/enums/__init__.py
--rw-rw-rw-   0        0        0      114 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/domain/enums/integration_types.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.498137 pdip-0.6.7/pdip/integrator/integration/types/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.519713 pdip-0.6.7/pdip/integrator/integration/types/base/
--rw-rw-rw-   0        0        0      121 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/types/base/__init__.py
--rw-rw-rw-   0        0        0      728 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/types/base/integration_adapter.py
--rw-rw-rw-   0        0        0     1845 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/types/base/integration_adapter_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.529223 pdip-0.6.7/pdip/integrator/integration/types/source/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.7/pdip/integrator/integration/types/source/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.545440 pdip-0.6.7/pdip/integrator/integration/types/source/base/
--rw-rw-rw-   0        0        0       51 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/source/base/__init__.py
--rw-rw-rw-   0        0        0     5127 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/source/base/source_integration.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.552926 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.566216 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/base/
--rw-rw-rw-   0        0        0       69 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/base/__init__.py
--rw-rw-rw-   0        0        0     6664 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/base/source_to_target_integration.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.573218 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.585671 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/base/
--rw-rw-rw-   0        0        0      101 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/base/__init__.py
--rw-rw-rw-   0        0        0      537 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/base/integration_source_to_target_execute_strategy.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.601669 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/factories/
--rw-rw-rw-   0        0        0       99 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/factories/__init__.py
--rw-rw-rw-   0        0        0     1723 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/factories/integration_execute_strategy_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.609708 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.625709 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/
--rw-rw-rw-   0        0        0       70 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/__init__.py
--rw-rw-rw-   0        0        0    18820 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/parallel_integration_execute.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.634788 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.651537 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/
--rw-rw-rw-   0        0        0       83 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/__init__.py
--rw-rw-rw-   0        0        0     7431 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/parallel_thread_integration_execute.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.660527 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.674764 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/
--rw-rw-rw-   0        0        0       56 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/__init__.py
--rw-rw-rw-   0        0        0     4368 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/source_read_operation.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.689287 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/
--rw-rw-rw-   0        0        0       58 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/__init__.py
--rw-rw-rw-   0        0        0     8709 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/target_write_operation.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.697347 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.722124 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/
--rw-rw-rw-   0        0        0      105 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/__init__.py
--rw-rw-rw-   0        0        0     7222 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_session_broker.py
--rw-rw-rw-   0        0        0     3887 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_worker.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.749290 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/
--rw-rw-rw-   0        0        0       74 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/__init__.py
--rw-rw-rw-   0        0        0      144 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/thread_info.py
--rw-rw-rw-   0        0        0      304 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/thread_task.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.765940 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/
--rw-rw-rw-   0        0        0       75 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/__init__.py
--rw-rw-rw-   0        0        0      438 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/parallel_session_broker_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.773990 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/
--rw-rw-rw-   0        0        0      166 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.787618 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/
--rw-rw-rw-   0        0        0       81 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/__init__.py
--rw-rw-rw-   0        0        0     3917 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/single_process_integration_execute.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.795962 pdip-0.6.7/pdip/integrator/integration/types/target/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/target/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.811862 pdip-0.6.7/pdip/integrator/integration/types/target/base/
--rw-rw-rw-   0        0        0       51 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/target/base/__init__.py
--rw-rw-rw-   0        0        0     2684 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/integration/types/target/base/target_integration.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.818863 pdip-0.6.7/pdip/integrator/operation/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/operation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.833900 pdip-0.6.7/pdip/integrator/operation/base/
--rw-rw-rw-   0        0        0       53 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/operation/base/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/operation/base/operation_execution.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.848898 pdip-0.6.7/pdip/integrator/operation/domain/
--rw-rw-rw-   0        0        0       64 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/operation/domain/__init__.py
--rw-rw-rw-   0        0        0      808 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/operation/domain/operation.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.855897 pdip-0.6.7/pdip/integrator/pubsub/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/pubsub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.889546 pdip-0.6.7/pdip/integrator/pubsub/base/
--rw-rw-rw-   0        0        0      183 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/pubsub/base/__init__.py
--rw-rw-rw-   0        0        0      342 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/pubsub/base/channel_queue.py
--rw-rw-rw-   0        0        0     1529 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/pubsub/base/event_listener.py
--rw-rw-rw-   0        0        0     3040 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/pubsub/base/message_broker.py
--rw-rw-rw-   0        0        0     1302 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/pubsub/base/message_broker_worker.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.903545 pdip-0.6.7/pdip/integrator/pubsub/domain/
--rw-rw-rw-   0        0        0       34 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/pubsub/domain/__init__.py
--rw-rw-rw-   0        0        0      168 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/pubsub/domain/message.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.917544 pdip-0.6.7/pdip/integrator/pubsub/publisher/
--rw-rw-rw-   0        0        0       34 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/pubsub/publisher/__init__.py
--rw-rw-rw-   0        0        0      252 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/pubsub/publisher/publisher.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.925543 pdip-0.6.7/pdip/integrator/pubsub/subscriber/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/integrator/pubsub/subscriber/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.947545 pdip-0.6.7/pdip/io/
--rw-rw-rw-   0        0        0       82 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/io/__init__.py
--rw-rw-rw-   0        0        0     1011 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/io/file_manager.py
--rw-rw-rw-   0        0        0     1326 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/io/folder_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.955543 pdip-0.6.7/pdip/json/
--rw-rw-rw-   0        0        0      320 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/json/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:37.978195 pdip-0.6.7/pdip/json/base/
--rw-rw-rw-   0        0        0        0 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/json/base/__init__.py
--rw-rw-rw-   0        0        0     3786 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/json/base/base_converter.py
--rw-rw-rw-   0        0        0     1037 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/json/base/json_convert.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.011193 pdip-0.6.7/pdip/json/encoders/
--rw-rw-rw-   0        0        0        0 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/json/encoders/__init__.py
--rw-rw-rw-   0        0        0      311 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/json/encoders/date_time_encoder.py
--rw-rw-rw-   0        0        0      734 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/json/encoders/mutliple_json_encoders.py
--rw-rw-rw-   0        0        0      272 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/json/encoders/uuid_encoder.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.028193 pdip-0.6.7/pdip/json/parsers/
--rw-rw-rw-   0        0        0        0 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/json/parsers/__init__.py
--rw-rw-rw-   0        0        0      528 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/json/parsers/date_time_parser.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.036191 pdip-0.6.7/pdip/logging/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/logging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.054542 pdip-0.6.7/pdip/logging/domain/
--rw-rw-rw-   0        0        0       31 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/logging/domain/__init__.py
--rw-rw-rw-   0        0        0      499 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/logging/domain/log_data.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.063542 pdip-0.6.7/pdip/logging/loggers/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/logging/loggers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.079316 pdip-0.6.7/pdip/logging/loggers/base/
--rw-rw-rw-   0        0        0       30 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/logging/loggers/base/__init__.py
--rw-rw-rw-   0        0        0     1015 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/logging/loggers/base/ilogger.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.095294 pdip-0.6.7/pdip/logging/loggers/console/
--rw-rw-rw-   0        0        0       43 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/logging/loggers/console/__init__.py
--rw-rw-rw-   0        0        0     1881 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/logging/loggers/console/console_logger.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.109285 pdip-0.6.7/pdip/logging/loggers/file/
--rw-rw-rw-   0        0        0       37 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/logging/loggers/file/__init__.py
--rw-rw-rw-   0        0        0     1977 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/logging/loggers/file/file_logger.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.123287 pdip-0.6.7/pdip/logging/loggers/sql/
--rw-rw-rw-   0        0        0       35 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/logging/loggers/sql/__init__.py
--rw-rw-rw-   0        0        0     4728 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/logging/loggers/sql/sql_logger.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.143291 pdip-0.6.7/pdip/processing/
--rw-rw-rw-   0        0        0       65 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/processing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.182355 pdip-0.6.7/pdip/processing/base/
--rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/processing/base/__init__.py
--rw-rw-rw-   0        0        0     7549 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/processing/base/process_manager.py
--rw-rw-rw-   0        0        0     2430 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/processing/base/subprocess.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.202111 pdip-0.6.7/pdip/processing/factories/
--rw-rw-rw-   0        0        0       60 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/processing/factories/__init__.py
--rw-rw-rw-   0        0        0      418 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/processing/factories/process_manager_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.233783 pdip-0.6.7/pdip/processing/models/
--rw-rw-rw-   0        0        0       78 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/processing/models/__init__.py
--rw-rw-rw-   0        0        0      348 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/processing/models/process_info.py
--rw-rw-rw-   0        0        0      776 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/processing/models/process_task.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:38.262183 pdip-0.6.7/pdip/utils/
--rw-rw-rw-   0        0        0      106 2024-03-22 10:41:09.000000 pdip-0.6.7/pdip/utils/__init__.py
--rw-rw-rw-   0        0        0     6676 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/utils/module_finder.py
--rw-rw-rw-   0        0        0     1531 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/utils/type_checker.py
--rw-rw-rw-   0        0        0     2936 2024-05-02 23:20:07.000000 pdip-0.6.7/pdip/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 01:18:33.979462 pdip-0.6.7/pdip.egg-info/
--rw-rw-rw-   0        0        0     1525 2024-05-03 01:18:33.000000 pdip-0.6.7/pdip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    21598 2024-05-03 01:18:33.000000 pdip-0.6.7/pdip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 01:18:33.000000 pdip-0.6.7/pdip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-03 01:18:33.000000 pdip-0.6.7/pdip.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      475 2024-05-03 01:18:33.000000 pdip-0.6.7/pdip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 01:18:33.000000 pdip-0.6.7/pdip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       69 2024-05-03 01:18:38.273601 pdip-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0     2720 2024-05-03 01:18:09.000000 pdip-0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.523003 pdip-0.6.9/
+-rw-rw-rw-   0        0        0     1097 2024-03-22 10:41:08.000000 pdip-0.6.9/LICENSE
+-rw-rw-rw-   0        0        0     1525 2024-05-10 08:09:23.524117 pdip-0.6.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.483847 pdip-0.6.9/pdip/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.545454 pdip-0.6.9/pdip/api/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.563798 pdip-0.6.9/pdip/api/app/
+-rw-rw-rw-   0        0        0       48 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/app/__init__.py
+-rw-rw-rw-   0        0        0     1941 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/app/flask_app_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.629900 pdip-0.6.9/pdip/api/base/
+-rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/base/__init__.py
+-rw-rw-rw-   0        0        0     3736 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/api/base/controller_base.py
+-rw-rw-rw-   0        0        0     4506 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/base/endpoint_base.py
+-rw-rw-rw-   0        0        0     8865 2024-05-03 12:37:08.000000 pdip-0.6.9/pdip/api/base/endpoint_wrapper.py
+-rw-rw-rw-   0        0        0      172 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/base/resource_base.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.648890 pdip-0.6.9/pdip/api/converter/
+-rw-rw-rw-   0        0        0       49 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/converter/__init__.py
+-rw-rw-rw-   0        0        0     3284 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/converter/request_converter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.664951 pdip-0.6.9/pdip/api/decorators/
+-rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/decorators/__init__.py
+-rw-rw-rw-   0        0        0      240 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/decorators/controller_base.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.686820 pdip-0.6.9/pdip/api/handlers/
+-rw-rw-rw-   0        0        0       88 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3755 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/handlers/error_handlers.py
+-rw-rw-rw-   0        0        0     1515 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/handlers/request_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.711133 pdip-0.6.9/pdip/api/request_parameter/
+-rw-rw-rw-   0        0        0       97 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/request_parameter/__init__.py
+-rw-rw-rw-   0        0        0      124 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/request_parameter/order_by_parameter.py
+-rw-rw-rw-   0        0        0      129 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/request_parameter/paging_parameter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.742192 pdip-0.6.9/pdip/api/specifications/
+-rw-rw-rw-   0        0        0      113 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/specifications/__init__.py
+-rw-rw-rw-   0        0        0     1492 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/specifications/order_by_specification.py
+-rw-rw-rw-   0        0        0     1252 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/api/specifications/paging_specification.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.760239 pdip-0.6.9/pdip/base/
+-rw-rw-rw-   0        0        0       22 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/base/__init__.py
+-rw-rw-rw-   0        0        0     1677 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/base/pdi.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.781599 pdip-0.6.9/pdip/configuration/
+-rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/__init__.py
+-rw-rw-rw-   0        0        0     5293 2024-05-02 23:21:00.000000 pdip-0.6.9/pdip/configuration/config_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.793121 pdip-0.6.9/pdip/configuration/models/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.810027 pdip-0.6.9/pdip/configuration/models/api/
+-rw-rw-rw-   0        0        0       35 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/models/api/__init__.py
+-rw-rw-rw-   0        0        0      334 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/models/api/api_config.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.833096 pdip-0.6.9/pdip/configuration/models/application/
+-rw-rw-rw-   0        0        0       51 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/models/application/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/models/application/application_config.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.868571 pdip-0.6.9/pdip/configuration/models/aps/
+-rw-rw-rw-   0        0        0       35 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/models/aps/__init__.py
+-rw-rw-rw-   0        0        0      380 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/models/aps/aps_config.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.889260 pdip-0.6.9/pdip/configuration/models/base/
+-rw-rw-rw-   0        0        0      236 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/configuration/models/base/__init__.py
+-rw-rw-rw-   0        0        0       87 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/models/base/base_config.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.913794 pdip-0.6.9/pdip/configuration/models/database/
+-rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/models/database/__init__.py
+-rw-rw-rw-   0        0        0      450 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/models/database/database_config.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.949475 pdip-0.6.9/pdip/configuration/services/
+-rw-rw-rw-   0        0        0       99 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/services/__init__.py
+-rw-rw-rw-   0        0        0      482 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/services/config_parameter_base.py
+-rw-rw-rw-   0        0        0     1051 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/configuration/services/config_service.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.054305 pdip-0.6.9/pdip/cqrs/
+-rw-rw-rw-   0        0        0      301 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/__init__.py
+-rw-rw-rw-   0        0        0      162 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/command_query_base.py
+-rw-rw-rw-   0        0        0      331 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/command_query_handler_base.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.108834 pdip-0.6.9/pdip/cqrs/decorators/
+-rw-rw-rw-   0        0        0      117 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/decorators/__init__.py
+-rw-rw-rw-   0        0        0      861 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/decorators/cls_to_dict.py
+-rw-rw-rw-   0        0        0      277 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/cqrs/decorators/dto_class.py
+-rw-rw-rw-   0        0        0      281 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/cqrs/decorators/request_class.py
+-rw-rw-rw-   0        0        0      282 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/cqrs/decorators/response_class.py
+-rw-rw-rw-   0        0        0     1586 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/dispatcher.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.134399 pdip-0.6.9/pdip/cqrs/generator/
+-rw-rw-rw-   0        0        0       66 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.194987 pdip-0.6.9/pdip/cqrs/generator/domain/
+-rw-rw-rw-   0        0        0      187 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/generator/domain/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/generator/domain/dao_generate_config.py
+-rw-rw-rw-   0        0        0      241 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/generator/domain/generate_config.py
+-rw-rw-rw-   0        0        0      167 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/generator/domain/generator.py
+-rw-rw-rw-   0        0        0      198 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/generator/domain/query_generate_config.py
+-rw-rw-rw-   0        0        0    12142 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/generator/query_generator.py
+-rw-rw-rw-   0        0        0      223 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/icommand.py
+-rw-rw-rw-   0        0        0      361 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/icommand_handler.py
+-rw-rw-rw-   0        0        0      221 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/iquery.py
+-rw-rw-rw-   0        0        0      354 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cqrs/iquery_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.221085 pdip-0.6.9/pdip/cryptography/
+-rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     1058 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/cryptography/crypto_service.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.234983 pdip-0.6.9/pdip/data/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.256124 pdip-0.6.9/pdip/data/base/
+-rw-rw-rw-   0        0        0       62 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/data/base/__init__.py
+-rw-rw-rw-   0        0        0     2757 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/data/base/database_session_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.277033 pdip-0.6.9/pdip/data/decorators/
+-rw-rw-rw-   0        0        0       53 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/data/decorators/__init__.py
+-rw-rw-rw-   0        0        0      633 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/data/decorators/transaction_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.312379 pdip-0.6.9/pdip/data/domain/
+-rw-rw-rw-   0        0        0       65 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/data/domain/__init__.py
+-rw-rw-rw-   0        0        0     1245 2024-05-06 06:43:37.000000 pdip-0.6.9/pdip/data/domain/entity.py
+-rw-rw-rw-   0        0        0      908 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/data/domain/entity_base.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.334796 pdip-0.6.9/pdip/data/domain/types/
+-rw-rw-rw-   0        0        0     1154 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/data/domain/types/GUID.py
+-rw-rw-rw-   0        0        0       22 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/data/domain/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.370300 pdip-0.6.9/pdip/data/repository/
+-rw-rw-rw-   0        0        0       89 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/data/repository/__init__.py
+-rw-rw-rw-   0        0        0     2997 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/data/repository/repository.py
+-rw-rw-rw-   0        0        0     2031 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/data/repository/repository_provider.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.408442 pdip-0.6.9/pdip/data/seed/
+-rw-rw-rw-   0        0        0       61 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/data/seed/__init__.py
+-rw-rw-rw-   0        0        0      115 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/data/seed/seed.py
+-rw-rw-rw-   0        0        0     1478 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/data/seed/seed_runner.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.438648 pdip-0.6.9/pdip/delivery/
+-rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/delivery/__init__.py
+-rw-rw-rw-   0        0        0     4042 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/delivery/email_provider.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.465524 pdip-0.6.9/pdip/dependency/
+-rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/dependency/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.505087 pdip-0.6.9/pdip/dependency/container/
+-rw-rw-rw-   0        0        0       55 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/dependency/container/__init__.py
+-rw-rw-rw-   0        0        0      945 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/dependency/container/dependency_container.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.537077 pdip-0.6.9/pdip/dependency/provider/
+-rw-rw-rw-   0        0        0       47 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/dependency/provider/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.567381 pdip-0.6.9/pdip/dependency/provider/api/
+-rw-rw-rw-   0        0        0       39 2024-05-02 23:21:00.000000 pdip-0.6.9/pdip/dependency/provider/api/__init__.py
+-rw-rw-rw-   0        0        0     4257 2024-05-03 00:13:59.000000 pdip-0.6.9/pdip/dependency/provider/api/api_provider.py
+-rw-rw-rw-   0        0        0     6728 2024-05-02 23:21:00.000000 pdip-0.6.9/pdip/dependency/provider/service_provider.py
+-rw-rw-rw-   0        0        0      159 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/dependency/scopes.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.651387 pdip-0.6.9/pdip/exceptions/
+-rw-rw-rw-   0        0        0      268 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/exceptions/__init__.py
+-rw-rw-rw-   0        0        0       58 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/exceptions/incompatible_adapter_exception.py
+-rw-rw-rw-   0        0        0      148 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/exceptions/not_supported_feature_exception.py
+-rw-rw-rw-   0        0        0       50 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/exceptions/operational_exception.py
+-rw-rw-rw-   0        0        0       52 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/exceptions/required_class_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.675499 pdip-0.6.9/pdip/html/
+-rw-rw-rw-   0        0        0       68 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/html/__init__.py
+-rw-rw-rw-   0        0        0     9512 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/html/html_template_service.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.687393 pdip-0.6.9/pdip/integrator/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.705532 pdip-0.6.9/pdip/integrator/base/
+-rw-rw-rw-   0        0        0       36 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/base/__init__.py
+-rw-rw-rw-   0        0        0     2233 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/base/integrator.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.714061 pdip-0.6.9/pdip/integrator/connection/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.738467 pdip-0.6.9/pdip/integrator/connection/base/
+-rw-rw-rw-   0        0        0      128 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/base/__init__.py
+-rw-rw-rw-   0        0        0      668 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/base/connection_source_adapter.py
+-rw-rw-rw-   0        0        0      576 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/base/connection_target_adapter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.747950 pdip-0.6.9/pdip/integrator/connection/domain/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.754076 pdip-0.6.9/pdip/integrator/connection/domain/authentication/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/authentication/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.770643 pdip-0.6.9/pdip/integrator/connection/domain/authentication/basic/
+-rw-rw-rw-   0        0        0       76 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/authentication/basic/__init__.py
+-rw-rw-rw-   0        0        0      137 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/authentication/basic/connection_basic_authentication.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.790975 pdip-0.6.9/pdip/integrator/connection/domain/authentication/kerberos/
+-rw-rw-rw-   0        0        0       61 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/authentication/kerberos/__init__.py
+-rw-rw-rw-   0        0        0      218 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/authentication/kerberos/kerberos_authentication.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.809775 pdip-0.6.9/pdip/integrator/connection/domain/authentication/mechanism/
+-rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/authentication/mechanism/__init__.py
+-rw-rw-rw-   0        0        0      144 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/authentication/mechanism/mechanism_types.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.827905 pdip-0.6.9/pdip/integrator/connection/domain/authentication/type/
+-rw-rw-rw-   0        0        0       55 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/authentication/type/__init__.py
+-rw-rw-rw-   0        0        0      134 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/authentication/type/authentication_types.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.850169 pdip-0.6.9/pdip/integrator/connection/domain/base/
+-rw-rw-rw-   0        0        0       42 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/base/__init__.py
+-rw-rw-rw-   0        0        0      263 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/base/column.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.885710 pdip-0.6.9/pdip/integrator/connection/domain/enums/
+-rw-rw-rw-   0        0        0       92 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/enums/__init__.py
+-rw-rw-rw-   0        0        0      154 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/enums/connection_types.py
+-rw-rw-rw-   0        0        0      233 2024-05-02 23:21:00.000000 pdip-0.6.9/pdip/integrator/connection/domain/enums/connector_types.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.897284 pdip-0.6.9/pdip/integrator/connection/domain/server/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/server/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.917719 pdip-0.6.9/pdip/integrator/connection/domain/server/base/
+-rw-rw-rw-   0        0        0       49 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/server/base/__init__.py
+-rw-rw-rw-   0        0        0      120 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/server/base/connection_server.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.938746 pdip-0.6.9/pdip/integrator/connection/domain/task/
+-rw-rw-rw-   0        0        0       44 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/task/__init__.py
+-rw-rw-rw-   0        0        0      406 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/task/data_queue_task.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.948835 pdip-0.6.9/pdip/integrator/connection/domain/types/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.956968 pdip-0.6.9/pdip/integrator/connection/domain/types/bigdata/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/bigdata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.975150 pdip-0.6.9/pdip/integrator/connection/domain/types/bigdata/base/
+-rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/bigdata/base/__init__.py
+-rw-rw-rw-   0        0        0      337 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/bigdata/base/big_data.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:20.985201 pdip-0.6.9/pdip/integrator/connection/domain/types/bigdata/configuration/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/bigdata/configuration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.000653 pdip-0.6.9/pdip/integrator/connection/domain/types/bigdata/configuration/base/
+-rw-rw-rw-   0        0        0       79 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/bigdata/configuration/base/__init__.py
+-rw-rw-rw-   0        0        0      902 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/bigdata/configuration/base/big_data_connection_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.023898 pdip-0.6.9/pdip/integrator/connection/domain/types/inmemory/
+-rw-rw-rw-   0        0        0       81 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/inmemory/__init__.py
+-rw-rw-rw-   0        0        0      346 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/inmemory/in_memory_connection_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.033913 pdip-0.6.9/pdip/integrator/connection/domain/types/sql/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.051371 pdip-0.6.9/pdip/integrator/connection/domain/types/sql/base/
+-rw-rw-rw-   0        0        0       36 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/sql/base/__init__.py
+-rw-rw-rw-   0        0        0      325 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/sql/base/sql.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.064068 pdip-0.6.9/pdip/integrator/connection/domain/types/sql/configuration/
+-rw-rw-rw-   0        0        0        2 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/sql/configuration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.085381 pdip-0.6.9/pdip/integrator/connection/domain/types/sql/configuration/base/
+-rw-rw-rw-   0        0        0       70 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/sql/configuration/base/__init__.py
+-rw-rw-rw-   0        0        0      855 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/sql/configuration/base/sql_connection_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.099913 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.121230 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/base/
+-rw-rw-rw-   0        0        0       51 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/base/__init__.py
+-rw-rw-rw-   0        0        0      314 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/base/web_service.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.131512 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/configuration/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/configuration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.150336 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/configuration/base/
+-rw-rw-rw-   0        0        0       85 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/configuration/base/__init__.py
+-rw-rw-rw-   0        0        0      572 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/configuration/base/web_service_connection_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.169041 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/configuration/soap/
+-rw-rw-rw-   0        0        0       51 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/configuration/soap/__init__.py
+-rw-rw-rw-   0        0        0       99 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/configuration/soap/soap_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.202945 pdip-0.6.9/pdip/integrator/connection/factories/
+-rw-rw-rw-   0        0        0      158 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/factories/__init__.py
+-rw-rw-rw-   0        0        0     3095 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/factories/connection_source_adapter_factory.py
+-rw-rw-rw-   0        0        0     3466 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/factories/connection_target_adapter_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.216732 pdip-0.6.9/pdip/integrator/connection/types/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.230069 pdip-0.6.9/pdip/integrator/connection/types/bigdata/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.241608 pdip-0.6.9/pdip/integrator/connection/types/bigdata/adapters/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.268091 pdip-0.6.9/pdip/integrator/connection/types/bigdata/adapters/source/
+-rw-rw-rw-   0        0        0       59 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/adapters/source/__init__.py
+-rw-rw-rw-   0        0        0     4642 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/adapters/source/big_data_source_adapter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.291803 pdip-0.6.9/pdip/integrator/connection/types/bigdata/adapters/target/
+-rw-rw-rw-   0        0        0       59 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/adapters/target/__init__.py
+-rw-rw-rw-   0        0        0     4589 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/adapters/target/big_data_target_adapter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.367711 pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/
+-rw-rw-rw-   0        0        0      282 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/__init__.py
+-rw-rw-rw-   0        0        0      458 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/big_data_connector.py
+-rw-rw-rw-   0        0        0     9560 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/big_data_context.py
+-rw-rw-rw-   0        0        0     2014 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/big_data_dialect.py
+-rw-rw-rw-   0        0        0     1842 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/big_data_iterator.py
+-rw-rw-rw-   0        0        0     1450 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/big_data_policy.py
+-rw-rw-rw-   0        0        0     2238 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/big_data_provider.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.379228 pdip-0.6.9/pdip/integrator/connection/types/bigdata/connectors/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.398012 pdip-0.6.9/pdip/integrator/connection/types/bigdata/connectors/impala/
+-rw-rw-rw-   0        0        0       47 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/connectors/impala/__init__.py
+-rw-rw-rw-   0        0        0     3597 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/connectors/impala/impala_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.408869 pdip-0.6.9/pdip/integrator/connection/types/bigdata/dialects/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.429213 pdip-0.6.9/pdip/integrator/connection/types/bigdata/dialects/impala/
+-rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/dialects/impala/__init__.py
+-rw-rw-rw-   0        0        0     5185 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/bigdata/dialects/impala/impala_dialect.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.441910 pdip-0.6.9/pdip/integrator/connection/types/file/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/file/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.457977 pdip-0.6.9/pdip/integrator/connection/types/file/adapters/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/file/adapters/__init__.py
+-rw-rw-rw-   0        0        0     8832 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/file/adapters/file_adapter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.500479 pdip-0.6.9/pdip/integrator/connection/types/file/base/
+-rw-rw-rw-   0        0        0      123 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/file/base/__init__.py
+-rw-rw-rw-   0        0        0     1061 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/file/base/file_connector.py
+-rw-rw-rw-   0        0        0     3837 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/file/base/file_context.py
+-rw-rw-rw-   0        0        0     1938 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/file/base/file_provider.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.511109 pdip-0.6.9/pdip/integrator/connection/types/file/connectors/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/file/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.529022 pdip-0.6.9/pdip/integrator/connection/types/file/connectors/csv/
+-rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/file/connectors/csv/__init__.py
+-rw-rw-rw-   0        0        0     3384 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/file/connectors/csv/csv_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.540064 pdip-0.6.9/pdip/integrator/connection/types/inmemory/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/inmemory/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.597510 pdip-0.6.9/pdip/integrator/connection/types/inmemory/base/
+-rw-rw-rw-   0        0        0      196 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/inmemory/base/__init__.py
+-rw-rw-rw-   0        0        0     1273 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/inmemory/base/in_memory_connector.py
+-rw-rw-rw-   0        0        0     4465 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/inmemory/base/in_memory_context.py
+-rw-rw-rw-   0        0        0     1056 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/inmemory/base/in_memory_policy.py
+-rw-rw-rw-   0        0        0     1361 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/inmemory/base/in_memory_provider.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.609776 pdip-0.6.9/pdip/integrator/connection/types/inmemory/connectors/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/inmemory/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.629124 pdip-0.6.9/pdip/integrator/connection/types/inmemory/connectors/sqlite/
+-rw-rw-rw-   0        0        0       48 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/inmemory/connectors/sqlite/__init__.py
+-rw-rw-rw-   0        0        0     1523 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/inmemory/connectors/sqlite/sq_lite_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.640580 pdip-0.6.9/pdip/integrator/connection/types/queue/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.668860 pdip-0.6.9/pdip/integrator/connection/types/queue/adapters/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/queue/adapters/__init__.py
+-rw-rw-rw-   0        0        0     4288 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/queue/adapters/queue_adapter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.717241 pdip-0.6.9/pdip/integrator/connection/types/queue/base/
+-rw-rw-rw-   0        0        0      129 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/queue/base/__init__.py
+-rw-rw-rw-   0        0        0     1094 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/queue/base/queue_connector.py
+-rw-rw-rw-   0        0        0     2257 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/queue/base/queue_context.py
+-rw-rw-rw-   0        0        0     2016 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/queue/base/queue_provider.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.739384 pdip-0.6.9/pdip/integrator/connection/types/queue/connectors/
+-rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/queue/connectors/__init__.py
+-rw-rw-rw-   0        0        0     6970 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/queue/connectors/kafka_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.749203 pdip-0.6.9/pdip/integrator/connection/types/sql/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.756431 pdip-0.6.9/pdip/integrator/connection/types/sql/adapters/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.776434 pdip-0.6.9/pdip/integrator/connection/types/sql/adapters/source/
+-rw-rw-rw-   0        0        0       50 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/adapters/source/__init__.py
+-rw-rw-rw-   0        0        0     3820 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/adapters/source/sql_source_adapter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.799896 pdip-0.6.9/pdip/integrator/connection/types/sql/adapters/target/
+-rw-rw-rw-   0        0        0       50 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/adapters/target/__init__.py
+-rw-rw-rw-   0        0        0     3672 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/adapters/target/sql_target_adapter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.870323 pdip-0.6.9/pdip/integrator/connection/types/sql/base/
+-rw-rw-rw-   0        0        0      228 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/base/__init__.py
+-rw-rw-rw-   0        0        0      478 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/base/sql_connector.py
+-rw-rw-rw-   0        0        0     9467 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/base/sql_context.py
+-rw-rw-rw-   0        0        0     2014 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/base/sql_dialect.py
+-rw-rw-rw-   0        0        0     1797 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/base/sql_iterator.py
+-rw-rw-rw-   0        0        0     2188 2024-05-02 23:21:00.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/base/sql_policy.py
+-rw-rw-rw-   0        0        0     4383 2024-05-02 23:21:00.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/base/sql_provider.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.881564 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.899824 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/clickhouse/
+-rw-rw-rw-   0        0        0       55 2024-05-02 23:21:00.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/clickhouse/__init__.py
+-rw-rw-rw-   0        0        0     3357 2024-05-02 23:21:00.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/clickhouse/clickhouse_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.918912 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/mssql/
+-rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/mssql/__init__.py
+-rw-rw-rw-   0        0        0     3340 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/mssql/mssql_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.946301 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/mysql/
+-rw-rw-rw-   0        0        0       45 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/mysql/__init__.py
+-rw-rw-rw-   0        0        0     2113 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/mysql/mysql_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:21.988060 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/oracle/
+-rw-rw-rw-   0        0        0       47 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/oracle/__init__.py
+-rw-rw-rw-   0        0        0     2640 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/oracle/oracle_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.031543 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/postgresql/
+-rw-rw-rw-   0        0        0       55 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/postgresql/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/postgresql/postgresql_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.049980 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.071730 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/clickhouse/
+-rw-rw-rw-   0        0        0       51 2024-05-02 23:21:00.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/clickhouse/__init__.py
+-rw-rw-rw-   0        0        0     5224 2024-05-02 23:21:00.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/clickhouse/clickhouse_dialect.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.095731 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/mssql/
+-rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/mssql/__init__.py
+-rw-rw-rw-   0        0        0     5467 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/mssql/mssql_dialect.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.121697 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/mysql/
+-rw-rw-rw-   0        0        0       41 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/mysql/__init__.py
+-rw-rw-rw-   0        0        0     5129 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/mysql/mysql_dialect.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.148657 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/oracle/
+-rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/oracle/__init__.py
+-rw-rw-rw-   0        0        0     5434 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/oracle/oracle_dialect.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.170863 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/postgresql/
+-rw-rw-rw-   0        0        0       51 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/postgresql/__init__.py
+-rw-rw-rw-   0        0        0     5225 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/postgresql/postgresql_dialect.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.180752 pdip-0.6.9/pdip/integrator/connection/types/webservice/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.188161 pdip-0.6.9/pdip/integrator/connection/types/webservice/adapters/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.205467 pdip-0.6.9/pdip/integrator/connection/types/webservice/adapters/source/
+-rw-rw-rw-   0        0        0       65 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/adapters/source/__init__.py
+-rw-rw-rw-   0        0        0     1079 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/adapters/source/web_service_source_adapter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.229808 pdip-0.6.9/pdip/integrator/connection/types/webservice/adapters/target/
+-rw-rw-rw-   0        0        0       65 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/adapters/target/__init__.py
+-rw-rw-rw-   0        0        0     3434 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/adapters/target/web_service_target_adapter.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.288894 pdip-0.6.9/pdip/integrator/connection/types/webservice/base/
+-rw-rw-rw-   0        0        0      212 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/base/__init__.py
+-rw-rw-rw-   0        0        0      540 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/base/web_service_connector.py
+-rw-rw-rw-   0        0        0     1779 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/base/web_service_context.py
+-rw-rw-rw-   0        0        0     1061 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/base/web_service_policy.py
+-rw-rw-rw-   0        0        0     1991 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/base/web_service_provider.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.300390 pdip-0.6.9/pdip/integrator/connection/types/webservice/connectors/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.319738 pdip-0.6.9/pdip/integrator/connection/types/webservice/connectors/soap/
+-rw-rw-rw-   0        0        0       43 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/connectors/soap/__init__.py
+-rw-rw-rw-   0        0        0     2122 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/connection/types/webservice/connectors/soap/soap_connector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.329279 pdip-0.6.9/pdip/integrator/domain/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.358507 pdip-0.6.9/pdip/integrator/domain/enums/
+-rw-rw-rw-   0        0        0       39 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/domain/enums/__init__.py
+-rw-rw-rw-   0        0        0      437 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/domain/enums/events.py
+-rw-rw-rw-   0        0        0      120 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/domain/enums/status_types.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.369477 pdip-0.6.9/pdip/integrator/event/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/event/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.416417 pdip-0.6.9/pdip/integrator/event/base/
+-rw-rw-rw-   0        0        0      216 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/event/base/__init__.py
+-rw-rw-rw-   0        0        0     3100 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/event/base/default_integrator_event_manager.py
+-rw-rw-rw-   0        0        0     1250 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/event/base/integrator_event_manager.py
+-rw-rw-rw-   0        0        0     1029 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/event/base/integrator_event_manager_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.426052 pdip-0.6.9/pdip/integrator/execution/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/execution/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.433958 pdip-0.6.9/pdip/integrator/execution/base/
+-rw-rw-rw-   0        0        0        2 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/execution/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.451635 pdip-0.6.9/pdip/integrator/execution/domain/
+-rw-rw-rw-   0        0        0      284 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/execution/domain/__init__.py
+-rw-rw-rw-   0        0        0     1080 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/execution/domain/execution.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.460434 pdip-0.6.9/pdip/integrator/initializer/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.476033 pdip-0.6.9/pdip/integrator/initializer/base/
+-rw-rw-rw-   0        0        0       38 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/base/__init__.py
+-rw-rw-rw-   0        0        0       60 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/base/initializer.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.484666 pdip-0.6.9/pdip/integrator/initializer/execution/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.519935 pdip-0.6.9/pdip/integrator/initializer/execution/base/
+-rw-rw-rw-   0        0        0      129 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/base/__init__.py
+-rw-rw-rw-   0        0        0     1457 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/base/default_execution_initializer.py
+-rw-rw-rw-   0        0        0      386 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/base/execution_initializer.py
+-rw-rw-rw-   0        0        0     1013 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/base/execution_initializer_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.556608 pdip-0.6.9/pdip/integrator/initializer/execution/integration/
+-rw-rw-rw-   0        0        0      327 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/integration/__init__.py
+-rw-rw-rw-   0        0        0      533 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/integration/default_operation_integration_execution_initializer.py
+-rw-rw-rw-   0        0        0      331 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer.py
+-rw-rw-rw-   0        0        0     1217 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.600779 pdip-0.6.9/pdip/integrator/initializer/execution/operation/
+-rw-rw-rw-   0        0        0      258 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/operation/__init__.py
+-rw-rw-rw-   0        0        0      431 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/operation/default_operation_execution_initializer.py
+-rw-rw-rw-   0        0        0      275 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/operation/operation_execution_initializer.py
+-rw-rw-rw-   0        0        0     1127 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/execution/operation/operation_execution_initializer_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.637433 pdip-0.6.9/pdip/integrator/initializer/integrator/
+-rw-rw-rw-   0        0        0      207 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/integrator/__init__.py
+-rw-rw-rw-   0        0        0     3286 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/integrator/default_integrator_initializer.py
+-rw-rw-rw-   0        0        0      469 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/integrator/integrator_initializer.py
+-rw-rw-rw-   0        0        0     1019 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/initializer/integrator/integrator_initializer_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.645081 pdip-0.6.9/pdip/integrator/integration/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.660998 pdip-0.6.9/pdip/integrator/integration/base/
+-rw-rw-rw-   0        0        0       57 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/base/__init__.py
+-rw-rw-rw-   0        0        0     3845 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/base/integration_execution.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.671050 pdip-0.6.9/pdip/integrator/integration/domain/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.687436 pdip-0.6.9/pdip/integrator/integration/domain/base/
+-rw-rw-rw-   0        0        0       94 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/domain/base/__init__.py
+-rw-rw-rw-   0        0        0     1031 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/domain/base/integration.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.703139 pdip-0.6.9/pdip/integrator/integration/domain/enums/
+-rw-rw-rw-   0        0        0       49 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/domain/enums/__init__.py
+-rw-rw-rw-   0        0        0      114 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/domain/enums/integration_types.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.708714 pdip-0.6.9/pdip/integrator/integration/types/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.734182 pdip-0.6.9/pdip/integrator/integration/types/base/
+-rw-rw-rw-   0        0        0      121 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/types/base/__init__.py
+-rw-rw-rw-   0        0        0      728 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/types/base/integration_adapter.py
+-rw-rw-rw-   0        0        0     1845 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/types/base/integration_adapter_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.741181 pdip-0.6.9/pdip/integrator/integration/types/source/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:08.000000 pdip-0.6.9/pdip/integrator/integration/types/source/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.755378 pdip-0.6.9/pdip/integrator/integration/types/source/base/
+-rw-rw-rw-   0        0        0       51 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/source/base/__init__.py
+-rw-rw-rw-   0        0        0     5127 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/source/base/source_integration.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.764298 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.779249 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/base/
+-rw-rw-rw-   0        0        0       69 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/base/__init__.py
+-rw-rw-rw-   0        0        0     6664 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/base/source_to_target_integration.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.788257 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.803817 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/base/
+-rw-rw-rw-   0        0        0      101 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/base/__init__.py
+-rw-rw-rw-   0        0        0      537 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/base/integration_source_to_target_execute_strategy.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.821381 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/factories/
+-rw-rw-rw-   0        0        0       99 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/factories/__init__.py
+-rw-rw-rw-   0        0        0     1723 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/factories/integration_execute_strategy_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.832810 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.848113 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/
+-rw-rw-rw-   0        0        0       70 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/__init__.py
+-rw-rw-rw-   0        0        0    18820 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/parallel_integration_execute.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.857155 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.871533 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/
+-rw-rw-rw-   0        0        0       83 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/__init__.py
+-rw-rw-rw-   0        0        0     7431 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/parallel_thread_integration_execute.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.882533 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.898110 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/
+-rw-rw-rw-   0        0        0       56 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/__init__.py
+-rw-rw-rw-   0        0        0     4368 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/source_read_operation.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.916246 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/
+-rw-rw-rw-   0        0        0       58 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/__init__.py
+-rw-rw-rw-   0        0        0     8709 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/target_write_operation.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.925763 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.954275 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/
+-rw-rw-rw-   0        0        0      105 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/__init__.py
+-rw-rw-rw-   0        0        0     7222 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_session_broker.py
+-rw-rw-rw-   0        0        0     3887 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_worker.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.980279 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/
+-rw-rw-rw-   0        0        0       74 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/__init__.py
+-rw-rw-rw-   0        0        0      144 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/thread_info.py
+-rw-rw-rw-   0        0        0      304 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/thread_task.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:22.997620 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/
+-rw-rw-rw-   0        0        0       75 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/__init__.py
+-rw-rw-rw-   0        0        0      438 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/parallel_session_broker_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.005164 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/
+-rw-rw-rw-   0        0        0      166 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.022062 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/
+-rw-rw-rw-   0        0        0       81 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/__init__.py
+-rw-rw-rw-   0        0        0     3917 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/single_process_integration_execute.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.037867 pdip-0.6.9/pdip/integrator/integration/types/target/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/target/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.053229 pdip-0.6.9/pdip/integrator/integration/types/target/base/
+-rw-rw-rw-   0        0        0       51 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/target/base/__init__.py
+-rw-rw-rw-   0        0        0     2684 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/integration/types/target/base/target_integration.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.063753 pdip-0.6.9/pdip/integrator/operation/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/operation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.078038 pdip-0.6.9/pdip/integrator/operation/base/
+-rw-rw-rw-   0        0        0       53 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/operation/base/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/operation/base/operation_execution.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.096670 pdip-0.6.9/pdip/integrator/operation/domain/
+-rw-rw-rw-   0        0        0       64 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/operation/domain/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/operation/domain/operation.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.106325 pdip-0.6.9/pdip/integrator/pubsub/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/pubsub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.146797 pdip-0.6.9/pdip/integrator/pubsub/base/
+-rw-rw-rw-   0        0        0      183 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/pubsub/base/__init__.py
+-rw-rw-rw-   0        0        0      342 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/pubsub/base/channel_queue.py
+-rw-rw-rw-   0        0        0     1529 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/pubsub/base/event_listener.py
+-rw-rw-rw-   0        0        0     3040 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/pubsub/base/message_broker.py
+-rw-rw-rw-   0        0        0     1302 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/pubsub/base/message_broker_worker.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.164589 pdip-0.6.9/pdip/integrator/pubsub/domain/
+-rw-rw-rw-   0        0        0       34 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/pubsub/domain/__init__.py
+-rw-rw-rw-   0        0        0      168 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/pubsub/domain/message.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.183007 pdip-0.6.9/pdip/integrator/pubsub/publisher/
+-rw-rw-rw-   0        0        0       34 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/pubsub/publisher/__init__.py
+-rw-rw-rw-   0        0        0      252 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/pubsub/publisher/publisher.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.191424 pdip-0.6.9/pdip/integrator/pubsub/subscriber/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/integrator/pubsub/subscriber/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.214532 pdip-0.6.9/pdip/io/
+-rw-rw-rw-   0        0        0       82 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/io/__init__.py
+-rw-rw-rw-   0        0        0     1011 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/io/file_manager.py
+-rw-rw-rw-   0        0        0     1326 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/io/folder_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.224230 pdip-0.6.9/pdip/json/
+-rw-rw-rw-   0        0        0      320 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/json/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.251713 pdip-0.6.9/pdip/json/base/
+-rw-rw-rw-   0        0        0        0 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/json/base/__init__.py
+-rw-rw-rw-   0        0        0     3786 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/json/base/base_converter.py
+-rw-rw-rw-   0        0        0     1037 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/json/base/json_convert.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.284143 pdip-0.6.9/pdip/json/encoders/
+-rw-rw-rw-   0        0        0        0 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/json/encoders/__init__.py
+-rw-rw-rw-   0        0        0      311 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/json/encoders/date_time_encoder.py
+-rw-rw-rw-   0        0        0      734 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/json/encoders/mutliple_json_encoders.py
+-rw-rw-rw-   0        0        0      272 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/json/encoders/uuid_encoder.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.300730 pdip-0.6.9/pdip/json/parsers/
+-rw-rw-rw-   0        0        0        0 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/json/parsers/__init__.py
+-rw-rw-rw-   0        0        0      528 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/json/parsers/date_time_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.309249 pdip-0.6.9/pdip/logging/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/logging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.324327 pdip-0.6.9/pdip/logging/domain/
+-rw-rw-rw-   0        0        0       31 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/logging/domain/__init__.py
+-rw-rw-rw-   0        0        0      499 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/logging/domain/log_data.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.334949 pdip-0.6.9/pdip/logging/loggers/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/logging/loggers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.349088 pdip-0.6.9/pdip/logging/loggers/base/
+-rw-rw-rw-   0        0        0       30 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/logging/loggers/base/__init__.py
+-rw-rw-rw-   0        0        0     1015 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/logging/loggers/base/ilogger.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.370265 pdip-0.6.9/pdip/logging/loggers/console/
+-rw-rw-rw-   0        0        0       43 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/logging/loggers/console/__init__.py
+-rw-rw-rw-   0        0        0     1881 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/logging/loggers/console/console_logger.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.386031 pdip-0.6.9/pdip/logging/loggers/file/
+-rw-rw-rw-   0        0        0       37 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/logging/loggers/file/__init__.py
+-rw-rw-rw-   0        0        0     1977 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/logging/loggers/file/file_logger.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.404735 pdip-0.6.9/pdip/logging/loggers/sql/
+-rw-rw-rw-   0        0        0       35 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/logging/loggers/sql/__init__.py
+-rw-rw-rw-   0        0        0     4728 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/logging/loggers/sql/sql_logger.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.414587 pdip-0.6.9/pdip/processing/
+-rw-rw-rw-   0        0        0       65 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/processing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.437555 pdip-0.6.9/pdip/processing/base/
+-rw-rw-rw-   0        0        0        0 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/processing/base/__init__.py
+-rw-rw-rw-   0        0        0     7549 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/processing/base/process_manager.py
+-rw-rw-rw-   0        0        0     2430 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/processing/base/subprocess.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.454230 pdip-0.6.9/pdip/processing/factories/
+-rw-rw-rw-   0        0        0       60 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/processing/factories/__init__.py
+-rw-rw-rw-   0        0        0      418 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/processing/factories/process_manager_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.482214 pdip-0.6.9/pdip/processing/models/
+-rw-rw-rw-   0        0        0       78 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/processing/models/__init__.py
+-rw-rw-rw-   0        0        0      348 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/processing/models/process_info.py
+-rw-rw-rw-   0        0        0      776 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/processing/models/process_task.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:23.516994 pdip-0.6.9/pdip/utils/
+-rw-rw-rw-   0        0        0      106 2024-03-22 10:41:09.000000 pdip-0.6.9/pdip/utils/__init__.py
+-rw-rw-rw-   0        0        0     6676 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/utils/module_finder.py
+-rw-rw-rw-   0        0        0     1531 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/utils/type_checker.py
+-rw-rw-rw-   0        0        0     2936 2024-05-02 23:20:07.000000 pdip-0.6.9/pdip/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:09:19.536775 pdip-0.6.9/pdip.egg-info/
+-rw-rw-rw-   0        0        0     1525 2024-05-10 08:09:18.000000 pdip-0.6.9/pdip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    21598 2024-05-10 08:09:18.000000 pdip-0.6.9/pdip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:09:18.000000 pdip-0.6.9/pdip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-10 08:09:18.000000 pdip-0.6.9/pdip.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      475 2024-05-10 08:09:18.000000 pdip-0.6.9/pdip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-10 08:09:18.000000 pdip-0.6.9/pdip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       69 2024-05-10 08:09:23.531127 pdip-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     2720 2024-05-10 06:53:37.000000 pdip-0.6.9/setup.py
```

### Comparing `pdip-0.6.7/LICENSE` & `pdip-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/PKG-INFO` & `pdip-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pdip
-Version: 0.6.7
+Version: 0.6.9
 Summary: Python Data Integrator infrastructures package
 Home-page: https://github.com/ahmetcagriakca/pdip
 Author: Ahmet Çağrı AKCA
 Author-email: ahmetcagriakca@gmail.com
 License: MIT
-Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/v0.6.7.tar.gz
+Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/v0.6.9.tar.gz
 Project-URL: Bug Reports, https://github.com/ahmetcagriakca/pdip/issues
 Project-URL: Source, https://github.com/ahmetcagriakca/pdip
 Description: <p align="left">
         	<a href="https://pypi.org/project/pdip" target="_blank">
         			<img src="https://img.shields.io/pypi/v/pdip?color=%2334D058&label=pypi%20package" alt="Package version">
         	</a>
         </p>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: pdip Version: 0.6.7 Summary: Python Data Integrator
+Metadata-Version: 2.1 Name: pdip Version: 0.6.9 Summary: Python Data Integrator
 infrastructures package Home-page: https://github.com/ahmetcagriakca/pdip
 Author: Ahmet ÃaÄrÄ± AKCA Author-email: ahmetcagriakca@gmail.com License: MIT
 Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/
-v0.6.7.tar.gz Project-URL: Bug Reports, https://github.com/ahmetcagriakca/pdip/
+v0.6.9.tar.gz Project-URL: Bug Reports, https://github.com/ahmetcagriakca/pdip/
 issues Project-URL: Source, https://github.com/ahmetcagriakca/pdip Description:
 _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
 # Introduction This package aim to perform the integration processes easily
 Keywords:
 PDI,API,ETL,PROCESS,MULTIPROCESS,IO,CQRS,MSSQL,ORACLE,POSTGRES,MYSQL,CSV
 Platform: UNKNOWN Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
```

### Comparing `pdip-0.6.7/pdip/api/app/flask_app_wrapper.py` & `pdip-0.6.9/pdip/api/app/flask_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/api/base/controller_base.py` & `pdip-0.6.9/pdip/api/base/controller_base.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/api/base/endpoint_base.py` & `pdip-0.6.9/pdip/api/base/endpoint_base.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/api/base/endpoint_wrapper.py` & `pdip-0.6.9/pdip/api/base/endpoint_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import typing
 from datetime import datetime
-
+import uuid
 from flask import request
 from flask_restx import Api, fields, inputs
 from flask_restx.reqparse import RequestParser, Argument
 from injector import inject
 
 from ...api.converter import RequestConverter
 from ...api.request_parameter import OrderByParameter
@@ -34,14 +34,16 @@
             'Result': fields.Raw(description='Service result values'),
         })
 
     @staticmethod
     def date_converter(o):
         if isinstance(o, datetime):
             return o.isoformat()
+        if isinstance(o, uuid.UUID):
+            return str(o)
 
     @staticmethod
     def get_response(result=None, message=None):
         return {'Result': result, 'Message': message}
 
     def field_resolver(self, value, key):
```

### Comparing `pdip-0.6.7/pdip/api/converter/request_converter.py` & `pdip-0.6.9/pdip/api/converter/request_converter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/api/handlers/error_handlers.py` & `pdip-0.6.9/pdip/api/handlers/error_handlers.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/api/handlers/request_handler.py` & `pdip-0.6.9/pdip/api/handlers/request_handler.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/api/specifications/order_by_specification.py` & `pdip-0.6.9/pdip/api/specifications/order_by_specification.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/api/specifications/paging_specification.py` & `pdip-0.6.9/pdip/api/specifications/paging_specification.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/base/pdi.py` & `pdip-0.6.9/pdip/base/pdi.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/configuration/config_manager.py` & `pdip-0.6.9/pdip/configuration/config_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/configuration/services/config_service.py` & `pdip-0.6.9/pdip/configuration/services/config_service.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/cqrs/decorators/cls_to_dict.py` & `pdip-0.6.9/pdip/cqrs/decorators/cls_to_dict.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/cqrs/dispatcher.py` & `pdip-0.6.9/pdip/cqrs/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/cqrs/generator/query_generator.py` & `pdip-0.6.9/pdip/cqrs/generator/query_generator.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/cryptography/crypto_service.py` & `pdip-0.6.9/pdip/cryptography/crypto_service.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/data/base/database_session_manager.py` & `pdip-0.6.9/pdip/data/base/database_session_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/data/decorators/transaction_handler.py` & `pdip-0.6.9/pdip/data/decorators/transaction_handler.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/data/domain/entity.py` & `pdip-0.6.9/pdip/data/domain/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from sqlalchemy.ext.declarative import declared_attr
 
 from .entity_base import EntityBase
 from .types import GUID
 
 
 class Entity(EntityBase):
+    __allow_unmapped__ = True
+    
     Id = Column(
         GUID(),
         primary_key=True,
         default=lambda: str(uuid.uuid4())
     )
 
     @declared_attr
```

### Comparing `pdip-0.6.7/pdip/data/domain/entity_base.py` & `pdip-0.6.9/pdip/data/domain/entity_base.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/data/domain/types/GUID.py` & `pdip-0.6.9/pdip/data/domain/types/GUID.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/data/repository/repository.py` & `pdip-0.6.9/pdip/data/repository/repository.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/data/repository/repository_provider.py` & `pdip-0.6.9/pdip/data/repository/repository_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/data/seed/seed_runner.py` & `pdip-0.6.9/pdip/data/seed/seed_runner.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/delivery/email_provider.py` & `pdip-0.6.9/pdip/delivery/email_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/dependency/container/dependency_container.py` & `pdip-0.6.9/pdip/dependency/container/dependency_container.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/dependency/provider/api/api_provider.py` & `pdip-0.6.9/pdip/dependency/provider/api/api_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/dependency/provider/service_provider.py` & `pdip-0.6.9/pdip/dependency/provider/service_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/html/html_template_service.py` & `pdip-0.6.9/pdip/html/html_template_service.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/base/integrator.py` & `pdip-0.6.9/pdip/integrator/base/integrator.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/base/connection_source_adapter.py` & `pdip-0.6.9/pdip/integrator/connection/base/connection_source_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/base/connection_target_adapter.py` & `pdip-0.6.9/pdip/integrator/connection/base/connection_target_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/domain/types/bigdata/configuration/base/big_data_connection_configuration.py` & `pdip-0.6.9/pdip/integrator/connection/domain/types/bigdata/configuration/base/big_data_connection_configuration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/domain/types/sql/configuration/base/sql_connection_configuration.py` & `pdip-0.6.9/pdip/integrator/connection/domain/types/sql/configuration/base/sql_connection_configuration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/domain/types/webservice/configuration/base/web_service_connection_configuration.py` & `pdip-0.6.9/pdip/integrator/connection/domain/types/webservice/configuration/base/web_service_connection_configuration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/factories/connection_source_adapter_factory.py` & `pdip-0.6.9/pdip/integrator/connection/factories/connection_source_adapter_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/factories/connection_target_adapter_factory.py` & `pdip-0.6.9/pdip/integrator/connection/factories/connection_target_adapter_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/bigdata/adapters/source/big_data_source_adapter.py` & `pdip-0.6.9/pdip/integrator/connection/types/bigdata/adapters/source/big_data_source_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/bigdata/adapters/target/big_data_target_adapter.py` & `pdip-0.6.9/pdip/integrator/connection/types/bigdata/adapters/target/big_data_target_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/big_data_context.py` & `pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/big_data_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/big_data_dialect.py` & `pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/big_data_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/big_data_iterator.py` & `pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/big_data_iterator.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/big_data_policy.py` & `pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/big_data_policy.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/bigdata/base/big_data_provider.py` & `pdip-0.6.9/pdip/integrator/connection/types/bigdata/base/big_data_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/bigdata/connectors/impala/impala_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/bigdata/connectors/impala/impala_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/bigdata/dialects/impala/impala_dialect.py` & `pdip-0.6.9/pdip/integrator/connection/types/bigdata/dialects/impala/impala_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/file/adapters/file_adapter.py` & `pdip-0.6.9/pdip/integrator/connection/types/file/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/file/base/file_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/file/base/file_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/file/base/file_context.py` & `pdip-0.6.9/pdip/integrator/connection/types/file/base/file_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/file/base/file_provider.py` & `pdip-0.6.9/pdip/integrator/connection/types/file/base/file_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/file/connectors/csv/csv_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/file/connectors/csv/csv_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/inmemory/base/in_memory_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/inmemory/base/in_memory_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/inmemory/base/in_memory_context.py` & `pdip-0.6.9/pdip/integrator/connection/types/inmemory/base/in_memory_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/inmemory/base/in_memory_policy.py` & `pdip-0.6.9/pdip/integrator/connection/types/inmemory/base/in_memory_policy.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/inmemory/base/in_memory_provider.py` & `pdip-0.6.9/pdip/integrator/connection/types/inmemory/base/in_memory_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/inmemory/connectors/sqlite/sq_lite_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/inmemory/connectors/sqlite/sq_lite_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/queue/adapters/queue_adapter.py` & `pdip-0.6.9/pdip/integrator/connection/types/queue/adapters/queue_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/queue/base/queue_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/queue/base/queue_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/queue/base/queue_context.py` & `pdip-0.6.9/pdip/integrator/connection/types/queue/base/queue_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/queue/base/queue_provider.py` & `pdip-0.6.9/pdip/integrator/connection/types/queue/base/queue_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/queue/connectors/kafka_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/queue/connectors/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/adapters/source/sql_source_adapter.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/adapters/source/sql_source_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/adapters/target/sql_target_adapter.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/adapters/target/sql_target_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/base/sql_context.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/base/sql_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/base/sql_dialect.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/base/sql_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/base/sql_iterator.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/base/sql_iterator.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/base/sql_policy.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/base/sql_policy.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/base/sql_provider.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/base/sql_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/clickhouse/clickhouse_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/clickhouse/clickhouse_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/mssql/mssql_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/mssql/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/mysql/mysql_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/mysql/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/oracle/oracle_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/oracle/oracle_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/connectors/postgresql/postgresql_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/connectors/postgresql/postgresql_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/clickhouse/clickhouse_dialect.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/clickhouse/clickhouse_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/mssql/mssql_dialect.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/mssql/mssql_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/mysql/mysql_dialect.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/mysql/mysql_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/oracle/oracle_dialect.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/oracle/oracle_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/sql/dialects/postgresql/postgresql_dialect.py` & `pdip-0.6.9/pdip/integrator/connection/types/sql/dialects/postgresql/postgresql_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/webservice/adapters/source/web_service_source_adapter.py` & `pdip-0.6.9/pdip/integrator/connection/types/webservice/adapters/source/web_service_source_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/webservice/adapters/target/web_service_target_adapter.py` & `pdip-0.6.9/pdip/integrator/connection/types/webservice/adapters/target/web_service_target_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/webservice/base/web_service_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/webservice/base/web_service_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/webservice/base/web_service_context.py` & `pdip-0.6.9/pdip/integrator/connection/types/webservice/base/web_service_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/webservice/base/web_service_policy.py` & `pdip-0.6.9/pdip/integrator/connection/types/webservice/base/web_service_policy.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/webservice/base/web_service_provider.py` & `pdip-0.6.9/pdip/integrator/connection/types/webservice/base/web_service_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/connection/types/webservice/connectors/soap/soap_connector.py` & `pdip-0.6.9/pdip/integrator/connection/types/webservice/connectors/soap/soap_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/event/base/default_integrator_event_manager.py` & `pdip-0.6.9/pdip/integrator/event/base/default_integrator_event_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/event/base/integrator_event_manager.py` & `pdip-0.6.9/pdip/integrator/event/base/integrator_event_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/event/base/integrator_event_manager_factory.py` & `pdip-0.6.9/pdip/integrator/event/base/integrator_event_manager_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/execution/domain/execution.py` & `pdip-0.6.9/pdip/integrator/execution/domain/execution.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/initializer/execution/base/default_execution_initializer.py` & `pdip-0.6.9/pdip/integrator/initializer/execution/base/default_execution_initializer.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/initializer/execution/base/execution_initializer_factory.py` & `pdip-0.6.9/pdip/integrator/initializer/execution/base/execution_initializer_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/initializer/execution/integration/default_operation_integration_execution_initializer.py` & `pdip-0.6.9/pdip/integrator/initializer/execution/integration/default_operation_integration_execution_initializer.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer_factory.py` & `pdip-0.6.9/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/initializer/execution/operation/operation_execution_initializer_factory.py` & `pdip-0.6.9/pdip/integrator/initializer/execution/operation/operation_execution_initializer_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/initializer/integrator/default_integrator_initializer.py` & `pdip-0.6.9/pdip/integrator/initializer/integrator/default_integrator_initializer.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/initializer/integrator/integrator_initializer_factory.py` & `pdip-0.6.9/pdip/integrator/initializer/integrator/integrator_initializer_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/base/integration_execution.py` & `pdip-0.6.9/pdip/integrator/integration/base/integration_execution.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/domain/base/integration.py` & `pdip-0.6.9/pdip/integrator/integration/domain/base/integration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/base/integration_adapter.py` & `pdip-0.6.9/pdip/integrator/integration/types/base/integration_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/base/integration_adapter_factory.py` & `pdip-0.6.9/pdip/integrator/integration/types/base/integration_adapter_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/source/base/source_integration.py` & `pdip-0.6.9/pdip/integrator/integration/types/source/base/source_integration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/base/source_to_target_integration.py` & `pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/base/source_to_target_integration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/base/integration_source_to_target_execute_strategy.py` & `pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/base/integration_source_to_target_execute_strategy.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/factories/integration_execute_strategy_factory.py` & `pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/factories/integration_execute_strategy_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/parallel_integration_execute.py` & `pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/parallel_integration_execute.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/parallel_thread_integration_execute.py` & `pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/parallel_thread_integration_execute.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/source_read_operation.py` & `pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/source_read_operation.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/target_write_operation.py` & `pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/target_write_operation.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_session_broker.py` & `pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_session_broker.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_worker.py` & `pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_worker.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/single_process_integration_execute.py` & `pdip-0.6.9/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/single_process_integration_execute.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/integration/types/target/base/target_integration.py` & `pdip-0.6.9/pdip/integrator/integration/types/target/base/target_integration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/operation/base/operation_execution.py` & `pdip-0.6.9/pdip/integrator/operation/base/operation_execution.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/operation/domain/operation.py` & `pdip-0.6.9/pdip/integrator/operation/domain/operation.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/pubsub/base/event_listener.py` & `pdip-0.6.9/pdip/integrator/pubsub/base/event_listener.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/pubsub/base/message_broker.py` & `pdip-0.6.9/pdip/integrator/pubsub/base/message_broker.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/integrator/pubsub/base/message_broker_worker.py` & `pdip-0.6.9/pdip/integrator/pubsub/base/message_broker_worker.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/io/file_manager.py` & `pdip-0.6.9/pdip/io/file_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/io/folder_manager.py` & `pdip-0.6.9/pdip/io/folder_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/json/base/base_converter.py` & `pdip-0.6.9/pdip/json/base/base_converter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/json/base/json_convert.py` & `pdip-0.6.9/pdip/json/base/json_convert.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/json/encoders/mutliple_json_encoders.py` & `pdip-0.6.9/pdip/json/encoders/mutliple_json_encoders.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/json/parsers/date_time_parser.py` & `pdip-0.6.9/pdip/json/parsers/date_time_parser.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/logging/loggers/base/ilogger.py` & `pdip-0.6.9/pdip/logging/loggers/base/ilogger.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/logging/loggers/console/console_logger.py` & `pdip-0.6.9/pdip/logging/loggers/console/console_logger.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/logging/loggers/file/file_logger.py` & `pdip-0.6.9/pdip/logging/loggers/file/file_logger.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/logging/loggers/sql/sql_logger.py` & `pdip-0.6.9/pdip/logging/loggers/sql/sql_logger.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/processing/base/process_manager.py` & `pdip-0.6.9/pdip/processing/base/process_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/processing/base/subprocess.py` & `pdip-0.6.9/pdip/processing/base/subprocess.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/processing/models/process_task.py` & `pdip-0.6.9/pdip/processing/models/process_task.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/utils/module_finder.py` & `pdip-0.6.9/pdip/utils/module_finder.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/utils/type_checker.py` & `pdip-0.6.9/pdip/utils/type_checker.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip/utils/utils.py` & `pdip-0.6.9/pdip/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/pdip.egg-info/PKG-INFO` & `pdip-0.6.9/pdip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pdip
-Version: 0.6.7
+Version: 0.6.9
 Summary: Python Data Integrator infrastructures package
 Home-page: https://github.com/ahmetcagriakca/pdip
 Author: Ahmet Çağrı AKCA
 Author-email: ahmetcagriakca@gmail.com
 License: MIT
-Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/v0.6.7.tar.gz
+Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/v0.6.9.tar.gz
 Project-URL: Bug Reports, https://github.com/ahmetcagriakca/pdip/issues
 Project-URL: Source, https://github.com/ahmetcagriakca/pdip
 Description: <p align="left">
         	<a href="https://pypi.org/project/pdip" target="_blank">
         			<img src="https://img.shields.io/pypi/v/pdip?color=%2334D058&label=pypi%20package" alt="Package version">
         	</a>
         </p>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: pdip Version: 0.6.7 Summary: Python Data Integrator
+Metadata-Version: 2.1 Name: pdip Version: 0.6.9 Summary: Python Data Integrator
 infrastructures package Home-page: https://github.com/ahmetcagriakca/pdip
 Author: Ahmet ÃaÄrÄ± AKCA Author-email: ahmetcagriakca@gmail.com License: MIT
 Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/
-v0.6.7.tar.gz Project-URL: Bug Reports, https://github.com/ahmetcagriakca/pdip/
+v0.6.9.tar.gz Project-URL: Bug Reports, https://github.com/ahmetcagriakca/pdip/
 issues Project-URL: Source, https://github.com/ahmetcagriakca/pdip Description:
 _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
 # Introduction This package aim to perform the integration processes easily
 Keywords:
 PDI,API,ETL,PROCESS,MULTIPROCESS,IO,CQRS,MSSQL,ORACLE,POSTGRES,MYSQL,CSV
 Platform: UNKNOWN Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
```

### Comparing `pdip-0.6.7/pdip.egg-info/SOURCES.txt` & `pdip-0.6.9/pdip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdip-0.6.7/setup.py` & `pdip-0.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 here = Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
-env_version = getenv('PYPI_PACKAGE_VERSION', default='0.6.7')
+env_version = getenv('PYPI_PACKAGE_VERSION', default='0.6.9')
 version = env_version.replace('v', '')
 setup(
     name='pdip',
     version=f'{version}',
     description='Python Data Integrator infrastructures package',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

