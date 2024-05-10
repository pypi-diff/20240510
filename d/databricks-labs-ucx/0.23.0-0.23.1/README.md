# Comparing `tmp/databricks_labs_ucx-0.23.0.tar.gz` & `tmp/databricks_labs_ucx-0.23.1.tar.gz`

## Comparing `databricks_labs_ucx-0.23.0.tar` & `databricks_labs_ucx-0.23.1.tar`

### file list

```diff
@@ -1,172 +1,172 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/__about__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/__init__.py
--rw-r--r--   0        0        0    19819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/cli.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/config.py
--rw-r--r--   0        0        0    30024 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/install.py
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/runtime.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/__init__.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/aggregate.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/metastores.py
--rw-r--r--   0        0        0    14043 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/workspaces.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/__init__.py
--rw-r--r--   0        0        0    16138 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/aws.py
--rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/azure.py
--rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/clusters.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/crawlers.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/init_scripts.py
--rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/jobs.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/pipelines.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/secrets.py
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/workflows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/__init__.py
--rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/access.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/credentials.py
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/locations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/__init__.py
--rw-r--r--   0        0        0    17739 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/access.py
--rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/credentials.py
--rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/locations.py
--rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/resources.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/__init__.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/account_cli.py
--rw-r--r--   0        0        0    15204 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/application.py
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/workflow_task.py
--rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/workspace_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/__init__.py
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/crawlers.py
--rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/dashboards.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/tasks.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/utils.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/__init__.py
--rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/catalog_schema.py
--rw-r--r--   0        0        0    29222 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/grants.py
--rw-r--r--   0        0        0    20209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/locations.py
--rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/mapping.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/migration_status.py
--rw-r--r--   0        0        0    21566 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_migrate.py
--rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_move.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_size.py
--rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/tables.py
--rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/tables.scala
--rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/udfs.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/verification.py
--rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/view_migrate.py
--rw-r--r--   0        0        0     8835 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/workflows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/__init__.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/hms_lineage.py
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/logs.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/mixins.py
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/policy.py
--rw-r--r--   0        0        0    33434 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/workflows.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/__init__.py
--rw-r--r--   0        0        0    47232 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/fixtures.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/redash.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/wspath.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/azure/05_0_azure_service_principals.sql
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/00_4_is_incompatible_submit_run_detected.sql
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/01_2_group_migration.sql
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/01_5_group_migration_complexity.sql
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/02_2_uc_data_modeling.sql
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/02_5_uc_data_modeling_complexity.sql
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/03_2_data_migration_summary.sql
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_0_compatibility.sql
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_1_count_total_databases.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_2_count_table_failures.sql
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_3_count_total_tables.sql
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_4_count_external_locations.sql
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_5_count_total_views.sql
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_6_count_total_udfs.sql
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00___assessment_overview.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/01_0_count_jobs.sql
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/05_0_object_readiness.sql
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/05_2_assessment_summary.sql
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/05___findings_summary.md
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10_0_all_udfs.sql
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10___data_summary.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/15_0_external_locations.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/15_3_mount_points.sql
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/15___storage_summary.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/20_0_cluster_policies.sql
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/20_0_clusters.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/20___compute_summary.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/30_0_job_summary.md
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/30_3_job_details.sql
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/30_3_jobs.sql
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/30_4_submit_runs.sql
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/30_5_submit_runs.sql
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/40_0_pipelines.sql
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/40_3_global_init_scripts.sql
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/40___last_summary.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/README.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/migration/main/00_0_migration_overview.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/migration/main/01_0_data_object_migration_status.md
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/migration/main/01_1_data_object_migration_status.sql
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/code_patterns.sql
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/grant_detail.sql
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/misc_patterns.sql
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/objects.sql
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/table_estimates.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/__init__.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/ast_helpers.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/base.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/dbfs.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/files.py
--rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/graph.py
--rw-r--r--   0        0        0    10736 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/jobs.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/languages.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/lsp.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/path_lookup.py
--rw-r--r--   0        0        0    16508 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/pyspark.py
--rw-r--r--   0        0        0    11559 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/python_linter.py
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/queries.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/redash.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/site_packages.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/spark_connect.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/table_creation.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/whitelist.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/workflows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/__init__.py
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/cells.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/loaders.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/migrator.py
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/sources.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.23.0_add_assessment_to_udf.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.4.0_added_log_dir.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/__init__.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/base.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/clusters.py
--rw-r--r--   0        0        0    18962 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/generic.py
--rw-r--r--   0        0        0    34574 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/groups.py
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/listing.py
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/manager.py
--rw-r--r--   0        0        0    12579 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/redash.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/scim.py
--rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/secrets.py
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/tacl.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/workflows.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/LICENSE
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/NOTICE
--rw-r--r--   0        0        0    65891 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/README.md
--rw-r--r--   0        0        0    28523 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/pyproject.toml
--rw-r--r--   0        0        0    67566 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/__about__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/__init__.py
+-rw-r--r--   0        0        0    19819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/cli.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/config.py
+-rw-r--r--   0        0        0    30024 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/install.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/runtime.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/__init__.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/aggregate.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/metastores.py
+-rw-r--r--   0        0        0    14043 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/workspaces.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/__init__.py
+-rw-r--r--   0        0        0    16138 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/aws.py
+-rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/azure.py
+-rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/clusters.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/crawlers.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/init_scripts.py
+-rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/jobs.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/pipelines.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/secrets.py
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/__init__.py
+-rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/access.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/credentials.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/locations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/__init__.py
+-rw-r--r--   0        0        0    17739 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/access.py
+-rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/credentials.py
+-rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/locations.py
+-rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/resources.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/account_cli.py
+-rw-r--r--   0        0        0    15204 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/application.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/workflow_task.py
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/workspace_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/__init__.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/crawlers.py
+-rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/dashboards.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/tasks.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/utils.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/__init__.py
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/catalog_schema.py
+-rw-r--r--   0        0        0    29222 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/grants.py
+-rw-r--r--   0        0        0    20209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/locations.py
+-rw-r--r--   0        0        0    10115 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/mapping.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/migration_status.py
+-rw-r--r--   0        0        0    22506 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_migrate.py
+-rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_move.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_size.py
+-rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/tables.py
+-rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/tables.scala
+-rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/udfs.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/verification.py
+-rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/view_migrate.py
+-rw-r--r--   0        0        0     8835 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/__init__.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/hms_lineage.py
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/logs.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/mixins.py
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/policy.py
+-rw-r--r--   0        0        0    33434 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/workflows.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/__init__.py
+-rw-r--r--   0        0        0    47495 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/fixtures.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/redash.py
+-rw-r--r--   0        0        0    14144 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/wspath.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/azure/05_0_azure_service_principals.sql
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/00_4_is_incompatible_submit_run_detected.sql
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/01_2_group_migration.sql
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/01_5_group_migration_complexity.sql
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/02_2_uc_data_modeling.sql
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/02_5_uc_data_modeling_complexity.sql
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/03_2_data_migration_summary.sql
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_0_compatibility.sql
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_1_count_total_databases.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_2_count_table_failures.sql
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_3_count_total_tables.sql
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_4_count_external_locations.sql
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_5_count_total_views.sql
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00_6_count_total_udfs.sql
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/00___assessment_overview.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/01_0_count_jobs.sql
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/05_0_object_readiness.sql
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/05_2_assessment_summary.sql
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/05___findings_summary.md
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10_0_all_udfs.sql
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10___data_summary.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/15_0_external_locations.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/15_3_mount_points.sql
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/15___storage_summary.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/20_0_cluster_policies.sql
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/20_0_clusters.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/20___compute_summary.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/30_0_job_summary.md
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/30_3_job_details.sql
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/30_3_jobs.sql
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/30_4_submit_runs.sql
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/30_5_submit_runs.sql
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/40_0_pipelines.sql
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/40_3_global_init_scripts.sql
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/40___last_summary.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/README.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/migration/main/00_0_migration_overview.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/migration/main/01_0_data_object_migration_status.md
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/migration/main/01_1_data_object_migration_status.sql
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/code_patterns.sql
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/grant_detail.sql
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/misc_patterns.sql
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/objects.sql
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/table_estimates.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/__init__.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/ast_helpers.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/base.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/dbfs.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/files.py
+-rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/graph.py
+-rw-r--r--   0        0        0    10736 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/jobs.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/languages.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/lsp.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/path_lookup.py
+-rw-r--r--   0        0        0    16508 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/pyspark.py
+-rw-r--r--   0        0        0    11559 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/python_linter.py
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/queries.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/redash.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/site_packages.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/spark_connect.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/table_creation.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/whitelist.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/__init__.py
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/cells.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/loaders.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/migrator.py
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/sources.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.23.0_add_assessment_to_udf.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.4.0_added_log_dir.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/__init__.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/base.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/clusters.py
+-rw-r--r--   0        0        0    18962 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/generic.py
+-rw-r--r--   0        0        0    34574 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/groups.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/listing.py
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/manager.py
+-rw-r--r--   0        0        0    12579 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/redash.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/scim.py
+-rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/secrets.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/tacl.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/workflows.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/LICENSE
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/NOTICE
+-rw-r--r--   0        0        0    65891 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/README.md
+-rw-r--r--   0        0        0    28530 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/pyproject.toml
+-rw-r--r--   0        0        0    67573 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.1/PKG-INFO
```

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/cli.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/cli.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/config.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/config.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/install.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/install.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/runtime.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/runtime.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/aggregate.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/aggregate.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/metastores.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/metastores.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/workspaces.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/account/workspaces.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/aws.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/aws.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/azure.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/azure.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/clusters.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/clusters.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/crawlers.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/crawlers.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/init_scripts.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/init_scripts.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/jobs.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/jobs.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/pipelines.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/pipelines.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/secrets.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/secrets.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/workflows.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/assessment/workflows.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/access.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/access.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/credentials.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/credentials.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/locations.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/aws/locations.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/access.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/access.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/credentials.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/credentials.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/locations.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/locations.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/resources.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/azure/resources.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/account_cli.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/account_cli.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/application.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/application.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/workflow_task.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/workflow_task.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/workspace_cli.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/contexts/workspace_cli.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/crawlers.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/crawlers.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/dashboards.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/dashboards.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/tasks.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/tasks.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/utils.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/framework/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/catalog_schema.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/catalog_schema.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/grants.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/grants.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/locations.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/locations.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/mapping.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/mapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import dataclass
 from functools import partial
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.parallel import Threads
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
-from databricks.sdk.errors import BadRequest, NotFound, ResourceConflict
+from databricks.sdk.errors import BadRequest, NotFound, ResourceConflict, DatabricksError
 from databricks.sdk.service.catalog import TableInfo, SchemaInfo
 
 from databricks.labs.ucx.account.workspaces import WorkspaceInfo
 from databricks.labs.ucx.framework.utils import escape_sql_identifier
 from databricks.labs.ucx.hive_metastore import TablesCrawler
 from databricks.labs.ucx.hive_metastore.tables import Table
 
