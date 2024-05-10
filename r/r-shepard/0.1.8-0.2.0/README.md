# Comparing `tmp/r_shepard-0.1.8.tar.gz` & `tmp/r_shepard-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r_shepard-0.1.8.tar", max compression
+gzip compressed data, was "r_shepard-0.2.0.tar", max compression
```

## Comparing `r_shepard-0.1.8.tar` & `r_shepard-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0     3517 2024-05-07 13:27:13.812834 r_shepard-0.1.8/README.md
--rwxr-xr-x   0        0        0      666 2024-05-01 08:42:22.525077 r_shepard-0.1.8/manage.py
--rw-r--r--   0        0        0      807 2024-05-09 08:29:34.425486 r_shepard-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      174 2024-05-06 20:18:43.831721 r_shepard-0.1.8/r_shepard/__init__.py
--rw-r--r--   0        0        0       52 2024-05-06 21:14:06.784472 r_shepard-0.1.8/r_shepard/api/__init__.py
--rw-r--r--   0        0        0     3793 2024-05-08 13:45:19.864296 r_shepard-0.1.8/r_shepard/api/admin.py
--rw-r--r--   0        0        0      457 2024-05-07 10:02:03.501832 r_shepard-0.1.8/r_shepard/api/apps.py
--rw-r--r--   0        0        0      179 2024-05-06 21:14:06.784472 r_shepard-0.1.8/r_shepard/api/appy.py
--rw-r--r--   0        0        0     1137 2024-05-07 10:01:34.041125 r_shepard-0.1.8/r_shepard/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      442 2024-05-07 10:01:34.041125 r_shepard-0.1.8/r_shepard/api/migrations/0002_project_is_active.py
--rw-r--r--   0        0        0      505 2024-05-07 10:01:34.041125 r_shepard-0.1.8/r_shepard/api/migrations/0003_project_url.py
--rw-r--r--   0        0        0      460 2024-05-07 10:01:34.041125 r_shepard-0.1.8/r_shepard/api/migrations/0004_project_rstudio_version.py
--rw-r--r--   0        0        0     1103 2024-05-07 10:01:34.042125 r_shepard-0.1.8/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
--rw-r--r--   0        0        0     3210 2024-05-07 10:01:34.042125 r_shepard-0.1.8/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
--rw-r--r--   0        0        0      491 2024-05-07 10:01:34.043125 r_shepard-0.1.8/r_shepard/api/migrations/0007_alter_container_container_id.py
--rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.1.8/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
--rw-r--r--   0        0        0      506 2024-05-07 10:01:34.043125 r_shepard-0.1.8/r_shepard/api/migrations/0009_alter_container_port.py
--rw-r--r--   0        0        0      479 2024-05-07 10:01:34.043125 r_shepard-0.1.8/r_shepard/api/migrations/0010_alter_container_port.py
--rw-r--r--   0        0        0      518 2024-05-07 10:01:34.043125 r_shepard-0.1.8/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
--rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.1.8/r_shepard/api/migrations/0012_project_slug.py
--rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.1.8/r_shepard/api/migrations/0013_remove_project_password_container_password.py
--rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.1.8/r_shepard/api/migrations/0014_project_max_containers.py
--rw-r--r--   0        0        0      918 2024-04-24 13:21:19.864083 r_shepard-0.1.8/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
--rw-r--r--   0        0        0     1381 2024-04-24 13:32:06.450029 r_shepard-0.1.8/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
--rw-r--r--   0        0        0     3177 2024-05-08 12:34:05.383598 r_shepard-0.1.8/r_shepard/api/migrations/0017_alter_container_container_id_alter_container_cpus_and_more.py
--rw-r--r--   0        0        0      512 2024-05-08 13:12:31.128211 r_shepard-0.1.8/r_shepard/api/migrations/0018_project_description.py
--rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.1.8/r_shepard/api/migrations/__init__.py
--rw-r--r--   0        0        0     5679 2024-05-08 13:12:27.806227 r_shepard-0.1.8/r_shepard/api/models.py
--rw-r--r--   0        0        0     4385 2024-05-08 14:11:32.874857 r_shepard-0.1.8/r_shepard/api/podman.py
--rw-r--r--   0        0        0     3104 2024-05-08 13:55:02.555158 r_shepard-0.1.8/r_shepard/api/static/custom.css
--rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.1.8/r_shepard/api/static/htmx.min.js
--rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.1.8/r_shepard/api/static/pico.blue.min.css
--rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.1.8/r_shepard/api/static/pico.colors.min.css
--rw-r--r--   0        0        0     2982 2024-04-23 09:15:45.253107 r_shepard-0.1.8/r_shepard/api/tailscale.py
--rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.1.8/r_shepard/api/tasks.py
--rw-r--r--   0        0        0     5807 2024-05-07 10:02:03.502833 r_shepard-0.1.8/r_shepard/api/views.py
--rw-r--r--   0        0        0      395 2024-04-26 07:51:03.905968 r_shepard-0.1.8/r_shepard/asgi.py
--rw-r--r--   0        0        0      226 2024-04-26 08:04:10.741465 r_shepard-0.1.8/r_shepard/celery.py
--rw-r--r--   0        0        0     4494 2024-05-09 08:29:09.882539 r_shepard-0.1.8/r_shepard/settings.py
--rw-r--r--   0        0        0     1983 2024-04-26 08:33:25.063331 r_shepard-0.1.8/r_shepard/tests/test_models.py
--rw-r--r--   0        0        0     1549 2024-04-30 14:46:22.169959 r_shepard-0.1.8/r_shepard/tests/test_views.py
--rw-r--r--   0        0        0     2275 2024-04-30 14:28:56.240315 r_shepard-0.1.8/r_shepard/tests/utils.py
--rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.1.8/r_shepard/urls.py
--rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.1.8/r_shepard/wsgi.py
--rw-r--r--   0        0        0      356 2024-04-23 06:43:01.074990 r_shepard-0.1.8/templates/admin/base.html
--rw-r--r--   0        0        0      739 2024-04-23 16:45:21.318848 r_shepard-0.1.8/templates/base.html
--rw-r--r--   0        0        0     4152 2024-05-08 13:25:20.796846 r_shepard-0.1.8/templates/container_list.html
--rw-r--r--   0        0        0     2590 2024-05-08 13:56:15.535676 r_shepard-0.1.8/templates/project_detail.html
--rw-r--r--   0        0        0     1150 2024-05-08 13:20:01.025476 r_shepard-0.1.8/templates/project_list.html
--rw-r--r--   0        0        0      234 2024-04-22 17:10:53.021583 r_shepard-0.1.8/templates/two_factor/_base_focus.html
--rw-r--r--   0        0        0      500 2024-04-22 16:49:01.953028 r_shepard-0.1.8/templates/two_factor/_wizard_actions.html
--rw-r--r--   0        0        0       90 2024-04-22 16:29:08.847147 r_shepard-0.1.8/templates/two_factor/_wizard_forms.html
--rw-r--r--   0        0        0     1145 2024-04-22 16:29:08.812144 r_shepard-0.1.8/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0        0        0     2008 2024-04-22 16:48:40.642014 r_shepard-0.1.8/templates/two_factor/core/login.html
--rw-r--r--   0        0        0      833 2024-04-22 16:29:08.813144 r_shepard-0.1.8/templates/two_factor/core/otp_required.html
--rw-r--r--   0        0        0     3149 2024-04-22 16:29:08.813144 r_shepard-0.1.8/templates/two_factor/core/setup.html
--rw-r--r--   0        0        0      963 2024-04-22 16:29:08.814144 r_shepard-0.1.8/templates/two_factor/core/setup_complete.html
--rw-r--r--   0        0        0      529 2024-04-22 16:29:08.801143 r_shepard-0.1.8/templates/two_factor/profile/disable.html
--rw-r--r--   0        0        0     2527 2024-04-23 08:51:59.180319 r_shepard-0.1.8/templates/two_factor/profile/profile.html
--rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 r_shepard-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3517 2024-05-10 09:23:02.387390 r_shepard-0.2.0/README.md
+-rwxr-xr-x   0        0        0      666 2024-05-01 08:42:22.525077 r_shepard-0.2.0/manage.py
+-rw-r--r--   0        0        0      805 2024-05-10 09:22:50.020327 r_shepard-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      174 2024-05-06 20:18:43.831721 r_shepard-0.2.0/r_shepard/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-06 21:14:06.784472 r_shepard-0.2.0/r_shepard/api/__init__.py
+-rw-r--r--   0        0        0     4387 2024-05-10 09:11:26.291425 r_shepard-0.2.0/r_shepard/api/admin.py
+-rw-r--r--   0        0        0      457 2024-05-07 10:02:03.501832 r_shepard-0.2.0/r_shepard/api/apps.py
+-rw-r--r--   0        0        0      179 2024-05-06 21:14:06.784472 r_shepard-0.2.0/r_shepard/api/appy.py
+-rw-r--r--   0        0        0     2063 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0002_project_is_active.py
+-rw-r--r--   0        0        0      567 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0003_project_url.py
+-rw-r--r--   0        0        0      522 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0004_project_rstudio_version.py
+-rw-r--r--   0        0        0     1291 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
+-rw-r--r--   0        0        0     4980 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
+-rw-r--r--   0        0        0      553 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0007_alter_container_container_id.py
+-rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.2.0/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
+-rw-r--r--   0        0        0      552 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0009_alter_container_port.py
+-rw-r--r--   0        0        0      525 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0010_alter_container_port.py
+-rw-r--r--   0        0        0      596 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
+-rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.2.0/r_shepard/api/migrations/0012_project_slug.py
+-rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.2.0/r_shepard/api/migrations/0013_remove_project_password_container_password.py
+-rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.2.0/r_shepard/api/migrations/0014_project_max_containers.py
+-rw-r--r--   0        0        0      822 2024-05-10 09:11:20.381386 r_shepard-0.2.0/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
+-rw-r--r--   0        0        0     1285 2024-05-10 09:12:21.754790 r_shepard-0.2.0/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
+-rw-r--r--   0        0        0     3837 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0017_alter_container_container_id_alter_container_cpus_and_more.py
+-rw-r--r--   0        0        0      574 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0018_project_description.py
+-rw-r--r--   0        0        0     2681 2024-05-10 09:10:56.833226 r_shepard-0.2.0/r_shepard/api/migrations/0019_alter_project_commit_interval_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.2.0/r_shepard/api/migrations/__init__.py
+-rw-r--r--   0        0        0     6612 2024-05-10 09:19:46.724377 r_shepard-0.2.0/r_shepard/api/models.py
+-rw-r--r--   0        0        0     4637 2024-05-10 08:47:24.802782 r_shepard-0.2.0/r_shepard/api/podman.py
+-rw-r--r--   0        0        0     3104 2024-05-08 13:55:02.555158 r_shepard-0.2.0/r_shepard/api/static/custom.css
+-rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.2.0/r_shepard/api/static/htmx.min.js
+-rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.2.0/r_shepard/api/static/pico.blue.min.css
+-rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.2.0/r_shepard/api/static/pico.colors.min.css
+-rw-r--r--   0        0        0     3006 2024-05-10 08:47:24.802782 r_shepard-0.2.0/r_shepard/api/tailscale.py
+-rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.2.0/r_shepard/api/tasks.py
+-rw-r--r--   0        0        0     5807 2024-05-07 10:02:03.502833 r_shepard-0.2.0/r_shepard/api/views.py
+-rw-r--r--   0        0        0      395 2024-04-26 07:51:03.905968 r_shepard-0.2.0/r_shepard/asgi.py
+-rw-r--r--   0        0        0      226 2024-04-26 08:04:10.741465 r_shepard-0.2.0/r_shepard/celery.py
+-rw-r--r--   0        0        0     4719 2024-05-10 09:21:17.170852 r_shepard-0.2.0/r_shepard/settings.py
+-rw-r--r--   0        0        0     1967 2024-05-10 09:20:02.868462 r_shepard-0.2.0/r_shepard/tests/test_models.py
+-rw-r--r--   0        0        0     1549 2024-04-30 14:46:22.169959 r_shepard-0.2.0/r_shepard/tests/test_views.py
+-rw-r--r--   0        0        0     2275 2024-04-30 14:28:56.240315 r_shepard-0.2.0/r_shepard/tests/utils.py
+-rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.2.0/r_shepard/urls.py
+-rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.2.0/r_shepard/wsgi.py
+-rw-r--r--   0        0        0      356 2024-04-23 06:43:01.074990 r_shepard-0.2.0/templates/admin/base.html
+-rw-r--r--   0        0        0      739 2024-04-23 16:45:21.318848 r_shepard-0.2.0/templates/base.html
+-rw-r--r--   0        0        0     4152 2024-05-08 13:25:20.796846 r_shepard-0.2.0/templates/container_list.html
+-rw-r--r--   0        0        0     2590 2024-05-08 13:56:15.535676 r_shepard-0.2.0/templates/project_detail.html
+-rw-r--r--   0        0        0     1150 2024-05-08 13:20:01.025476 r_shepard-0.2.0/templates/project_list.html
+-rw-r--r--   0        0        0      234 2024-04-22 17:10:53.021583 r_shepard-0.2.0/templates/two_factor/_base_focus.html
+-rw-r--r--   0        0        0      500 2024-04-22 16:49:01.953028 r_shepard-0.2.0/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0        0        0       90 2024-04-22 16:29:08.847147 r_shepard-0.2.0/templates/two_factor/_wizard_forms.html
+-rw-r--r--   0        0        0     1145 2024-04-22 16:29:08.812144 r_shepard-0.2.0/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0        0        0     2008 2024-04-22 16:48:40.642014 r_shepard-0.2.0/templates/two_factor/core/login.html
+-rw-r--r--   0        0        0      833 2024-04-22 16:29:08.813144 r_shepard-0.2.0/templates/two_factor/core/otp_required.html
+-rw-r--r--   0        0        0     3149 2024-04-22 16:29:08.813144 r_shepard-0.2.0/templates/two_factor/core/setup.html
+-rw-r--r--   0        0        0      963 2024-04-22 16:29:08.814144 r_shepard-0.2.0/templates/two_factor/core/setup_complete.html
+-rw-r--r--   0        0        0      529 2024-04-22 16:29:08.801143 r_shepard-0.2.0/templates/two_factor/profile/disable.html
+-rw-r--r--   0        0        0     2527 2024-04-23 08:51:59.180319 r_shepard-0.2.0/templates/two_factor/profile/profile.html
+-rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 r_shepard-0.2.0/PKG-INFO
```

### Comparing `r_shepard-0.1.8/README.md` & `r_shepard-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/manage.py` & `r_shepard-0.2.0/manage.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/pyproject.toml` & `r_shepard-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 packages = [{ include = "r_shepard", from = "." }, { include = "manage.py" }]
 name = "r-shepard"
