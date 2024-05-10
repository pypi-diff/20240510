# Comparing `tmp/heat-tempest-plugin-2.1.0.tar.gz` & `tmp/heat-tempest-plugin-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heat-tempest-plugin-2.1.0.tar", last modified: Mon Feb 19 07:23:19 2024, max compression
+gzip compressed data, was "heat-tempest-plugin-2.2.0.tar", last modified: Fri May 10 13:45:24 2024, max compression
```

## Comparing `heat-tempest-plugin-2.1.0.tar` & `heat-tempest-plugin-2.2.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.958876 heat-tempest-plugin-2.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3186 2024-02-19 07:23:19.000000 heat-tempest-plugin-2.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21814 2024-02-19 07:23:19.000000 heat-tempest-plugin-2.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1879 2024-02-19 07:23:19.962876 heat-tempest-plugin-2.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.938878 heat-tempest-plugin-2.1.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.938878 heat-tempest-plugin-2.1.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.942878 heat-tempest-plugin-2.1.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2025 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/doc/source/contributor/contributing.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.942878 heat-tempest-plugin-2.1.0/heat_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.946878 heat-tempest-plugin-2.1.0/heat_tempest_plugin/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7881 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/common/remote_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31827 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/common/test.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8463 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2706 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.946878 heat-tempest-plugin-2.1.0/heat_tempest_plugin/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6941 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/services/clients.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.946878 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.946878 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.950877 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1431 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/environments.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2483 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/resources.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/resourcetypes.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2358 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/softwareconfig.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4032 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/stacks.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1127 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/templates.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4628 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/test_heat_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.954877 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1311 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/functional_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3702 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5945 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12004 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_trunk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2174 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_encrypted_parameter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3785 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_encryption_vol_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3444 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_event_sinks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3792 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_external_ref.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4545 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_extra_route_set.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13606 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15732 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_nova_server_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4110 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_os_wait_condition.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8506 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_preview.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8460 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_remote_stack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_resources_list.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10031 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_software_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4642 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_stack_events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5693 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_stack_outputs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_stack_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13232 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_template_validate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2365 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_templates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5026 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_unicode_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2921 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_waitcondition.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.958876 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2939 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/scenario_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.958876 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/app_server_neutron.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/boot_config_none_env.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/id_ed25519.pub
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/netcat-webapp.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/octavia_lbaas.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_base.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_intermediate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_root.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_aodh_alarm.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_base_resources.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2751 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_server_cfn_init.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2865 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_server_signal.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3968 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_server_software_config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3502 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_volumes_create_from_backup.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3633 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_volumes_delete_snapshot.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_aodh_alarm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3004 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_base_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4419 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_octavia_lbaas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_remote_deeply_nested.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5298 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_server_cfn_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4185 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_server_signal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6540 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_server_software_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6013 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_volumes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.946878 heat-tempest-plugin-2.1.0/heat_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1879 2024-02-19 07:23:19.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4558 2024-02-19 07:23:19.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-19 07:23:19.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2024-02-19 07:23:19.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-19 07:23:19.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-02-19 07:23:19.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2024-02-19 07:23:19.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2024-02-19 07:23:19.000000 heat-tempest-plugin-2.1.0/heat_tempest_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.938878 heat-tempest-plugin-2.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-19 07:23:19.958876 heat-tempest-plugin-2.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/releasenotes/notes/honor-service_available-heat-03755bb4b092e753.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/releasenotes/notes/support-check-uuid-aa577427e4d32e4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      969 2024-02-19 07:23:19.962876 heat-tempest-plugin-2.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2024-02-19 07:22:49.000000 heat-tempest-plugin-2.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.609080 heat-tempest-plugin-2.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3186 2024-05-10 13:45:24.000000 heat-tempest-plugin-2.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21991 2024-05-10 13:45:24.000000 heat-tempest-plugin-2.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1879 2024-05-10 13:45:24.609080 heat-tempest-plugin-2.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.593080 heat-tempest-plugin-2.2.0/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.593080 heat-tempest-plugin-2.2.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.597080 heat-tempest-plugin-2.2.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2025 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/doc/source/contributor/contributing.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.597080 heat-tempest-plugin-2.2.0/heat_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.597080 heat-tempest-plugin-2.2.0/heat_tempest_plugin/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7881 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/common/remote_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31827 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/common/test.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8463 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2706 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.601080 heat-tempest-plugin-2.2.0/heat_tempest_plugin/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6941 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/services/clients.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.601080 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.601080 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.601080 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1431 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/environments.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2483 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/resources.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/resourcetypes.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2358 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/softwareconfig.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4032 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/stacks.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1127 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/templates.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4628 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/test_heat_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.605080 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1311 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/functional_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3702 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5945 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12004 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_trunk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2174 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_encrypted_parameter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3785 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_encryption_vol_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3444 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_event_sinks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3792 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_external_ref.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4545 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_extra_route_set.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13606 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15732 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_nova_server_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4110 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_os_wait_condition.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8506 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_preview.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8460 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_remote_stack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_resources_list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10031 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_software_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4642 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_stack_events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5693 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_stack_outputs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_stack_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13232 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_template_validate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2365 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_templates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5026 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_unicode_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2921 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_waitcondition.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.605080 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2939 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/scenario_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.609080 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/app_server_neutron.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/boot_config_none_env.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/id_ed25519.pub
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/netcat-webapp.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/octavia_lbaas.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_base.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_intermediate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_root.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_aodh_alarm.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_base_resources.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2751 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_server_cfn_init.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2888 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_server_signal.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3968 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_server_software_config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3501 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_volumes_create_from_backup.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3632 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_volumes_delete_snapshot.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_aodh_alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3004 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_base_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4419 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_octavia_lbaas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_remote_deeply_nested.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5298 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_server_cfn_init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4185 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_server_signal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6540 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_server_software_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6013 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_volumes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.597080 heat-tempest-plugin-2.2.0/heat_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1879 2024-05-10 13:45:24.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4558 2024-05-10 13:45:24.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-10 13:45:24.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2024-05-10 13:45:24.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-10 13:45:24.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-05-10 13:45:24.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2024-05-10 13:45:24.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2024-05-10 13:45:24.000000 heat-tempest-plugin-2.2.0/heat_tempest_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.593080 heat-tempest-plugin-2.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:45:24.609080 heat-tempest-plugin-2.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/releasenotes/notes/honor-service_available-heat-03755bb4b092e753.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/releasenotes/notes/support-check-uuid-aa577427e4d32e4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      969 2024-05-10 13:45:24.609080 heat-tempest-plugin-2.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2024-05-10 13:44:50.000000 heat-tempest-plugin-2.2.0/tox.ini
```

### Comparing `heat-tempest-plugin-2.1.0/.zuul.yaml` & `heat-tempest-plugin-2.2.0/.zuul.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 - job:
+    name: heat-functional-2024-1
+    parent: heat-functional
+    nodeset: openstack-single-node-jammy
+    override-checkout: stable/2024.1
+
+- job:
     name: heat-functional-2023-2
     parent: heat-functional
     nodeset: openstack-single-node-jammy
     override-checkout: stable/2023.2
 
 - job:
     name: heat-functional-2023-1
     parent: heat-functional
     nodeset: openstack-single-node-jammy
     override-checkout: stable/2023.1
 
