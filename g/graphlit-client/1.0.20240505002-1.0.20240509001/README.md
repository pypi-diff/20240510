# Comparing `tmp/graphlit_client-1.0.20240505002.tar.gz` & `tmp/graphlit_client-1.0.20240509001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-1.0.20240505002.tar", last modified: Mon May  6 02:07:15 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240509001.tar", last modified: Thu May  9 09:52:41 2024, max compression
```

## Comparing `graphlit_client-1.0.20240505002.tar` & `graphlit_client-1.0.20240509001.tar`

### file list

```diff
@@ -1,184 +1,190 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 02:07:15.834303 graphlit_client-1.0.20240505002/
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-06 02:07:15.834303 graphlit_client-1.0.20240505002/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 02:07:15.774303 graphlit_client-1.0.20240505002/graphlit/
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1878 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit/graphlit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 02:07:15.830304 graphlit_client-1.0.20240505002/graphlit_api/
--rw-r--r--   0 vsts      (1001) docker     (127)    82101 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/add_contents_to_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/async_base_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/base_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/clear_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    95409 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/close_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      440 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/count_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8528 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/create_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      477 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_all_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      506 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/delete_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/disable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/disable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/enable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/enable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17117 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/extract_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9686 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4286 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7128 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      387 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1164 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      763 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5193 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7962 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/get_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      931 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/ingest_encoded_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      804 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/ingest_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)      790 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/ingest_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)    78455 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/input_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/is_content_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/is_feed_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/lookup_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/lookup_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    66376 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3382 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/prompt_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2390 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/prompt_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/publish_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/publish_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/publish_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10533 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11920 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_contents_facets.py
--rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_contents_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4895 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1004 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1576 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7932 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      553 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1399 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1318 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1250 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      592 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5666 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1502 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8940 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/query_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/remove_contents_from_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/suggest_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/summarize_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8528 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/graphlit_api/update_workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 02:07:15.830304 graphlit_client-1.0.20240505002/graphlit_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-06 02:07:15.000000 graphlit_client-1.0.20240505002/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     5600 2024-05-06 02:07:15.000000 graphlit_client-1.0.20240505002/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-06 02:07:15.000000 graphlit_client-1.0.20240505002/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-06 02:07:15.000000 graphlit_client-1.0.20240505002/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-06 02:07:15.000000 graphlit_client-1.0.20240505002/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-06 02:07:15.834303 graphlit_client-1.0.20240505002/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-05-06 02:06:57.000000 graphlit_client-1.0.20240505002/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 09:52:41.272390 graphlit_client-1.0.20240509001/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-09 09:52:41.272390 graphlit_client-1.0.20240509001/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 09:52:41.224389 graphlit_client-1.0.20240509001/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1878 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 09:52:41.268390 graphlit_client-1.0.20240509001/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    84570 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    99560 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      440 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/count_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8528 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      477 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      506 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17117 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9686 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4286 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7153 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      387 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1164 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      763 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_share_point_consent_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5193 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7962 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/get_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      931 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      804 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      790 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    79384 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    68108 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3382 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2390 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/publish_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10533 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11920 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_contents_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_contents_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4895 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1004 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1576 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7957 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      553 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      834 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_microsoft_teams_channels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      782 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_microsoft_teams_teams.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      718 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_one_drive_folders.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1399 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1318 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1250 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      592 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      807 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_share_point_folders.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      961 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_share_point_libraries.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5666 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1502 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8940 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8528 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/graphlit_api/update_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 09:52:41.272390 graphlit_client-1.0.20240509001/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-09 09:52:41.000000 graphlit_client-1.0.20240509001/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-05-09 09:52:41.000000 graphlit_client-1.0.20240509001/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 09:52:41.000000 graphlit_client-1.0.20240509001/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-09 09:52:41.000000 graphlit_client-1.0.20240509001/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-09 09:52:41.000000 graphlit_client-1.0.20240509001/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-09 09:52:41.272390 graphlit_client-1.0.20240509001/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-05-09 09:52:24.000000 graphlit_client-1.0.20240509001/setup.py
```

### Comparing `graphlit_client-1.0.20240505002/LICENSE` & `graphlit_client-1.0.20240509001/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/PKG-INFO` & `graphlit_client-1.0.20240509001/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240505002
+Version: 1.0.20240509001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240505002/README.md` & `graphlit_client-1.0.20240509001/README.md`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit/graphlit.py` & `graphlit_client-1.0.20240509001/graphlit/graphlit.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/__init__.py` & `graphlit_client-1.0.20240509001/graphlit_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -395,14 +395,18 @@
     GetProject,
     GetProjectProject,
     GetProjectProjectQuota,
     GetProjectProjectSpecification,
     GetProjectProjectWorkflow,
 )
 from .get_repo import GetRepo, GetRepoRepo
+from .get_share_point_consent_uri import (
+    GetSharePointConsentUri,
+    GetSharePointConsentUriSharePointConsentUri,
+)
 from .get_software import GetSoftware, GetSoftwareSoftware
 from .get_specification import (
     GetSpecification,
     GetSpecificationSpecification,
     GetSpecificationSpecificationAnthropic,
     GetSpecificationSpecificationAzureOpenAi,
     GetSpecificationSpecificationCohere,
@@ -564,29 +568,32 @@
     LinearFeedPropertiesUpdateInput,
     LinkStrategyInput,
     MetadataFilter,
     MetadataInput,
     MetadataUpdateInput,
     MicrosoftEmailFeedPropertiesInput,
     MicrosoftEmailFeedPropertiesUpdateInput,
+    MicrosoftTeamsChannelsInput,
     MicrosoftTeamsFeedPropertiesInput,
     MicrosoftTeamsFeedPropertiesUpdateInput,
+    MicrosoftTeamsTeamsInput,
     MistralModelPropertiesInput,
     MistralModelPropertiesUpdateInput,
     ModelTextExtractionPropertiesInput,
     NamedEntityReferenceInput,
     NotionFeedPropertiesInput,
     NotionFeedPropertiesUpdateInput,
     ObservationCriteriaInput,
     ObservationInput,
     ObservationOccurrenceInput,
     ObservationReferenceFilter,
     ObservationUpdateInput,
     OneDriveFeedPropertiesInput,
     OneDriveFeedPropertiesUpdateInput,
+    OneDriveFoldersInput,
     OpenAIImageExtractionPropertiesInput,
     OpenAIModelPropertiesInput,
     OpenAIModelPropertiesUpdateInput,
     OrganizationFacetInput,
     OrganizationFilter,
     OrganizationInput,
     OrganizationUpdateInput,
@@ -627,14 +634,15 @@
     RetrievalStrategyInput,
     RetrievalStrategyUpdateInput,
     RSSFeedPropertiesInput,
     RSSFeedPropertiesUpdateInput,
     ShapeMetadataInput,
     SharePointFeedPropertiesInput,
     SharePointFeedPropertiesUpdateInput,
+    SharePointFoldersInput,
     SharePointLibrariesInput,
     SiteFeedPropertiesInput,
     SiteFeedPropertiesUpdateInput,
     SlackFeedPropertiesInput,
     SlackFeedPropertiesUpdateInput,
     SlackIntegrationPropertiesInput,
     SoftwareFacetInput,
@@ -761,14 +769,15 @@
     GET_LABEL_GQL,
     GET_ORGANIZATION_GQL,
     GET_PERSON_GQL,
     GET_PLACE_GQL,
     GET_PRODUCT_GQL,
     GET_PROJECT_GQL,
     GET_REPO_GQL,
+    GET_SHARE_POINT_CONSENT_URI_GQL,
     GET_SOFTWARE_GQL,
     GET_SPECIFICATION_GQL,
     GET_WORKFLOW_GQL,
     INGEST_ENCODED_FILE_GQL,
     INGEST_TEXT_GQL,
     INGEST_URI_GQL,
     IS_CONTENT_DONE_GQL,
@@ -787,19 +796,24 @@
     QUERY_CONTENTS_GQL,
     QUERY_CONTENTS_GRAPH_GQL,
     QUERY_CONVERSATIONS_GQL,
     QUERY_CREDITS_GQL,
     QUERY_EVENTS_GQL,
     QUERY_FEEDS_GQL,
     QUERY_LABELS_GQL,
+    QUERY_MICROSOFT_TEAMS_CHANNELS_GQL,
+    QUERY_MICROSOFT_TEAMS_TEAMS_GQL,
+    QUERY_ONE_DRIVE_FOLDERS_GQL,
     QUERY_ORGANIZATIONS_GQL,
     QUERY_PERSONS_GQL,
     QUERY_PLACES_GQL,
     QUERY_PRODUCTS_GQL,
     QUERY_REPOS_GQL,
+    QUERY_SHARE_POINT_FOLDERS_GQL,
+    QUERY_SHARE_POINT_LIBRARIES_GQL,
     QUERY_SOFTWARES_GQL,
     QUERY_SPECIFICATIONS_GQL,
     QUERY_USAGE_GQL,
     QUERY_WORKFLOWS_GQL,
     REMOVE_CONTENTS_FROM_COLLECTION_GQL,
     SUGGEST_CONVERSATION_GQL,
     SUMMARIZE_CONTENTS_GQL,
@@ -1018,14 +1032,29 @@
     QueryFeedsFeedsResultsSiteSharePoint,
     QueryFeedsFeedsResultsSlack,
     QueryFeedsFeedsResultsWeb,
     QueryFeedsFeedsResultsWorkflow,
     QueryFeedsFeedsResultsYoutube,
 )
 from .query_labels import QueryLabels, QueryLabelsLabels, QueryLabelsLabelsResults
+from .query_microsoft_teams_channels import (
+    QueryMicrosoftTeamsChannels,
+    QueryMicrosoftTeamsChannelsMicrosoftTeamsChannels,
+    QueryMicrosoftTeamsChannelsMicrosoftTeamsChannelsResults,
+)
+from .query_microsoft_teams_teams import (
+    QueryMicrosoftTeamsTeams,
+    QueryMicrosoftTeamsTeamsMicrosoftTeamsTeams,
+    QueryMicrosoftTeamsTeamsMicrosoftTeamsTeamsResults,
+)
+from .query_one_drive_folders import (
+    QueryOneDriveFolders,
+    QueryOneDriveFoldersOneDriveFolders,
+    QueryOneDriveFoldersOneDriveFoldersResults,
+)
 from .query_organizations import (
     QueryOrganizations,
     QueryOrganizationsOrganizations,
     QueryOrganizationsOrganizationsResults,
     QueryOrganizationsOrganizationsResultsAddress,
 )
 from .query_persons import (
@@ -1043,14 +1072,24 @@
 from .query_products import (
     QueryProducts,
     QueryProductsProducts,
     QueryProductsProductsResults,
     QueryProductsProductsResultsAddress,
 )
 from .query_repos import QueryRepos, QueryReposRepos, QueryReposReposResults
+from .query_share_point_folders import (
+    QuerySharePointFolders,
+    QuerySharePointFoldersSharePointFolders,
+    QuerySharePointFoldersSharePointFoldersResults,
+)
+from .query_share_point_libraries import (
+    QuerySharePointLibraries,
+    QuerySharePointLibrariesSharePointLibraries,
+    QuerySharePointLibrariesSharePointLibrariesResults,
+)
 from .query_softwares import (
     QuerySoftwares,
     QuerySoftwaresSoftwares,
     QuerySoftwaresSoftwaresResults,
 )
 from .query_specifications import (
     QuerySpecifications,
@@ -1600,14 +1639,15 @@
     "GET_LABEL_GQL",
     "GET_ORGANIZATION_GQL",
     "GET_PERSON_GQL",
     "GET_PLACE_GQL",
     "GET_PRODUCT_GQL",
     "GET_PROJECT_GQL",
     "GET_REPO_GQL",
+    "GET_SHARE_POINT_CONSENT_URI_GQL",
     "GET_SOFTWARE_GQL",
     "GET_SPECIFICATION_GQL",
     "GET_WORKFLOW_GQL",
     "GeometryMetadataInput",
     "GetAlert",
     "GetAlertAlert",
     "GetAlertAlertFilter",
@@ -1724,14 +1764,16 @@
     "GetProject",
     "GetProjectProject",
     "GetProjectProjectQuota",
     "GetProjectProjectSpecification",
     "GetProjectProjectWorkflow",
     "GetRepo",
     "GetRepoRepo",
+    "GetSharePointConsentUri",
+    "GetSharePointConsentUriSharePointConsentUri",
     "GetSoftware",
     "GetSoftwareSoftware",
     "GetSpecification",
     "GetSpecificationSpecification",
     "GetSpecificationSpecificationAnthropic",
     "GetSpecificationSpecificationAzureOpenAi",
     "GetSpecificationSpecificationCohere",
@@ -1841,16 +1883,18 @@
     "MailSensitivity",
     "MetadataFilter",
     "MetadataInput",
     "MetadataTypes",
     "MetadataUpdateInput",
     "MicrosoftEmailFeedPropertiesInput",
     "MicrosoftEmailFeedPropertiesUpdateInput",
+    "MicrosoftTeamsChannelsInput",
     "MicrosoftTeamsFeedPropertiesInput",
     "MicrosoftTeamsFeedPropertiesUpdateInput",
+    "MicrosoftTeamsTeamsInput",
     "MistralModelPropertiesInput",
     "MistralModelPropertiesUpdateInput",
     "MistralModels",
     "ModelServiceTypes",
     "ModelTextExtractionPropertiesInput",
     "NamedEntityReferenceInput",
     "NotionFeedPropertiesInput",
@@ -1861,14 +1905,15 @@
     "ObservationInput",
     "ObservationOccurrenceInput",
     "ObservationReferenceFilter",
     "ObservationUpdateInput",
     "OccurrenceTypes",
     "OneDriveFeedPropertiesInput",
     "OneDriveFeedPropertiesUpdateInput",
+    "OneDriveFoldersInput",
     "OpenAIImageExtractionPropertiesInput",
     "OpenAIModelPropertiesInput",
     "OpenAIModelPropertiesUpdateInput",
     "OpenAIModels",
     "OpenAIVisionDetailLevels",
     "OrderByTypes",
     "OrderDirectionTypes",
@@ -1944,19 +1989,24 @@
     "QUERY_CONTENTS_GQL",
     "QUERY_CONTENTS_GRAPH_GQL",
     "QUERY_CONVERSATIONS_GQL",
     "QUERY_CREDITS_GQL",
     "QUERY_EVENTS_GQL",
     "QUERY_FEEDS_GQL",
     "QUERY_LABELS_GQL",
+    "QUERY_MICROSOFT_TEAMS_CHANNELS_GQL",
+    "QUERY_MICROSOFT_TEAMS_TEAMS_GQL",
+    "QUERY_ONE_DRIVE_FOLDERS_GQL",
     "QUERY_ORGANIZATIONS_GQL",
     "QUERY_PERSONS_GQL",
     "QUERY_PLACES_GQL",
     "QUERY_PRODUCTS_GQL",
     "QUERY_REPOS_GQL",
+    "QUERY_SHARE_POINT_FOLDERS_GQL",
+    "QUERY_SHARE_POINT_LIBRARIES_GQL",
     "QUERY_SOFTWARES_GQL",
     "QUERY_SPECIFICATIONS_GQL",
     "QUERY_USAGE_GQL",
     "QUERY_WORKFLOWS_GQL",
     "QueryAlerts",
     "QueryAlertsAlerts",
     "QueryAlertsAlertsResults",
@@ -2103,14 +2153,23 @@
     "QueryFeedsFeedsResultsSlack",
     "QueryFeedsFeedsResultsWeb",
     "QueryFeedsFeedsResultsWorkflow",
     "QueryFeedsFeedsResultsYoutube",
     "QueryLabels",
     "QueryLabelsLabels",
     "QueryLabelsLabelsResults",
+    "QueryMicrosoftTeamsChannels",
+    "QueryMicrosoftTeamsChannelsMicrosoftTeamsChannels",
+    "QueryMicrosoftTeamsChannelsMicrosoftTeamsChannelsResults",
+    "QueryMicrosoftTeamsTeams",
+    "QueryMicrosoftTeamsTeamsMicrosoftTeamsTeams",
+    "QueryMicrosoftTeamsTeamsMicrosoftTeamsTeamsResults",
+    "QueryOneDriveFolders",
+    "QueryOneDriveFoldersOneDriveFolders",
+    "QueryOneDriveFoldersOneDriveFoldersResults",
     "QueryOrganizations",
     "QueryOrganizationsOrganizations",
     "QueryOrganizationsOrganizationsResults",
     "QueryOrganizationsOrganizationsResultsAddress",
     "QueryPersons",
     "QueryPersonsPersons",
     "QueryPersonsPersonsResults",
@@ -2122,14 +2181,20 @@
     "QueryProducts",
     "QueryProductsProducts",
     "QueryProductsProductsResults",
     "QueryProductsProductsResultsAddress",
     "QueryRepos",
     "QueryReposRepos",
     "QueryReposReposResults",
+    "QuerySharePointFolders",
+    "QuerySharePointFoldersSharePointFolders",
+    "QuerySharePointFoldersSharePointFoldersResults",
+    "QuerySharePointLibraries",
+    "QuerySharePointLibrariesSharePointLibraries",
+    "QuerySharePointLibrariesSharePointLibrariesResults",
     "QuerySoftwares",
     "QuerySoftwaresSoftwares",
     "QuerySoftwaresSoftwaresResults",
     "QuerySpecifications",
     "QuerySpecificationsSpecifications",
     "QuerySpecificationsSpecificationsResults",
     "QuerySpecificationsSpecificationsResultsAnthropic",
@@ -2204,14 +2269,15 @@
     "SUMMARIZE_CONTENTS_GQL",
     "SearchQueryTypes",
     "SearchTypes",
     "ShapeMetadataInput",
     "SharePointAuthenticationTypes",
     "SharePointFeedPropertiesInput",
     "SharePointFeedPropertiesUpdateInput",
+    "SharePointFoldersInput",
     "SharePointLibrariesInput",
     "SiteFeedPropertiesInput",
     "SiteFeedPropertiesUpdateInput",
     "SiteTypes",
     "SlackFeedPropertiesInput",
     "SlackFeedPropertiesUpdateInput",
     "SlackIntegrationPropertiesInput",
```

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/add_contents_to_collections.py` & `graphlit_client-1.0.20240509001/graphlit_api/add_contents_to_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/async_base_client.py` & `graphlit_client-1.0.20240509001/graphlit_api/async_base_client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/base_model.py` & `graphlit_client-1.0.20240509001/graphlit_api/base_model.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/clear_conversation.py` & `graphlit_client-1.0.20240509001/graphlit_api/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/client.py` & `graphlit_client-1.0.20240509001/graphlit_api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 from .get_label import GetLabel
 from .get_organization import GetOrganization
 from .get_person import GetPerson
 from .get_place import GetPlace
 from .get_product import GetProduct
 from .get_project import GetProject
 from .get_repo import GetRepo
