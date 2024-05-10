# Comparing `tmp/django_tasks_scheduler-1.3.2.tar.gz` & `tmp/django_tasks_scheduler-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tasks_scheduler-1.3.2.tar", max compression
+gzip compressed data, was "django_tasks_scheduler-1.3.3.tar", max compression
```

## Comparing `django_tasks_scheduler-1.3.2.tar` & `django_tasks_scheduler-1.3.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1107 2024-03-20 19:17:52.864126 django_tasks_scheduler-1.3.2/LICENSE
--rw-r--r--   0        0        0      758 2024-03-20 19:17:52.864126 django_tasks_scheduler-1.3.2/README.md
--rw-r--r--   0        0        0     2037 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      137 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/__init__.py
--rw-r--r--   0        0        0      113 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/admin/__init__.py
--rw-r--r--   0        0        0     1471 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/admin/redis_models.py
--rw-r--r--   0        0        0     6088 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/admin/task_models.py
--rw-r--r--   0        0        0      277 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/apps.py
--rw-r--r--   0        0        0     1216 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/decorators.py
--rw-r--r--   0        0        0        0 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/management/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/management/commands/__init__.py
--rw-r--r--   0        0        0     1285 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/management/commands/delete_failed_executions.py
--rw-r--r--   0        0        0     1907 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/management/commands/export.py
--rw-r--r--   0        0        0     4077 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/management/commands/import.py
--rw-r--r--   0        0        0     3439 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/management/commands/rqstats.py
--rw-r--r--   0        0        0     3176 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/management/commands/rqworker.py
--rw-r--r--   0        0        0     1374 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/management/commands/run_job.py
--rw-r--r--   0        0        0     6402 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
--rw-r--r--   0        0        0      898 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
--rw-r--r--   0        0        0     4196 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0003_auto_20220329_2107.py
--rw-r--r--   0        0        0      791 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      896 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      728 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0006_auto_20230118_1640.py
--rw-r--r--   0        0        0     1302 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0007_add_result_ttl.py
--rw-r--r--   0        0        0     1982 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
--rw-r--r--   0        0        0     1362 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
--rw-r--r--   0        0        0      661 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0010_queue.py
--rw-r--r--   0        0        0     7643 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
--rw-r--r--   0        0        0      934 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py
--rw-r--r--   0        0        0     1320 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py
--rw-r--r--   0        0        0     1261 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0014_alter_cronjob_created_alter_cronjob_modified_and_more.py
--rw-r--r--   0        0        0      608 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0015_rename_cronjob_crontask_and_more.py
--rw-r--r--   0        0        0     1116 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0016_rename_jobarg_taskarg_rename_jobkwarg_taskkwarg_and_more.py
--rw-r--r--   0        0        0     2410 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/0017_remove_crontask_repeat_crontask_failed_runs_and_more.py
--rw-r--r--   0        0        0        0 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/migrations/__init__.py
--rw-r--r--   0        0        0      195 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/models/__init__.py
--rw-r--r--   0        0        0     3123 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/models/args.py
--rw-r--r--   0        0        0      364 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/models/queue.py
--rw-r--r--   0        0        0    17440 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/models/scheduled_task.py
--rw-r--r--   0        0        0      366 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/models/worker.py
--rw-r--r--   0        0        0        0 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/py.typed
--rw-r--r--   0        0        0     5056 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/queues.py
--rw-r--r--   0        0        0     9224 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/rq_classes.py
--rw-r--r--   0        0        0     1247 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/settings.py
--rw-r--r--   0        0        0      163 2024-03-20 19:17:52.868126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/change_form.html
--rw-r--r--   0        0        0      127 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/change_list.html
--rw-r--r--   0        0        0     1595 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/confirm_action.html
--rw-r--r--   0        0        0     7783 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/job_detail.html
--rw-r--r--   0        0        0     2697 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/jobs-list.partial.html
--rw-r--r--   0        0        0     6360 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/jobs.html
--rw-r--r--   0        0        0      915 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/queue_workers.html
--rw-r--r--   0        0        0      568 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/scheduler_base.html
--rw-r--r--   0        0        0     1325 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/single_job_action.html
--rw-r--r--   0        0        0     4224 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/stats.html
--rw-r--r--   0        0        0     3032 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/worker_details.html
--rw-r--r--   0        0        0     1891 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/workers-list.partial.html
--rw-r--r--   0        0        0      935 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/workers.html
--rw-r--r--   0        0        0        0 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templatetags/__init__.py
--rw-r--r--   0        0        0     1658 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/templatetags/scheduler_tags.py
--rw-r--r--   0        0        0        0 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/__init__.py
--rw-r--r--   0        0        0      672 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/jobs.py
--rw-r--r--   0        0        0     3051 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/test_cron_task.py
--rw-r--r--   0        0        0      685 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/test_internals.py
--rw-r--r--   0        0        0     5962 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/test_job_arg_models.py
--rw-r--r--   0        0        0     2355 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/test_job_decorator.py
--rw-r--r--   0        0        0    11035 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/test_mgmt_cmds.py
--rw-r--r--   0        0        0    21024 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/test_models.py
--rw-r--r--   0        0        0      807 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/test_redis_models.py
--rw-r--r--   0        0        0     8116 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/test_repeatable_task.py
--rw-r--r--   0        0        0     2261 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/test_settings.py
--rw-r--r--   0        0        0    20707 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/test_views.py
--rw-r--r--   0        0        0     1580 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/test_worker.py
--rw-r--r--   0        0        0     3441 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tests/testtools.py
--rw-r--r--   0        0        0     2728 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/tools.py
--rw-r--r--   0        0        0     1121 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/urls.py
--rw-r--r--   0        0        0    16626 2024-03-20 19:17:52.872126 django_tasks_scheduler-1.3.2/scheduler/views.py
--rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 django_tasks_scheduler-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1107 2024-05-10 13:46:43.431240 django_tasks_scheduler-1.3.3/LICENSE
+-rw-r--r--   0        0        0      758 2024-05-10 13:46:43.431240 django_tasks_scheduler-1.3.3/README.md
+-rw-r--r--   0        0        0     2035 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      137 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/admin/__init__.py
+-rw-r--r--   0        0        0     1471 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/admin/redis_models.py
+-rw-r--r--   0        0        0     6088 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/admin/task_models.py
+-rw-r--r--   0        0        0      427 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/apps.py
+-rw-r--r--   0        0        0     1216 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/decorators.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/management/commands/__init__.py
+-rw-r--r--   0        0        0     1285 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/management/commands/delete_failed_executions.py
+-rw-r--r--   0        0        0     1907 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/management/commands/export.py
+-rw-r--r--   0        0        0     4077 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/management/commands/import.py
+-rw-r--r--   0        0        0     3439 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/management/commands/rqstats.py
+-rw-r--r--   0        0        0     3176 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/management/commands/rqworker.py
+-rw-r--r--   0        0        0     1374 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/management/commands/run_job.py
+-rw-r--r--   0        0        0     6402 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
+-rw-r--r--   0        0        0      898 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
+-rw-r--r--   0        0        0     4196 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0003_auto_20220329_2107.py
+-rw-r--r--   0        0        0      791 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      896 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      728 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0006_auto_20230118_1640.py
+-rw-r--r--   0        0        0     1302 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0007_add_result_ttl.py
+-rw-r--r--   0        0        0     1982 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
+-rw-r--r--   0        0        0     1362 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
+-rw-r--r--   0        0        0      661 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0010_queue.py
+-rw-r--r--   0        0        0     7643 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
+-rw-r--r--   0        0        0      934 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py
+-rw-r--r--   0        0        0     1320 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py
+-rw-r--r--   0        0        0     1261 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0014_alter_cronjob_created_alter_cronjob_modified_and_more.py
+-rw-r--r--   0        0        0      608 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0015_rename_cronjob_crontask_and_more.py
+-rw-r--r--   0        0        0     1116 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0016_rename_jobarg_taskarg_rename_jobkwarg_taskkwarg_and_more.py
+-rw-r--r--   0        0        0     2410 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/0017_remove_crontask_repeat_crontask_failed_runs_and_more.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/migrations/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/models/__init__.py
+-rw-r--r--   0        0        0     3123 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/models/args.py
+-rw-r--r--   0        0        0      364 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/models/queue.py
+-rw-r--r--   0        0        0    17452 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/models/scheduled_task.py
+-rw-r--r--   0        0        0      366 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/models/worker.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/py.typed
+-rw-r--r--   0        0        0     5056 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/queues.py
+-rw-r--r--   0        0        0     9224 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/rq_classes.py
+-rw-r--r--   0        0        0     1247 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/settings.py
+-rw-r--r--   0        0        0      163 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/change_form.html
+-rw-r--r--   0        0        0      127 2024-05-10 13:46:43.435240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/change_list.html
+-rw-r--r--   0        0        0     1595 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/confirm_action.html
+-rw-r--r--   0        0        0     7783 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/job_detail.html
+-rw-r--r--   0        0        0     2697 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/jobs-list.partial.html
+-rw-r--r--   0        0        0     6360 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/jobs.html
+-rw-r--r--   0        0        0      915 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/queue_workers.html
+-rw-r--r--   0        0        0      568 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/scheduler_base.html
+-rw-r--r--   0        0        0     1325 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/single_job_action.html
+-rw-r--r--   0        0        0     4224 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/stats.html
+-rw-r--r--   0        0        0     3032 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/worker_details.html
+-rw-r--r--   0        0        0     1891 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/workers-list.partial.html
+-rw-r--r--   0        0        0      935 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/workers.html
+-rw-r--r--   0        0        0        0 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templatetags/__init__.py
+-rw-r--r--   0        0        0     1658 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/templatetags/scheduler_tags.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/__init__.py
+-rw-r--r--   0        0        0      672 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/jobs.py
+-rw-r--r--   0        0        0     3051 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/test_cron_task.py
+-rw-r--r--   0        0        0      685 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/test_internals.py
+-rw-r--r--   0        0        0     5962 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/test_job_arg_models.py
+-rw-r--r--   0        0        0     2355 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/test_job_decorator.py
+-rw-r--r--   0        0        0    11035 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/test_mgmt_cmds.py
+-rw-r--r--   0        0        0    21024 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/test_models.py
+-rw-r--r--   0        0        0      807 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/test_redis_models.py
+-rw-r--r--   0        0        0     8116 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/test_repeatable_task.py
+-rw-r--r--   0        0        0     2261 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/test_settings.py
+-rw-r--r--   0        0        0    20707 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/test_views.py
+-rw-r--r--   0        0        0     1580 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/test_worker.py
+-rw-r--r--   0        0        0     3441 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tests/testtools.py
+-rw-r--r--   0        0        0     2728 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/tools.py
+-rw-r--r--   0        0        0     1121 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/urls.py
+-rw-r--r--   0        0        0    16626 2024-05-10 13:46:43.439240 django_tasks_scheduler-1.3.3/scheduler/views.py
+-rw-r--r--   0        0        0     2513 1970-01-01 00:00:00.000000 django_tasks_scheduler-1.3.3/PKG-INFO
```

### Comparing `django_tasks_scheduler-1.3.2/LICENSE` & `django_tasks_scheduler-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/README.md` & `django_tasks_scheduler-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/pyproject.toml` & `django_tasks_scheduler-1.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-tasks-scheduler"
 packages = [
     { include = "scheduler" },
 ]