@@ -178,32 +178,39 @@
     def _get_table_in_scope_task(self, table_to_migrate: TableToMigrate) -> TableToMigrate | None:
         table = table_to_migrate.src
         rule = table_to_migrate.rule
 
         if self.exists_in_uc(table, rule.as_uc_table_key):
             logger.info(f"The intended target for {table.key}, {rule.as_uc_table_key}, already exists.")
             return None
-        result = self._sql_backend.fetch(
-            f"SHOW TBLPROPERTIES {escape_sql_identifier(table.database)}.{escape_sql_identifier(table.name)}"
-        )
+        try:
+            result = self._sql_backend.fetch(
+                f"SHOW TBLPROPERTIES {escape_sql_identifier(table.database)}.{escape_sql_identifier(table.name)}"
+            )
+        except DatabricksError as err:
+            logger.warning(f"Failed to get properties for Table {table.key}: {err}")
+            return None
         for value in result:
             if value["key"] == self.UCX_SKIP_PROPERTY:
                 logger.info(f"{table.key} is marked to be skipped")
                 return None
             if value["key"] == "upgraded_to":
                 logger.info(f"{table.key} is set as upgraded to {value['value']}")
                 if self.exists_in_uc(table, value["value"]):
                     logger.info(
                         f"The table {table.key} was previously migrated to {value['value']}. "
                         f"To revert the table and allow it to be migrated again use the CLI command:"
                         f"databricks labs ucx revert --schema {table.database} --table {table.name}"
                     )
                     return None
                 logger.info(f"The upgrade_to target for {table.key} is missing. Unsetting the upgrade_to property")
