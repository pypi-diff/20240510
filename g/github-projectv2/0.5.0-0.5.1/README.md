# Comparing `tmp/github_projectv2-0.5.0.tar.gz` & `tmp/github_projectv2-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_projectv2-0.5.0.tar", max compression
+gzip compressed data, was "github_projectv2-0.5.1.tar", max compression
```

## Comparing `github_projectv2-0.5.0.tar` & `github_projectv2-0.5.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1074 2023-02-21 15:50:06.038377 github_projectv2-0.5.0/LICENSE
--rw-r--r--   0        0        0    13309 2024-04-26 15:44:41.040308 github_projectv2-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-02-21 15:24:45.992776 github_projectv2-0.5.0/github_projectv2/__init__.py
--rw-r--r--   0        0        0     2015 2023-11-02 19:48:53.750376 github_projectv2-0.5.0/github_projectv2/base.py
--rw-r--r--   0        0        0      757 2024-04-16 14:12:05.526795 github_projectv2-0.5.0/github_projectv2/comment.py
--rw-r--r--   0        0        0      512 2023-10-05 18:04:32.628033 github_projectv2-0.5.0/github_projectv2/field.py
--rw-r--r--   0        0        0    13727 2024-05-09 14:38:31.782913 github_projectv2-0.5.0/github_projectv2/item.py
--rw-r--r--   0        0        0      525 2024-04-16 14:12:05.514207 github_projectv2-0.5.0/github_projectv2/label.py
--rw-r--r--   0        0        0     1316 2024-04-25 13:02:27.427227 github_projectv2-0.5.0/github_projectv2/milestone.py
--rw-r--r--   0        0        0      219 2023-02-24 14:48:46.043408 github_projectv2-0.5.0/github_projectv2/option.py
--rw-r--r--   0        0        0     2465 2023-02-24 14:48:46.102689 github_projectv2-0.5.0/github_projectv2/organization.py
--rw-r--r--   0        0        0     9357 2023-11-02 20:41:43.175923 github_projectv2-0.5.0/github_projectv2/project.py
--rw-r--r--   0        0        0     2789 2024-05-09 14:35:59.583230 github_projectv2-0.5.0/github_projectv2/queries/partial/issue-timeline-events.graphql
--rw-r--r--   0        0        0     1293 2024-04-25 13:00:43.455136 github_projectv2-0.5.0/github_projectv2/queries/partial/item.graphql
--rw-r--r--   0        0        0       40 2023-02-21 18:52:04.451097 github_projectv2-0.5.0/github_projectv2/queries/partial/milestone.graphql
--rw-r--r--   0        0        0      227 2024-04-25 13:03:36.638594 github_projectv2-0.5.0/github_projectv2/queries/partial/repository.graphql
--rw-r--r--   0        0        0      414 2024-04-16 14:12:03.207811 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/assigned.graphql
--rw-r--r--   0        0        0      183 2024-04-26 15:11:06.196794 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/closed.graphql
--rw-r--r--   0        0        0      169 2024-05-09 14:35:29.149476 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/comment-deleted.graphql
--rw-r--r--   0        0        0      661 2024-05-08 16:48:45.097992 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/cross-referenced.graphql
--rw-r--r--   0        0        0      295 2024-04-16 14:12:03.214562 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/issue-comment.graphql
--rw-r--r--   0        0        0      176 2024-04-16 14:12:03.214387 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/labeled.graphql
--rw-r--r--   0        0        0      152 2024-04-16 14:12:03.214519 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/locked.graphql
--rw-r--r--   0        0        0       98 2024-04-16 14:12:03.197382 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/mentioned.graphql
--rw-r--r--   0        0        0      383 2024-05-08 16:54:00.343063 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/renamed-title.graphql
--rw-r--r--   0        0        0      166 2024-04-26 15:21:15.250903 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/reopened.graphql
--rw-r--r--   0        0        0      135 2024-04-16 14:12:03.196663 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/subscribed.graphql
--rw-r--r--   0        0        0      376 2024-04-16 14:12:03.197061 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/unassigned.graphql
--rw-r--r--   0        0        0      185 2024-04-16 14:12:03.214358 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/unlabeled.graphql
--rw-r--r--   0        0        0      137 2024-05-08 16:55:49.594304 github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/unsubscribed.graphql
--rw-r--r--   0        0        0      134 2023-11-02 19:48:53.116087 github_projectv2-0.5.0/github_projectv2/queries/partial/tracked-in-issues.graphql
--rw-r--r--   0        0        0      132 2023-11-02 19:48:53.115550 github_projectv2-0.5.0/github_projectv2/queries/partial/tracked-issues.graphql
--rw-r--r--   0        0        0      320 2023-11-02 19:48:53.115762 github_projectv2-0.5.0/github_projectv2/queries/project/get.graphql
--rw-r--r--   0        0        0      528 2023-11-02 19:48:53.115860 github_projectv2-0.5.0/github_projectv2/queries/project/get_field.graphql
--rw-r--r--   0        0        0      722 2023-11-02 19:48:53.115674 github_projectv2-0.5.0/github_projectv2/queries/project/get_fields.graphql
--rw-r--r--   0        0        0      633 2023-11-02 19:48:53.115721 github_projectv2-0.5.0/github_projectv2/queries/project/get_items.graphql
--rw-r--r--   0        0        0      811 2023-11-02 19:48:53.115839 github_projectv2-0.5.0/github_projectv2/queries/project/get_views.graphql
--rw-r--r--   0        0        0     3246 2024-04-25 13:02:46.554062 github_projectv2-0.5.0/github_projectv2/repository.py
--rw-r--r--   0        0        0       35 2023-11-02 19:49:33.434927 github_projectv2-0.5.0/github_projectv2/requirements.txt
--rw-r--r--   0        0        0     1322 2024-05-09 14:38:31.232024 github_projectv2-0.5.0/github_projectv2/search.py
--rw-r--r--   0        0        0     1201 2024-04-16 14:12:05.551040 github_projectv2-0.5.0/github_projectv2/timeline_event/AssignedEvent.py
--rw-r--r--   0        0        0     1048 2024-04-26 15:19:29.747432 github_projectv2-0.5.0/github_projectv2/timeline_event/ClosedEvent.py
--rw-r--r--   0        0        0     1252 2024-05-09 14:38:31.243917 github_projectv2-0.5.0/github_projectv2/timeline_event/CommentDeletedEvent.py
--rw-r--r--   0        0        0     1383 2024-05-09 14:38:29.958666 github_projectv2-0.5.0/github_projectv2/timeline_event/CrossReferencedEvent.py
--rw-r--r--   0        0        0     1255 2024-04-16 14:12:05.557829 github_projectv2-0.5.0/github_projectv2/timeline_event/IssueComment.py
--rw-r--r--   0        0        0      834 2024-04-16 14:12:07.175833 github_projectv2-0.5.0/github_projectv2/timeline_event/LabeledEvent.py
--rw-r--r--   0        0        0      833 2024-04-16 14:12:05.523389 github_projectv2-0.5.0/github_projectv2/timeline_event/MentionedEvent.py
--rw-r--r--   0        0        0     1058 2024-05-09 14:38:29.958855 github_projectv2-0.5.0/github_projectv2/timeline_event/RenamedTitleEvent.py
--rw-r--r--   0        0        0      911 2024-04-26 15:19:22.101780 github_projectv2-0.5.0/github_projectv2/timeline_event/ReopenedEvent.py
--rw-r--r--   0        0        0      896 2024-04-16 14:12:05.530202 github_projectv2-0.5.0/github_projectv2/timeline_event/SubscribedEvent.py
--rw-r--r--   0        0        0     1114 2024-04-16 14:12:05.538596 github_projectv2-0.5.0/github_projectv2/timeline_event/UnassignedEvent.py
--rw-r--r--   0        0        0      622 2024-04-16 14:12:05.512270 github_projectv2-0.5.0/github_projectv2/timeline_event/UnlabeledEvent.py
--rw-r--r--   0        0        0      900 2024-05-08 16:55:10.193507 github_projectv2-0.5.0/github_projectv2/timeline_event/UnsubscribedEvent.py
--rw-r--r--   0        0        0      288 2024-05-09 14:38:32.332720 github_projectv2-0.5.0/github_projectv2/timeline_event/__init__.py
--rw-r--r--   0        0        0      759 2023-02-24 14:48:46.072500 github_projectv2-0.5.0/github_projectv2/user.py
--rw-r--r--   0        0        0     1310 2023-03-09 18:00:37.291826 github_projectv2-0.5.0/github_projectv2/view.py
--rw-r--r--   0        0        0      335 2024-05-09 14:39:06.432299 github_projectv2-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    14355 1970-01-01 00:00:00.000000 github_projectv2-0.5.0/setup.py
--rw-r--r--   0        0        0    13654 1970-01-01 00:00:00.000000 github_projectv2-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-02-21 15:50:06.038377 github_projectv2-0.5.1/LICENSE
+-rw-r--r--   0        0        0    13309 2024-04-26 15:44:41.040308 github_projectv2-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-02-21 15:24:45.992776 github_projectv2-0.5.1/github_projectv2/__init__.py
+-rw-r--r--   0        0        0     2015 2023-11-02 19:48:53.750376 github_projectv2-0.5.1/github_projectv2/base.py
+-rw-r--r--   0        0        0      757 2024-04-16 14:12:05.526795 github_projectv2-0.5.1/github_projectv2/comment.py
+-rw-r--r--   0        0        0      512 2023-10-05 18:04:32.628033 github_projectv2-0.5.1/github_projectv2/field.py
+-rw-r--r--   0        0        0    13727 2024-05-09 14:38:31.782913 github_projectv2-0.5.1/github_projectv2/item.py
+-rw-r--r--   0        0        0      525 2024-04-16 14:12:05.514207 github_projectv2-0.5.1/github_projectv2/label.py
+-rw-r--r--   0        0        0     1316 2024-04-25 13:02:27.427227 github_projectv2-0.5.1/github_projectv2/milestone.py
+-rw-r--r--   0        0        0      219 2023-02-24 14:48:46.043408 github_projectv2-0.5.1/github_projectv2/option.py
+-rw-r--r--   0        0        0     2465 2023-02-24 14:48:46.102689 github_projectv2-0.5.1/github_projectv2/organization.py
+-rw-r--r--   0        0        0     9357 2023-11-02 20:41:43.175923 github_projectv2-0.5.1/github_projectv2/project.py
+-rw-r--r--   0        0        0     2789 2024-05-09 14:35:59.583230 github_projectv2-0.5.1/github_projectv2/queries/partial/issue-timeline-events.graphql
+-rw-r--r--   0        0        0     1293 2024-04-25 13:00:43.455136 github_projectv2-0.5.1/github_projectv2/queries/partial/item.graphql
+-rw-r--r--   0        0        0       40 2023-02-21 18:52:04.451097 github_projectv2-0.5.1/github_projectv2/queries/partial/milestone.graphql
+-rw-r--r--   0        0        0      227 2024-04-25 13:03:36.638594 github_projectv2-0.5.1/github_projectv2/queries/partial/repository.graphql
+-rw-r--r--   0        0        0      414 2024-04-16 14:12:03.207811 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/assigned.graphql
+-rw-r--r--   0        0        0      183 2024-04-26 15:11:06.196794 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/closed.graphql
+-rw-r--r--   0        0        0      169 2024-05-09 14:35:29.149476 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/comment-deleted.graphql
+-rw-r--r--   0        0        0      661 2024-05-08 16:48:45.097992 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/cross-referenced.graphql
+-rw-r--r--   0        0        0      295 2024-04-16 14:12:03.214562 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/issue-comment.graphql
+-rw-r--r--   0        0        0      190 2024-05-09 14:50:18.001316 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/labeled.graphql
+-rw-r--r--   0        0        0      152 2024-04-16 14:12:03.214519 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/locked.graphql
+-rw-r--r--   0        0        0       98 2024-04-16 14:12:03.197382 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/mentioned.graphql
+-rw-r--r--   0        0        0      383 2024-05-08 16:54:00.343063 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/renamed-title.graphql
+-rw-r--r--   0        0        0      166 2024-04-26 15:21:15.250903 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/reopened.graphql
+-rw-r--r--   0        0        0      135 2024-04-16 14:12:03.196663 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/subscribed.graphql
+-rw-r--r--   0        0        0      376 2024-04-16 14:12:03.197061 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/unassigned.graphql
+-rw-r--r--   0        0        0      185 2024-04-16 14:12:03.214358 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/unlabeled.graphql
+-rw-r--r--   0        0        0      137 2024-05-08 16:55:49.594304 github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/unsubscribed.graphql
+-rw-r--r--   0        0        0      134 2023-11-02 19:48:53.116087 github_projectv2-0.5.1/github_projectv2/queries/partial/tracked-in-issues.graphql
+-rw-r--r--   0        0        0      132 2023-11-02 19:48:53.115550 github_projectv2-0.5.1/github_projectv2/queries/partial/tracked-issues.graphql
+-rw-r--r--   0        0        0      320 2023-11-02 19:48:53.115762 github_projectv2-0.5.1/github_projectv2/queries/project/get.graphql
+-rw-r--r--   0        0        0      528 2023-11-02 19:48:53.115860 github_projectv2-0.5.1/github_projectv2/queries/project/get_field.graphql
+-rw-r--r--   0        0        0      722 2023-11-02 19:48:53.115674 github_projectv2-0.5.1/github_projectv2/queries/project/get_fields.graphql
+-rw-r--r--   0        0        0      633 2023-11-02 19:48:53.115721 github_projectv2-0.5.1/github_projectv2/queries/project/get_items.graphql
+-rw-r--r--   0        0        0      811 2023-11-02 19:48:53.115839 github_projectv2-0.5.1/github_projectv2/queries/project/get_views.graphql
+-rw-r--r--   0        0        0     3246 2024-04-25 13:02:46.554062 github_projectv2-0.5.1/github_projectv2/repository.py
+-rw-r--r--   0        0        0       35 2023-11-02 19:49:33.434927 github_projectv2-0.5.1/github_projectv2/requirements.txt
+-rw-r--r--   0        0        0     1322 2024-05-09 14:38:31.232024 github_projectv2-0.5.1/github_projectv2/search.py
+-rw-r--r--   0        0        0     1201 2024-04-16 14:12:05.551040 github_projectv2-0.5.1/github_projectv2/timeline_event/AssignedEvent.py
+-rw-r--r--   0        0        0     1048 2024-04-26 15:19:29.747432 github_projectv2-0.5.1/github_projectv2/timeline_event/ClosedEvent.py
+-rw-r--r--   0        0        0     1252 2024-05-09 14:38:31.243917 github_projectv2-0.5.1/github_projectv2/timeline_event/CommentDeletedEvent.py
+-rw-r--r--   0        0        0     1383 2024-05-09 14:38:29.958666 github_projectv2-0.5.1/github_projectv2/timeline_event/CrossReferencedEvent.py
+-rw-r--r--   0        0        0     1255 2024-04-16 14:12:05.557829 github_projectv2-0.5.1/github_projectv2/timeline_event/IssueComment.py
+-rw-r--r--   0        0        0      913 2024-05-09 14:50:08.947339 github_projectv2-0.5.1/github_projectv2/timeline_event/LabeledEvent.py
+-rw-r--r--   0        0        0      833 2024-04-16 14:12:05.523389 github_projectv2-0.5.1/github_projectv2/timeline_event/MentionedEvent.py
+-rw-r--r--   0        0        0     1058 2024-05-09 14:38:29.958855 github_projectv2-0.5.1/github_projectv2/timeline_event/RenamedTitleEvent.py
+-rw-r--r--   0        0        0      911 2024-04-26 15:19:22.101780 github_projectv2-0.5.1/github_projectv2/timeline_event/ReopenedEvent.py
+-rw-r--r--   0        0        0      896 2024-04-16 14:12:05.530202 github_projectv2-0.5.1/github_projectv2/timeline_event/SubscribedEvent.py
+-rw-r--r--   0        0        0     1114 2024-04-16 14:12:05.538596 github_projectv2-0.5.1/github_projectv2/timeline_event/UnassignedEvent.py
+-rw-r--r--   0        0        0      622 2024-04-16 14:12:05.512270 github_projectv2-0.5.1/github_projectv2/timeline_event/UnlabeledEvent.py
+-rw-r--r--   0        0        0      900 2024-05-08 16:55:10.193507 github_projectv2-0.5.1/github_projectv2/timeline_event/UnsubscribedEvent.py
+-rw-r--r--   0        0        0      288 2024-05-09 14:38:32.332720 github_projectv2-0.5.1/github_projectv2/timeline_event/__init__.py
+-rw-r--r--   0        0        0      759 2023-02-24 14:48:46.072500 github_projectv2-0.5.1/github_projectv2/user.py
+-rw-r--r--   0        0        0     1310 2023-03-09 18:00:37.291826 github_projectv2-0.5.1/github_projectv2/view.py
+-rw-r--r--   0        0        0      335 2024-05-09 14:53:59.546750 github_projectv2-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    14355 1970-01-01 00:00:00.000000 github_projectv2-0.5.1/setup.py
+-rw-r--r--   0        0        0    13654 1970-01-01 00:00:00.000000 github_projectv2-0.5.1/PKG-INFO
```

### Comparing `github_projectv2-0.5.0/LICENSE` & `github_projectv2-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/README.md` & `github_projectv2-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/base.py` & `github_projectv2-0.5.1/github_projectv2/base.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/comment.py` & `github_projectv2-0.5.1/github_projectv2/comment.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/field.py` & `github_projectv2-0.5.1/github_projectv2/field.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/item.py` & `github_projectv2-0.5.1/github_projectv2/item.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/label.py` & `github_projectv2-0.5.1/github_projectv2/label.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/milestone.py` & `github_projectv2-0.5.1/github_projectv2/milestone.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/organization.py` & `github_projectv2-0.5.1/github_projectv2/organization.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/project.py` & `github_projectv2-0.5.1/github_projectv2/project.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/queries/partial/issue-timeline-events.graphql` & `github_projectv2-0.5.1/github_projectv2/queries/partial/issue-timeline-events.graphql`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/queries/partial/item.graphql` & `github_projectv2-0.5.1/github_projectv2/queries/partial/item.graphql`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/queries/partial/timeline-events/cross-referenced.graphql` & `github_projectv2-0.5.1/github_projectv2/queries/partial/timeline-events/cross-referenced.graphql`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/queries/project/get_field.graphql` & `github_projectv2-0.5.1/github_projectv2/queries/project/get_field.graphql`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/queries/project/get_fields.graphql` & `github_projectv2-0.5.1/github_projectv2/queries/project/get_fields.graphql`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/queries/project/get_items.graphql` & `github_projectv2-0.5.1/github_projectv2/queries/project/get_items.graphql`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/queries/project/get_views.graphql` & `github_projectv2-0.5.1/github_projectv2/queries/project/get_views.graphql`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/repository.py` & `github_projectv2-0.5.1/github_projectv2/repository.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/search.py` & `github_projectv2-0.5.1/github_projectv2/search.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/AssignedEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/AssignedEvent.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/ClosedEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/ClosedEvent.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/CommentDeletedEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/CommentDeletedEvent.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/CrossReferencedEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/CrossReferencedEvent.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/IssueComment.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/IssueComment.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/LabeledEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/UnsubscribedEvent.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from github_projectv2.base import Base
-from github_projectv2.label import Label
 from github_projectv2.user import User
 
 
-class LabeledEvent(Base):
+class UnsubscribedEvent(Base):
     def __init__(self, node=None):
-        """Initialize the LabeledEvent object"""
+        """Initialize the UnsubscribedEvent object"""
 
-        super().__init__()
+        super().__init__(node)
 
         # Initialize the variables
         self.id = None
-        self.actor = []
-        self.label = []
+        self.actor = None
+        self.createdAt = None
+        self.subscribable = None
 
         if node is not None:
             self.load(node)
 
     def load(self, node):
         """Load the timeline item data"""
         self.id = node.get("id")
+        self.createdAt = node.get("createdAt")
+        self.subscribable = node.get("subscribable")
+
         self.load_actor(node.get("actor"))
-        self.label = Label(node.get("label"))
 
-    def load_actor(self, author):
+    def load_actor(self, actor):
         """Load the author data"""
-        type = author.get("__typename")
+        type = actor.get("__typename")
         if type == "User":
-            self.actor = User(author)
+            self.actor = User(actor)
         else:
             self.actor = None
```

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/MentionedEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/MentionedEvent.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/RenamedTitleEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/RenamedTitleEvent.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/ReopenedEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/ReopenedEvent.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/SubscribedEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/SubscribedEvent.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/UnassignedEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/UnassignedEvent.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/UnlabeledEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/UnlabeledEvent.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/timeline_event/UnsubscribedEvent.py` & `github_projectv2-0.5.1/github_projectv2/timeline_event/LabeledEvent.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from github_projectv2.base import Base
+from github_projectv2.label import Label
 from github_projectv2.user import User
 
 