-- job:
-    name: heat-functional-zed
-    parent: heat-functional
-    nodeset: openstack-single-node-focal
-    override-checkout: stable/zed
-
 - project:
     queue: heat
     templates:
       - check-requirements
       - tempest-plugin-jobs
     check:
       jobs:
         - heat-functional
         - heat-functional-legacy
+        - heat-functional-2024-1
         - heat-functional-2023-2
         - heat-functional-2023-1
-        - heat-functional-zed
     gate:
       jobs:
         - heat-functional
         - heat-functional-legacy
```

### Comparing `heat-tempest-plugin-2.1.0/AUTHORS` & `heat-tempest-plugin-2.2.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/CONTRIBUTING.rst` & `heat-tempest-plugin-2.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/ChangeLog` & `heat-tempest-plugin-2.2.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+2.2.0
+-----
+
+* Remove old excludes
+* Remove stable/zed job
+* Add 2024.1 job
+* Use native heat's WaitCondition in volume tests
+* Depend on corresponding server in WaitCondition
+
 2.1.0
 -----
 
 * Bump hacking
 * Update stable branch jobs
 * Remove unnecessary setup\_hook
 * Remove note about old pip's behavior
```

### Comparing `heat-tempest-plugin-2.1.0/LICENSE` & `heat-tempest-plugin-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/PKG-INFO` & `heat-tempest-plugin-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: heat-tempest-plugin
-Version: 2.1.0
+Version: 2.2.0
 Summary: OpenStack Orchestration Tempest Plugin
 Home-page: http://docs.openstack.org/developer/heat-tempest-plugin
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===================
         Heat Tempest Plugin