-                self._sql_backend.execute(table.sql_unset_upgraded_to())
+                try:
+                    self._sql_backend.execute(table.sql_unset_upgraded_to())
+                except DatabricksError as err:
+                    logger.warning(f"Failed to unset upgraded_to property for Table {table.key}: {err}")
 
         return table_to_migrate
 
     def exists_in_uc(self, src_table: Table, target_key: str):
         # Attempts to get the target table info from UC returns True if it exists.
         try:
             table_info = self._ws.tables.get(target_key)
```

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/migration_status.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/migration_status.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_migrate.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_migrate.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     HiveSerdeType,
 )
 from databricks.labs.ucx.hive_metastore.view_migrate import (
     ViewsMigrationSequencer,
     ViewToMigrate,
 )
 from databricks.labs.ucx.workspace_access.groups import GroupManager, MigratedGroup
-from databricks.sdk.errors.platform import BadRequest, NotFound
+from databricks.sdk.errors.platform import DatabricksError
 
 logger = logging.getLogger(__name__)
 
 
 class TablesMigrator:
     def __init__(
         self,
@@ -206,17 +206,23 @@
                 logger.info(f"View {view.src.key} cannot be migrated because {table.key} is not migrated yet")
                 return False
         return True
 
     def _migrate_view_table(self, src_view: ViewToMigrate, grants: list[Grant] | None = None):
         view_migrate_sql = self._sql_migrate_view(src_view)
         logger.debug(f"Migrating view {src_view.src.key} to using SQL query: {view_migrate_sql}")
-        self._backend.execute(view_migrate_sql)
-        self._backend.execute(src_view.src.sql_alter_to(src_view.rule.as_uc_table_key))
-        self._backend.execute(src_view.src.sql_alter_from(src_view.rule.as_uc_table_key, self._ws.get_workspace_id()))
+        try:
+            self._backend.execute(view_migrate_sql)
+            self._backend.execute(src_view.src.sql_alter_to(src_view.rule.as_uc_table_key))
+            self._backend.execute(
+                src_view.src.sql_alter_from(src_view.rule.as_uc_table_key, self._ws.get_workspace_id())
+            )
+        except DatabricksError as e:
+            logger.warning(f"Failed to migrate view {src_view.src.key} to {src_view.rule.as_uc_table_key}: {e}")
+            return False
         return self._migrate_acl(src_view.src, src_view.rule, grants)
 
     def _sql_migrate_view(self, src_view: ViewToMigrate) -> str:
         # We have to fetch create statement this way because of columns in:
         # CREATE VIEW x.y (col1, col2) AS SELECT * FROM w.t
         create_statement = self._backend.fetch(f"SHOW CREATE TABLE {src_view.src.safe_sql_key}")
         src_view.src.view_text = next(iter(create_statement))["createtab_stmt"]
@@ -227,15 +233,16 @@
         target_table_key = rule.as_uc_table_key
         table_migrate_sql = src_table.sql_migrate_external(target_table_key)
         logger.debug(f"Migrating external table {src_table.key} to using SQL query: {table_migrate_sql}")
         # have to wrap the fetch result with iter() for now, because StatementExecutionBackend returns iterator but RuntimeBackend returns list.
         sync_result = next(iter(self._backend.fetch(table_migrate_sql)))
         if sync_result.status_code != "SUCCESS":
             logger.warning(
-                f"SYNC command failed to migrate {src_table.key} to {target_table_key}. Status code: {sync_result.status_code}. Description: {sync_result.description}"
+                f"SYNC command failed to migrate table {src_table.key} to {target_table_key}. "
+                f"Status code: {sync_result.status_code}. Description: {sync_result.description}"
             )
             return False
         self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
         return self._migrate_acl(src_table, rule, grants)
 
     def _migrate_external_table_hiveserde_in_place(
         self,
@@ -267,59 +274,71 @@
                 f"Failed to generate in-place migration DDL for {src_table.key}, skip the in-place migration. It can be migrated in CTAS workflow"
             )
             return False
 
         logger.debug(
             f"Migrating external table {src_table.key} to {rule.as_uc_table_key} using SQL query: {table_migrate_sql}"
         )
-        self._backend.execute(table_migrate_sql)
-        self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
-        self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
+        try:
+            self._backend.execute(table_migrate_sql)
+            self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
+            self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
+        except DatabricksError as e:
+            logger.warning(f"Failed to migrate table {src_table.key} to {rule.as_uc_table_key}: {e}")
+            return False
         return self._migrate_acl(src_table, rule, grants)
 
     def _migrate_dbfs_root_table(self, src_table: Table, rule: Rule, grants: list[Grant] | None = None):
         target_table_key = rule.as_uc_table_key
         table_migrate_sql = src_table.sql_migrate_dbfs(target_table_key)
         logger.debug(
             f"Migrating managed table {src_table.key} to {rule.as_uc_table_key} using SQL query: {table_migrate_sql}"
         )
-        self._backend.execute(table_migrate_sql)
-        self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
-        self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
+        try:
+            self._backend.execute(table_migrate_sql)
+            self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
+            self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
+        except DatabricksError as e:
+            logger.warning(f"Failed to migrate table {src_table.key} to {rule.as_uc_table_key}: {e}")
+            return False
         return self._migrate_acl(src_table, rule, grants)
 
     def _migrate_table_create_ctas(self, src_table: Table, rule: Rule, grants: list[Grant], mounts: list[Mount]):
         if src_table.what not in [What.EXTERNAL_NO_SYNC, What.EXTERNAL_HIVESERDE]:
             table_migrate_sql = src_table.sql_migrate_ctas_managed(rule.as_uc_table_key)
         elif not src_table.location:
             table_migrate_sql = src_table.sql_migrate_ctas_managed(rule.as_uc_table_key)
         else:
             # if external table and src tabel location is not missing, migrate to external UC table
             dst_table_location = src_table.location + "_ctas_migrated"
             if mounts and src_table.is_dbfs_mnt:
                 dst_table_location = ExternalLocations.resolve_mount(src_table.location, mounts) + "_ctas_migrated"
             table_migrate_sql = src_table.sql_migrate_ctas_external(rule.as_uc_table_key, dst_table_location)
         logger.debug(f"Migrating table {src_table.key} to {rule.as_uc_table_key} using SQL query: {table_migrate_sql}")
-        self._backend.execute(table_migrate_sql)
-        self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
-        self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
+        try:
+            self._backend.execute(table_migrate_sql)
+            self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
+            self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
+        except DatabricksError as e:
+            logger.warning(f"Failed to migrate table {src_table.key} to {rule.as_uc_table_key}: {e}")
+            return False
         return self._migrate_acl(src_table, rule, grants)
 
     def _migrate_acl(self, src: Table, rule: Rule, grants: list[Grant] | None):
         if grants is None:
             return True
         for grant in grants:
             acl_migrate_sql = grant.uc_grant_sql(src.kind, rule.as_uc_table_key)
             if acl_migrate_sql is None:
                 logger.warning(f"Cannot identify UC grant for {src.kind} {rule.as_uc_table_key}. Skipping.")
                 continue
             logger.debug(f"Migrating acls on {rule.as_uc_table_key} using SQL query: {acl_migrate_sql}")
             try:
                 self._backend.execute(acl_migrate_sql)
-            except (BadRequest, NotFound) as e:
+            except DatabricksError as e:
                 logger.warning(f"Failed to migrate ACL for {src.key} to {rule.as_uc_table_key}: {e}")
         return True
 
     def _table_already_migrated(self, target) -> bool:
         return target in self._seen_tables
 
     def _get_tables_to_revert(self, schema: str | None = None, table: str | None = None) -> list[Table]:
@@ -356,16 +375,19 @@
             )
         Threads.strict("revert migrated tables", tasks)
 
     def _revert_migrated_table(self, table: Table, target_table_key: str):
         logger.info(
             f"Reverting {table.object_type} table {table.database}.{table.name} upgraded_to {table.upgraded_to}"
         )
-        self._backend.execute(table.sql_unset_upgraded_to())
-        self._backend.execute(f"DROP {table.kind} IF EXISTS {target_table_key}")
+        try:
+            self._backend.execute(table.sql_unset_upgraded_to())
+            self._backend.execute(f"DROP {table.kind} IF EXISTS {target_table_key}")
+        except DatabricksError as e:
+            logger.warning(f"Failed to revert table {table.key}: {e}")
 
     def _get_revert_count(self, schema: str | None = None, table: str | None = None) -> list[MigrationCount]:
         self._init_seen_tables()
         migrated_tables = self._get_tables_to_revert(schema=schema, table=table)
 
         table_by_database = defaultdict(list)
         for cur_table in migrated_tables:
```

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_move.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_move.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_size.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/table_size.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/tables.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/tables.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/tables.scala` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/tables.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/udfs.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/udfs.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/verification.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/verification.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/view_migrate.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/view_migrate.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/workflows.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/hive_metastore/workflows.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/hms_lineage.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/hms_lineage.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/logs.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/logs.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/mixins.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/mixins.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/policy.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/policy.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/workflows.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/installer/workflows.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/fixtures.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -621,14 +621,15 @@
     @retried(on=[ResourceConflict], timeout=timedelta(seconds=30))
     def create(
         *,
         members: list[str] | None = None,
         roles: list[str] | None = None,
         entitlements: list[str] | None = None,
         display_name: str | None = None,
+        wait_for_provisioning: bool = False,
         **kwargs,
     ):
         kwargs["display_name"] = f"sdk-{make_random(4)}" if display_name is None else display_name
         if members is not None:
             kwargs["members"] = _scim_values(members)
         if roles is not None:
             kwargs["roles"] = _scim_values(roles)
@@ -636,14 +637,22 @@
             kwargs["entitlements"] = _scim_values(entitlements)
         # TODO: REQUEST_LIMIT_EXCEEDED: GetUserPermissionsRequest RPC token bucket limit has been exceeded.
         group = interface.create(**kwargs)
         if cfg.is_account_client:
             logger.info(f"Account group {group.display_name}: {cfg.host}/users/groups/{group.id}/members")
         else:
             logger.info(f"Workspace group {group.display_name}: {cfg.host}#setting/accounts/groups/{group.id}")
+
+        @retried(on=[NotFound], timeout=timedelta(minutes=2))
+        def _wait_for_provisioning() -> None:
+            interface.get(group.id)
+
+        if wait_for_provisioning:
+            _wait_for_provisioning()
+
         return group
 
     yield from factory(name, create, lambda item: interface.delete(item.id))
 
 
 @pytest.fixture
 def make_group(ws, make_random):
```

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/redash.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/mixins/redash.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/wspath.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/lsp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,340 +1,347 @@
-import abc
-import locale
+import enum
+import functools
+import http.server
+import json
 import logging