-version = "0.1.8"
+version = "0.2.0"
 description = ""
 authors = ["linozen <linus@sehn.dev>"]
 license = "GPL-3.0"
 readme = "README.md"
 include = ["templates/*"]
 
 [tool.poetry.dependencies]
@@ -23,12 +23,12 @@
 [tool.poetry.scripts]
 r-shepard = "manage:main"
 
 [tool.poetry.group.dev.dependencies]
 djlint = "^1.34.1"
 bumpversion = "^0.6.0"
 coverage = "^7.5.0"
-genbadge = { extras = ["coverage"], version = "^1.1.1" }
+genbadge = {extras = ["coverage"], version = "^1.1.1"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `r_shepard-0.1.8/r_shepard/api/admin.py` & `r_shepard-0.2.0/r_shepard/api/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,15 +96,42 @@
     def response_add(self, request, obj, post_url_continue=None):
         return HttpResponseRedirect(reverse("project_detail", args=[obj.project.pk]))
 
     def response_change(self, request: HttpRequest, obj: Any) -> HttpResponse:
         return HttpResponseRedirect(reverse("project_detail", args=[obj.project.pk]))
 
 
+class ProjectAddForm(forms.ModelForm):
+    class Meta:
+        model = Project
+        fields = [
+            "name",
+            "description",
+            "max_containers",
+            "max_ram",
+            "max_cpus",
+            "auto_commit_enabled",
+            "git_repo_url",
+            "commit_interval",
+        ]
+
+
+class ProjectChangeForm(forms.ModelForm):
+    class Meta:
+        model = Project
+        fields = "__all__"
+
+
 class ProjectAdmin(admin.ModelAdmin):
+    def get_form(self, request, obj=None, **kwargs):
+        if obj:
+            return ProjectChangeForm
+        else:
+            return ProjectAddForm
+
     def response_add(self, request, obj, post_url_continue=None):
         return HttpResponseRedirect(reverse("project_list"))
 
     def response_change(self, request: HttpRequest, obj: Any) -> HttpResponse:
         return HttpResponseRedirect(reverse("project_detail", args=[obj.pk]))
```

### Comparing `r_shepard-0.1.8/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py` & `r_shepard-0.2.0/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 # Generated by Django 5.0.4 on 2024-04-21 17:44
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('api', '0004_project_rstudio_version'),
+        ("api", "0004_project_rstudio_version"),
     ]
 
     operations = [
         migrations.RemoveField(
-            model_name='project',
-            name='url',
+            model_name="project",
+            name="url",
         ),
         migrations.AddField(
-            model_name='project',
-            name='local_url',
-            field=models.URLField(default='', help_text="Local URL to access the project's RStudio instance", max_length=1024),
+            model_name="project",
+            name="local_url",
+            field=models.URLField(
+                default="",
+                help_text="Local URL to access the project's RStudio instance",
+                max_length=1024,
+            ),
         ),
         migrations.AddField(
-            model_name='project',
-            name='tailscale_funnel_url',
-            field=models.URLField(default='', help_text="Tailscale Funnel URL to access the project's RStudio instance from the web", max_length=1024),
+            model_name="project",
+            name="tailscale_funnel_url",
+            field=models.URLField(
+                default="",
+                help_text="Tailscale Funnel URL to access the project's RStudio instance from the web",
+                max_length=1024,
+            ),
         ),
         migrations.AddField(
-            model_name='project',
-            name='tailscale_serve_url',
-            field=models.URLField(default='', help_text="Tailscale Serve URL to access the project's RStudio instance from the tailnet", max_length=1024),
+            model_name="project",
+            name="tailscale_serve_url",
+            field=models.URLField(
+                default="",
+                help_text="Tailscale Serve URL to access the project's RStudio instance from the tailnet",
+                max_length=1024,
+            ),
         ),
     ]