+from .get_share_point_consent_uri import GetSharePointConsentUri
 from .get_software import GetSoftware
 from .get_specification import GetSpecification
 from .get_workflow import GetWorkflow
 from .ingest_encoded_file import IngestEncodedFile
 from .ingest_text import IngestText
 from .ingest_uri import IngestUri
 from .input_types import (
@@ -139,16 +140,19 @@
     EventUpdateInput,
     FeedFilter,
     FeedInput,
     FeedUpdateInput,
     LabelFilter,
     LabelInput,
     LabelUpdateInput,
+    MicrosoftTeamsChannelsInput,
+    MicrosoftTeamsTeamsInput,
     ObservationInput,
     ObservationUpdateInput,
+    OneDriveFoldersInput,
     OrganizationFilter,
     OrganizationInput,
     OrganizationUpdateInput,
     PersonFilter,
     PersonInput,
     PersonUpdateInput,
     PlaceFilter,
@@ -157,14 +161,16 @@
     ProductFilter,
     ProductInput,
     ProductUpdateInput,
     ProjectUpdateInput,
     RepoFilter,
     RepoInput,
     RepoUpdateInput,
+    SharePointFoldersInput,
+    SharePointLibrariesInput,
     SoftwareFilter,
     SoftwareInput,
     SoftwareUpdateInput,
     SpecificationFilter,
     SpecificationInput,
     SpecificationUpdateInput,
     SummarizationStrategyInput,
@@ -276,14 +282,15 @@
     GET_LABEL_GQL,
     GET_ORGANIZATION_GQL,
     GET_PERSON_GQL,
     GET_PLACE_GQL,
     GET_PRODUCT_GQL,
     GET_PROJECT_GQL,
     GET_REPO_GQL,
+    GET_SHARE_POINT_CONSENT_URI_GQL,
     GET_SOFTWARE_GQL,
     GET_SPECIFICATION_GQL,
     GET_WORKFLOW_GQL,
     INGEST_ENCODED_FILE_GQL,
     INGEST_TEXT_GQL,
     INGEST_URI_GQL,
     IS_CONTENT_DONE_GQL,
@@ -302,19 +309,24 @@
     QUERY_CONTENTS_GQL,
     QUERY_CONTENTS_GRAPH_GQL,
     QUERY_CONVERSATIONS_GQL,
     QUERY_CREDITS_GQL,
     QUERY_EVENTS_GQL,
     QUERY_FEEDS_GQL,
     QUERY_LABELS_GQL,
+    QUERY_MICROSOFT_TEAMS_CHANNELS_GQL,
+    QUERY_MICROSOFT_TEAMS_TEAMS_GQL,
+    QUERY_ONE_DRIVE_FOLDERS_GQL,
     QUERY_ORGANIZATIONS_GQL,
     QUERY_PERSONS_GQL,
     QUERY_PLACES_GQL,
     QUERY_PRODUCTS_GQL,
     QUERY_REPOS_GQL,
+    QUERY_SHARE_POINT_FOLDERS_GQL,
+    QUERY_SHARE_POINT_LIBRARIES_GQL,
     QUERY_SOFTWARES_GQL,
     QUERY_SPECIFICATIONS_GQL,
     QUERY_USAGE_GQL,
     QUERY_WORKFLOWS_GQL,
     REMOVE_CONTENTS_FROM_COLLECTION_GQL,
     SUGGEST_CONVERSATION_GQL,
     SUMMARIZE_CONTENTS_GQL,
@@ -349,19 +361,24 @@
 from .query_contents_facets import QueryContentsFacets
 from .query_contents_graph import QueryContentsGraph
 from .query_conversations import QueryConversations
 from .query_credits import QueryCredits
 from .query_events import QueryEvents
 from .query_feeds import QueryFeeds
 from .query_labels import QueryLabels
+from .query_microsoft_teams_channels import QueryMicrosoftTeamsChannels
+from .query_microsoft_teams_teams import QueryMicrosoftTeamsTeams
+from .query_one_drive_folders import QueryOneDriveFolders
 from .query_organizations import QueryOrganizations
 from .query_persons import QueryPersons
 from .query_places import QueryPlaces
 from .query_products import QueryProducts
 from .query_repos import QueryRepos
+from .query_share_point_folders import QuerySharePointFolders
+from .query_share_point_libraries import QuerySharePointLibraries
 from .query_softwares import QuerySoftwares
 from .query_specifications import QuerySpecifications
 from .query_usage import QueryUsage
 from .query_workflows import QueryWorkflows
 from .remove_contents_from_collection import RemoveContentsFromCollection
 from .suggest_conversation import SuggestConversation
 from .summarize_contents import SummarizeContents
@@ -1549,14 +1566,27 @@
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
             query=GET_FEED_GQL, operation_name="GetFeed", variables=variables, **kwargs
         )
         data = self.get_data(response)
         return GetFeed.model_validate(data)
 
