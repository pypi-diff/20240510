# Comparing `tmp/django_flow_forge-0.3.4.tar.gz` & `tmp/django_flow_forge-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_flow_forge-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_flow_forge-0.3.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_flow_forge-0.3.4.tar` & `django_flow_forge-0.3.6.tar`

### file list

```diff
@@ -1,122 +1,123 @@
--rw-r--r--   0        0        0     6148 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.DS_Store
--rw-r--r--   0        0        0       66 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.gitattributes
--rw-r--r--   0        0        0      862 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.github/workflows/deploy-mkdocs.yml
--rw-r--r--   0        0        0      620 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     2879 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.gitignore
--rw-r--r--   0        0        0     1613 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.vscode/launch.json
--rw-r--r--   0        0        0     1103 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/Dockerfile
--rw-r--r--   0        0        0     1061 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/LICENSE
--rw-r--r--   0        0        0      151 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/MANIFEST.in
--rw-r--r--   0        0        0      865 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/README.md
--rwxr-xr-x   0        0        0        0 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/__init__.py
--rwxr-xr-x   0        0        0     2914 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/admin.py
--rwxr-xr-x   0        0        0      160 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/apps.py
--rw-r--r--   0        0        0     2306 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/async_utils.py
--rw-r--r--   0        0        0     2950 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/authorization.py
--rw-r--r--   0        0        0     1190 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/batch_utils.py
--rw-r--r--   0        0        0    15970 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/flow_engine.py
--rw-r--r--   0        0        0     5435 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0001_initial.py
--rw-r--r--   0        0        0      816 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py
--rw-r--r--   0        0        0      449 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0003_alter_executedtask_exceptions.py
--rw-r--r--   0        0        0      624 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py
--rw-r--r--   0        0        0      428 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0005_alter_flow_options.py
--rw-r--r--   0        0        0      564 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py
--rw-r--r--   0        0        0      436 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0007_executedflow_params.py
--rw-r--r--   0        0        0      419 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0008_executedflow_meta.py
--rw-r--r--   0        0        0     1411 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0009_flowbatch_flowbatchtempdata.py
--rw-r--r--   0        0        0     1066 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0010_batchhandler.py
--rw-r--r--   0        0        0     2004 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0011_remove_flowbatchtempdata_batch_and_more.py
--rw-r--r--   0        0        0      416 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0012_rename_total_batches_batchhandler_total_batch_count.py
--rw-r--r--   0        0        0     1346 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0013_remove_batchtempdata_batch_handler_flowbatch_and_more.py
--rw-r--r--   0        0        0      345 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0014_delete_batchtempdata.py
--rwxr-xr-x   0        0        0        0 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/__init__.py
--rw-r--r--   0        0        0      778 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0001_initial.py
--rw-r--r--   0        0        0      392 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0002_processtask_task_output.py
--rw-r--r--   0        0        0     1236 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py
--rw-r--r--   0        0        0      451 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0004_processtask_nested_task.py
--rw-r--r--   0        0        0      400 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0005_rename_nested_task_processtask_bidirectional_task.py
--rw-r--r--   0        0        0      627 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py
--rw-r--r--   0        0        0      448 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0007_rename_bidirectional_dependencies_processtask_depends_bidirectionally_with.py
--rw-r--r--   0        0        0      444 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0008_rename_dependencies_processtask_depends_on.py
--rw-r--r--   0        0        0     1717 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py
--rw-r--r--   0        0        0      414 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0010_processtask_nested.py
--rw-r--r--   0        0        0      573 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py
--rw-r--r--   0        0        0      980 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py
--rw-r--r--   0        0        0      537 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py
--rw-r--r--   0        0        0      732 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py
--rw-r--r--   0        0        0      432 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0015_alter_taskrun_output.py
--rw-r--r--   0        0        0      467 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0016_rename_processrun_executedprocess_and_more.py
--rw-r--r--   0        0        0      613 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py
--rw-r--r--   0        0        0      740 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py
--rw-r--r--   0        0        0      673 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py
--rw-r--r--   0        0        0      451 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0020_executedtask_task_name_snapshot.py
--rw-r--r--   0        0        0      841 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py
--rw-r--r--   0        0        0      554 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py
--rw-r--r--   0        0        0     1295 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0023_mlresult.py
--rw-r--r--   0        0        0      550 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py
--rw-r--r--   0        0        0      542 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py
--rw-r--r--   0        0        0      647 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py
--rw-r--r--   0        0        0      446 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0027_executedtask_task_status.py
--rw-r--r--   0        0        0      639 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py
--rw-r--r--   0        0        0      436 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0029_executedtask_exceptions.py
--rw-r--r--   0        0        0      771 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py
--rwxr-xr-x   0        0        0     6549 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/models.py
--rw-r--r--   0        0        0      627 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/static/django_flow_forge/cytoscape_setup.js
--rw-r--r--   0        0        0    47755 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/static/django_flow_forge/htmx.min.js
--rw-r--r--   0        0        0    10754 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/task_utils.py
--rw-r--r--   0        0        0      957 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html
--rw-r--r--   0        0        0      570 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html
--rw-r--r--   0        0        0     3526 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html
--rw-r--r--   0        0        0      806 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html
--rw-r--r--   0        0        0     2701 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html
--rw-r--r--   0        0        0      825 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html
--rw-r--r--   0        0        0     1422 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_result.html
--rw-r--r--   0        0        0     1808 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html
--rw-r--r--   0        0        0     2699 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html
--rw-r--r--   0        0        0     3194 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html
--rw-r--r--   0        0        0     3723 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html
--rw-r--r--   0        0        0     5888 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html
--rwxr-xr-x   0        0        0     2962 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/tests.py
--rw-r--r--   0        0        0      680 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/urls.py
--rwxr-xr-x   0        0        0     9581 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/views.py
--rw-r--r--   0        0        0      767 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docker-compose-local.yml
--rw-r--r--   0        0        0      846 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/authorization.md
--rw-r--r--   0        0        0     3996 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/considerations.md
--rw-r--r--   0        0        0      866 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/data_science_experiments.md
--rw-r--r--   0        0        0     1031 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/debugging.md
--rw-r--r--   0        0        0     1295 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/flows_dashboard.md
--rw-r--r--   0        0        0     4269 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/index.md
--rw-r--r--   0        0        0     3613 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/installation.md
--rw-r--r--   0        0        0      270 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/roadmap.md
--rw-r--r--   0        0        0     1037 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/strategies.md
--rw-r--r--   0        0        0        0 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/conf/__init__.py
--rw-r--r--   0        0        0      396 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/conf/asgi.py
--rw-r--r--   0        0        0     4130 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/conf/settings.py
--rw-r--r--   0        0        0      898 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/conf/urls.py
--rw-r--r--   0        0        0      396 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/conf/wsgi.py
--rw-r--r--   0        0        0    32768 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/db.sqlite3-shm
--rw-r--r--   0        0        0  2904632 2024-04-15 10:06:36.512723 django_flow_forge-0.3.4/example_project/db.sqlite3-wal
--rw-r--r--   0        0        0      177 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/admin.py
--rw-r--r--   0        0        0      605 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/apps.py
--rw-r--r--   0        0        0      831 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/celery_app.py
--rw-r--r--   0        0        0     4720 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__ml_grid_search.py
--rw-r--r--   0        0        0     1394 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__parallel_celery.py
--rw-r--r--   0        0        0     1409 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__simple.py
--rw-r--r--   0        0        0     2980 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__simple_ml.py
--rw-r--r--   0        0        0     1555 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__simple_with_celery.py
--rw-r--r--   0        0        0     2137 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__with_nested_tasks.py
--rw-r--r--   0        0        0        0 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/models.py
--rw-r--r--   0        0        0     2134 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html
--rw-r--r--   0        0        0      994 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html
--rw-r--r--   0        0        0     1922 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/templates/example_app/index.html
--rw-r--r--   0        0        0       60 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/tests.py
--rw-r--r--   0        0        0      962 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/urls.py
--rw-r--r--   0        0        0     2531 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/views.py
--rwxr-xr-x   0        0        0      660 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/manage.py
--rw-r--r--   0        0        0      522 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/run_tasks_no_server.py
--rw-r--r--   0        0        0      399 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/mkdocs.yml
--rw-r--r--   0        0        0      873 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/requirements.txt
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 django_flow_forge-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/.DS_Store
+-rw-r--r--   0        0        0       66 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/.gitattributes
+-rw-r--r--   0        0        0      862 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/.github/workflows/deploy-mkdocs.yml
+-rw-r--r--   0        0        0      620 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     2879 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1613 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/.vscode/launch.json
+-rw-r--r--   0        0        0     1103 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/Dockerfile
+-rw-r--r--   0        0        0     1061 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/LICENSE
+-rw-r--r--   0        0        0      151 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/MANIFEST.in
+-rw-r--r--   0        0        0      865 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/__init__.py
+-rwxr-xr-x   0        0        0     3638 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/admin.py
+-rwxr-xr-x   0        0        0      160 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/apps.py
+-rw-r--r--   0        0        0     2306 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/async_utils.py
+-rw-r--r--   0        0        0     3006 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/authorization.py
+-rw-r--r--   0        0        0     1190 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/batch_utils.py
+-rw-r--r--   0        0        0    15970 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/flow_engine.py
+-rw-r--r--   0        0        0     5435 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0001_initial.py
+-rw-r--r--   0        0        0      816 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py
+-rw-r--r--   0        0        0      449 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0003_alter_executedtask_exceptions.py
+-rw-r--r--   0        0        0      624 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py
+-rw-r--r--   0        0        0      428 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0005_alter_flow_options.py
+-rw-r--r--   0        0        0      564 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py
+-rw-r--r--   0        0        0      436 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0007_executedflow_params.py
+-rw-r--r--   0        0        0      419 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0008_executedflow_meta.py
+-rw-r--r--   0        0        0     1411 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0009_flowbatch_flowbatchtempdata.py
+-rw-r--r--   0        0        0     1066 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0010_batchhandler.py
+-rw-r--r--   0        0        0     2004 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0011_remove_flowbatchtempdata_batch_and_more.py
+-rw-r--r--   0        0        0      416 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0012_rename_total_batches_batchhandler_total_batch_count.py
+-rw-r--r--   0        0        0     1346 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0013_remove_batchtempdata_batch_handler_flowbatch_and_more.py
+-rw-r--r--   0        0        0      345 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0014_delete_batchtempdata.py
+-rw-r--r--   0        0        0      555 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/0015_batchhandler_date_initialised.py
+-rwxr-xr-x   0        0        0        0 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/__init__.py
+-rw-r--r--   0        0        0      778 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0001_initial.py
+-rw-r--r--   0        0        0      392 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0002_processtask_task_output.py
+-rw-r--r--   0        0        0     1236 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py
+-rw-r--r--   0        0        0      451 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0004_processtask_nested_task.py
+-rw-r--r--   0        0        0      400 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0005_rename_nested_task_processtask_bidirectional_task.py
+-rw-r--r--   0        0        0      627 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py
+-rw-r--r--   0        0        0      448 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0007_rename_bidirectional_dependencies_processtask_depends_bidirectionally_with.py
+-rw-r--r--   0        0        0      444 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0008_rename_dependencies_processtask_depends_on.py
+-rw-r--r--   0        0        0     1717 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py
+-rw-r--r--   0        0        0      414 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0010_processtask_nested.py
+-rw-r--r--   0        0        0      573 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py
+-rw-r--r--   0        0        0      980 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py
+-rw-r--r--   0        0        0      537 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py
+-rw-r--r--   0        0        0      732 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py
+-rw-r--r--   0        0        0      432 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0015_alter_taskrun_output.py
+-rw-r--r--   0        0        0      467 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0016_rename_processrun_executedprocess_and_more.py
+-rw-r--r--   0        0        0      613 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py
+-rw-r--r--   0        0        0      740 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py
+-rw-r--r--   0        0        0      673 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py
+-rw-r--r--   0        0        0      451 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0020_executedtask_task_name_snapshot.py
+-rw-r--r--   0        0        0      841 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py
+-rw-r--r--   0        0        0      554 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py
+-rw-r--r--   0        0        0     1295 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0023_mlresult.py
+-rw-r--r--   0        0        0      550 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py
+-rw-r--r--   0        0        0      542 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py
+-rw-r--r--   0        0        0      647 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py
+-rw-r--r--   0        0        0      446 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0027_executedtask_task_status.py
+-rw-r--r--   0        0        0      639 2024-05-10 21:09:27.794256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py
+-rw-r--r--   0        0        0      436 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0029_executedtask_exceptions.py
+-rw-r--r--   0        0        0      771 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py
+-rwxr-xr-x   0        0        0     6712 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/models.py
+-rw-r--r--   0        0        0      627 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/static/django_flow_forge/cytoscape_setup.js
+-rw-r--r--   0        0        0    47755 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/static/django_flow_forge/htmx.min.js
+-rw-r--r--   0        0        0    10754 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/task_utils.py
+-rw-r--r--   0        0        0      957 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html
+-rw-r--r--   0        0        0      570 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html
+-rw-r--r--   0        0        0     3526 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html
+-rw-r--r--   0        0        0      806 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html
+-rw-r--r--   0        0        0     2701 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html
+-rw-r--r--   0        0        0      825 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html
+-rw-r--r--   0        0        0     1422 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/ml_result.html
+-rw-r--r--   0        0        0     1808 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html
+-rw-r--r--   0        0        0     2699 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html
+-rw-r--r--   0        0        0     3194 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html
+-rw-r--r--   0        0        0     3723 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html
+-rw-r--r--   0        0        0     5888 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html
+-rwxr-xr-x   0        0        0     2962 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/tests.py
+-rw-r--r--   0        0        0      680 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/urls.py
+-rwxr-xr-x   0        0        0     9525 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/django_flow_forge/views.py
+-rw-r--r--   0        0        0      767 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/docker-compose-local.yml
+-rw-r--r--   0        0        0      846 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/docs/authorization.md
+-rw-r--r--   0        0        0     3996 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/docs/considerations.md
+-rw-r--r--   0        0        0      866 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/docs/data_science_experiments.md
+-rw-r--r--   0        0        0     1031 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/docs/debugging.md
+-rw-r--r--   0        0        0     1295 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/docs/flows_dashboard.md
+-rw-r--r--   0        0        0     4269 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/docs/index.md
+-rw-r--r--   0        0        0     3613 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/docs/installation.md
+-rw-r--r--   0        0        0      270 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/docs/roadmap.md
+-rw-r--r--   0        0        0     1037 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/docs/strategies.md
+-rw-r--r--   0        0        0        0 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/example_project/conf/__init__.py
+-rw-r--r--   0        0        0      396 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/example_project/conf/asgi.py
+-rw-r--r--   0        0        0     4130 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/example_project/conf/settings.py
+-rw-r--r--   0        0        0      898 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/example_project/conf/urls.py
+-rw-r--r--   0        0        0      396 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/example_project/conf/wsgi.py
+-rw-r--r--   0        0        0    32768 2024-05-10 21:09:27.798256 django_flow_forge-0.3.6/example_project/db.sqlite3-shm
+-rw-r--r--   0        0        0  2904632 2024-05-10 21:09:27.806256 django_flow_forge-0.3.6/example_project/db.sqlite3-wal
+-rw-r--r--   0        0        0      177 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/admin.py
+-rw-r--r--   0        0        0      605 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/apps.py
+-rw-r--r--   0        0        0      831 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/celery_app.py
+-rw-r--r--   0        0        0     4720 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/flow__ml_grid_search.py
+-rw-r--r--   0        0        0     1394 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/flow__parallel_celery.py
+-rw-r--r--   0        0        0     1409 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/flow__simple.py
+-rw-r--r--   0        0        0     2980 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/flow__simple_ml.py
+-rw-r--r--   0        0        0     1555 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/flow__simple_with_celery.py
+-rw-r--r--   0        0        0     2137 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/flow__with_nested_tasks.py
+-rw-r--r--   0        0        0        0 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/models.py
+-rw-r--r--   0        0        0     2134 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html
+-rw-r--r--   0        0        0      994 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html
+-rw-r--r--   0        0        0     1922 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/templates/example_app/index.html
+-rw-r--r--   0        0        0       60 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/tests.py
+-rw-r--r--   0        0        0      962 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/urls.py
+-rw-r--r--   0        0        0     2531 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/example_app/views.py
+-rwxr-xr-x   0        0        0      660 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/manage.py
+-rw-r--r--   0        0        0      522 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/example_project/run_tasks_no_server.py
+-rw-r--r--   0        0        0      399 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/mkdocs.yml
+-rw-r--r--   0        0        0      873 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-05-10 21:09:27.810256 django_flow_forge-0.3.6/requirements.txt
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 django_flow_forge-0.3.6/PKG-INFO
```