```

### Comparing `r_shepard-0.1.8/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py` & `r_shepard-0.2.0/r_shepard/api/migrations/0019_alter_project_commit_interval_and_more.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,79 @@
-# Generated by Django 5.0.4 on 2024-04-21 18:32
+# Generated by Django 5.0.4 on 2024-05-10 09:10
 
-import django.db.models.deletion
+import django.core.validators
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('api', '0005_remove_project_url_project_local_url_and_more'),
+        ("api", "0018_project_description"),
     ]
 
     operations = [
-        migrations.RemoveField(
-            model_name='project',
-            name='cpus',
-        ),
-        migrations.RemoveField(
-            model_name='project',
-            name='is_active',
-        ),
-        migrations.RemoveField(
-            model_name='project',
-            name='local_url',
-        ),
-        migrations.RemoveField(
-            model_name='project',
-            name='ram',
-        ),
-        migrations.RemoveField(
-            model_name='project',
-            name='rstudio_version',
-        ),
-        migrations.RemoveField(
-            model_name='project',
-            name='tailscale_funnel_url',
-        ),
-        migrations.RemoveField(
-            model_name='project',
-            name='tailscale_serve_url',
-        ),
-        migrations.AddField(
-            model_name='project',
-            name='max_cpus',
-            field=models.PositiveIntegerField(default=8, help_text='Maximum number of CPUs allocated to the project.'),
-        ),
-        migrations.AddField(
-            model_name='project',
-            name='max_ram',
-            field=models.PositiveIntegerField(default=32, help_text='Maximum amount of RAM in GB allocated for the project.'),
-        ),
-        migrations.CreateModel(
-            name='Container',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('image', models.CharField(default='rocker/rstudio', help_text='The name of the container image.', max_length=255)),
-                ('tag', models.CharField(default='latest', help_text='The tag of the container image.', max_length=255)),
-                ('container_id', models.CharField(default='4Dj19', help_text='The unique identifier of the container.', max_length=5, unique=True)),
-                ('ram', models.PositiveIntegerField(default=2, help_text='Amount of RAM in GB allocated for the container.')),
-                ('cpus', models.PositiveIntegerField(default=2, help_text='Number of CPUs allocated to the container.')),
-                ('local_url', models.URLField(default='', help_text="Local URL to access this container's RStudio instance", max_length=1024)),
-                ('tailscale_funnel_url', models.URLField(default='', help_text="Tailscale Funnel URL to access this container's RStudio instance from the web", max_length=1024)),
-                ('tailscale_serve_url', models.URLField(default='', help_text="Tailscale Serve URL to access this container's RStudio instance from the tailnet", max_length=1024)),
-                ('is_running', models.BooleanField(default=False, help_text='Indicates whether the container is running')),
-                ('project', models.ForeignKey(help_text='The project to which this container belongs.', on_delete=django.db.models.deletion.CASCADE, related_name='containers', to='api.project')),
-            ],
+        migrations.AlterField(
+            model_name="project",
+            name="commit_interval",
+            field=models.PositiveIntegerField(
+                default=15, help_text="Commit interval in minutes.", null=True
+            ),
+        ),
+        migrations.AlterField(
+            model_name="project",
+            name="git_repo_url",
+            field=models.CharField(
+                blank=True,
+                help_text="URL of the Git repository.",
+                max_length=255,
+                null=True,
+                validators=[
+                    django.core.validators.RegexValidator(
+                        "(git@|http:\\/\\/|https:\\/\\/)([\\w\\.@:]+)(\\/|:)([\\w\\.\\/\\-]+\\.git)",
+                        "Enter a valid Git URL.",
+                    )
+                ],
+                verbose_name="Git Repository URL",
+            ),
+        ),
+        migrations.AlterField(
+            model_name="project",
+            name="max_containers",
+            field=models.PositiveIntegerField(
+                default=4,
+                help_text="Maximum number of containers that can be run for the project.",
+                verbose_name="Max. number of containers",
+            ),
+        ),
+        migrations.AlterField(
+            model_name="project",
+            name="max_cpus",
+            field=models.PositiveIntegerField(
+                default=8,
+                help_text="Maximum number of CPUs allocated to the project.",
+                verbose_name="Max. CPUs",
+            ),
+        ),
+        migrations.AlterField(
+            model_name="project",
+            name="max_ram",
+            field=models.PositiveIntegerField(
+                default=32,
+                help_text="Maximum amount of RAM in GB allocated for the project.",
+                verbose_name="Max. RAM",
+            ),
+        ),
+        migrations.AlterField(
+            model_name="project",
+            name="name",
+            field=models.CharField(
+                help_text="The name of the project.",
+                max_length=255,
+                unique=True,
+                validators=[
+                    django.core.validators.RegexValidator(
+                        "^[\\w\\s]+$",
+                        "Enter a valid project name. This value may contain only letters, numbers, and whitespace.",
+                    )
+                ],
+            ),
         ),
     ]