-import os
-import pathlib
-from functools import cached_property
-
-# pylint: disable-next=import-private-name
-from pathlib import Path, _PosixFlavour  # type: ignore
-from urllib.parse import quote_from_bytes as urlquote_from_bytes
-from io import BytesIO, StringIO
-
-from databricks.sdk import WorkspaceClient
-from databricks.sdk.errors import NotFound, DatabricksError
-from databricks.sdk.service.workspace import ObjectInfo, ObjectType, ExportFormat, ImportFormat, Language
+from collections.abc import Sequence
+from dataclasses import dataclass
+from pathlib import Path
+from typing import Any
+from urllib.parse import parse_qsl
+
+from databricks.labs.blueprint.logger import install_logger
+from databricks.sdk.service.workspace import Language
+
+from databricks.labs.ucx.hive_metastore.migration_status import (
+    MigrationStatus,
+)
+from databricks.labs.ucx.hive_metastore.migration_status import MigrationIndex
+from databricks.labs.ucx.source_code.base import (
+    Advice,
+    Advisory,
+    Convention,
+    Deprecation,
+    Failure,
+)
+from databricks.labs.ucx.source_code.languages import Languages
 
 logger = logging.getLogger(__name__)
 
 
-class _DatabricksFlavour(_PosixFlavour):
-    def __init__(self, ws: WorkspaceClient):
-        super().__init__()
-        self._ws = ws
-
-    def make_uri(self, path):
-        return self._ws.config.host + '#workspace' + urlquote_from_bytes(bytes(path))
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} for {self._ws}>"
-
-
-def _na(fn: str):
-    def _inner(*_, **__):
-        __tracebackhide__ = True  # pylint: disable=unused-variable
-        raise NotImplementedError(f"{fn}() is not available for Databricks Workspace")
-
-    return _inner
-
-
-class _ScandirItem:
-    def __init__(self, object_info):
-        self._object_info = object_info
-
-    def __fspath__(self):
-        return self._object_info.path
-
-    def is_dir(self):
-        return self._object_info.object_type == ObjectType.DIRECTORY
-
-    def is_file(self):
-        # TODO: check if we want to show notebooks as files
-        return self._object_info.object_type == ObjectType.FILE
-
-    def is_symlink(self):
-        return False
-
-    @property
-    def name(self):
-        return os.path.basename(self._object_info.path)
-
-
-class _ScandirIterator:
-    def __init__(self, objects):
-        self._it = objects
-
-    def __iter__(self):
-        for object_info in self._it:
-            yield _ScandirItem(object_info)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *args):
-        pass
-
-
-class _DatabricksAccessor:
-    chmod = _na('accessor.chmod')
-    getcwd = _na('accessor.getcwd')
-    group = _na('accessor.group')
-    link = _na('accessor.link')
-    mkdir = _na('accessor.mkdir')
-    owner = _na('accessor.owner')
-    readlink = _na('accessor.readlink')
-    realpath = _na('accessor.realpath')
-    rename = _na('accessor.rename')
-    replace = _na('accessor.replace')
-    rmdir = _na('accessor.rmdir')
-    stat = _na('accessor.stat')
-    symlink = _na('accessor.symlink')
-    unlink = _na('accessor.unlink')
-
-    def __init__(self, ws: WorkspaceClient):
-        self._ws = ws
-
-    def expanduser(self, path):
-        home = f"/Users/{self._ws.current_user.me().user_name}"
-        return path.replace("~", home)
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} for {self._ws}>"
-
-    def scandir(self, path):
-        return _ScandirIterator(self._ws.workspace.list(path))
-
-    def listdir(self, path):
-        return [item.name for item in self.scandir(path)]
-
-
-class _UploadIO(abc.ABC):
-    def __init__(self, ws: WorkspaceClient, path: str):
-        self._ws = ws
-        self._path = path
-
-    def close(self):
-        # pylint: disable-next=no-member
-        io_stream = self.getvalue()  # noqa
-        self._ws.workspace.upload(self._path, io_stream, format=ImportFormat.AUTO)
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} for {self._path} on {self._ws}>"
-
-
-class _BinaryUploadIO(_UploadIO, BytesIO):  # type: ignore
-    def __init__(self, ws: WorkspaceClient, path: str):
-        _UploadIO.__init__(self, ws, path)
-        BytesIO.__init__(self)
-
-
-class _TextUploadIO(_UploadIO, StringIO):  # type: ignore
-    def __init__(self, ws: WorkspaceClient, path: str):
-        _UploadIO.__init__(self, ws, path)
-        StringIO.__init__(self)
-
-
-class WorkspacePath(Path):
-    """Experimental implementation of pathlib.Path for Databricks Workspace."""
-
-    _SUFFIXES = {'.py': Language.PYTHON, '.sql': Language.SQL, '.scala': Language.SCALA, '.R': Language.R}
-
-    _ws: WorkspaceClient
-    _flavour: _DatabricksFlavour
-    _accessor: _DatabricksAccessor
-
-    cwd = _na('cwd')
-    resolve = _na('resolve')
-    stat = _na('stat')
-    chmod = _na('chmod')
-    lchmod = _na('lchmod')
-    lstat = _na('lstat')
-    owner = _na('owner')
-    group = _na('group')
-    readlink = _na('readlink')
-    symlink_to = _na('symlink_to')
-    hardlink_to = _na('hardlink_to')
-    touch = _na('touch')
-    link_to = _na('link_to')
-    samefile = _na('samefile')
-
-    def __new__(cls, ws: WorkspaceClient, path: str | Path):
-        this = object.__new__(cls)
-        # pathlib does a lot of clever performance tricks, and it's not designed to be subclassed,
-        # so we need to set the attributes directly, bypassing the most of a common sense.
-        this._flavour = _DatabricksFlavour(ws)
-        drv, root, parts = this._parse_args([path])
-        return this.__from_raw_parts(this, ws, this._flavour, drv, root, parts)
-
-    @staticmethod
-    def __from_raw_parts(this, ws: WorkspaceClient, flavour: _DatabricksFlavour, drv, root, parts) -> 'WorkspacePath':
-        # pylint: disable=protected-access
-        this._accessor = _DatabricksAccessor(ws)
-        this._flavour = flavour
-        this._drv = drv
-        this._root = root
-        this._parts = parts
-        this._ws = ws
-        return this
-
-    def _make_child_relpath(self, part):
-        # used in dir walking
-        path = self._flavour.join(self._parts + [part])
-        # self._flavour.join duplicates leading '/' (possibly a python bug)
-        # but we can't override join in _DatabricksFlavour because it's built-in
-        # and if we remove the leading '/' part then we don't get any
-        # so let's just do a slow but safe sanity check afterward
-        if os.sep == path[0] == path[1]:
-            path = path[1:]
-        return WorkspacePath(self._ws, path)
-
-    def _parse_args(self, args):  # pylint: disable=arguments-differ
-        # instance method adapted from pathlib.Path
-        parts = []
-        for a in args:
-            if isinstance(a, pathlib.PurePath):
-                parts += a._parts  # pylint: disable=protected-access
-                continue
-            parts.append(str(a))
-        return self._flavour.parse_parts(parts)
-
-    def _format_parsed_parts(self, drv, root, parts):  # pylint: disable=arguments-differ
-        # instance method adapted from pathlib.Path
-        if drv or root:
-            return drv + root + self._flavour.join(parts[1:])
-        return self._flavour.join(parts)
-
-    def _from_parsed_parts(self, drv, root, parts):  # pylint: disable=arguments-differ
-        # instance method adapted from pathlib.Path
-        this = object.__new__(self.__class__)
-        return self.__from_raw_parts(this, self._ws, self._flavour, drv, root, parts)
-
-    def _from_parts(self, args):  # pylint: disable=arguments-differ
-        # instance method adapted from pathlib.Path
-        drv, root, parts = self._parse_args(args)
-        return self._from_parsed_parts(drv, root, parts)
-
-    def relative_to(self, *other) -> pathlib.PurePath:  # type: ignore
-        """Databricks Workspace works only with absolute paths, so we make sure to
-        return pathlib.Path instead of WorkspacePath to avoid confusion."""
-        return pathlib.PurePath(super().relative_to(*other))
-
-    def as_fuse(self):
-        """Return FUSE-mounted path in Databricks Runtime."""
-        if 'DATABRICKS_RUNTIME_VERSION' not in os.environ:
-            logger.warning("This method is only available in Databricks Runtime")
-        return Path('/Workspace', self.as_posix())
-
-    def home(self):  # pylint: disable=arguments-differ
-        # instance method adapted from pathlib.Path
-        return WorkspacePath(self._ws, "~").expanduser()
-
-    def exists(self, *, follow_symlinks=True):
-        if not follow_symlinks:
-            raise NotImplementedError("follow_symlinks=False is not supported for Databricks Workspace")
-        try:
-            self._ws.workspace.get_status(self.as_posix())
-            return True
-        except NotFound:
-            return False
-
-    def mkdir(self, mode=0o600, parents=True, exist_ok=True):
-        if not exist_ok:
-            raise ValueError("exist_ok must be True for Databricks Workspace")
-        if not parents:
-            raise ValueError("parents must be True for Databricks Workspace")
-        if mode != 0o600:
-            raise ValueError("other modes than 0o600 are not yet supported")
-        self._ws.workspace.mkdirs(self.as_posix())
-
-    def rmdir(self, recursive=False):
-        self._ws.workspace.delete(self.as_posix(), recursive=recursive)
-
-    def rename(self, target, overwrite=False):
-        dst = WorkspacePath(self._ws, target)
-        with self._ws.workspace.download(self.as_posix(), format=ExportFormat.AUTO) as f:
-            self._ws.workspace.upload(dst.as_posix(), f.read(), format=ImportFormat.AUTO, overwrite=overwrite)
-        self.unlink()
-
-    def replace(self, target):
-        return self.rename(target, overwrite=True)
-
-    def unlink(self, missing_ok=False):
-        if not missing_ok and not self.exists():
-            raise FileNotFoundError(f"{self.as_posix()} does not exist")
-        self._ws.workspace.delete(self.as_posix())
-
-    def open(self, mode="r", buffering=-1, encoding=None, errors=None, newline=None):
-        if encoding is None or encoding == "locale":
-            encoding = locale.getpreferredencoding(False)
-        if "b" in mode and "r" in mode:
-            return self._ws.workspace.download(self.as_posix(), format=ExportFormat.AUTO)
-        if "b" in mode and "w" in mode:
-            return _BinaryUploadIO(self._ws, self.as_posix())
-        if "r" in mode:
-            with self._ws.workspace.download(self.as_posix(), format=ExportFormat.AUTO) as f:
-                return StringIO(f.read().decode(encoding))
-        if "w" in mode:
-            return _TextUploadIO(self._ws, self.as_posix())
-        raise ValueError(f"invalid mode: {mode}")
-
-    @property
-    def suffix(self):
-        """Return the file extension. If the file is a notebook, return the suffix based on the language."""
-        suffix = super().suffix
-        if suffix:
-            return suffix
-        if not self.is_notebook():
-            return ""
-        for sfx, lang in self._SUFFIXES.items():
-            try:
-                if self._object_info.language == lang:
-                    return sfx
-            except DatabricksError:
-                return ""
-        return ""
-
-    def __lt__(self, other: pathlib.PurePath):
-        if not isinstance(other, pathlib.PurePath):
-            return NotImplemented
-        return self.as_posix() < other.as_posix()
-
-    @cached_property
-    def _object_info(self) -> ObjectInfo:
-        # this method is cached because it is used in multiple is_* methods.
-        # DO NOT use this method in methods, where fresh result is required.
-        return self._ws.workspace.get_status(self.as_posix())
-
-    def _return_false(self) -> bool:
-        return False
-
-    is_symlink = _return_false
-    is_block_device = _return_false
-    is_char_device = _return_false
-    is_fifo = _return_false
-    is_socket = _return_false
-    is_mount = _return_false
-    is_junction = _return_false
-
-    def is_dir(self):
-        try:
-            return self._object_info.object_type == ObjectType.DIRECTORY
-        except DatabricksError:
-            return False
-
-    def is_file(self):
-        try:
-            return self._object_info.object_type == ObjectType.FILE
-        except DatabricksError:
-            return False
-
-    def is_notebook(self):
-        try:
-            return self._object_info.object_type == ObjectType.NOTEBOOK
-        except DatabricksError:
-            return False
-
-    def __eq__(self, other):
-        return isinstance(other, Path) and self.as_posix() == other.as_posix()
-
-    def __hash__(self):
-        return Path.__hash__(self)
+@dataclass
+class Position:
+    line: int
+    character: int
+
+    def as_dict(self) -> dict:
+        return {"line": self.line, "character": self.character}
+
+    @classmethod
+    def from_dict(cls, raw: dict) -> 'Position':
+        return cls(raw['line'], raw['character'])
+
+
+@dataclass
+class Range:
+    start: Position
+    end: Position
+
+    @classmethod
+    def from_dict(cls, raw: dict) -> 'Range':
+        return cls(Position.from_dict(raw['start']), Position.from_dict(raw['end']))
+
+    @classmethod
+    def make(cls, start_line: int, start_character: int, end_line: int, end_character: int) -> 'Range':
+        return cls(start=Position(start_line - 1, start_character), end=Position(end_line - 1, end_character))
+
+    def as_dict(self) -> dict:
+        return {"start": self.start.as_dict(), "end": self.end.as_dict()}
+
+    def fragment(self, code: str) -> str:
+        out = []
+        splitlines = code.splitlines()
+        for line, part in enumerate(splitlines):
+            if line == self.start.line and line == self.end.line:
+                out.append(part[self.start.character : self.end.character])
+            elif line == self.start.line:
+                out.append(part[self.start.character :])
+            elif line == self.end.line:
+                out.append(part[: self.end.character])
+            elif self.start.line < line < self.end.line:
+                out.append(part)
+        return "".join(out)
+
+
+class Severity(enum.IntEnum):
+    ERROR = 1
+    WARN = 2
+    INFO = 3
+    HINT = 4
+
+
+class DiagnosticTag(enum.IntEnum):
+    UNNECESSARY = 1
+    DEPRECATED = 2
+
+
+@dataclass
+class Diagnostic:
+    # the range at which the message applies.
+    range: Range
+
+    # The diagnostic's code, which might appear in the user interface.
+    code: str
+
+    # An optional property to describe the error code.
+    source: str
+
+    # The diagnostic's message.
+    message: str
+
+    # The diagnostic's severity. Can be omitted. If omitted it is up to the
+    # client to interpret diagnostics as error, warning, info or hint.
+    severity: Severity
+
+    tags: list[DiagnosticTag] | None = None
+
+    @classmethod
+    def from_advice(cls, advice: Advice) -> 'Diagnostic':
+        severity, tags = cls._severity_and_tags(advice)
+        return cls(
+            range=Range.make(advice.start_line, advice.start_col, advice.end_line, advice.end_col),
+            code=advice.code,
+            source="databricks.labs.ucx",
+            message=advice.message,
+            severity=severity,
+            tags=tags,
+        )
+
+    @classmethod
+    def _severity_and_tags(cls, advice):
+        if isinstance(advice, Convention):
+            return Severity.HINT, [DiagnosticTag.UNNECESSARY]
+        if isinstance(advice, Deprecation):
+            return Severity.WARN, [DiagnosticTag.DEPRECATED]
+        if isinstance(advice, Advisory):
+            return Severity.WARN, []
+        if isinstance(advice, Failure):
+            return Severity.ERROR, []
+        return Severity.INFO, []
+
+    def as_dict(self) -> dict:
+        return {
+            "range": self.range.as_dict(),
+            "code": self.code,
+            "source": self.source,
+            "message": self.message,
+            "severity": self.severity.value if self.severity else Severity.WARN,
+            "tags": [t.value for t in self.tags] if self.tags else [],
+        }
+
+
+@dataclass
+class TextDocumentIdentifier:
+    uri: str
+
+    def as_dict(self) -> dict:
+        return {
+            "uri": self.uri,
+        }
+
+
+@dataclass
+class OptionalVersionedTextDocumentIdentifier:
+    uri: str
+    version: int | None = None
+
+    def as_dict(self) -> dict:
+        return {
+            "uri": self.uri,
+            "version": self.version,
+        }
+
+
+@dataclass
+class TextEdit:
+    range: Range
+    new_text: str
+
+    def as_dict(self) -> dict:
+        return {
+            "range": self.range.as_dict(),
+            "newText": self.new_text,
+        }
+
+
+@dataclass
+class TextDocumentEdit:
+    text_document: OptionalVersionedTextDocumentIdentifier
+    edits: Sequence[TextEdit]
+
+    def as_dict(self) -> dict:
+        return {
+            "textDocument": self.text_document.as_dict(),
+            "edits": [e.as_dict() for e in self.edits],
+        }
+
+
+@dataclass
+class WorkspaceEdit:
+    # we also can have CreateFile | RenameFile | DeleteFile, but we won't do it for now.
+    document_changes: Sequence[TextDocumentEdit]
+
+    def as_dict(self) -> dict:
+        return {
+            "documentChanges": [e.as_dict() for e in self.document_changes],
+        }
+
+
+@dataclass
+class CodeAction:
+    title: str
+    edit: WorkspaceEdit
+    is_preferred: bool = False
+
+    def as_dict(self) -> dict:
+        return {
+            "title": self.title,
+            "edit": self.edit.as_dict(),
+            "isPreferred": self.is_preferred,
+        }
+
+
+@dataclass
+class AnalyseResponse:
+    diagnostics: list[Diagnostic]
+
+    def as_dict(self):
+        return {"diagnostics": [d.as_dict() for d in self.diagnostics]}
+
+
+@dataclass
+class QuickFixResponse:
+    code_actions: list[CodeAction]
+
+    def as_dict(self):
+        return {"code_actions": [ca.as_dict() for ca in self.code_actions]}
+
+
+class LspServer:
+    def __init__(self, language_support: Languages):
+        self._languages = language_support
+        self._extensions = {".py": Language.PYTHON, ".sql": Language.SQL}
+
+    def _read(self, file_uri: str):
+        file = Path(file_uri.removeprefix("file://"))
+        if file.suffix not in self._extensions:
+            raise KeyError(f"no language for {file.suffix}")
+        language = self._extensions[file.suffix]
+        with file.open('r', encoding='utf8') as f:
+            return f.read(), language
+
+    def lint(self, file_uri: str):
+        code, language = self._read(file_uri)
+        analyser = self._languages.linter(language)
+        diagnostics = [Diagnostic.from_advice(_) for _ in analyser.lint(code)]
+        return AnalyseResponse(diagnostics)
+
+    def quickfix(self, file_uri: str, code_range: Range, diagnostic_code: str):
+        code, language = self._read(file_uri)
+        fixer = self._languages.fixer(language, diagnostic_code)
+        if not fixer:
+            return QuickFixResponse(code_actions=[])
+        fragment = code_range.fragment(code)
+        apply = fixer.apply(fragment)
+        return QuickFixResponse(
+            code_actions=[
+                CodeAction(
+                    title=f"Replace with: {apply}",
+                    edit=WorkspaceEdit(
+                        document_changes=[
+                            TextDocumentEdit(
+                                text_document=OptionalVersionedTextDocumentIdentifier(file_uri),
+                                edits=[TextEdit(code_range, apply)],
+                            ),
+                        ]
+                    ),
+                    is_preferred=True,
+                )
+            ]
+        )
+
+    def serve(self):
+        server_address = ('localhost', 8000)
+        handler_class = functools.partial(_RequestHandler, self)
+        httpd = http.server.ThreadingHTTPServer(server_address, handler_class)
+        httpd.serve_forever()
+
+
+class _RequestHandler(http.server.BaseHTTPRequestHandler):
+    def __init__(self, lsp_server: LspServer, *args):
+        self._lsp_server = lsp_server
+        super().__init__(*args)
+
+    def log_message(self, fmt: str, *args: Any):  # pylint: disable=arguments-differ
+        logger.debug(fmt % args)  # pylint: disable=logging-not-lazy
+
+    def do_POST(self):  # pylint: disable=invalid-name
+        if not self.path.startswith('/quickfix'):
+            self.send_error(400, 'Wrong input')
+            return
+        self.send_response(200)
+        self.end_headers()
+
+        content_length = int(self.headers['Content-Length'])
+        post_data = self.rfile.read(content_length)
+        raw = json.loads(post_data.decode('utf-8'))
+        logger.debug(f"Received:\n{raw}")
+
+        rng = Range.from_dict(raw['range'])
+        response = self._lsp_server.quickfix(raw['file_uri'], rng, raw['code'])
+
+        raw = json.dumps(response.as_dict()).encode('utf-8')
+        self.wfile.write(raw)
+
+    def do_GET(self):  # pylint: disable=invalid-name
+        if not self.path.startswith('/lint'):
+            self.send_error(400, 'Wrong input')
+            return
+        parts = self.path.split('?')
+        if len(parts) != 2:
+            self.send_error(400, 'Missing Query')
+            return
+        _, query_string = parts
+        query = dict(parse_qsl(query_string))
+        response = self._lsp_server.lint(query['file_uri'])
+        if not response:
+            self.send_error(404, 'no analyser for file type')
+            return
+
+        self.send_response(200)
+        self.end_headers()
+        raw = json.dumps(response.as_dict()).encode('utf-8')
+        self.wfile.write(raw)
+        self.wfile.flush()
+
+
+if __name__ == '__main__':
+    install_logger()
+    logging.root.setLevel('DEBUG')
+    languages = Languages(
+        MigrationIndex(
+            [
+                MigrationStatus(
+                    src_schema='old', src_table='things', dst_catalog='brand', dst_schema='new', dst_table='stuff'
+                ),
+                MigrationStatus(
+                    src_schema='other',
+                    src_table='matters',
+                    dst_catalog='some',
+                    dst_schema='certain',
+                    dst_table='issues',
+                ),
+            ]
+        )
+    )
+    lsp = LspServer(languages)
+    lsp.serve()
```

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/migration/main/01_0_data_object_migration_status.md` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/migration/main/01_0_data_object_migration_status.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/migration/main/01_1_data_object_migration_status.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/migration/main/01_1_data_object_migration_status.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/code_patterns.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/code_patterns.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/grant_detail.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/grant_detail.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/misc_patterns.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/misc_patterns.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/objects.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/objects.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/table_estimates.sql` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/queries/views/table_estimates.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/ast_helpers.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/base.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/base.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/dbfs.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/dbfs.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/files.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/files.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/graph.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/graph.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/jobs.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/jobs.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/languages.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/languages.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/path_lookup.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/path_lookup.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/pyspark.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/pyspark.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/python_linter.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/python_linter.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/queries.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/queries.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/redash.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/redash.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/site_packages.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/site_packages.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/spark_connect.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/spark_connect.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/table_creation.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/table_creation.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/whitelist.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/whitelist.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/workflows.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/workflows.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/cells.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/cells.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/loaders.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/loaders.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/migrator.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/migrator.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/sources.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/source_code/notebooks/sources.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.23.0_add_assessment_to_udf.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/upgrades/v0.23.0_add_assessment_to_udf.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/base.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/base.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/clusters.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/clusters.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/generic.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/generic.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/groups.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/groups.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/listing.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/listing.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/manager.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/manager.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/redash.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/redash.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/scim.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/scim.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/secrets.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/secrets.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/tacl.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/tacl.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/workflows.py` & `databricks_labs_ucx-0.23.1/databricks/labs/ucx/workspace_access/workflows.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/.gitignore` & `databricks_labs_ucx-0.23.1/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/LICENSE` & `databricks_labs_ucx-0.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/NOTICE` & `databricks_labs_ucx-0.23.1/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/README.md` & `databricks_labs_ucx-0.23.1/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.23.0/pyproject.toml` & `databricks_labs_ucx-0.23.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "Operating System :: Microsoft :: Windows",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
 
 dependencies = ["databricks-sdk~=0.27.0",
                 "databricks-labs-lsql~=0.4.0",
-                "databricks-labs-blueprint~=0.4.3",
+                "databricks-labs-blueprint>=0.4.3,<0.6.0",
                 "PyYAML>=6.0.0,<7.0.0",
                 "sqlglot>=23.9,<23.15"]
 
 [project.entry-points.databricks]
 runtime = "databricks.labs.ucx.runtime:main"
 
 [project.urls]
```