```

### Comparing `heat-tempest-plugin-2.1.0/README.rst` & `heat-tempest-plugin-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/doc/source/contributor/contributing.rst` & `heat-tempest-plugin-2.2.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/common/exceptions.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/common/remote_client.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/common/remote_client.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/common/test.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/common/test.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/config.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/plugin.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/services/clients.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/services/clients.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/fixtures.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/fixtures.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/environments.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/environments.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/resources.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/resources.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/resourcetypes.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/resourcetypes.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/softwareconfig.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/softwareconfig.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/stacks.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/stacks.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/gabbits/templates.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/gabbits/templates.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/api/test_heat_api.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/api/test_heat_api.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/functional_base.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/functional_base.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_port.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_port.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_subnet.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_subnet.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_trunk.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_create_update_neutron_trunk.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_encrypted_parameter.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_encrypted_parameter.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_encryption_vol_type.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_encryption_vol_type.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_event_sinks.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_event_sinks.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_external_ref.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_external_ref.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_extra_route_set.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_extra_route_set.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_hooks.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_hooks.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_nova_server_networks.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_nova_server_networks.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_os_wait_condition.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_os_wait_condition.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_preview.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_preview.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_remote_stack.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_remote_stack.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_resources_list.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_resources_list.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_software_config.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_software_config.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_stack_events.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_stack_events.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_stack_outputs.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_stack_outputs.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_stack_tags.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_stack_tags.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_template_validate.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_template_validate.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_templates.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_templates.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_unicode_template.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_unicode_template.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/functional/test_waitcondition.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/functional/test_waitcondition.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/scenario_base.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/scenario_base.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/app_server_neutron.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/app_server_neutron.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/netcat-webapp.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/netcat-webapp.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/octavia_lbaas.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/octavia_lbaas.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_base.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_base.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_intermediate.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_intermediate.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_root.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/remote_nested_root.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_aodh_alarm.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_aodh_alarm.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_base_resources.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_base_resources.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_server_cfn_init.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_server_cfn_init.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_server_signal.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_server_signal.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -104,14 +104,15 @@
     type: OS::Neutron::FloatingIPAssociation
     properties:
       floatingip_id: {get_resource: floating_ip}
       port_id: {get_attr: [server, addresses, {get_resource: network}, 0, port]}
 
   wait_condition:
     type: OS::Heat::WaitCondition
+    depends_on: server
     properties:
       handle: {get_resource: wait_handle}
       timeout: {get_param: timeout}
 
 outputs:
   server_ip:
     value: {get_attr: [floating_ip, floating_ip_address]}
```

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_server_software_config.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_server_software_config.yaml`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_volumes_create_from_backup.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_volumes_delete_snapshot.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -18,42 +18,49 @@
     description: Stack creation timeout
 
   dev_name:
     type: string
     description: Expected device name for volume
     default: vdb
 
+  test_string:
+    type: string
+    description: Test string which is written to volume
+    default: ateststring
+
   rescan_timeout:
     type: number
     description: Max number of seconds to wait for volume after rescan
     default: 120
 
-  backup_id:
-    type: string
-    description: backup_id to create volume from
-
   network:
     type: string
 
   volume_description:
     type: string
     description: Description of volume
     default: A volume description
 
+  volume_size:
+    type: number
+    description: Size of volume
+    default: 1
+
   wc_extra_args:
     type: string
     description: extra options to add to CURL command
     default: ""
 
 resources:
   volume:
+    deletion_policy: 'Snapshot'
     type: OS::Cinder::Volume
     properties:
-      backup_id: { get_param: backup_id }
-      description: { get_param: volume_description }
+      size: {get_param: volume_size}
+      description: {get_param: volume_description}
 
   volume_attachment:
     type: OS::Cinder::VolumeAttachment
     properties:
       volume_id: { get_resource: volume }
       instance_uuid: { get_resource: instance }
 
@@ -76,35 +83,38 @@
             for i in $(seq 1 rescan_timeout)
             do
               grep -q dev_name /proc/partitions && break
               sleep 1
             done
             if grep -q dev_name /proc/partitions
             then
+              mkfs.ext4 /dev/dev_name
               mount /dev/dev_name /mnt
-              TESTDATA=$(cat /mnt/testfile)
-              curl wc_extra_args -X PUT -H 'Content-Type:' --data-binary '{"Status": "SUCCESS", "Reason": "Test Complete", "Data": "Volume Data:'$TESTDATA'", "UniqueId": "instance1"}' "wc_url"
+              echo "test_string" > /mnt/testfile
+              umount /mnt
+              curl wc_extra_args -X PUT -H 'Content-Type:' --data-binary '{"Status": "SUCCESS", "Reason": "Test Complete", "Data": "Completed volume configuration.", "UniqueId": "instance1"}' "wc_url"
             else
               curl wc_extra_args -X PUT -H 'Content-Type:' --data-binary '{"Status": "FAILURE", "Reason": "Test Failed", "Data": "Expected device dev_name not found.", "UniqueId": "instance1"}' "wc_url"
             fi
           params:
             wc_url: { get_resource: wait_handle }
             dev_name: { get_param: dev_name }
             rescan_timeout: { get_param: rescan_timeout }
+            test_string: { get_param: test_string }
             wc_extra_args: { get_param: wc_extra_args }
 
   wait_handle:
     type: OS::Heat::UpdateWaitConditionHandle
 
   wait_condition:
-    type: AWS::CloudFormation::WaitCondition
+    type: OS::Heat::WaitCondition
+    depends_on: instance
     properties:
-      Count: 1
-      Handle: { get_resource: wait_handle }
-      Timeout: { get_param: timeout }
+      handle: { get_resource: wait_handle }
+      timeout: { get_param: timeout }
 
 
 outputs:
   status:
     description: status
     value: { get_attr: ['volume', 'status'] }
 
@@ -114,11 +124,7 @@
 
   display_description:
     description: display_description
     value: { get_attr: ['volume', 'display_description'] }
 
   volume_id:
     value: { get_resource: volume }
-
-  testfile_data:
-    description: Contents of /mnt/testfile from the mounted volume
-    value: { get_attr: ['wait_condition', 'Data'] }
```

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/templates/test_volumes_delete_snapshot.yaml` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/templates/test_volumes_create_from_backup.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -18,49 +18,42 @@
     description: Stack creation timeout
 
   dev_name:
     type: string
     description: Expected device name for volume
     default: vdb
 
-  test_string:
-    type: string
-    description: Test string which is written to volume
-    default: ateststring
-
   rescan_timeout:
     type: number
     description: Max number of seconds to wait for volume after rescan
     default: 120
 
+  backup_id:
+    type: string
+    description: backup_id to create volume from
+
   network:
     type: string
 
   volume_description:
     type: string
     description: Description of volume
     default: A volume description
 
-  volume_size:
-    type: number
-    description: Size of volume
-    default: 1
-
   wc_extra_args:
     type: string
     description: extra options to add to CURL command
     default: ""
 
 resources:
   volume:
-    deletion_policy: 'Snapshot'
     type: OS::Cinder::Volume
     properties:
-      size: {get_param: volume_size}
-      description: {get_param: volume_description}
+      backup_id: { get_param: backup_id }
+      description: { get_param: volume_description }
 
   volume_attachment:
     type: OS::Cinder::VolumeAttachment
     properties:
       volume_id: { get_resource: volume }
       instance_uuid: { get_resource: instance }
 