```

### Comparing `r_shepard-0.1.8/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py` & `r_shepard-0.2.0/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py` & `r_shepard-0.2.0/r_shepard/api/migrations/0009_alter_container_port.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-# Generated by Django 5.0.4 on 2024-04-22 08:59
+# Generated by Django 5.0.4 on 2024-04-22 07:28
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('api', '0010_alter_container_port'),
+        ("api", "0008_container_port_alter_container_container_id_and_more"),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name='container',
-            name='tailscale_serve_url',
-            field=models.URLField(default='', help_text="Tailscale Serve URL to access this container's RStudio instance from the tailnet", max_length=1024, null=True),
+            model_name="container",
+            name="port",
+            field=models.PositiveIntegerField(
+                default=8787,
+                help_text="The port on which the container's RStudio instance is accessible.",
+            ),
         ),
     ]
```

### Comparing `r_shepard-0.1.8/r_shepard/api/migrations/0012_project_slug.py` & `r_shepard-0.2.0/r_shepard/api/migrations/0012_project_slug.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/api/migrations/0013_remove_project_password_container_password.py` & `r_shepard-0.2.0/r_shepard/api/migrations/0013_remove_project_password_container_password.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/api/migrations/0014_project_max_containers.py` & `r_shepard-0.2.0/r_shepard/api/migrations/0014_project_max_containers.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py` & `r_shepard-0.2.0/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-# Generated by Django 5.0.4 on 2024-04-24 13:21
+# Generated by Django 5.0.4 on 2024-04-24 13:32
 