+    async def get_share_point_consent_uri(
+        self, tenant_id: str, **kwargs: Any
+    ) -> GetSharePointConsentUri:
+        variables: Dict[str, object] = {"tenantId": tenant_id}
+        response = await self.execute(
+            query=GET_SHARE_POINT_CONSENT_URI_GQL,
+            operation_name="GetSharePointConsentUri",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return GetSharePointConsentUri.model_validate(data)
+
     async def is_feed_done(self, id: str, **kwargs: Any) -> IsFeedDone:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
             query=IS_FEED_DONE_GQL,
             operation_name="IsFeedDone",
             variables=variables,
             **kwargs
@@ -1573,14 +1603,90 @@
             operation_name="QueryFeeds",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return QueryFeeds.model_validate(data)
 
+    async def query_microsoft_teams_channels(
+        self, properties: MicrosoftTeamsChannelsInput, team_id: str, **kwargs: Any
+    ) -> QueryMicrosoftTeamsChannels:
+        variables: Dict[str, object] = {"properties": properties, "teamId": team_id}
+        response = await self.execute(
+            query=QUERY_MICROSOFT_TEAMS_CHANNELS_GQL,
+            operation_name="QueryMicrosoftTeamsChannels",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryMicrosoftTeamsChannels.model_validate(data)
+
+    async def query_microsoft_teams_teams(
+        self, properties: MicrosoftTeamsTeamsInput, **kwargs: Any
+    ) -> QueryMicrosoftTeamsTeams:
+        variables: Dict[str, object] = {"properties": properties}
+        response = await self.execute(
+            query=QUERY_MICROSOFT_TEAMS_TEAMS_GQL,
+            operation_name="QueryMicrosoftTeamsTeams",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryMicrosoftTeamsTeams.model_validate(data)
+
+    async def query_one_drive_folders(
+        self,
+        properties: OneDriveFoldersInput,
+        folder_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> QueryOneDriveFolders:
+        variables: Dict[str, object] = {"properties": properties, "folderId": folder_id}
+        response = await self.execute(
+            query=QUERY_ONE_DRIVE_FOLDERS_GQL,
+            operation_name="QueryOneDriveFolders",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QueryOneDriveFolders.model_validate(data)
+
+    async def query_share_point_folders(
+        self,
+        properties: SharePointFoldersInput,
+        drive_id: str,
+        folder_id: Union[Optional[str], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> QuerySharePointFolders:
+        variables: Dict[str, object] = {
+            "properties": properties,
+            "driveId": drive_id,
+            "folderId": folder_id,
+        }
+        response = await self.execute(
+            query=QUERY_SHARE_POINT_FOLDERS_GQL,
+            operation_name="QuerySharePointFolders",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QuerySharePointFolders.model_validate(data)
+
+    async def query_share_point_libraries(
+        self, properties: SharePointLibrariesInput, **kwargs: Any
+    ) -> QuerySharePointLibraries:
+        variables: Dict[str, object] = {"properties": properties}
+        response = await self.execute(
+            query=QUERY_SHARE_POINT_LIBRARIES_GQL,
+            operation_name="QuerySharePointLibraries",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return QuerySharePointLibraries.model_validate(data)
+
     async def update_feed(self, feed: FeedUpdateInput, **kwargs: Any) -> UpdateFeed:
         variables: Dict[str, object] = {"feed": feed}
         response = await self.execute(
             query=UPDATE_FEED_GQL,
             operation_name="UpdateFeed",
             variables=variables,
             **kwargs
```

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/close_conversation.py` & `graphlit_client-1.0.20240509001/graphlit_api/close_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/create_collection.py` & `graphlit_client-1.0.20240509001/graphlit_api/create_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/create_conversation.py` & `graphlit_client-1.0.20240509001/graphlit_api/create_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/create_specification.py` & `graphlit_client-1.0.20240509001/graphlit_api/create_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/create_workflow.py` & `graphlit_client-1.0.20240509001/graphlit_api/create_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/delete_all_conversations.py` & `graphlit_client-1.0.20240509001/graphlit_api/delete_all_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/delete_all_organizations.py` & `graphlit_client-1.0.20240509001/graphlit_api/delete_all_organizations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/delete_all_specifications.py` & `graphlit_client-1.0.20240509001/graphlit_api/delete_all_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/enums.py` & `graphlit_client-1.0.20240509001/graphlit_api/enums.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/exceptions.py` & `graphlit_client-1.0.20240509001/graphlit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/extract_contents.py` & `graphlit_client-1.0.20240509001/graphlit_api/extract_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_alert.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_alert.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_collection.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_content.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_conversation.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_event.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_event.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_feed.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,19 +94,20 @@
 class GetFeedFeedSiteGoogle(BaseModel):
     credentials: Optional[str]
     container_name: Optional[str] = Field(alias="containerName")
     prefix: Optional[str]
 
 
 class GetFeedFeedSiteSharePoint(BaseModel):
-    authentication_type: Optional[SharePointAuthenticationTypes] = Field(
+    authentication_type: SharePointAuthenticationTypes = Field(
         alias="authenticationType"
     )
-    account_name: Optional[str] = Field(alias="accountName")
-    library_id: Optional[str] = Field(alias="libraryId")
+    account_name: str = Field(alias="accountName")
+    library_id: str = Field(alias="libraryId")
+    folder_id: Optional[str] = Field(alias="folderId")
     tenant_id: Optional[str] = Field(alias="tenantId")
     refresh_token: Optional[str] = Field(alias="refreshToken")
 
 
 class GetFeedFeedSiteOneDrive(BaseModel):
     folder_id: Optional[str] = Field(alias="folderId")
     refresh_token: str = Field(alias="refreshToken")
```

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_organization.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_organization.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_person.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_person.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_place.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_place.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_product.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_product.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_project.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_project.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_software.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_software.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_specification.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/get_workflow.py` & `graphlit_client-1.0.20240509001/graphlit_api/get_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/ingest_encoded_file.py` & `graphlit_client-1.0.20240509001/graphlit_api/ingest_encoded_file.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/ingest_text.py` & `graphlit_client-1.0.20240509001/graphlit_api/ingest_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/ingest_uri.py` & `graphlit_client-1.0.20240509001/graphlit_api/ingest_uri.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/input_types.py` & `graphlit_client-1.0.20240509001/graphlit_api/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1109,16 +1109,16 @@
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
 
 
 class MicrosoftTeamsFeedPropertiesInput(BaseModel):
     type: Optional[FeedListingTypes] = None
     tenant_id: str = Field(alias="tenantId")
     refresh_token: str = Field(alias="refreshToken")
-    team: str
-    channel: str
+    team_id: str = Field(alias="teamId")
+    channel_id: str = Field(alias="channelId")
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
 
 
 class DiscordFeedPropertiesInput(BaseModel):
     type: Optional[FeedListingTypes] = None
     token: str
     channel: str
@@ -1396,16 +1396,16 @@
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
 
 
 class MicrosoftTeamsFeedPropertiesUpdateInput(BaseModel):
     type: Optional[FeedListingTypes] = None
     tenant_id: Optional[str] = Field(alias="tenantId", default=None)
     refresh_token: Optional[str] = Field(alias="refreshToken", default=None)
-    team: str
-    channel: str
+    team_id: str = Field(alias="teamId")
+    channel_id: str = Field(alias="channelId")
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
 
 
 class DiscordFeedPropertiesUpdateInput(BaseModel):
     type: Optional[FeedListingTypes] = None
     token: Optional[str] = None
     channel: Optional[str] = None
@@ -1587,18 +1587,19 @@
     prefix: Optional[str] = None
 
 
 class SharePointFeedPropertiesInput(BaseModel):
     authentication_type: SharePointAuthenticationTypes = Field(
         alias="authenticationType"
     )
-    account_name: str = Field(alias="accountName")
-    library_id: str = Field(alias="libraryId")
     tenant_id: Optional[str] = Field(alias="tenantId", default=None)
     refresh_token: Optional[str] = Field(alias="refreshToken", default=None)
+    account_name: str = Field(alias="accountName")
+    library_id: str = Field(alias="libraryId")
+    folder_id: Optional[str] = Field(alias="folderId", default=None)
 
 
 class OneDriveFeedPropertiesInput(BaseModel):
     folder_id: Optional[str] = Field(alias="folderId", default=None)
     refresh_token: str = Field(alias="refreshToken")
 
 
@@ -1720,18 +1721,19 @@
     prefix: Optional[str] = None
 
 
 class SharePointFeedPropertiesUpdateInput(BaseModel):
     authentication_type: Optional[SharePointAuthenticationTypes] = Field(
         alias="authenticationType", default=None
     )
-    account_name: Optional[str] = Field(alias="accountName", default=None)
-    library_id: Optional[str] = Field(alias="libraryId", default=None)
     tenant_id: Optional[str] = Field(alias="tenantId", default=None)
     refresh_token: Optional[str] = Field(alias="refreshToken", default=None)
+    account_name: Optional[str] = Field(alias="accountName", default=None)
+    library_id: Optional[str] = Field(alias="libraryId", default=None)
+    folder_id: Optional[str] = Field(alias="folderId", default=None)
 
 
 class OneDriveFeedPropertiesUpdateInput(BaseModel):
     folder_id: Optional[str] = Field(alias="folderId", default=None)
     refresh_token: Optional[str] = Field(alias="refreshToken", default=None)
 
 
@@ -1896,14 +1898,36 @@
     authentication_type: SharePointAuthenticationTypes = Field(
         alias="authenticationType"
     )
     tenant_id: Optional[str] = Field(alias="tenantId", default=None)
     refresh_token: Optional[str] = Field(alias="refreshToken", default=None)
 
 
+class SharePointFoldersInput(BaseModel):
+    authentication_type: SharePointAuthenticationTypes = Field(
+        alias="authenticationType"
+    )
+    tenant_id: Optional[str] = Field(alias="tenantId", default=None)
+    refresh_token: Optional[str] = Field(alias="refreshToken", default=None)
+
+
+class OneDriveFoldersInput(BaseModel):
+    refresh_token: str = Field(alias="refreshToken")
+
+
+class MicrosoftTeamsTeamsInput(BaseModel):
+    tenant_id: str = Field(alias="tenantId")
+    refresh_token: str = Field(alias="refreshToken")
+
+
+class MicrosoftTeamsChannelsInput(BaseModel):
+    tenant_id: str = Field(alias="tenantId")
+    refresh_token: str = Field(alias="refreshToken")
+
+
 class LabelFacetInput(BaseModel):
     time_interval: Optional[TimeIntervalTypes] = Field(
         alias="timeInterval", default=None
     )
     time_offset: Optional[int] = Field(alias="timeOffset", default=None)
     facet: Optional[LabelFacetTypes] = None
```

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/lookup_credits.py` & `graphlit_client-1.0.20240509001/graphlit_api/lookup_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/lookup_usage.py` & `graphlit_client-1.0.20240509001/graphlit_api/lookup_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/operations.py` & `graphlit_client-1.0.20240509001/graphlit_api/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     "GET_LABEL_GQL",
     "GET_ORGANIZATION_GQL",
     "GET_PERSON_GQL",
     "GET_PLACE_GQL",
     "GET_PRODUCT_GQL",
     "GET_PROJECT_GQL",
     "GET_REPO_GQL",
+    "GET_SHARE_POINT_CONSENT_URI_GQL",
     "GET_SOFTWARE_GQL",
     "GET_SPECIFICATION_GQL",
     "GET_WORKFLOW_GQL",
     "INGEST_ENCODED_FILE_GQL",
     "INGEST_TEXT_GQL",
     "INGEST_URI_GQL",
     "IS_CONTENT_DONE_GQL",
@@ -127,19 +128,24 @@
     "QUERY_CONTENTS_GQL",
     "QUERY_CONTENTS_GRAPH_GQL",
     "QUERY_CONVERSATIONS_GQL",
     "QUERY_CREDITS_GQL",
     "QUERY_EVENTS_GQL",
     "QUERY_FEEDS_GQL",
     "QUERY_LABELS_GQL",
+    "QUERY_MICROSOFT_TEAMS_CHANNELS_GQL",
+    "QUERY_MICROSOFT_TEAMS_TEAMS_GQL",
+    "QUERY_ONE_DRIVE_FOLDERS_GQL",
     "QUERY_ORGANIZATIONS_GQL",
     "QUERY_PERSONS_GQL",
     "QUERY_PLACES_GQL",
     "QUERY_PRODUCTS_GQL",
     "QUERY_REPOS_GQL",
+    "QUERY_SHARE_POINT_FOLDERS_GQL",
+    "QUERY_SHARE_POINT_LIBRARIES_GQL",
     "QUERY_SOFTWARES_GQL",
     "QUERY_SPECIFICATIONS_GQL",
     "QUERY_USAGE_GQL",
     "QUERY_WORKFLOWS_GQL",
     "REMOVE_CONTENTS_FROM_COLLECTION_GQL",
     "SUGGEST_CONVERSATION_GQL",
     "SUMMARIZE_CONTENTS_GQL",
@@ -2122,14 +2128,15 @@
         containerName
         prefix
       }
       sharePoint {
         authenticationType
         accountName
         libraryId
+        folderId
         tenantId
         refreshToken
       }
       oneDrive {
         folderId
         refreshToken
       }
@@ -2225,14 +2232,22 @@
       recurrenceType
       repeatInterval
     }
   }
 }
 """
 
+GET_SHARE_POINT_CONSENT_URI_GQL = """
+query GetSharePointConsentUri($tenantId: ID!) {
+  sharePointConsentUri(tenantId: $tenantId) {
+    uri
+  }
+}
+"""
+
 IS_FEED_DONE_GQL = """
 query IsFeedDone($id: ID!) {
   isFeedDone(id: $id) {
     result
   }
 }
 """
@@ -2278,14 +2293,15 @@
           containerName
           prefix
         }
         sharePoint {
           authenticationType
           accountName
           libraryId
+          folderId
           tenantId
           refreshToken
         }
         oneDrive {
           folderId
           refreshToken
         }
@@ -2382,14 +2398,77 @@
         repeatInterval
       }
     }
   }
 }
 """
 
+QUERY_MICROSOFT_TEAMS_CHANNELS_GQL = """
+query QueryMicrosoftTeamsChannels($properties: MicrosoftTeamsChannelsInput!, $teamId: ID!) {
+  microsoftTeamsChannels(properties: $properties, teamId: $teamId) {
+    results {
+      channelName
+      channelId
+    }
+  }
+}
+"""
+
+QUERY_MICROSOFT_TEAMS_TEAMS_GQL = """
+query QueryMicrosoftTeamsTeams($properties: MicrosoftTeamsTeamsInput!) {
+  microsoftTeamsTeams(properties: $properties) {
+    results {
+      teamName
+      teamId
+    }
+  }
+}
+"""
+
+QUERY_ONE_DRIVE_FOLDERS_GQL = """
+query QueryOneDriveFolders($properties: OneDriveFoldersInput!, $folderId: ID) {
+  oneDriveFolders(properties: $properties, folderId: $folderId) {
+    results {
+      folderName
+      folderId
+    }
+  }
+}
+"""
+
+QUERY_SHARE_POINT_FOLDERS_GQL = """
+query QuerySharePointFolders($properties: SharePointFoldersInput!, $driveId: ID!, $folderId: ID) {
+  sharePointFolders(
+    properties: $properties
+    driveId: $driveId
+    folderId: $folderId
+  ) {
+    accountName
+    results {
+      folderName
+      folderId
+    }
+  }
+}
+"""
+
+QUERY_SHARE_POINT_LIBRARIES_GQL = """
+query QuerySharePointLibraries($properties: SharePointLibrariesInput!) {
+  sharePointLibraries(properties: $properties) {
+    accountName
+    results {
+      libraryName
+      libraryId
+      siteName
+      siteId
+    }
+  }
+}
+"""
+
 UPDATE_FEED_GQL = """
 mutation UpdateFeed($feed: FeedUpdateInput!) {
   updateFeed(feed: $feed) {
     id
     name
     state
     type
```

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/prompt_conversation.py` & `graphlit_client-1.0.20240509001/graphlit_api/prompt_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/prompt_specifications.py` & `graphlit_client-1.0.20240509001/graphlit_api/prompt_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/publish_contents.py` & `graphlit_client-1.0.20240509001/graphlit_api/publish_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/publish_conversation.py` & `graphlit_client-1.0.20240509001/graphlit_api/publish_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/publish_text.py` & `graphlit_client-1.0.20240509001/graphlit_api/publish_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_alerts.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_alerts.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_categories.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_categories.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_collections.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_contents.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_contents_facets.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_contents_facets.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_contents_graph.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_contents_graph.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_conversations.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_credits.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_events.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_events.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_feeds.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_feeds.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,19 +106,20 @@
 class QueryFeedsFeedsResultsSiteGoogle(BaseModel):
     credentials: Optional[str]
     container_name: Optional[str] = Field(alias="containerName")
     prefix: Optional[str]
 
 
 class QueryFeedsFeedsResultsSiteSharePoint(BaseModel):
-    authentication_type: Optional[SharePointAuthenticationTypes] = Field(
+    authentication_type: SharePointAuthenticationTypes = Field(
         alias="authenticationType"
     )
-    account_name: Optional[str] = Field(alias="accountName")
-    library_id: Optional[str] = Field(alias="libraryId")
+    account_name: str = Field(alias="accountName")
+    library_id: str = Field(alias="libraryId")
+    folder_id: Optional[str] = Field(alias="folderId")
     tenant_id: Optional[str] = Field(alias="tenantId")
     refresh_token: Optional[str] = Field(alias="refreshToken")
 
 
 class QueryFeedsFeedsResultsSiteOneDrive(BaseModel):
     folder_id: Optional[str] = Field(alias="folderId")
     refresh_token: str = Field(alias="refreshToken")
```

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_labels.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_labels.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_organizations.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_organizations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_persons.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_persons.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_places.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_places.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_products.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_products.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_repos.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_repos.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_softwares.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_softwares.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_specifications.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_usage.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/query_workflows.py` & `graphlit_client-1.0.20240509001/graphlit_api/query_workflows.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/remove_contents_from_collection.py` & `graphlit_client-1.0.20240509001/graphlit_api/remove_contents_from_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/summarize_contents.py` & `graphlit_client-1.0.20240509001/graphlit_api/summarize_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/update_collection.py` & `graphlit_client-1.0.20240509001/graphlit_api/update_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/update_content.py` & `graphlit_client-1.0.20240509001/graphlit_api/update_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/update_conversation.py` & `graphlit_client-1.0.20240509001/graphlit_api/update_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/update_specification.py` & `graphlit_client-1.0.20240509001/graphlit_api/update_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_api/update_workflow.py` & `graphlit_client-1.0.20240509001/graphlit_api/update_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240505002/graphlit_client.egg-info/PKG-INFO` & `graphlit_client-1.0.20240509001/graphlit_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240505002
+Version: 1.0.20240509001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240505002/graphlit_client.egg-info/SOURCES.txt` & `graphlit_client-1.0.20240509001/graphlit_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 graphlit_api/get_label.py
 graphlit_api/get_organization.py
 graphlit_api/get_person.py
 graphlit_api/get_place.py
 graphlit_api/get_product.py
 graphlit_api/get_project.py
 graphlit_api/get_repo.py
+graphlit_api/get_share_point_consent_uri.py
 graphlit_api/get_software.py
 graphlit_api/get_specification.py
 graphlit_api/get_workflow.py
 graphlit_api/ingest_encoded_file.py
 graphlit_api/ingest_text.py
 graphlit_api/ingest_uri.py
 graphlit_api/input_types.py
@@ -137,19 +138,24 @@
 graphlit_api/query_contents_facets.py
 graphlit_api/query_contents_graph.py
 graphlit_api/query_conversations.py
 graphlit_api/query_credits.py
 graphlit_api/query_events.py
 graphlit_api/query_feeds.py
 graphlit_api/query_labels.py
+graphlit_api/query_microsoft_teams_channels.py
+graphlit_api/query_microsoft_teams_teams.py
+graphlit_api/query_one_drive_folders.py
 graphlit_api/query_organizations.py
 graphlit_api/query_persons.py
 graphlit_api/query_places.py
 graphlit_api/query_products.py
 graphlit_api/query_repos.py
+graphlit_api/query_share_point_folders.py
+graphlit_api/query_share_point_libraries.py
 graphlit_api/query_softwares.py
 graphlit_api/query_specifications.py
 graphlit_api/query_usage.py
 graphlit_api/query_workflows.py
 graphlit_api/remove_contents_from_collection.py
 graphlit_api/suggest_conversation.py
 graphlit_api/summarize_contents.py
```

### Comparing `graphlit_client-1.0.20240505002/setup.py` & `graphlit_client-1.0.20240509001/setup.py`

 * *Files identical despite different names*