### Comparing `django_flow_forge-0.3.4/.DS_Store` & `django_flow_forge-0.3.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/.github/workflows/deploy-mkdocs.yml` & `django_flow_forge-0.3.6/.github/workflows/deploy-mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/.github/workflows/publish-to-pypi.yml` & `django_flow_forge-0.3.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/.gitignore` & `django_flow_forge-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/.vscode/launch.json` & `django_flow_forge-0.3.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/Dockerfile` & `django_flow_forge-0.3.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/LICENSE` & `django_flow_forge-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/README.md` & `django_flow_forge-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/admin.py` & `django_flow_forge-0.3.6/django_flow_forge/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from django.contrib import admin
+from django.utils.text import Truncator
+
 from . import models
 
 @admin.register(models.Flow)
 class FlowAdmin(admin.ModelAdmin):
     list_display = ('flow_name',)
     search_fields = ['flow_name']
 
@@ -50,12 +52,23 @@
             return self.readonly_fields + ('task', 'flow_run', 
                                         #    'start_time', 'end_time',
                                              'task_complete')
         return self.readonly_fields
 
 @admin.register(models.BatchHandler)
 class BatchHandlerAdmin(admin.ModelAdmin):
-    list_display = ('id', 'batch_ref_name', 'total_batch_count', 'temp_data',)
+    list_filter = ('batch_ref_name', 'date_initialised',)
+    search_fields = ['task__task_name', 'date_initialised', 'flow_run__flow__flow_name']
+    list_display = ('id', 'date_initialised', 'batch_ref_name', 'total_batch_count', 'temp_data',)
 
 @admin.register(models.FlowBatch)
 class FlowBatchAdmin(admin.ModelAdmin):