-import r_shepard.api.models
+import datetime
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
-        ("api", "0014_project_max_containers"),
+        ("api", "0015_project_auto_commit_enabled_project_git_repo_url"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="project",
-            name="auto_commit_enabled",
-            field=models.BooleanField(
-                default=False,
-                help_text="Whether automatic commits are enabled for the workspace_path.",
+            name="commit_interval",
+            field=models.PositiveIntegerField(
+                default=60, help_text="Commit interval in seconds."
             ),
         ),
         migrations.AddField(
             model_name="project",
+            name="last_commit_time",
+            field=models.DateTimeField(
+                auto_now_add=True,
+                default=datetime.datetime(
+                    2024, 4, 24, 13, 32, 6, 347026, tzinfo=datetime.timezone.utc
+                ),
+                help_text="Last time the project was committed to the Git repository.",
+            ),
+            preserve_default=False,
+        ),
+        migrations.AlterField(
+            model_name="project",
             name="git_repo_url",
-            field=models.URLField(
+            field=models.CharField(
                 blank=True,
                 help_text="URL of the Git repository.",
                 max_length=255,
                 null=True,
-                validators=[r_shepard.api.models.validate_git_url],
             ),
         ),
     ]
```

### Comparing `r_shepard-0.1.8/r_shepard/api/models.py` & `r_shepard-0.2.0/r_shepard/api/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+import os
 import random
-import re
 import string
 
+from django.conf import settings
 from django.contrib.auth.hashers import check_password, make_password
-from django.core.exceptions import ValidationError
+from django.core.validators import RegexValidator
 from django.db import models
 from django.utils import timezone
 
-# Create your models here.
-
-
-def validate_git_url(value):
-    pattern = r"(git@|http:\/\/|https:\/\/)([\w\.@:]+)(\/|:)([\w\.\/\-]+\.git)"
-    if not re.match(pattern, value):
-        raise ValidationError(f"{value} is not a valid Git URL")
+DATA_DIR = settings.DATA_DIR
+WORKSPACE_DIR = settings.WORKSPACE_DIR
 
 
 class Project(models.Model):
     name = models.CharField(
         max_length=255,
         unique=True,
+        validators=[
+            RegexValidator(
+                r"^[\w\s]+$",
+                "Enter a valid project name. This value may contain only letters, numbers, and whitespace.",
+            )
+        ],
         help_text="The name of the project.",
     )
     description = models.CharField(
         default="",
         max_length=1024,
         help_text="A short description of your project (max. 1025 characters)",
     )
@@ -38,51 +40,77 @@
     )
     workspace_path = models.CharField(
         max_length=1024,
         help_text="Filesystem path where R scripts are stored. The containers have write access here.",
     )
     max_containers = models.PositiveIntegerField(
         default=4,
+        verbose_name="Max. number of containers",
         help_text="Maximum number of containers that can be run for the project.",
     )
     max_ram = models.PositiveIntegerField(
         default=32,
+        verbose_name="Max. RAM",
         help_text="Maximum amount of RAM in GB allocated for the project.",
     )
     max_cpus = models.PositiveIntegerField(
         default=8,
+        verbose_name="Max. CPUs",
         help_text="Maximum number of CPUs allocated to the project.",
     )
     auto_commit_enabled = models.BooleanField(
         default=False,
         help_text="Whether automatic commits are enabled for the workspace_path.",
     )
     git_repo_url = models.CharField(
         max_length=255,
         blank=True,
         null=True,
-        validators=[validate_git_url],
+        validators=[
+            RegexValidator(
+                r"(git@|http:\/\/|https:\/\/)([\w\.@:]+)(\/|:)([\w\.\/\-]+\.git)",
+                "Enter a valid Git URL.",
+            )
+        ],
+        verbose_name="Git Repository URL",
         help_text="URL of the Git repository.",
     )
     commit_interval = models.PositiveIntegerField(
-        default=15, help_text="Commit interval in minutes."
+        null=True,
+        default=15,
+        help_text="Commit interval in minutes.",
     )
     last_commit_time = models.DateTimeField(
         default=timezone.now,
         help_text="Last time the project was committed to the Git repository.",
     )
 
     # Generate a URL-safe slug for the project
     def generate_slug(self):
         """Generate a URL-safe slug from the project name."""
