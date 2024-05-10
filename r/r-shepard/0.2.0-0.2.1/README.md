# Comparing `tmp/r_shepard-0.2.0.tar.gz` & `tmp/r_shepard-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r_shepard-0.2.0.tar", max compression
+gzip compressed data, was "r_shepard-0.2.1.tar", max compression
```

## Comparing `r_shepard-0.2.0.tar` & `r_shepard-0.2.1.tar`

### file list

```diff
@@ -1,61 +1,60 @@
--rw-r--r--   0        0        0     3517 2024-05-10 09:23:02.387390 r_shepard-0.2.0/README.md
--rwxr-xr-x   0        0        0      666 2024-05-01 08:42:22.525077 r_shepard-0.2.0/manage.py
--rw-r--r--   0        0        0      805 2024-05-10 09:22:50.020327 r_shepard-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      174 2024-05-06 20:18:43.831721 r_shepard-0.2.0/r_shepard/__init__.py
--rw-r--r--   0        0        0       52 2024-05-06 21:14:06.784472 r_shepard-0.2.0/r_shepard/api/__init__.py
--rw-r--r--   0        0        0     4387 2024-05-10 09:11:26.291425 r_shepard-0.2.0/r_shepard/api/admin.py
--rw-r--r--   0        0        0      457 2024-05-07 10:02:03.501832 r_shepard-0.2.0/r_shepard/api/apps.py
--rw-r--r--   0        0        0      179 2024-05-06 21:14:06.784472 r_shepard-0.2.0/r_shepard/api/appy.py
--rw-r--r--   0        0        0     2063 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      488 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0002_project_is_active.py
--rw-r--r--   0        0        0      567 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0003_project_url.py
--rw-r--r--   0        0        0      522 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0004_project_rstudio_version.py
--rw-r--r--   0        0        0     1291 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
--rw-r--r--   0        0        0     4980 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
--rw-r--r--   0        0        0      553 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0007_alter_container_container_id.py
--rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.2.0/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
--rw-r--r--   0        0        0      552 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0009_alter_container_port.py
--rw-r--r--   0        0        0      525 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0010_alter_container_port.py
--rw-r--r--   0        0        0      596 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
--rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.2.0/r_shepard/api/migrations/0012_project_slug.py
--rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.2.0/r_shepard/api/migrations/0013_remove_project_password_container_password.py
--rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.2.0/r_shepard/api/migrations/0014_project_max_containers.py
--rw-r--r--   0        0        0      822 2024-05-10 09:11:20.381386 r_shepard-0.2.0/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
--rw-r--r--   0        0        0     1285 2024-05-10 09:12:21.754790 r_shepard-0.2.0/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
--rw-r--r--   0        0        0     3837 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0017_alter_container_container_id_alter_container_cpus_and_more.py
--rw-r--r--   0        0        0      574 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0018_project_description.py
--rw-r--r--   0        0        0     2681 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0019_alter_project_commit_interval_and_more.py
--rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.2.0/r_shepard/api/migrations/__init__.py
--rw-r--r--   0        0        0     6612 2024-05-10 09:19:46.724377 r_shepard-0.2.0/r_shepard/api/models.py
--rw-r--r--   0        0        0     4637 2024-05-10 08:47:24.802782 r_shepard-0.2.0/r_shepard/api/podman.py
--rw-r--r--   0        0        0     3104 2024-05-08 13:55:02.555158 r_shepard-0.2.0/r_shepard/api/static/custom.css
--rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.2.0/r_shepard/api/static/htmx.min.js
--rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.2.0/r_shepard/api/static/pico.blue.min.css
--rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.2.0/r_shepard/api/static/pico.colors.min.css
--rw-r--r--   0        0        0     3006 2024-05-10 08:47:24.802782 r_shepard-0.2.0/r_shepard/api/tailscale.py
--rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.2.0/r_shepard/api/tasks.py
--rw-r--r--   0        0        0     5807 2024-05-07 10:02:03.502833 r_shepard-0.2.0/r_shepard/api/views.py
--rw-r--r--   0        0        0      395 2024-04-26 07:51:03.905968 r_shepard-0.2.0/r_shepard/asgi.py
--rw-r--r--   0        0        0      226 2024-04-26 08:04:10.741465 r_shepard-0.2.0/r_shepard/celery.py
--rw-r--r--   0        0        0     4719 2024-05-10 09:21:17.170852 r_shepard-0.2.0/r_shepard/settings.py
--rw-r--r--   0        0        0     1967 2024-05-10 09:20:02.868462 r_shepard-0.2.0/r_shepard/tests/test_models.py
--rw-r--r--   0        0        0     1549 2024-04-30 14:46:22.169959 r_shepard-0.2.0/r_shepard/tests/test_views.py
--rw-r--r--   0        0        0     2275 2024-04-30 14:28:56.240315 r_shepard-0.2.0/r_shepard/tests/utils.py
--rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.2.0/r_shepard/urls.py
--rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.2.0/r_shepard/wsgi.py
--rw-r--r--   0        0        0      356 2024-04-23 06:43:01.074990 r_shepard-0.2.0/templates/admin/base.html
--rw-r--r--   0        0        0      739 2024-04-23 16:45:21.318848 r_shepard-0.2.0/templates/base.html
--rw-r--r--   0        0        0     4152 2024-05-08 13:25:20.796846 r_shepard-0.2.0/templates/container_list.html
--rw-r--r--   0        0        0     2590 2024-05-08 13:56:15.535676 r_shepard-0.2.0/templates/project_detail.html
--rw-r--r--   0        0        0     1150 2024-05-08 13:20:01.025476 r_shepard-0.2.0/templates/project_list.html
--rw-r--r--   0        0        0      234 2024-04-22 17:10:53.021583 r_shepard-0.2.0/templates/two_factor/_base_focus.html
--rw-r--r--   0        0        0      500 2024-04-22 16:49:01.953028 r_shepard-0.2.0/templates/two_factor/_wizard_actions.html
--rw-r--r--   0        0        0       90 2024-04-22 16:29:08.847147 r_shepard-0.2.0/templates/two_factor/_wizard_forms.html
--rw-r--r--   0        0        0     1145 2024-04-22 16:29:08.812144 r_shepard-0.2.0/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0        0        0     2008 2024-04-22 16:48:40.642014 r_shepard-0.2.0/templates/two_factor/core/login.html
--rw-r--r--   0        0        0      833 2024-04-22 16:29:08.813144 r_shepard-0.2.0/templates/two_factor/core/otp_required.html
--rw-r--r--   0        0        0     3149 2024-04-22 16:29:08.813144 r_shepard-0.2.0/templates/two_factor/core/setup.html
--rw-r--r--   0        0        0      963 2024-04-22 16:29:08.814144 r_shepard-0.2.0/templates/two_factor/core/setup_complete.html
--rw-r--r--   0        0        0      529 2024-04-22 16:29:08.801143 r_shepard-0.2.0/templates/two_factor/profile/disable.html
--rw-r--r--   0        0        0     2527 2024-04-23 08:51:59.180319 r_shepard-0.2.0/templates/two_factor/profile/profile.html
--rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 r_shepard-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3517 2024-05-10 09:23:02.387390 r_shepard-0.2.1/README.md
+-rwxr-xr-x   0        0        0      666 2024-05-01 08:42:22.525077 r_shepard-0.2.1/manage.py
+-rw-r--r--   0        0        0      810 2024-05-10 09:47:56.857800 r_shepard-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      174 2024-05-06 20:18:43.831721 r_shepard-0.2.1/r_shepard/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-06 21:14:06.784472 r_shepard-0.2.1/r_shepard/api/__init__.py
+-rw-r--r--   0        0        0     4387 2024-05-10 09:11:26.291425 r_shepard-0.2.1/r_shepard/api/admin.py
+-rw-r--r--   0        0        0      457 2024-05-07 10:02:03.501832 r_shepard-0.2.1/r_shepard/api/apps.py
+-rw-r--r--   0        0        0      179 2024-05-06 21:14:06.784472 r_shepard-0.2.1/r_shepard/api/appy.py
+-rw-r--r--   0        0        0     2063 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0002_project_is_active.py
+-rw-r--r--   0        0        0      567 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0003_project_url.py
+-rw-r--r--   0        0        0      522 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0004_project_rstudio_version.py
+-rw-r--r--   0        0        0     1291 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
+-rw-r--r--   0        0        0     4980 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
+-rw-r--r--   0        0        0      553 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0007_alter_container_container_id.py
+-rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.2.1/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
+-rw-r--r--   0        0        0      552 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0009_alter_container_port.py
+-rw-r--r--   0        0        0      525 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0010_alter_container_port.py
+-rw-r--r--   0        0        0      596 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
+-rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.2.1/r_shepard/api/migrations/0012_project_slug.py
+-rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.2.1/r_shepard/api/migrations/0013_remove_project_password_container_password.py
+-rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.2.1/r_shepard/api/migrations/0014_project_max_containers.py
+-rw-r--r--   0        0        0      822 2024-05-10 09:11:20.381386 r_shepard-0.2.1/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
+-rw-r--r--   0        0        0     1285 2024-05-10 09:12:21.754790 r_shepard-0.2.1/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
+-rw-r--r--   0        0        0     3837 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0017_alter_container_container_id_alter_container_cpus_and_more.py
+-rw-r--r--   0        0        0      574 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0018_project_description.py
+-rw-r--r--   0        0        0     2681 2024-05-10 09:10:56.833226 r_shepard-0.2.1/r_shepard/api/migrations/0019_alter_project_commit_interval_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.2.1/r_shepard/api/migrations/__init__.py
+-rw-r--r--   0        0        0     6612 2024-05-10 09:19:46.724377 r_shepard-0.2.1/r_shepard/api/models.py
+-rw-r--r--   0        0        0     4637 2024-05-10 08:47:24.802782 r_shepard-0.2.1/r_shepard/api/podman.py
+-rw-r--r--   0        0        0     3104 2024-05-08 13:55:02.555158 r_shepard-0.2.1/r_shepard/api/static/custom.css
+-rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.2.1/r_shepard/api/static/htmx.min.js
+-rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.2.1/r_shepard/api/static/pico.blue.min.css
+-rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.2.1/r_shepard/api/static/pico.colors.min.css
+-rw-r--r--   0        0        0     3006 2024-05-10 08:47:24.802782 r_shepard-0.2.1/r_shepard/api/tailscale.py
+-rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.2.1/r_shepard/api/tasks.py
+-rw-r--r--   0        0        0     5807 2024-05-07 10:02:03.502833 r_shepard-0.2.1/r_shepard/api/views.py
+-rw-r--r--   0        0        0      395 2024-04-26 07:51:03.905968 r_shepard-0.2.1/r_shepard/asgi.py
+-rw-r--r--   0        0        0      226 2024-04-26 08:04:10.741465 r_shepard-0.2.1/r_shepard/celery.py
+-rw-r--r--   0        0        0     4719 2024-05-10 09:29:20.434239 r_shepard-0.2.1/r_shepard/settings.py
+-rw-r--r--   0        0        0     1967 2024-05-10 09:20:02.868462 r_shepard-0.2.1/r_shepard/tests/test_models.py
+-rw-r--r--   0        0        0     1549 2024-04-30 14:46:22.169959 r_shepard-0.2.1/r_shepard/tests/test_views.py
+-rw-r--r--   0        0        0     2275 2024-04-30 14:28:56.240315 r_shepard-0.2.1/r_shepard/tests/utils.py
+-rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.2.1/r_shepard/urls.py
+-rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.2.1/r_shepard/wsgi.py
+-rw-r--r--   0        0        0      739 2024-04-23 16:45:21.318848 r_shepard-0.2.1/templates/base.html
+-rw-r--r--   0        0        0     4152 2024-05-08 13:25:20.796846 r_shepard-0.2.1/templates/container_list.html
+-rw-r--r--   0        0        0     2590 2024-05-08 13:56:15.535676 r_shepard-0.2.1/templates/project_detail.html
+-rw-r--r--   0        0        0     1150 2024-05-08 13:20:01.025476 r_shepard-0.2.1/templates/project_list.html
+-rw-r--r--   0        0        0      234 2024-04-22 17:10:53.021583 r_shepard-0.2.1/templates/two_factor/_base_focus.html
+-rw-r--r--   0        0        0      500 2024-04-22 16:49:01.953028 r_shepard-0.2.1/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0        0        0       90 2024-04-22 16:29:08.847147 r_shepard-0.2.1/templates/two_factor/_wizard_forms.html
+-rw-r--r--   0        0        0     1145 2024-04-22 16:29:08.812144 r_shepard-0.2.1/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0        0        0     2008 2024-04-22 16:48:40.642014 r_shepard-0.2.1/templates/two_factor/core/login.html
+-rw-r--r--   0        0        0      833 2024-04-22 16:29:08.813144 r_shepard-0.2.1/templates/two_factor/core/otp_required.html
+-rw-r--r--   0        0        0     3149 2024-04-22 16:29:08.813144 r_shepard-0.2.1/templates/two_factor/core/setup.html
+-rw-r--r--   0        0        0      963 2024-04-22 16:29:08.814144 r_shepard-0.2.1/templates/two_factor/core/setup_complete.html
+-rw-r--r--   0        0        0      529 2024-04-22 16:29:08.801143 r_shepard-0.2.1/templates/two_factor/profile/disable.html
+-rw-r--r--   0        0        0     2527 2024-04-23 08:51:59.180319 r_shepard-0.2.1/templates/two_factor/profile/profile.html
+-rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 r_shepard-0.2.1/PKG-INFO
```

### Comparing `r_shepard-0.2.0/README.md` & `r_shepard-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/manage.py` & `r_shepard-0.2.1/manage.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/admin.py` & `r_shepard-0.2.1/r_shepard/api/admin.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0001_initial.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0003_project_url.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0003_project_url.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0004_project_rstudio_version.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0004_project_rstudio_version.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0007_alter_container_container_id.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0007_alter_container_container_id.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0009_alter_container_port.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0009_alter_container_port.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0010_alter_container_port.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0010_alter_container_port.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0012_project_slug.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0012_project_slug.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0013_remove_project_password_container_password.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0013_remove_project_password_container_password.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0014_project_max_containers.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0014_project_max_containers.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0017_alter_container_container_id_alter_container_cpus_and_more.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0017_alter_container_container_id_alter_container_cpus_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0018_project_description.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0018_project_description.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/migrations/0019_alter_project_commit_interval_and_more.py` & `r_shepard-0.2.1/r_shepard/api/migrations/0019_alter_project_commit_interval_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/models.py` & `r_shepard-0.2.1/r_shepard/api/models.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/podman.py` & `r_shepard-0.2.1/r_shepard/api/podman.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/static/custom.css` & `r_shepard-0.2.1/r_shepard/api/static/custom.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/static/htmx.min.js` & `r_shepard-0.2.1/r_shepard/api/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/static/pico.blue.min.css` & `r_shepard-0.2.1/r_shepard/api/static/pico.blue.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/static/pico.colors.min.css` & `r_shepard-0.2.1/r_shepard/api/static/pico.colors.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/tailscale.py` & `r_shepard-0.2.1/r_shepard/api/tailscale.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/tasks.py` & `r_shepard-0.2.1/r_shepard/api/tasks.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/api/views.py` & `r_shepard-0.2.1/r_shepard/api/views.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/settings.py` & `r_shepard-0.2.1/r_shepard/settings.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/tests/test_models.py` & `r_shepard-0.2.1/r_shepard/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/tests/test_views.py` & `r_shepard-0.2.1/r_shepard/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/tests/utils.py` & `r_shepard-0.2.1/r_shepard/tests/utils.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/r_shepard/urls.py` & `r_shepard-0.2.1/r_shepard/urls.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/templates/base.html` & `r_shepard-0.2.1/templates/base.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/templates/container_list.html` & `r_shepard-0.2.1/templates/container_list.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/templates/project_detail.html` & `r_shepard-0.2.1/templates/project_detail.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/templates/project_list.html` & `r_shepard-0.2.1/templates/project_list.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/templates/two_factor/core/backup_tokens.html` & `r_shepard-0.2.1/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/templates/two_factor/core/login.html` & `r_shepard-0.2.1/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/templates/two_factor/core/otp_required.html` & `r_shepard-0.2.1/templates/two_factor/core/otp_required.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/templates/two_factor/core/setup.html` & `r_shepard-0.2.1/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/templates/two_factor/core/setup_complete.html` & `r_shepard-0.2.1/templates/two_factor/core/setup_complete.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/templates/two_factor/profile/disable.html` & `r_shepard-0.2.1/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/templates/two_factor/profile/profile.html` & `r_shepard-0.2.1/templates/two_factor/profile/profile.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.2.0/PKG-INFO` & `r_shepard-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r-shepard
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: GPL-3.0
 Author: linozen
 Author-email: linus@sehn.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