-    list_display = ('id', 'batch_handler', 'flow_batch_number', 'temp_data',)
+    list_display = ('id', 'get_date_initialised', 'batch_handler', 'flow_batch_number', 'truncated_temp_data',)
+
+    def get_date_initialised(self, obj):
+        return obj.batch_handler.date_initialised
+    get_date_initialised.admin_order_field = 'batch_handler__date_initialised'  # Allows column order sorting
+    get_date_initialised.short_description = 'Date Initialised'  # Renames the column header
+
+    def truncated_temp_data(self, obj):
+        return Truncator(obj.temp_data).chars(50)
+    truncated_temp_data.short_description = 'Temp Data'  # Custom header for the truncated field
```

### Comparing `django_flow_forge-0.3.4/django_flow_forge/async_utils.py` & `django_flow_forge-0.3.6/django_flow_forge/async_utils.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/authorization.py` & `django_flow_forge-0.3.6/django_flow_forge/authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.contrib.auth.mixins import LoginRequiredMixin, AccessMixin
 from django.conf import settings
 from django.core.exceptions import PermissionDenied
 from . import models
 
 from django.contrib.auth.mixins import PermissionRequiredMixin
 from django.views.generic import ListView
-
+from django.contrib.auth.views import redirect_to_login 
 from django.contrib.auth.decorators import login_required
 
 def check_user_has_permission(request, permission, allow_superuser):
     if request.user.has_perm(permission):
         return True
     elif allow_superuser and request.user.is_superuser:
         return True