-        return self.name.lower().replace(" ", "_")
+        return self.name.lower().replace(" ", "-")
 
     def running_containers(self):
         return self.containers.filter(is_running=True)
 
+    def save(self, *args, **kwargs):
+        if not self.pk:
+            # Generate slug from project name
+            self.slug = self.generate_slug()
+
+            # Set the paths with slug
+            self.data_path = f"{DATA_DIR}/{self.slug}"
+            self.workspace_path = f"{WORKSPACE_DIR}/{self.slug}"
+
+            # Create the project directories
+            os.makedirs(self.data_path, exist_ok=True)
+            os.makedirs(self.workspace_path, exist_ok=True)
+
+        super().save(*args, **kwargs)
+
     def __str__(self):
         return self.name
 
 
 class Container(models.Model):
     class Meta:
         unique_together = ("project", "container_id")
```

### Comparing `r_shepard-0.1.8/r_shepard/api/podman.py` & `r_shepard-0.2.0/r_shepard/api/podman.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import os
-
+from django.conf import settings
 from podman import PodmanClient
 from podman.errors import NotFound
 
 from .models import Container, Project
 
-HOST_IP = "localhost"
-PODMAN_SOCKET = os.getenv("PODMAN_SOCKET", "unix:/run/user/1000/podman/podman.sock")
+# Get the podman settings from the Django settings
+PODMAN_HOST_ADDRESS = settings.PODMAN_HOST_ADDRESS
+PODMAN_SOCKET = settings.PODMAN_SOCKET
 
 
 # 'container' always refers to the Container model instance whereas
 # 'podman_container' refers to the podman container instance
 
 
 class PodmanError(Exception):
