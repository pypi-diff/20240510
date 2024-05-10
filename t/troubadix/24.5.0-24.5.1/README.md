# Comparing `tmp/troubadix-24.5.0.tar.gz` & `tmp/troubadix-24.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troubadix-24.5.0.tar", max compression
+gzip compressed data, was "troubadix-24.5.1.tar", max compression
```

## Comparing `troubadix-24.5.0.tar` & `troubadix-24.5.1.tar`

### file list

```diff
@@ -1,201 +1,201 @@
--rw-r--r--   0        0        0    35149 2024-05-08 11:59:27.141145 troubadix-24.5.0/LICENSE
--rw-r--r--   0        0        0     2730 2024-05-08 11:59:27.141145 troubadix-24.5.0/README.md
--rw-r--r--   0        0        0     2567 2024-05-08 11:59:27.145145 troubadix-24.5.0/pyproject.toml
--rw-r--r--   0        0        0      716 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/__init__.py
--rw-r--r--   0        0        0      716 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/helper/__init__.py
--rw-r--r--   0        0        0     8416 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/helper/test_linguistic_exception_handler.py
--rw-r--r--   0        0        0     1940 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/helper/test_patterns.py
--rw-r--r--   0        0        0     2396 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/__init__.py
--rw-r--r--   0        0        0     1012 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/fail.nasl
--rw-r--r--   0        0        0     1291 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/fail2.nasl
--rw-r--r--   0        0        0     2100 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test.nasl
--rw-r--r--   0        0        0     2585 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_badwords.py
--rw-r--r--   0        0        0     5109 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_copyright_text.py
--rw-r--r--   0        0        0     6961 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_copyright_year.py
--rw-r--r--   0        0        0     5004 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_creation_date.py
--rw-r--r--   0        0        0     5878 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_cve_format.py
--rw-r--r--   0        0        0     4914 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_cvss_format.py
--rw-r--r--   0        0        0     8970 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_dependencies.py
--rw-r--r--   0        0        0     5808 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_dependency_category_order.py
--rw-r--r--   0        0        0     5589 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_deprecated_dependency.py
--rw-r--r--   0        0        0     4545 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_deprecated_functions.py
--rw-r--r--   0        0        0     2394 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_double_end_points.py
--rw-r--r--   0        0        0     3504 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_duplicate_oid.py
--rw-r--r--   0        0        0     4686 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_duplicated_script_tags.py
--rw-r--r--   0        0        0     3964 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_encoding.py
--rw-r--r--   0        0        0     1982 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/fail_bad_new_line.nasl
--rw-r--r--   0        0        0      246 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/fail_badwords.nasl
--rw-r--r--   0        0        0     1979 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1965 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/fail_name_newline.nasl
--rwxr-xr-x   0        0        0     1012 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/fail_permissions.nasl
--rw-r--r--   0        0        0      150 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/fail_spelling.nasl
--rw-r--r--   0        0        0     2213 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/fail.nasl
--rw-r--r--   0        0        0      246 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
--rw-r--r--   0        0        0     1990 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1987 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
--rw-r--r--   0        0        0     2134 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
--rw-r--r--   0        0        0     1023 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
--rw-r--r--   0        0        0     1302 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
--rw-r--r--   0        0        0     2122 2024-05-08 11:59:27.145145 troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/runner/test.nasl
--rw-r--r--   0        0        0     2119 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
--rw-r--r--   0        0        0     1023 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/test.inc
--rw-r--r--   0        0        0     2122 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/test.nasl
--rw-r--r--   0        0        0     2976 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_files/nasl/warning.nasl
--rw-r--r--   0        0        0     1012 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_files/ok_permissions.nasl
--rw-r--r--   0        0        0     2100 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_files/test_oid.nasl
--rw-r--r--   0        0        0     4548 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_forking_nasl_functions.py
--rw-r--r--   0        0        0     2271 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_get_kb_on_services.py
--rw-r--r--   0        0        0     9438 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_grammar.py
--rw-r--r--   0        0        0     6936 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_http_links_in_tags.py
--rw-r--r--   0        0        0     4730 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_illegal_characters.py
--rw-r--r--   0        0        0     5965 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_log_messages.py
--rw-r--r--   0        0        0     6174 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_malformed_dependencies.py
--rw-r--r--   0        0        0    21051 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_misplaced_compare_in_if.py
--rw-r--r--   0        0        0     3585 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_missing_desc_exit.py
--rw-r--r--   0        0        0     3101 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_missing_tag_solution.py
--rw-r--r--   0        0        0     4688 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_newlines.py
--rw-r--r--   0        0        0     5001 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_overlong_description_lines.py
--rw-r--r--   0        0        0    40813 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_overlong_script_tags.py
--rw-r--r--   0        0        0     4294 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     4594 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_qod.py
--rw-r--r--   0        0        0     5844 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_reporting_consistency.py
--rw-r--r--   0        0        0     3371 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_add_preference_type.py
--rw-r--r--   0        0        0     2480 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_calls_empty_values.py
--rw-r--r--   0        0        0     2799 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_calls_recommended.py
--rw-r--r--   0        0        0     2650 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_category.py
--rw-r--r--   0        0        0     3469 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_copyright.py
--rw-r--r--   0        0        0     3877 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_family.py
--rw-r--r--   0        0        0     3153 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_tag_form.py
--rw-r--r--   0        0        0     9487 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_tag_whitespaces.py
--rw-r--r--   0        0        0     3313 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_tags_mandatory.py
--rw-r--r--   0        0        0     8542 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     3942 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_xref_form.py
--rw-r--r--   0        0        0     5019 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_script_xref_url.py
--rw-r--r--   0        0        0     6599 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_security_messages.py
--rw-r--r--   0        0        0     3021 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_set_get_kb_calls.py
--rw-r--r--   0        0        0     7260 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_solution_text.py
--rw-r--r--   0        0        0     3306 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_solution_type.py
--rw-r--r--   0        0        0     1087 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_spaces_in_filename.py
--rw-r--r--   0        0        0     2827 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_spelling.py
--rw-r--r--   0        0        0     1813 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_tabs.py
--rw-r--r--   0        0        0     6297 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_todo_tbd.py
--rw-r--r--   0        0        0     2570 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_trailing_spaces_tabs.py
--rw-r--r--   0        0        0     3868 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_using_display.py
--rw-r--r--   0        0        0    24134 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_valid_oid.py
--rw-r--r--   0        0        0     4154 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_valid_script_tag_names.py
--rw-r--r--   0        0        0     1947 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_vt_file_permissions.py
--rw-r--r--   0        0        0     5189 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/plugins/test_vt_placement.py
--rw-r--r--   0        0        0      716 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/__init__.py
--rw-r--r--   0        0        0      716 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/changed_packages/__init__.py
--rw-r--r--   0        0        0      716 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/__init__.py
--rw-r--r--   0        0        0     3075 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
--rw-r--r--   0        0        0     2620 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/test_added_release.py
--rw-r--r--   0        0        0     1792 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
--rw-r--r--   0        0        0     3258 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
--rw-r--r--   0        0        0     3584 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
--rw-r--r--   0        0        0     3780 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/changed_packages/test_changed_packages.py
--rw-r--r--   0        0        0     2427 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/changed_packages/test_package.py
--rw-r--r--   0        0        0     2977 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/test_changed_cves.py
--rw-r--r--   0        0        0     2952 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/test_changed_oid.py
--rw-r--r--   0        0        0     5507 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/test_file_extensions.py
--rw-r--r--   0        0        0     3962 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/test_last_modification.py
--rw-r--r--   0        0        0     8879 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/test_no_solution.py
--rw-r--r--   0        0        0     6293 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/standalone_plugins/test_version_updated.py
--rw-r--r--   0        0        0     4768 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/test_argparser.py
--rw-r--r--   0        0        0     3947 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/test_helper.py
--rw-r--r--   0        0        0     3671 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/test_naslinter.py
--rw-r--r--   0        0        0     3399 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/test_reporter.py
--rw-r--r--   0        0        0     2517 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/test_results.py
--rw-r--r--   0        0        0    17972 2024-05-08 11:59:27.149145 troubadix-24.5.0/tests/test_runner.py
--rw-r--r--   0        0        0      716 2024-05-08 11:59:27.149145 troubadix-24.5.0/troubadix/__init__.py
--rw-r--r--   0        0        0      103 2024-05-08 11:59:27.149145 troubadix-24.5.0/troubadix/__version__.py
--rw-r--r--   0        0        0     6999 2024-05-08 11:59:27.149145 troubadix-24.5.0/troubadix/argparser.py
--rw-r--r--   0        0        0      338 2024-05-08 11:59:27.149145 troubadix-24.5.0/troubadix/codespell/codespell.additions
--rw-r--r--   0        0        0   134180 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/codespell/codespell.exclude
--rw-r--r--   0        0        0     1175 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/codespell/codespell.ignore
--rw-r--r--   0        0        0     1061 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/helper/__init__.py
--rw-r--r--   0        0        0     3105 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/helper/helper.py
--rw-r--r--   0        0        0     6811 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/helper/linguistic_exception_handler.py
--rw-r--r--   0        0        0     9174 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/helper/patterns.py
--rw-r--r--   0        0        0     3508 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugin.py
--rw-r--r--   0        0        0     7216 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/__init__.py
--rw-r--r--   0        0        0     4578 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/badwords.py
--rw-r--r--   0        0        0     3583 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/copyright_text.py
--rw-r--r--   0        0        0     3334 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/copyright_year.py
--rw-r--r--   0        0        0     3357 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/creation_date.py
--rw-r--r--   0        0        0     3400 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/cve_format.py
--rw-r--r--   0        0        0     2309 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/cvss_format.py
--rw-r--r--   0        0        0     4456 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/dependencies.py
--rw-r--r--   0        0        0     7316 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/dependency_category_order.py
--rw-r--r--   0        0        0     4137 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/deprecated_dependency.py
--rw-r--r--   0        0        0     2568 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/deprecated_functions.py
--rw-r--r--   0        0        0     2509 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/double_end_points.py
--rw-r--r--   0        0        0     2652 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/duplicate_oid.py
--rw-r--r--   0        0        0     3179 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/duplicated_script_tags.py
--rw-r--r--   0        0        0     2066 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/encoding.py
--rw-r--r--   0        0        0     6014 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/forking_nasl_functions.py
--rw-r--r--   0        0        0     3401 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/get_kb_on_services.py
--rw-r--r--   0        0        0     8566 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/grammar.py
--rw-r--r--   0        0        0     7256 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/http_links_in_tags.py
--rw-r--r--   0        0        0     4406 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/illegal_characters.py
--rw-r--r--   0        0        0     2960 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/log_messages.py
--rw-r--r--   0        0        0     3000 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/malformed_dependencies.py
--rw-r--r--   0        0        0     5330 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/misplaced_compare_in_if.py
--rw-r--r--   0        0        0     2411 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/missing_desc_exit.py
--rw-r--r--   0        0        0     2828 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/missing_tag_solution.py
--rw-r--r--   0        0        0     2788 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/newlines.py
--rw-r--r--   0        0        0     2757 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/overlong_description_lines.py
--rw-r--r--   0        0        0     2373 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/overlong_script_tags.py
--rw-r--r--   0        0        0     4584 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     3816 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/qod.py
--rw-r--r--   0        0        0     4081 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/reporting_consistency.py
--rw-r--r--   0        0        0     3193 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_add_preference_type.py
--rw-r--r--   0        0        0     2512 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_calls_empty_values.py
--rw-r--r--   0        0        0     3137 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_calls_recommended.py
--rw-r--r--   0        0        0     2184 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_category.py
--rw-r--r--   0        0        0     2310 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_copyright.py
--rw-r--r--   0        0        0     4023 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_family.py
--rw-r--r--   0        0        0     1773 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_tag_form.py
--rw-r--r--   0        0        0     2319 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_tag_whitespaces.py
--rw-r--r--   0        0        0     2630 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_tags_mandatory.py
--rw-r--r--   0        0        0     7638 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     1848 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_xref_form.py
--rw-r--r--   0        0        0     2875 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/script_xref_url.py
--rw-r--r--   0        0        0     4708 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/security_messages.py
--rw-r--r--   0        0        0     3415 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/set_get_kb_calls.py
--rw-r--r--   0        0        0     5852 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/solution_text.py
--rw-r--r--   0        0        0     2602 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/solution_type.py
--rw-r--r--   0        0        0      611 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/spaces_in_filename.py
--rw-r--r--   0        0        0     9557 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/spelling.py
--rw-r--r--   0        0        0     1319 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/tabs.py
--rw-r--r--   0        0        0     1733 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/todo_tbd.py
--rw-r--r--   0        0        0     1873 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/trailing_spaces_tabs.py
--rw-r--r--   0        0        0     4046 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/using_display.py
--rw-r--r--   0        0        0    16627 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/valid_oid.py
--rw-r--r--   0        0        0     3447 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/valid_script_tag_names.py
--rw-r--r--   0        0        0     3285 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/variable_assigned_in_if.py
--rw-r--r--   0        0        0     1521 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/vt_file_permissions.py
--rw-r--r--   0        0        0     2800 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/plugins/vt_placement.py
--rw-r--r--   0        0        0     9176 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/reporter.py
--rw-r--r--   0        0        0     2632 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/results.py
--rw-r--r--   0        0        0     5172 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/runner.py
--rw-r--r--   0        0        0       22 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/standalone_plugins/__init__.py
--rw-r--r--   0        0        0     4145 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/standalone_plugins/allowed_rev_diff.py
--rw-r--r--   0        0        0     2921 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/standalone_plugins/changed_cves.py
--rw-r--r--   0        0        0     4047 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/standalone_plugins/changed_oid.py
--rw-r--r--   0        0        0     5742 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/changed_packages.py
--rw-r--r--   0        0        0      923 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/__init__.py
--rw-r--r--   0        0        0     1797 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
--rw-r--r--   0        0        0     1486 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/added_release.py
--rw-r--r--   0        0        0     1124 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
--rw-r--r--   0        0        0     1952 2024-05-08 11:59:27.153145 troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
--rw-r--r--   0        0        0     1634 2024-05-08 11:59:27.157145 troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
--rw-r--r--   0        0        0     1278 2024-05-08 11:59:27.157145 troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/marker.py
--rw-r--r--   0        0        0     2743 2024-05-08 11:59:27.157145 troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/package.py
--rw-r--r--   0        0        0     1028 2024-05-08 11:59:27.157145 troubadix-24.5.0/troubadix/standalone_plugins/common.py
--rw-r--r--   0        0        0     2327 2024-05-08 11:59:27.157145 troubadix-24.5.0/troubadix/standalone_plugins/file_extensions.py
--rw-r--r--   0        0        0     4616 2024-05-08 11:59:27.157145 troubadix-24.5.0/troubadix/standalone_plugins/last_modification.py
--rw-r--r--   0        0        0     8877 2024-05-08 11:59:27.157145 troubadix-24.5.0/troubadix/standalone_plugins/no_solution.py
--rw-r--r--   0        0        0     4263 2024-05-08 11:59:27.157145 troubadix-24.5.0/troubadix/standalone_plugins/version_updated.py
--rw-r--r--   0        0        0     6045 2024-05-08 11:59:27.157145 troubadix-24.5.0/troubadix/troubadix.py
--rw-r--r--   0        0        0     3965 1970-01-01 00:00:00.000000 troubadix-24.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-10 12:45:06.997157 troubadix-24.5.1/LICENSE
+-rw-r--r--   0        0        0     2730 2024-05-10 12:45:06.997157 troubadix-24.5.1/README.md
+-rw-r--r--   0        0        0     2567 2024-05-10 12:45:07.001157 troubadix-24.5.1/pyproject.toml
+-rw-r--r--   0        0        0      716 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      716 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/helper/__init__.py
+-rw-r--r--   0        0        0     8416 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/helper/test_linguistic_exception_handler.py
+-rw-r--r--   0        0        0     1940 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/helper/test_patterns.py
+-rw-r--r--   0        0        0     2396 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     1012 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/fail.nasl
+-rw-r--r--   0        0        0     1291 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/fail2.nasl
+-rw-r--r--   0        0        0     2100 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test.nasl
+-rw-r--r--   0        0        0     2585 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_badwords.py
+-rw-r--r--   0        0        0     5109 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_copyright_text.py
+-rw-r--r--   0        0        0     6961 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_copyright_year.py
+-rw-r--r--   0        0        0     5004 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_creation_date.py
+-rw-r--r--   0        0        0     5878 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_cve_format.py
+-rw-r--r--   0        0        0     4914 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_cvss_format.py
+-rw-r--r--   0        0        0     8970 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_dependencies.py
+-rw-r--r--   0        0        0     5808 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_dependency_category_order.py
+-rw-r--r--   0        0        0     5589 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_deprecated_dependency.py
+-rw-r--r--   0        0        0     4545 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_deprecated_functions.py
+-rw-r--r--   0        0        0     2394 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_double_end_points.py
+-rw-r--r--   0        0        0     3504 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_duplicate_oid.py
+-rw-r--r--   0        0        0     4686 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_duplicated_script_tags.py
+-rw-r--r--   0        0        0     3964 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_encoding.py
+-rw-r--r--   0        0        0     1982 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_files/fail_bad_new_line.nasl
+-rw-r--r--   0        0        0      246 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_files/fail_badwords.nasl
+-rw-r--r--   0        0        0     1979 2024-05-10 12:45:07.001157 troubadix-24.5.1/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1965 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/fail_name_newline.nasl
+-rwxr-xr-x   0        0        0     1012 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/fail_permissions.nasl
+-rw-r--r--   0        0        0      150 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/fail_spelling.nasl
+-rw-r--r--   0        0        0     2213 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/fail.nasl
+-rw-r--r--   0        0        0      246 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
+-rw-r--r--   0        0        0     1990 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1987 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
+-rw-r--r--   0        0        0     2134 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
+-rw-r--r--   0        0        0     1023 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
+-rw-r--r--   0        0        0     1302 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
+-rw-r--r--   0        0        0     2122 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/runner/test.nasl
+-rw-r--r--   0        0        0     2119 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
+-rw-r--r--   0        0        0     1023 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/test.inc
+-rw-r--r--   0        0        0     2122 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/test.nasl
+-rw-r--r--   0        0        0     2976 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/nasl/warning.nasl
+-rw-r--r--   0        0        0     1012 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/ok_permissions.nasl
+-rw-r--r--   0        0        0     2100 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_files/test_oid.nasl
+-rw-r--r--   0        0        0     4548 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_forking_nasl_functions.py
+-rw-r--r--   0        0        0     2271 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_get_kb_on_services.py
+-rw-r--r--   0        0        0     9438 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_grammar.py
+-rw-r--r--   0        0        0     6936 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_http_links_in_tags.py
+-rw-r--r--   0        0        0     4730 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_illegal_characters.py
+-rw-r--r--   0        0        0     5965 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_log_messages.py
+-rw-r--r--   0        0        0     6174 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_malformed_dependencies.py
+-rw-r--r--   0        0        0    21051 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     3585 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_missing_desc_exit.py
+-rw-r--r--   0        0        0     3101 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_missing_tag_solution.py
+-rw-r--r--   0        0        0     4688 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_newlines.py
+-rw-r--r--   0        0        0     5001 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_overlong_description_lines.py
+-rw-r--r--   0        0        0    40813 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_overlong_script_tags.py
+-rw-r--r--   0        0        0     4294 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     4594 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_qod.py
+-rw-r--r--   0        0        0     5844 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_reporting_consistency.py
+-rw-r--r--   0        0        0     3371 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_add_preference_type.py
+-rw-r--r--   0        0        0     2480 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_calls_empty_values.py
+-rw-r--r--   0        0        0     2799 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_calls_recommended.py
+-rw-r--r--   0        0        0     2650 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_category.py
+-rw-r--r--   0        0        0     3469 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_copyright.py
+-rw-r--r--   0        0        0     3877 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_family.py
+-rw-r--r--   0        0        0     3153 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_tag_form.py
+-rw-r--r--   0        0        0     9487 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_tag_whitespaces.py
+-rw-r--r--   0        0        0     3313 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_tags_mandatory.py
+-rw-r--r--   0        0        0     8542 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     3942 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_xref_form.py
+-rw-r--r--   0        0        0     5019 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_script_xref_url.py
+-rw-r--r--   0        0        0     6599 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_security_messages.py
+-rw-r--r--   0        0        0     3021 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_set_get_kb_calls.py
+-rw-r--r--   0        0        0     7260 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_solution_text.py
+-rw-r--r--   0        0        0     3306 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_solution_type.py
+-rw-r--r--   0        0        0     1087 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_spaces_in_filename.py
+-rw-r--r--   0        0        0     2827 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_spelling.py
+-rw-r--r--   0        0        0     1813 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_tabs.py
+-rw-r--r--   0        0        0     6297 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_todo_tbd.py
+-rw-r--r--   0        0        0     2570 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     3868 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_using_display.py
+-rw-r--r--   0        0        0    24134 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_valid_oid.py
+-rw-r--r--   0        0        0     4154 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_valid_script_tag_names.py
+-rw-r--r--   0        0        0     1947 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_vt_file_permissions.py
+-rw-r--r--   0        0        0     5189 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/plugins/test_vt_placement.py
+-rw-r--r--   0        0        0      716 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0      716 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/changed_packages/__init__.py
+-rw-r--r--   0        0        0      716 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/__init__.py
+-rw-r--r--   0        0        0     3075 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
+-rw-r--r--   0        0        0     2620 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/test_added_release.py
+-rw-r--r--   0        0        0     1792 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
+-rw-r--r--   0        0        0     3258 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
+-rw-r--r--   0        0        0     3584 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
+-rw-r--r--   0        0        0     3780 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/changed_packages/test_changed_packages.py
+-rw-r--r--   0        0        0     2427 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/changed_packages/test_package.py
+-rw-r--r--   0        0        0     2977 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/test_changed_cves.py
+-rw-r--r--   0        0        0     2952 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/test_changed_oid.py
+-rw-r--r--   0        0        0     5507 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/test_file_extensions.py
+-rw-r--r--   0        0        0     3962 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/test_last_modification.py
+-rw-r--r--   0        0        0     8879 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/test_no_solution.py
+-rw-r--r--   0        0        0     6293 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/standalone_plugins/test_version_updated.py
+-rw-r--r--   0        0        0     4768 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/test_argparser.py
+-rw-r--r--   0        0        0     3947 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/test_helper.py
+-rw-r--r--   0        0        0     3671 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/test_naslinter.py
+-rw-r--r--   0        0        0     3399 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/test_reporter.py
+-rw-r--r--   0        0        0     2517 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/test_results.py
+-rw-r--r--   0        0        0    17972 2024-05-10 12:45:07.005157 troubadix-24.5.1/tests/test_runner.py
+-rw-r--r--   0        0        0      716 2024-05-10 12:45:07.005157 troubadix-24.5.1/troubadix/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-10 12:45:07.005157 troubadix-24.5.1/troubadix/__version__.py
+-rw-r--r--   0        0        0     6999 2024-05-10 12:45:07.005157 troubadix-24.5.1/troubadix/argparser.py
+-rw-r--r--   0        0        0      338 2024-05-10 12:45:07.005157 troubadix-24.5.1/troubadix/codespell/codespell.additions
+-rw-r--r--   0        0        0   134180 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/codespell/codespell.exclude
+-rw-r--r--   0        0        0     1175 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/codespell/codespell.ignore
+-rw-r--r--   0        0        0     1061 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/helper/__init__.py
+-rw-r--r--   0        0        0     3105 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/helper/helper.py
+-rw-r--r--   0        0        0     6811 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/helper/linguistic_exception_handler.py
+-rw-r--r--   0        0        0     9174 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/helper/patterns.py
+-rw-r--r--   0        0        0     3508 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugin.py
+-rw-r--r--   0        0        0     7216 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/__init__.py
+-rw-r--r--   0        0        0     4578 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/badwords.py
+-rw-r--r--   0        0        0     3583 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/copyright_text.py
+-rw-r--r--   0        0        0     3334 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/copyright_year.py
+-rw-r--r--   0        0        0     3357 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/creation_date.py
+-rw-r--r--   0        0        0     3400 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/cve_format.py
+-rw-r--r--   0        0        0     2309 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/cvss_format.py
+-rw-r--r--   0        0        0     4456 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/dependencies.py
+-rw-r--r--   0        0        0     7316 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/dependency_category_order.py
+-rw-r--r--   0        0        0     4137 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/deprecated_dependency.py
+-rw-r--r--   0        0        0     2568 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/deprecated_functions.py
+-rw-r--r--   0        0        0     2509 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/double_end_points.py
+-rw-r--r--   0        0        0     2652 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/duplicate_oid.py
+-rw-r--r--   0        0        0     3179 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/duplicated_script_tags.py
+-rw-r--r--   0        0        0     2066 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/encoding.py
+-rw-r--r--   0        0        0     6014 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/forking_nasl_functions.py
+-rw-r--r--   0        0        0     3401 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/get_kb_on_services.py
+-rw-r--r--   0        0        0     8566 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/grammar.py
+-rw-r--r--   0        0        0     7283 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/http_links_in_tags.py
+-rw-r--r--   0        0        0     4406 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/illegal_characters.py
+-rw-r--r--   0        0        0     2960 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/log_messages.py
+-rw-r--r--   0        0        0     3000 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/malformed_dependencies.py
+-rw-r--r--   0        0        0     5330 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     2411 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/missing_desc_exit.py
+-rw-r--r--   0        0        0     2828 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/missing_tag_solution.py
+-rw-r--r--   0        0        0     2788 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/newlines.py
+-rw-r--r--   0        0        0     2757 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/overlong_description_lines.py
+-rw-r--r--   0        0        0     2373 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/overlong_script_tags.py
+-rw-r--r--   0        0        0     4584 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     3816 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/qod.py
+-rw-r--r--   0        0        0     4081 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/reporting_consistency.py
+-rw-r--r--   0        0        0     3193 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_add_preference_type.py
+-rw-r--r--   0        0        0     2512 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_calls_empty_values.py
+-rw-r--r--   0        0        0     3137 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_calls_recommended.py
+-rw-r--r--   0        0        0     2184 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_category.py
+-rw-r--r--   0        0        0     2310 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_copyright.py
+-rw-r--r--   0        0        0     4023 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_family.py
+-rw-r--r--   0        0        0     1773 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_tag_form.py
+-rw-r--r--   0        0        0     2319 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_tag_whitespaces.py
+-rw-r--r--   0        0        0     2630 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_tags_mandatory.py
+-rw-r--r--   0        0        0     7638 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     1848 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_xref_form.py
+-rw-r--r--   0        0        0     2875 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/script_xref_url.py
+-rw-r--r--   0        0        0     4708 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/security_messages.py
+-rw-r--r--   0        0        0     3415 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/set_get_kb_calls.py
+-rw-r--r--   0        0        0     5852 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/solution_text.py
+-rw-r--r--   0        0        0     2602 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/solution_type.py
+-rw-r--r--   0        0        0      611 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/spaces_in_filename.py
+-rw-r--r--   0        0        0     9557 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/spelling.py
+-rw-r--r--   0        0        0     1319 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/tabs.py
+-rw-r--r--   0        0        0     1733 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/todo_tbd.py
+-rw-r--r--   0        0        0     1873 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     4046 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/using_display.py
+-rw-r--r--   0        0        0    16627 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/valid_oid.py
+-rw-r--r--   0        0        0     3447 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/valid_script_tag_names.py
+-rw-r--r--   0        0        0     3285 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/variable_assigned_in_if.py
+-rw-r--r--   0        0        0     1521 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/vt_file_permissions.py
+-rw-r--r--   0        0        0     2800 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/plugins/vt_placement.py
+-rw-r--r--   0        0        0     9176 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/reporter.py
+-rw-r--r--   0        0        0     2632 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/results.py
+-rw-r--r--   0        0        0     5172 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/runner.py
+-rw-r--r--   0        0        0       22 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0     4145 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/standalone_plugins/allowed_rev_diff.py
+-rw-r--r--   0        0        0     2921 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/standalone_plugins/changed_cves.py
+-rw-r--r--   0        0        0     4047 2024-05-10 12:45:07.009157 troubadix-24.5.1/troubadix/standalone_plugins/changed_oid.py
+-rw-r--r--   0        0        0     5742 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/changed_packages.py
+-rw-r--r--   0        0        0      923 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/__init__.py
+-rw-r--r--   0        0        0     1797 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
+-rw-r--r--   0        0        0     1486 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/added_release.py
+-rw-r--r--   0        0        0     1124 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
+-rw-r--r--   0        0        0     1952 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
+-rw-r--r--   0        0        0     1634 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
+-rw-r--r--   0        0        0     1278 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/marker.py
+-rw-r--r--   0        0        0     2743 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/package.py
+-rw-r--r--   0        0        0     1028 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/common.py
+-rw-r--r--   0        0        0     2327 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/file_extensions.py
+-rw-r--r--   0        0        0     4616 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/last_modification.py
+-rw-r--r--   0        0        0     8877 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/no_solution.py
+-rw-r--r--   0        0        0     4263 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/standalone_plugins/version_updated.py
+-rw-r--r--   0        0        0     6045 2024-05-10 12:45:07.013157 troubadix-24.5.1/troubadix/troubadix.py
+-rw-r--r--   0        0        0     3965 1970-01-01 00:00:00.000000 troubadix-24.5.1/PKG-INFO
```

### Comparing `troubadix-24.5.0/LICENSE` & `troubadix-24.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/README.md` & `troubadix-24.5.1/README.md`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/pyproject.toml` & `troubadix-24.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troubadix"
-version = "24.5.0"
+version = "24.5.1"
 description = "A linting and QA check tool for NASL files"
 authors = ["Greenbone <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/greenbone/troubadix"
 homepage = "https://github.com/greenbone/troubadix"
```