```

### Comparing `django_flow_forge-0.3.4/django_flow_forge/batch_utils.py` & `django_flow_forge-0.3.6/django_flow_forge/batch_utils.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/flow_engine.py` & `django_flow_forge-0.3.6/django_flow_forge/flow_engine.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/0001_initial.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/0009_flowbatch_flowbatchtempdata.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/0009_flowbatch_flowbatchtempdata.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/0010_batchhandler.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/0010_batchhandler.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/0011_remove_flowbatchtempdata_batch_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/0011_remove_flowbatchtempdata_batch_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/0013_remove_batchtempdata_batch_handler_flowbatch_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/0013_remove_batchtempdata_batch_handler_flowbatch_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0001_initial.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0023_mlresult.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0023_mlresult.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py` & `django_flow_forge-0.3.6/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/models.py` & `django_flow_forge-0.3.6/django_flow_forge/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,18 @@
 
 class BatchHandler(models.Model):
     '''Model to handle batch processing using the same Flow - sometimes you want to run the flow in batches not batches within a flow.
        This is also a useful option if you want to chain together Flows in a batch'''
     batch_ref_name = models.CharField(null=True, blank=True, max_length=255) # Optional reference name
     total_batch_count = models.IntegerField(default=0, null=False, blank=False,)
     temp_data = models.JSONField(null=True, default=dict, encoder=DjangoJSONEncoder)