@@ -30,15 +30,15 @@
 def start_and_save_container(podman_container, container):
     """Start the podman container and save the container details."""
     podman_container.start()
     podman_container.reload()
 
     if not container.tailscale_serve_url:
         container.port = podman_container.ports["8787/tcp"][0]["HostPort"]
-        container.local_url = f"http://{HOST_IP}:{container.port}"
+        container.local_url = f"http://{PODMAN_HOST_ADDRESS}:{container.port}"
         container.save()
 
     print(f"Container started at {container.local_url}")
 
 
 def create_container_config(project, container, password):
     """Create the container configuration. Right now, it only supports RStudio."""
@@ -82,14 +82,17 @@
         else:
             print("Container does not exist, creating...")
             container_config = create_container_config(project, container, password)
             try:
                 podman_container = client.containers.create(**container_config)
                 start_and_save_container(podman_container, container)
             except Exception as e:
+                # TODO Handle cases where the container creation fails because
+                # of a missing directory and create it during project creation
+                # ideally
                 raise PodmanError(f"Failed to start container: {e}")
 
 
 def stop_container(project: Project, container: Container):
     with PodmanClient(base_url=PODMAN_SOCKET) as client:
         try:
             podman_container = client.containers.get(
```

### Comparing `r_shepard-0.1.8/r_shepard/api/static/custom.css` & `r_shepard-0.2.0/r_shepard/api/static/custom.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/api/static/htmx.min.js` & `r_shepard-0.2.0/r_shepard/api/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/api/static/pico.blue.min.css` & `r_shepard-0.2.0/r_shepard/api/static/pico.blue.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/api/static/pico.colors.min.css` & `r_shepard-0.2.0/r_shepard/api/static/pico.colors.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/api/tailscale.py` & `r_shepard-0.2.0/r_shepard/api/tailscale.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import subprocess
 
 from podman import PodmanClient
 
 from .models import Container
-from .podman import HOST_IP, PODMAN_SOCKET
+from .podman import PODMAN_HOST_ADDRESS, PODMAN_SOCKET
 
 
 def tailscale_serve(port: int, bg: bool = True, path: str = None):
     command = "tailscale serve"
     if bg:
         command += " --bg"
     if path:
@@ -71,15 +71,15 @@
             ],
             privileged=True,
             detach=True,
         )
         podman_container.restart()
 
     container.tailscale_serve_url = ""
-    container.local_url = f"http://{HOST_IP}:{container.port}"
+    container.local_url = f"http://{PODMAN_HOST_ADDRESS}:{container.port}"
     container.save()
 
 
 def tailscale_funnel(port: int, bg: bool = True, path: str = None):
     command = "tailscale funnel"
     if bg:
         command += " --bg"