### Comparing `troubadix-24.5.0/tests/__init__.py` & `troubadix-24.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/helper/__init__.py` & `troubadix-24.5.1/tests/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/helper/test_linguistic_exception_handler.py` & `troubadix-24.5.1/tests/helper/test_linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/helper/test_patterns.py` & `troubadix-24.5.1/tests/helper/test_patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/__init__.py` & `troubadix-24.5.1/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/fail.nasl` & `troubadix-24.5.1/tests/plugins/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/fail2.nasl` & `troubadix-24.5.1/tests/plugins/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test.nasl` & `troubadix-24.5.1/tests/plugins/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_badwords.py` & `troubadix-24.5.1/tests/plugins/test_badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_copyright_text.py` & `troubadix-24.5.1/tests/plugins/test_copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_copyright_year.py` & `troubadix-24.5.1/tests/plugins/test_copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_creation_date.py` & `troubadix-24.5.1/tests/plugins/test_creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_cve_format.py` & `troubadix-24.5.1/tests/plugins/test_cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_cvss_format.py` & `troubadix-24.5.1/tests/plugins/test_cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_dependencies.py` & `troubadix-24.5.1/tests/plugins/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_dependency_category_order.py` & `troubadix-24.5.1/tests/plugins/test_dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_deprecated_dependency.py` & `troubadix-24.5.1/tests/plugins/test_deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_deprecated_functions.py` & `troubadix-24.5.1/tests/plugins/test_deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_double_end_points.py` & `troubadix-24.5.1/tests/plugins/test_double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_duplicate_oid.py` & `troubadix-24.5.1/tests/plugins/test_duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_duplicated_script_tags.py` & `troubadix-24.5.1/tests/plugins/test_duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_encoding.py` & `troubadix-24.5.1/tests/plugins/test_encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/fail_bad_new_line.nasl` & `troubadix-24.5.1/tests/plugins/test_files/fail_bad_new_line.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/fail_name_and_copyright_newline.nasl` & `troubadix-24.5.1/tests/plugins/test_files/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/fail_name_newline.nasl` & `troubadix-24.5.1/tests/plugins/test_files/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/fail_permissions.nasl` & `troubadix-24.5.1/tests/plugins/test_files/fail_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/fail.nasl` & `troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl` & `troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl` & `troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl` & `troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/runner/fail.nasl` & `troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/runner/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl` & `troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/runner/test.nasl` & `troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/runner/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl` & `troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/test.inc` & `troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/test.inc`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/nasl/21.04/test.nasl` & `troubadix-24.5.1/tests/plugins/test_files/nasl/21.04/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/nasl/warning.nasl` & `troubadix-24.5.1/tests/plugins/test_files/nasl/warning.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/ok_permissions.nasl` & `troubadix-24.5.1/tests/plugins/test_files/ok_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_files/test_oid.nasl` & `troubadix-24.5.1/tests/plugins/test_files/test_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_forking_nasl_functions.py` & `troubadix-24.5.1/tests/plugins/test_forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_get_kb_on_services.py` & `troubadix-24.5.1/tests/plugins/test_get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_grammar.py` & `troubadix-24.5.1/tests/plugins/test_grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_http_links_in_tags.py` & `troubadix-24.5.1/tests/plugins/test_http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_illegal_characters.py` & `troubadix-24.5.1/tests/plugins/test_illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_log_messages.py` & `troubadix-24.5.1/tests/plugins/test_log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_malformed_dependencies.py` & `troubadix-24.5.1/tests/plugins/test_malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_misplaced_compare_in_if.py` & `troubadix-24.5.1/tests/plugins/test_misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_missing_desc_exit.py` & `troubadix-24.5.1/tests/plugins/test_missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_missing_tag_solution.py` & `troubadix-24.5.1/tests/plugins/test_missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_newlines.py` & `troubadix-24.5.1/tests/plugins/test_newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_overlong_description_lines.py` & `troubadix-24.5.1/tests/plugins/test_overlong_description_lines.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_overlong_script_tags.py` & `troubadix-24.5.1/tests/plugins/test_overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_prod_svc_detect_in_vulnvt.py` & `troubadix-24.5.1/tests/plugins/test_prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_qod.py` & `troubadix-24.5.1/tests/plugins/test_qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_reporting_consistency.py` & `troubadix-24.5.1/tests/plugins/test_reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_add_preference_type.py` & `troubadix-24.5.1/tests/plugins/test_script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_calls_empty_values.py` & `troubadix-24.5.1/tests/plugins/test_script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_calls_recommended.py` & `troubadix-24.5.1/tests/plugins/test_script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_category.py` & `troubadix-24.5.1/tests/plugins/test_script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_copyright.py` & `troubadix-24.5.1/tests/plugins/test_script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_family.py` & `troubadix-24.5.1/tests/plugins/test_script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_tag_form.py` & `troubadix-24.5.1/tests/plugins/test_script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_tag_whitespaces.py` & `troubadix-24.5.1/tests/plugins/test_script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_tags_mandatory.py` & `troubadix-24.5.1/tests/plugins/test_script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_version_and_last_modification_tags.py` & `troubadix-24.5.1/tests/plugins/test_script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_xref_form.py` & `troubadix-24.5.1/tests/plugins/test_script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_script_xref_url.py` & `troubadix-24.5.1/tests/plugins/test_script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_security_messages.py` & `troubadix-24.5.1/tests/plugins/test_security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_set_get_kb_calls.py` & `troubadix-24.5.1/tests/plugins/test_set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_solution_text.py` & `troubadix-24.5.1/tests/plugins/test_solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_solution_type.py` & `troubadix-24.5.1/tests/plugins/test_solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_spaces_in_filename.py` & `troubadix-24.5.1/tests/plugins/test_spaces_in_filename.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_spelling.py` & `troubadix-24.5.1/tests/plugins/test_spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_tabs.py` & `troubadix-24.5.1/tests/plugins/test_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_todo_tbd.py` & `troubadix-24.5.1/tests/plugins/test_todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_trailing_spaces_tabs.py` & `troubadix-24.5.1/tests/plugins/test_trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_using_display.py` & `troubadix-24.5.1/tests/plugins/test_using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_valid_oid.py` & `troubadix-24.5.1/tests/plugins/test_valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_valid_script_tag_names.py` & `troubadix-24.5.1/tests/plugins/test_valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_vt_file_permissions.py` & `troubadix-24.5.1/tests/plugins/test_vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/plugins/test_vt_placement.py` & `troubadix-24.5.1/tests/plugins/test_vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/__init__.py` & `troubadix-24.5.1/tests/standalone_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/changed_packages/__init__.py` & `troubadix-24.5.1/tests/standalone_plugins/changed_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/__init__.py` & `troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py` & `troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/test_added_release.py` & `troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/test_added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py` & `troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/test_changed_update.py` & `troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/test_changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py` & `troubadix-24.5.1/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/changed_packages/test_changed_packages.py` & `troubadix-24.5.1/tests/standalone_plugins/changed_packages/test_changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/changed_packages/test_package.py` & `troubadix-24.5.1/tests/standalone_plugins/changed_packages/test_package.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/test_changed_cves.py` & `troubadix-24.5.1/tests/standalone_plugins/test_changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/test_changed_oid.py` & `troubadix-24.5.1/tests/standalone_plugins/test_changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/test_file_extensions.py` & `troubadix-24.5.1/tests/standalone_plugins/test_file_extensions.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/test_last_modification.py` & `troubadix-24.5.1/tests/standalone_plugins/test_last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/test_no_solution.py` & `troubadix-24.5.1/tests/standalone_plugins/test_no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/standalone_plugins/test_version_updated.py` & `troubadix-24.5.1/tests/standalone_plugins/test_version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/test_argparser.py` & `troubadix-24.5.1/tests/test_argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/test_helper.py` & `troubadix-24.5.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/test_naslinter.py` & `troubadix-24.5.1/tests/test_naslinter.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/test_reporter.py` & `troubadix-24.5.1/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/test_results.py` & `troubadix-24.5.1/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/tests/test_runner.py` & `troubadix-24.5.1/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/__init__.py` & `troubadix-24.5.1/troubadix/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/argparser.py` & `troubadix-24.5.1/troubadix/argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/codespell/codespell.exclude` & `troubadix-24.5.1/troubadix/codespell/codespell.exclude`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/codespell/codespell.ignore` & `troubadix-24.5.1/troubadix/codespell/codespell.ignore`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/helper/__init__.py` & `troubadix-24.5.1/troubadix/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/helper/helper.py` & `troubadix-24.5.1/troubadix/helper/helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/helper/linguistic_exception_handler.py` & `troubadix-24.5.1/troubadix/helper/linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/helper/patterns.py` & `troubadix-24.5.1/troubadix/helper/patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugin.py` & `troubadix-24.5.1/troubadix/plugin.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/__init__.py` & `troubadix-24.5.1/troubadix/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/badwords.py` & `troubadix-24.5.1/troubadix/plugins/badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/copyright_text.py` & `troubadix-24.5.1/troubadix/plugins/copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/copyright_year.py` & `troubadix-24.5.1/troubadix/plugins/copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/creation_date.py` & `troubadix-24.5.1/troubadix/plugins/creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/cve_format.py` & `troubadix-24.5.1/troubadix/plugins/cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/cvss_format.py` & `troubadix-24.5.1/troubadix/plugins/cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/dependencies.py` & `troubadix-24.5.1/troubadix/plugins/dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/dependency_category_order.py` & `troubadix-24.5.1/troubadix/plugins/dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/deprecated_dependency.py` & `troubadix-24.5.1/troubadix/plugins/deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/deprecated_functions.py` & `troubadix-24.5.1/troubadix/plugins/deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/double_end_points.py` & `troubadix-24.5.1/troubadix/plugins/double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/duplicate_oid.py` & `troubadix-24.5.1/troubadix/plugins/duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/duplicated_script_tags.py` & `troubadix-24.5.1/troubadix/plugins/duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/encoding.py` & `troubadix-24.5.1/troubadix/plugins/encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/forking_nasl_functions.py` & `troubadix-24.5.1/troubadix/plugins/forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/get_kb_on_services.py` & `troubadix-24.5.1/troubadix/plugins/get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/grammar.py` & `troubadix-24.5.1/troubadix/plugins/grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/http_links_in_tags.py` & `troubadix-24.5.1/troubadix/plugins/http_links_in_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,12 +165,13 @@
             "http://internal-host$1 is still insecure",
             "http:// ",
             "https:// ",
             "such as 'http://:80'",
             "<http://localhost/moodle/admin/>",
             "https://username:password@proxy:8080",
             "sun.net.www.http.KeepAliveCache",