@@ -83,38 +76,35 @@
             for i in $(seq 1 rescan_timeout)
             do
               grep -q dev_name /proc/partitions && break
               sleep 1
             done
             if grep -q dev_name /proc/partitions
             then
-              mkfs.ext4 /dev/dev_name
               mount /dev/dev_name /mnt
-              echo "test_string" > /mnt/testfile
-              umount /mnt
-              curl wc_extra_args -X PUT -H 'Content-Type:' --data-binary '{"Status": "SUCCESS", "Reason": "Test Complete", "Data": "Completed volume configuration.", "UniqueId": "instance1"}' "wc_url"
+              TESTDATA=$(cat /mnt/testfile)
+              curl wc_extra_args -X PUT -H 'Content-Type:' --data-binary '{"Status": "SUCCESS", "Reason": "Test Complete", "Data": "Volume Data:'$TESTDATA'", "UniqueId": "instance1"}' "wc_url"
             else
               curl wc_extra_args -X PUT -H 'Content-Type:' --data-binary '{"Status": "FAILURE", "Reason": "Test Failed", "Data": "Expected device dev_name not found.", "UniqueId": "instance1"}' "wc_url"
             fi
           params:
             wc_url: { get_resource: wait_handle }
             dev_name: { get_param: dev_name }
             rescan_timeout: { get_param: rescan_timeout }
-            test_string: { get_param: test_string }
             wc_extra_args: { get_param: wc_extra_args }
 
   wait_handle:
     type: OS::Heat::UpdateWaitConditionHandle
 
   wait_condition:
-    type: AWS::CloudFormation::WaitCondition
+    type: OS::Heat::WaitCondition
+    depends_on: instance
     properties:
-      Count: 1
-      Handle: { get_resource: wait_handle }
-      Timeout: { get_param: timeout }
+      handle: { get_resource: wait_handle }
+      timeout: { get_param: timeout }
 
 
 outputs:
   status:
     description: status
     value: { get_attr: ['volume', 'status'] }
 
@@ -124,7 +114,11 @@
 
   display_description:
     description: display_description
     value: { get_attr: ['volume', 'display_description'] }
 
   volume_id:
     value: { get_resource: volume }
+
+  testfile_data:
+    description: Contents of /mnt/testfile from the mounted volume
+    value: { get_attr: ['wait_condition', 'data'] }
```

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_aodh_alarm.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_aodh_alarm.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_base_resources.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_base_resources.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_octavia_lbaas.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_octavia_lbaas.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_remote_deeply_nested.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_remote_deeply_nested.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_server_cfn_init.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_server_cfn_init.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_server_signal.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_server_signal.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_server_software_config.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_server_software_config.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin/tests/scenario/test_volumes.py` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin/tests/scenario/test_volumes.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin.egg-info/PKG-INFO` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: heat-tempest-plugin
-Version: 2.1.0
+Version: 2.2.0
 Summary: OpenStack Orchestration Tempest Plugin
 Home-page: http://docs.openstack.org/developer/heat-tempest-plugin
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===================
         Heat Tempest Plugin
```

### Comparing `heat-tempest-plugin-2.1.0/heat_tempest_plugin.egg-info/SOURCES.txt` & `heat-tempest-plugin-2.2.0/heat_tempest_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/requirements.txt` & `heat-tempest-plugin-2.2.0/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 python-novaclient>=9.1.0 # Apache-2.0
 python-swiftclient>=3.2.0 # Apache-2.0
 python-zaqarclient>=1.0.0 # Apache-2.0
 testtools>=2.2.0 # MIT
 testscenarios>=0.4 # Apache-2.0/BSD
 tempest>=17.1.0 # Apache-2.0
 gabbi>=1.42.1 # Apache-2.0
-kombu!=4.0.2,>=4.0.0 # BSD
+kombu>=4.0.0 # BSD
```

### Comparing `heat-tempest-plugin-2.1.0/setup.cfg` & `heat-tempest-plugin-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/setup.py` & `heat-tempest-plugin-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `heat-tempest-plugin-2.1.0/tox.ini` & `heat-tempest-plugin-2.2.0/tox.ini`

 * *Files identical despite different names*