```

### Comparing `r_shepard-0.1.8/r_shepard/api/tasks.py` & `r_shepard-0.2.0/r_shepard/api/tasks.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/api/views.py` & `r_shepard-0.2.0/r_shepard/api/views.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/settings.py` & `r_shepard-0.2.0/r_shepard/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 BASE_DIR = Path(__file__).resolve().parent.parent
 
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/5.0/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
-SECRET_KEY = "django-insecure-yc+#%@i2_hyrl1ut+c-9#ejwrv6(cv2de=-2+dv375a+oal*n7"
+SECRET_KEY = os.getenv(
+    "SECRET_KEY", "django-insecure-yc+#%@i2_hyrl1ut+c-9#ejwrv6(cv2de=-2+dv375a+oal*n7"
+)
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
 ALLOWED_HOSTS = os.getenv("ALLOWED_HOSTS", "127.0.0.1").split(",")
 CSRF_TRUSTED_ORIGINS = os.getenv("CSRF_TRUSTED_ORIGINS", "http://127.0.0.1").split(",")
 
@@ -130,15 +132,15 @@
 USE_TZ = True
 
 
 # Static files (CSS, JavaScript, Images)
 # https://docs.djangoproject.com/en/5.0/howto/static-files/
 
 STATIC_URL = "static/"
-STATIC_ROOT = os.environ.get("STATIC_ROOT", "/home/r-shepard/static/")
+STATIC_ROOT = os.environ.get("STATIC_ROOT", "/var/www/r-shepard/")
 
 # Default primary key field type
 # https://docs.djangoproject.com/en/5.0/ref/settings/#default-auto-field
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 
 # Celery settings
@@ -149,8 +151,13 @@
     "auto_commit": {
         "task": "r_shepard.api.tasks.auto_commit",
         "schedule": 15,
     }
 }
 
 # Podman settings
+PODMAN_HOST_ADDRESS = os.getenv("HOST_ADDRESS", "localhost")
 PODMAN_SOCKET = os.getenv("PODMAN_SOCKET", "unix:/run/user/1000/podman/podman.sock")
+
+# R-Shepard data directories
+DATA_DIR = os.getenv("DATA_DIR", "/tmp/data")
+WORKSPACE_DIR = os.getenv("WORKSPACE_DIR", "/tmp/workspace")
```

### Comparing `r_shepard-0.1.8/r_shepard/tests/test_models.py` & `r_shepard-0.2.0/r_shepard/tests/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 
 
 class ProjectModelTest(TestCase):
     def setUp(self):
         self.project = Project.objects.create(
             name="Test Project",
             slug="test-project",
-            data_path="/path/to/data",
-            workspace_path="/path/to/workspace",
+            data_path="/tmp/data",
+            workspace_path="/tmp/workspace",
             max_containers=4,
             max_ram=32,
             max_cpus=8,
             auto_commit_enabled=False,
             git_repo_url="https://github.com/user/repo.git",
             commit_interval=15,
         )
 
     def test_project_creation(self):
         self.assertIsInstance(self.project, Project)
         self.assertEqual(self.project.__str__(), "Test Project")
 
     def test_generate_slug(self):
-        self.assertEqual(self.project.generate_slug(), "test_project")
+        self.assertEqual(self.project.generate_slug(), "test-project")
 
 
 class ContainerModelTest(TestCase):
     def setUp(self):
         self.project = Project.objects.create(
             name="Test Project",
             slug="test-project",
-            data_path="/path/to/data",
-            workspace_path="/path/to/workspace",
+            data_path="/tmp/data",
+            workspace_path="/tmp/workspace",
             max_containers=4,
             max_ram=32,
             max_cpus=8,
             auto_commit_enabled=False,
             git_repo_url="https://github.com/user/repo.git",
             commit_interval=15,
         )
```

### Comparing `r_shepard-0.1.8/r_shepard/tests/test_views.py` & `r_shepard-0.2.0/r_shepard/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/tests/utils.py` & `r_shepard-0.2.0/r_shepard/tests/utils.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/r_shepard/urls.py` & `r_shepard-0.2.0/r_shepard/urls.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/templates/base.html` & `r_shepard-0.2.0/templates/base.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/templates/container_list.html` & `r_shepard-0.2.0/templates/container_list.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/templates/project_detail.html` & `r_shepard-0.2.0/templates/project_detail.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/templates/project_list.html` & `r_shepard-0.2.0/templates/project_list.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/templates/two_factor/core/backup_tokens.html` & `r_shepard-0.2.0/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/templates/two_factor/core/login.html` & `r_shepard-0.2.0/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/templates/two_factor/core/otp_required.html` & `r_shepard-0.2.0/templates/two_factor/core/otp_required.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/templates/two_factor/core/setup.html` & `r_shepard-0.2.0/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/templates/two_factor/core/setup_complete.html` & `r_shepard-0.2.0/templates/two_factor/core/setup_complete.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/templates/two_factor/profile/disable.html` & `r_shepard-0.2.0/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/templates/two_factor/profile/profile.html` & `r_shepard-0.2.0/templates/two_factor/profile/profile.html`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.8/PKG-INFO` & `r_shepard-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r-shepard
-Version: 0.1.8
+Version: 0.2.0
 Summary: 
 License: GPL-3.0
 Author: linozen
 Author-email: linus@sehn.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