### Comparing `databricks_labs_ucx-0.23.0/PKG-INFO` & `databricks_labs_ucx-0.23.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-ucx
-Version: 0.23.0
+Version: 0.23.1
 Summary: UCX - Unity Catalog Migration Toolkit
 Project-URL: Issues, https://github.com/databricks/ucx/issues
 Project-URL: Source, https://github.com/databricks/ucx
 Author-email: Serge Smertin <serge.smertin@databricks.com>
 Maintainer-email: Serge Smertin <serge.smertin@databricks.com>, Liran Bareket <liran.bareket@databricks.com>, Marcin Wojtyczka <marcin.wojtyczka@databricks.com>, Ziyuan Qin <ziyuan.qin@databricks.com>, William Conti <william.conti@databricks.com>, Hari Selvarajan <hari.selvarajan@databricks.com>, Vuong Nguyen <vuong.nguyen@databricks.com>
 License-File: LICENSE
 License-File: NOTICE
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
-Requires-Dist: databricks-labs-blueprint~=0.4.3
+Requires-Dist: databricks-labs-blueprint<0.6.0,>=0.4.3
 Requires-Dist: databricks-labs-lsql~=0.4.0
 Requires-Dist: databricks-sdk~=0.27.0
 Requires-Dist: pyyaml<7.0.0,>=6.0.0
 Requires-Dist: sqlglot<23.15,>=23.9
 Description-Content-Type: text/markdown
 
 Databricks Labs UCX
```