-class UnsubscribedEvent(Base):
+class LabeledEvent(Base):
     def __init__(self, node=None):
-        """Initialize the UnsubscribedEvent object"""
+        """Initialize the LabeledEvent object"""
 
-        super().__init__(node)
+        super().__init__()
 
         # Initialize the variables
         self.id = None
-        self.actor = None
+        self.actor = []
+        self.label = None
         self.createdAt = None
-        self.subscribable = None
 
         if node is not None:
             self.load(node)
 
     def load(self, node):
         """Load the timeline item data"""
         self.id = node.get("id")
         self.createdAt = node.get("createdAt")
-        self.subscribable = node.get("subscribable")
-
         self.load_actor(node.get("actor"))
+        self.label = Label(node.get("label"))
 
-    def load_actor(self, actor):
+    def load_actor(self, author):
         """Load the author data"""
-        type = actor.get("__typename")
+        type = author.get("__typename")
         if type == "User":
-            self.actor = User(actor)
+            self.actor = User(author)
         else:
             self.actor = None
```

### Comparing `github_projectv2-0.5.0/github_projectv2/user.py` & `github_projectv2-0.5.1/github_projectv2/user.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/github_projectv2/view.py` & `github_projectv2-0.5.1/github_projectv2/view.py`

 * *Files identical despite different names*

### Comparing `github_projectv2-0.5.0/setup.py` & `github_projectv2-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'],
  'github_projectv2': ['queries/partial/*',
                       'queries/partial/timeline-events/*',
                       'queries/project/*']}
 
 setup_kwargs = {
     'name': 'github-projectv2',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': '',
     'long_description': '# ProjectV2 Client\n\nThis is an in-progress client to use the ProjectV2 functionality through the GitHub GraphQL API.\n\n## Setup\n\n1. Install the `projectv2` module: `pip3 install github-projectv2`\n2. Create a `.env` file in the root containing a value for `GITHUB_API_TOKEN` (this will be loaded using `python-dotenv`)\n3. Use the `requirements.txt` file to ensure you have all of the dependencies you need.\n4. Enjoy!\n\n**NOTE:** You can use an actual environment variable instead of the `.env` approach, setting the same `GITHUB_API_TOKEN` value\n\n## Example Usage\n\n```python\nfrom projectv2.project import Project\n\nproject = Project()\nproject.get(\'myorg\', \'1234\')\nprint(project.title)\n\n# Find the field with the name "Test Field 1"\nfound = None\nfor field in project.fields:\n    if field.name == "Test Field 1":\n        found = field\n\nif found is None:\n    raise Exception("Field not found")\n\nitems = project.get_items(\'myorg\')\nprint(items)\n\n# Look on the project fields and find the one with the name "Test Field 1" and get its options\n# Then, find the option with the name "Option 1" and get its id\n\nfor option in found.options:\n    if option.name == "test3":\n        newOption = option\n\nfor item in items:\n    result = item.update_field_value(project, field, newOption)\n    print(result)\n```\n\n## Modules\n\n### Project\nThe `Project` module is used to get the information about a project. It results in an instance with the following properties:\n\n- `title` (string)\n- `description` (string)\n- `id` (string): internal ID of project record\n- `number` (integer): public-facing ID number of project\n- `fields` (list): Set of fields in the project, default and custom\n- `items` (list): Set of "items" in the project, usually issue instances\n- `org` (string): Name of the organization the project belongs to\n- `createdAt` (datetime): Date/time of project creation\n- `closedAt` (datetime): Date/time when project was closed\n- `closed` (boolean): The open/closed state of the project\n- `shortDescription` (string): Short description of the project\n- `public` (boolean): Visibility for the project (public=`True`, private=`False`)\n- `readme` (string): Full readme for the project\n- `url` (string): Full public-facing URL location of the project\n\n**NOTE:** When the `get` method is called on the `Project`, the `get_fields` method will automatically be called to populate the `fields` property with instances of the `Field` class.\n\n#### Methods\n\n`get(org, projectNumber)`: Get a project by organization name and public-facing project number\nWhere:\n- `org` (string): the name of the organization\n- `projectNumber` (string): the public-facing ID for the project\n\n`get_fields(org)`: Get the fields for a project given the organization name and public-facing project number\nWhere:\n- `org` is the name of the organization (optional)\n\n`get_items(args)`: Get the items currently in the project (issues)\nWhere `args` are one or more named variables:\n- `org` (string) is the name of the organization\n- `options` (dict) are options for the query (see "Query Options" section below)\nReturns:\n- A set of `Item` object types\n\n`get_views(args)`: Get the current list of views for the project\nWhere `args` are one or more named variables:\n- `org` (string): optional name of the organization\n- `options` (dict) are options for the query (see "Query Options" section below)\nReturns:\n- A set of `View` object types\n\n`create(data)`: Create a new project\nWhere:\n- `data` (list): Data to use in the creation of the project (required values: `title`, `ownerId`)\nReturns:\n- A `Project` instance with the new data set\n\n`remove_item(item)`: Removes an item from a project\nWhere:\n- `item` must be a record as fetched by `get_items`, not from a call to `Item.get`\nReturns:\n- The internal ID of the deleted item\n\n`add_item(item)`: Adds an item/issue to a project\nWhere:\n- `item` is a record as fetched by `Item.get` or from the list from `Project.get_items`\nReturns:\n- The internal ID of the item that was added\n\n`save()`: Saves the current state of the project record (fields saved are title, shortDescription, readme, closed)\nReturns:\n- The current instance, a `Project` with the updated information\n\n**NOTE:** the `get_fields` and `get_items` require that the project is fetched using `get` first and will throw an error otherwise.\n\n### Item\nThe `Item` module is used to represent an item in a project (an issue record). It results in an instance with the following properties:\n\n- `id` (string): internal ID of the item record\n- `type` (string): type of item (ex: `ISSUE`)\n- `created` (string): A date/time of when the item was created\n- `assignees` (list): A set of `User` instances\n- `title` (string): Title of the item (issue)\n- `number` (string): The public-facing number of the item\n- `updatedAt` (string): A date/time of when the item was last updated\n- `url` (string): The public-facing URL\n- `body` (string): Unrendered body content\n- `closed` (boolean): Closed/not closed state\n- `closedAt` (string): A date/time of when the issue was closed\n- `author` (list): A set of `User` instances\n- `labels` (list): A set of `Label` instances\n- `projectNodeId` (string): The internal ID of the item (used when relating to a project, otherwise `None`)\n- `trackedIssues` (list): A set of `Item` instances\n- `trackedInIssues` (list): A set of `Item` instances\n- `timeline` (list): A set of `*Event` instances (see below for which events are currently supported)\n\n#### Methods\n\n`update_field_value(project, field, input)`: Update a single select field to a new value\nWhere:\n- `project` = a `Project` instance\n- `field` = a `Field` instance representing the field to update the value on\n- `option` = Either an an `Option` instance representing the new value or a string value\n\n`get(org, repo, itemId)`\nWhere:\n- `org` (string): the name of the organization\n- `repo` (string): the name of the repository\n- `itemId` (string): the ID number of the item\n\n`clear_field_value(project, field)`\nWhere:\n- `project`: a `Project` instance\n- `field`: a `Field` instance for the field to clear (a result of the objects loaded from a `Project.get_fields()` method call)\n\n`create(repository, data)`\nWhere:\n- `repository`: a `Repository` instance\n- `data`: a data set containing: `assigneeIds`, `body`, `title` (optional: `labelIds`, `milestoneId`)\n\n`add_label(label_name)`\nWhere:\n- `label_name` is the "name" of the label to add (not the ID)\n\n`close(reason)`\nWhere:\n- `reason` (string, optional) either `COMPLETED` or `NOT_PLANNED` (default is `COMPLETED`)\n\n`make_comment(comment)`\nWhere:\n- `comment` (string) is the contents of the comment\n\n### Option\nThe `Option` module is used to represent an option on a single-select field. It results in an instance with the following properties:\n\n- `id` (string): internal ID of the option record\n- `name` (string): the name of the option (this is the option\'s value)\n\n### Field\nThe `Field` module is used to represent a field in the project. It results in an instance with the following properties:\n\n- `id` (string): internal ID of the field record\n- `name` (string): name of the field\n- `dataType` (string): type of field (Ex: `TEXT` or `SINGLE_SELECT`)\n- `options` (list): when the `dataType` is `SINGLE_SELECT` the options array will be populated with the options records as instances of `Option`\n\n### Label\nThe `Label` module is used to represent a label on an item. It results in an instance with the following properties:\n\n- `id` (string): internal ID of the label record\n- `name` (string): name of the label\n- `description` (string): description of the label\n\n### User\nThe `User` module is used to represent a user in the system. It results in an instance with the following properties:\n\n- `id` (string): internal ID of the user record\n- `email` (string): email address of the user\n- `login` (string): login/username of the user\n- `name` (string): user\'s name\n\n### Milestone\nThe `Milestone` module is used to represent a milestone in the system. It results in an instance with the following properties:\n\n- `id` (string): internal ID of the milestone record\n- `description` (string): description of the milestone\n- `number` (integer): public-facing ID\n- `title` (string): title of the milestone\n- `state` (string): open/closed status\n- `dueOn` (string): datetime string of when the milestone is\n\n#### Methods\n\n`get(org)`\nWhere:\n- `org` (string): the name of the organization\n\n### Repository\nThe `Repository` module is used to represent a repository in the system. It results in an instance with the following properties:\n\n- `id` (string): internal ID of the repository record\n- `name` (string): name of the repository\n- `description` (string): repository description\n- `isPrivate` (boolean): public/private status\n- `isArchived` (boolean): archived/not archived\n- `isDisabled` (boolean): disabled/not disabled\n- `isFork` (boolean): is a fork/not a fork\n- `isLocked` (boolean): is locked/not locked\n- `isMirror` (boolean): is a mirror/not a mirror\n- `isTemplate` (boolean): is a template/not a template\n\n#### Methods\n\n`get(org, name)`\nWhere:\n- `org` (string): organization name\n- `name` (string): repository name\n\n`get_milestones()`\n\n**NOTE:** `get_milestones` requires that `get()` is called first\n\n### Organization\nThe `Organization` module is used to represent an organization in the system. It results in an instance with the following properties:\n\n- `id` (string): internal ID of the organization record\n- `name` (string): name of the organization (ex: `GitHub`)\n- `login` (string): the login of the organization (ex: `github`)\n- `description` (string): the description of the organization\n- `createdAt` (string): datetime string\n- `location` (string): location value of the organization\n- `url` (string): external URL location\n- `repositories` (list): a list of all repositories in the organization (loads as `Repository objects`)\n\n**NOTE:** Repositories are not loaded by default. `get_repositories` must be called to load them. The method will also return the repository list.\n\n#### Methods\n`get(login)`\nWhere:\n- `login` (string) the name of the organization\nReturns:\n- A single object of type `Organization`\n\n`get_repositories(login)`\nWhere:\n- `login` (string): the name of the organization (`name` is optional, but if not set `get` must be called first)\nReturns:\n- A set of `Repository` class objects populated with repository data\n\n### Search\nThe `Search` module is used to make searches using the `search()` method on the GraphQL API using a format similar to those used in the search on the website.\n\n- No properties defined\n\n#### Methods\n`issues`\nWhere:\n- `filter` (string): the search filter string\nReturns:\n- Set of `Item` class objects populated with matching issue data\n\n### View\nThe `View` module represents a view in the project (a tab). It results in an instance with the following properties:\n\n- `id` (string): internal ID of the view\n- `number` (string): the public ID of the view\n- `sortBy` (array): populated when a view is sorted (contains: `field.name`, `field.id` (internal), `field.dataType`, `direction`)\n- `groupBy` (array): populated when a view is grouped (contains: `id` (internal), `name`)\n- `layout` (string): Layout of the view (ex: `TABLE_LAYOUT` or `BOARD_LAYOUT`)\n\nResource: [https://mathspp.com/blog/how-to-create-a-python-package-in-2022](https://mathspp.com/blog/how-to-create-a-python-package-in-2022)\n\n### Timeline Events\nSeveral of the methods, including `item.get` and `project.get_items` (if the value for `includeTimelineEvents` is `True`) will also pull in the timeline events for an item. This timeline provides details about actions like: when an issue was labeled, when someone subscribed to an issue, and when a user was mentioned in an issue. We currently support several event types:\n\n- `AssignedEvent`\n- `UnassignedEvent`\n- `IssueComment`\n- `LabeledEvent`\n- `UnlabeledEvent`\n- `MentionedEvent`\n- `SubscribedEvent`\n- `ReopenedEvent`\n- `ClosedEvent`\n\nYou can find out more about what properties each of these support [in the GitHub API object documentation](https://docs.github.com/en/graphql/reference/objects).\n\n## Query Options\nIn some methods (such as `project.get_items`) use can used named arguments to configure the requests made to the API (see method definitions above to determine which support the `options` named variable)\n\n### Supported options:\n- `includeTrackedInIssues`: Includes information about the other item(s) the current item is tracked in (Values: `True`/`False`)\n- `includeTrackedIssues`: Include information about the item(s) being tracked by this item  (Values: `True`/`False`)\n- `includeTimelineEvents`: Include the timeline events that were taken on the item (Values: `True`/`False`)\n\n\n### Development\n\nThis package makes use of the [Poetry](https://python-poetry.org/) packaging tool. In order to do development work, you should perform the following steps:\n\n```\ncd projectv2\npoetry shell\n```\n\nThen you can run your script from there. In my case, it\'s one called `test.py` that lives one directory up, so: `python3 ../test.py`\n\nThen, to package, build, and push it up to the PyPi platform:\n\n1. Update the `version` in `pyproject.toml`\n2. Commit the changes and add a new tag\n3. Push the updates to the repo (including the new tag)\n4. Run the build and push commands from outside of the `poetry` shell:\n\n```\npoetry build\npoetry publish\n```\n',
     'author': 'Chris Cornutt',
     'author_email': 'enygma@github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `github_projectv2-0.5.0/PKG-INFO` & `github_projectv2-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-projectv2
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Author: Chris Cornutt
 Author-email: enygma@github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