+    date_initialised = models.DateField(auto_now_add=True)
+
+    def __str__(self):
+        return f'{self.batch_ref_name} (Batch count: {self.total_batch_count})'
 
 class FlowBatch(models.Model):
     batch_handler = models.ForeignKey(BatchHandler, on_delete=models.CASCADE, related_name='batch', null=True, blank=True)
     flow_batch_number = models.IntegerField(default=0, null=False, blank=False,)
     temp_data = models.JSONField(null=True, default=dict, encoder=DjangoJSONEncoder)
 
 class MLResult(models.Model):
```

### Comparing `django_flow_forge-0.3.4/django_flow_forge/static/django_flow_forge/cytoscape_setup.js` & `django_flow_forge-0.3.6/django_flow_forge/static/django_flow_forge/cytoscape_setup.js`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/static/django_flow_forge/htmx.min.js` & `django_flow_forge-0.3.6/django_flow_forge/static/django_flow_forge/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/task_utils.py` & `django_flow_forge-0.3.6/django_flow_forge/task_utils.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_result.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/ml_result.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html` & `django_flow_forge-0.3.6/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/tests.py` & `django_flow_forge-0.3.6/django_flow_forge/tests.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/urls.py` & `django_flow_forge-0.3.6/django_flow_forge/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/django_flow_forge/views.py` & `django_flow_forge-0.3.6/django_flow_forge/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,33 +158,33 @@
 def update_task_run_node_info(request):
 
     if request.htmx:
 
         node_id = request.GET.get('clicked_node_id', None) # this is the id of the task it was when the task was first run
         executed_flow_id = request.GET.get('current_executed_flow_option', None)
 
-        if node_id:
+        context = {}
 
-            executed_flow = models.ExecutedFlow.objects.get(id=executed_flow_id)
+        if node_id:
 
-            if models.ExecutedTask.objects.filter(task_snapshot_id=node_id, flow_run=executed_flow).exists():
+            if models.ExecutedTask.objects.filter(task_snapshot_id=node_id, flow_run_id=executed_flow_id).exists():
 
                 executed_task = models.ExecutedTask.objects.get(task_snapshot_id=node_id, flow_run=executed_flow)
                 executed_task_summary = {}
                 executed_task_summary['Task Status'] = executed_task.status
                 executed_task_summary['Start Time'] = executed_task.start_time
                 executed_task_summary['End Time'] = executed_task.end_time
 
                 if executed_task.status == 'failed':
                     executed_task_summary['Exception'] = executed_task.exceptions
 
                 else:    
                     executed_task_summary['Output'] = executed_task.output
                 
-                context = {'executed_task_summary': executed_task_summary}
+                context['executed_task_summary'] = executed_task_summary
 
                 ''' Check if any machine learning experiments associated with node'''
                 ml_results = models.MLResult.objects.filter(executed_flow=executed_flow)
                 context['ml_result_count'] = len(ml_results)
                 context['ml_results'] = ml_results
 
             else:
```