-version = "1.3.2"
+version = "1.3.3"
 description = "An async job scheduler for django using redis"
 readme = "README.md"
 keywords = ["redis", "django", "background-jobs", "job-queue", "task-queue", "redis-queue", "scheduled-jobs"]
 authors = [
     "Daniel Moran <daniel@moransoftware.ca>",
 ]
 maintainers = [
@@ -44,22 +44,22 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/dsoftwareinc/django-tasks-scheduler/issues"
 "Funding" = "https://github.com/sponsors/cunla"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 django = ">=3.2"
-croniter = "^2.0.3"
+croniter = "^2.0"
 click = "^8.1"
 rq = "^1.16"
 pyyaml = { version = "^6.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 poetry = "^1.8.2"
-coverage = "^7.4"
+coverage = "^7.5"
 fakeredis = { version = "^2.21.1", extras = ['lua'] }
 Flake8-pyproject = "^1.2"
 pyyaml = "^6"
 freezegun = "^1.3"
 
 
 [tool.poetry.extras]
```

### Comparing `django_tasks_scheduler-1.3.2/scheduler/admin/redis_models.py` & `django_tasks_scheduler-1.3.3/scheduler/admin/redis_models.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/admin/task_models.py` & `django_tasks_scheduler-1.3.3/scheduler/admin/task_models.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/decorators.py` & `django_tasks_scheduler-1.3.3/scheduler/decorators.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/management/commands/delete_failed_executions.py` & `django_tasks_scheduler-1.3.3/scheduler/management/commands/delete_failed_executions.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/management/commands/export.py` & `django_tasks_scheduler-1.3.3/scheduler/management/commands/export.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/management/commands/import.py` & `django_tasks_scheduler-1.3.3/scheduler/management/commands/import.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/management/commands/rqstats.py` & `django_tasks_scheduler-1.3.3/scheduler/management/commands/rqstats.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/management/commands/rqworker.py` & `django_tasks_scheduler-1.3.3/scheduler/management/commands/rqworker.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/management/commands/run_job.py` & `django_tasks_scheduler-1.3.3/scheduler/management/commands/run_job.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0003_auto_20220329_2107.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0003_auto_20220329_2107.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0006_auto_20230118_1640.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0006_auto_20230118_1640.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0007_add_result_ttl.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0007_add_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0010_queue.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0010_queue.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0014_alter_cronjob_created_alter_cronjob_modified_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0014_alter_cronjob_created_alter_cronjob_modified_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0015_rename_cronjob_crontask_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0015_rename_cronjob_crontask_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0016_rename_jobarg_taskarg_rename_jobkwarg_taskkwarg_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0016_rename_jobarg_taskarg_rename_jobkwarg_taskkwarg_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/migrations/0017_remove_crontask_repeat_crontask_failed_runs_and_more.py` & `django_tasks_scheduler-1.3.3/scheduler/migrations/0017_remove_crontask_repeat_crontask_failed_runs_and_more.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/models/args.py` & `django_tasks_scheduler-1.3.3/scheduler/models/args.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/models/scheduled_task.py` & `django_tasks_scheduler-1.3.3/scheduler/models/scheduled_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         task.last_successful_run = timezone.now()
     task.save(schedule_job=True)
 
 
 class BaseTask(models.Model):
     created = models.DateTimeField(auto_now_add=True)
     modified = models.DateTimeField(auto_now=True)
-    QUEUES = [(key, key) for key in settings.QUEUES.keys()]
+    QUEUES = [("default", "default"), ("low", "low"), ("high", "high")]
     TASK_TYPE = 'BaseTask'
     name = models.CharField(
         _('name'), max_length=128, unique=True,
         help_text='Name of the job.', )
     callable = models.CharField(_('callable'), max_length=2048)
     callable_args = GenericRelation(TaskArg, related_query_name='args')
     callable_kwargs = GenericRelation(TaskKwarg, related_query_name='kwargs')
```

### Comparing `django_tasks_scheduler-1.3.2/scheduler/queues.py` & `django_tasks_scheduler-1.3.3/scheduler/queues.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/rq_classes.py` & `django_tasks_scheduler-1.3.3/scheduler/rq_classes.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/settings.py` & `django_tasks_scheduler-1.3.3/scheduler/settings.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/confirm_action.html` & `django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/confirm_action.html`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/job_detail.html` & `django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/job_detail.html`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/jobs-list.partial.html` & `django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/jobs-list.partial.html`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/jobs.html` & `django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/jobs.html`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/queue_workers.html` & `django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/queue_workers.html`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/scheduler_base.html` & `django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/scheduler_base.html`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/single_job_action.html` & `django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/single_job_action.html`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/stats.html` & `django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/stats.html`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/worker_details.html` & `django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/worker_details.html`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/workers-list.partial.html` & `django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/workers-list.partial.html`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templates/admin/scheduler/workers.html` & `django_tasks_scheduler-1.3.3/scheduler/templates/admin/scheduler/workers.html`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/templatetags/scheduler_tags.py` & `django_tasks_scheduler-1.3.3/scheduler/templatetags/scheduler_tags.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/jobs.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/jobs.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/test_cron_task.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/test_cron_task.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/test_internals.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/test_job_arg_models.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/test_job_arg_models.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/test_job_decorator.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/test_job_decorator.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/test_mgmt_cmds.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/test_mgmt_cmds.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/test_models.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/test_redis_models.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/test_redis_models.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/test_repeatable_task.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/test_repeatable_task.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/test_settings.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/test_views.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/test_worker.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tests/testtools.py` & `django_tasks_scheduler-1.3.3/scheduler/tests/testtools.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/tools.py` & `django_tasks_scheduler-1.3.3/scheduler/tools.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/urls.py` & `django_tasks_scheduler-1.3.3/scheduler/urls.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/scheduler/views.py` & `django_tasks_scheduler-1.3.3/scheduler/views.py`

 * *Files identical despite different names*

### Comparing `django_tasks_scheduler-1.3.2/PKG-INFO` & `django_tasks_scheduler-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tasks-scheduler
-Version: 1.3.2
+Version: 1.3.3
 Summary: An async job scheduler for django using redis
 Home-page: https://github.com/dsoftwareinc/django-tasks-scheduler
 License: MIT
 Keywords: redis,django,background-jobs,job-queue,task-queue,redis-queue,scheduled-jobs
 Author: Daniel Moran
 Author-email: daniel@moransoftware.ca
 Maintainer: Daniel Moran
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: yaml
 Requires-Dist: click (>=8.1,<9.0)
-Requires-Dist: croniter (>=2.0.3,<3.0.0)
+Requires-Dist: croniter (>=2.0,<3.0)
 Requires-Dist: django (>=3.2)
 Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml"
 Requires-Dist: rq (>=1.16,<2.0)
 Project-URL: Bug Tracker, https://github.com/dsoftwareinc/django-tasks-scheduler/issues
 Project-URL: Documentation, https://django-tasks-scheduler.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/cunla
 Description-Content-Type: text/markdown
```