+            "www.foo.com",
         ]
 
         return any(
             exclusion in http_link_match_group for exclusion in exclusions
         )
```

### Comparing `troubadix-24.5.0/troubadix/plugins/illegal_characters.py` & `troubadix-24.5.1/troubadix/plugins/illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/log_messages.py` & `troubadix-24.5.1/troubadix/plugins/log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/malformed_dependencies.py` & `troubadix-24.5.1/troubadix/plugins/malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/misplaced_compare_in_if.py` & `troubadix-24.5.1/troubadix/plugins/misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/missing_desc_exit.py` & `troubadix-24.5.1/troubadix/plugins/missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/missing_tag_solution.py` & `troubadix-24.5.1/troubadix/plugins/missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/newlines.py` & `troubadix-24.5.1/troubadix/plugins/newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/overlong_description_lines.py` & `troubadix-24.5.1/troubadix/plugins/overlong_description_lines.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/overlong_script_tags.py` & `troubadix-24.5.1/troubadix/plugins/overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/prod_svc_detect_in_vulnvt.py` & `troubadix-24.5.1/troubadix/plugins/prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/qod.py` & `troubadix-24.5.1/troubadix/plugins/qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/reporting_consistency.py` & `troubadix-24.5.1/troubadix/plugins/reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_add_preference_type.py` & `troubadix-24.5.1/troubadix/plugins/script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_calls_empty_values.py` & `troubadix-24.5.1/troubadix/plugins/script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_calls_recommended.py` & `troubadix-24.5.1/troubadix/plugins/script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_category.py` & `troubadix-24.5.1/troubadix/plugins/script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_copyright.py` & `troubadix-24.5.1/troubadix/plugins/script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_family.py` & `troubadix-24.5.1/troubadix/plugins/script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_tag_form.py` & `troubadix-24.5.1/troubadix/plugins/script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_tag_whitespaces.py` & `troubadix-24.5.1/troubadix/plugins/script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_tags_mandatory.py` & `troubadix-24.5.1/troubadix/plugins/script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_version_and_last_modification_tags.py` & `troubadix-24.5.1/troubadix/plugins/script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_xref_form.py` & `troubadix-24.5.1/troubadix/plugins/script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/script_xref_url.py` & `troubadix-24.5.1/troubadix/plugins/script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/security_messages.py` & `troubadix-24.5.1/troubadix/plugins/security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/set_get_kb_calls.py` & `troubadix-24.5.1/troubadix/plugins/set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/solution_text.py` & `troubadix-24.5.1/troubadix/plugins/solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/solution_type.py` & `troubadix-24.5.1/troubadix/plugins/solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/spaces_in_filename.py` & `troubadix-24.5.1/troubadix/plugins/spaces_in_filename.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/spelling.py` & `troubadix-24.5.1/troubadix/plugins/spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/tabs.py` & `troubadix-24.5.1/troubadix/plugins/tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/todo_tbd.py` & `troubadix-24.5.1/troubadix/plugins/todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/trailing_spaces_tabs.py` & `troubadix-24.5.1/troubadix/plugins/trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/using_display.py` & `troubadix-24.5.1/troubadix/plugins/using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/valid_oid.py` & `troubadix-24.5.1/troubadix/plugins/valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/valid_script_tag_names.py` & `troubadix-24.5.1/troubadix/plugins/valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/variable_assigned_in_if.py` & `troubadix-24.5.1/troubadix/plugins/variable_assigned_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/vt_file_permissions.py` & `troubadix-24.5.1/troubadix/plugins/vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/plugins/vt_placement.py` & `troubadix-24.5.1/troubadix/plugins/vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/reporter.py` & `troubadix-24.5.1/troubadix/reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/results.py` & `troubadix-24.5.1/troubadix/results.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/runner.py` & `troubadix-24.5.1/troubadix/runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/allowed_rev_diff.py` & `troubadix-24.5.1/troubadix/standalone_plugins/allowed_rev_diff.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/changed_cves.py` & `troubadix-24.5.1/troubadix/standalone_plugins/changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/changed_oid.py` & `troubadix-24.5.1/troubadix/standalone_plugins/changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/changed_packages.py` & `troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/__init__.py` & `troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py` & `troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/added_release.py` & `troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py` & `troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/changed_update.py` & `troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py` & `troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/marker/marker.py` & `troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/marker/marker.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/changed_packages/package.py` & `troubadix-24.5.1/troubadix/standalone_plugins/changed_packages/package.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/common.py` & `troubadix-24.5.1/troubadix/standalone_plugins/common.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/file_extensions.py` & `troubadix-24.5.1/troubadix/standalone_plugins/file_extensions.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/last_modification.py` & `troubadix-24.5.1/troubadix/standalone_plugins/last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/no_solution.py` & `troubadix-24.5.1/troubadix/standalone_plugins/no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/standalone_plugins/version_updated.py` & `troubadix-24.5.1/troubadix/standalone_plugins/version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/troubadix/troubadix.py` & `troubadix-24.5.1/troubadix/troubadix.py`

 * *Files identical despite different names*

### Comparing `troubadix-24.5.0/PKG-INFO` & `troubadix-24.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troubadix
-Version: 24.5.0
+Version: 24.5.1
 Summary: A linting and QA check tool for NASL files
 Home-page: https://github.com/greenbone/troubadix
 License: GPL-3.0-or-later
 Author: Greenbone
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