### Comparing `django_flow_forge-0.3.4/docker-compose-local.yml` & `django_flow_forge-0.3.6/docker-compose-local.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/docs/authorization.md` & `django_flow_forge-0.3.6/docs/authorization.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/docs/considerations.md` & `django_flow_forge-0.3.6/docs/considerations.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/docs/data_science_experiments.md` & `django_flow_forge-0.3.6/docs/data_science_experiments.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/docs/debugging.md` & `django_flow_forge-0.3.6/docs/debugging.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/docs/flows_dashboard.md` & `django_flow_forge-0.3.6/docs/flows_dashboard.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/docs/index.md` & `django_flow_forge-0.3.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/docs/installation.md` & `django_flow_forge-0.3.6/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/docs/strategies.md` & `django_flow_forge-0.3.6/docs/strategies.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/conf/settings.py` & `django_flow_forge-0.3.6/example_project/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/conf/urls.py` & `django_flow_forge-0.3.6/example_project/conf/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/db.sqlite3-shm` & `django_flow_forge-0.3.6/example_project/db.sqlite3-shm`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/db.sqlite3-wal` & `django_flow_forge-0.3.6/example_project/db.sqlite3-wal`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/apps.py` & `django_flow_forge-0.3.6/example_project/example_app/apps.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/celery_app.py` & `django_flow_forge-0.3.6/example_project/example_app/celery_app.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/flow__ml_grid_search.py` & `django_flow_forge-0.3.6/example_project/example_app/flow__ml_grid_search.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/flow__parallel_celery.py` & `django_flow_forge-0.3.6/example_project/example_app/flow__parallel_celery.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/flow__simple.py` & `django_flow_forge-0.3.6/example_project/example_app/flow__simple.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/flow__simple_ml.py` & `django_flow_forge-0.3.6/example_project/example_app/flow__simple_ml.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/flow__simple_with_celery.py` & `django_flow_forge-0.3.6/example_project/example_app/flow__simple_with_celery.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/flow__with_nested_tasks.py` & `django_flow_forge-0.3.6/example_project/example_app/flow__with_nested_tasks.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html` & `django_flow_forge-0.3.6/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html` & `django_flow_forge-0.3.6/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/templates/example_app/index.html` & `django_flow_forge-0.3.6/example_project/example_app/templates/example_app/index.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/urls.py` & `django_flow_forge-0.3.6/example_project/example_app/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/example_app/views.py` & `django_flow_forge-0.3.6/example_project/example_app/views.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/manage.py` & `django_flow_forge-0.3.6/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/example_project/run_tasks_no_server.py` & `django_flow_forge-0.3.6/example_project/run_tasks_no_server.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.4/pyproject.toml` & `django_flow_forge-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-flow-forge"
-version = "0.3.4"
+version = "0.3.6"
 description = "Eliminate unnecessary system complexity in Data Ops and in Machine Learning Ops (MLOps) with this Django module for defining, running and monitoring flows."
 authors = [{name = "Ed Burmicz", email = "eddyojb@gmail.com"}]
 readme = "README.md"
 license = {text = "MIT"} 
 keywords = ["django", "mlops", "data", "machine learning", "data science", "pipelines", "flow", "orchestration", "AI",]
 classifiers = [
     "Framework :: Django",
```

### Comparing `django_flow_forge-0.3.4/PKG-INFO` & `django_flow_forge-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flow-forge
-Version: 0.3.4
+Version: 0.3.6
 Summary: Eliminate unnecessary system complexity in Data Ops and in Machine Learning Ops (MLOps) with this Django module for defining, running and monitoring flows.
 Keywords: django,mlops,data,machine learning,data science,pipelines,flow,orchestration,AI
 Author-email: Ed Burmicz <eddyojb@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

