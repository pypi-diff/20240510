# Comparing `tmp/neutron-tempest-plugin-2.7.0.tar.gz` & `tmp/neutron-tempest-plugin-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutron-tempest-plugin-2.7.0.tar", last modified: Wed Mar 20 14:16:16 2024, max compression
+gzip compressed data, was "neutron-tempest-plugin-2.8.0.tar", last modified: Fri May 10 13:40:16 2024, max compression
```

## Comparing `neutron-tempest-plugin-2.7.0.tar` & `neutron-tempest-plugin-2.8.0.tar`

### file list

```diff
@@ -1,310 +1,311 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.692143 neutron-tempest-plugin-2.7.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7317 2024-03-20 14:16:16.000000 neutron-tempest-plugin-2.7.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46666 2024-03-20 14:16:16.000000 neutron-tempest-plugin-2.7.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2024-03-20 14:16:16.692143 neutron-tempest-plugin-2.7.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.636110 neutron-tempest-plugin-2.7.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5198 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/devstack/customize_image.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3019 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/devstack/functions.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.636110 neutron-tempest-plugin-2.7.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.640113 neutron-tempest-plugin-2.7.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2849 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/doc/source/test_descriptions.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.640113 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.652120 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.656122 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2190 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_agent_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4585 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_agent_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12566 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_default_security_group_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_extension_driver_port_security_admin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12255 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_external_network_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3418 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_floating_ips_admin_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3597 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_l3_agent_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4200 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2429 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_logging_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11860 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_network_segment_range.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4195 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11964 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_ports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7054 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_quotas_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4891 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_routers_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5715 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_routers_ha.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21580 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_shared_network_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16723 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_tag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    65319 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/base_routers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/base_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6437 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13909 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_address_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11752 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_address_scopes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_address_scopes_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5296 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_auto_allocated_topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6072 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_conntrack_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6679 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_extension_driver_port_security.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2235 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6897 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_flavors_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7691 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_floating_ips.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2546 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_floating_ips_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5852 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_local_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7288 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_metering_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_metering_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4923 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_ndp_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6210 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_ndp_proxy_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8565 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_network_ip_availability.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_network_ip_availability_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9210 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_networks_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4848 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_port_forwarding_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10876 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_port_forwardings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13699 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_ports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_ports_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77683 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_qos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11965 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_qos_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20655 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_revisions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4949 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_router_interface_fip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24463 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_routers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7582 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_routers_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32815 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10499 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_security_groups_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_service_type_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3840 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_subnetpool_prefix_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26629 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_subnetpools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14769 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_subnetpools_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4536 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16121 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_timestamp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15376 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_trunk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2760 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_trunk_details.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13558 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_trunk_negative.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.660124 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.660124 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17305 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/api/test_bgpvpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3553 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.660124 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6126 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/scenario/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    63992 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/scenario/test_bgpvpn_basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.660124 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4809 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/services/bgpvpn_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.660124 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6862 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16929 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6607 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11868 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/ssh.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/tempest_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8568 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12114 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3170 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.660124 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.664127 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/api/fwaas_v2_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14899 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/api/test_fwaasv2_extensions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.664127 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7110 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/common/fwaas_v2_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.664127 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2988 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13063 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/scenario/test_fwaas_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.664127 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4681 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/services/v2_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.664127 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.664127 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14711 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6503 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions_negative.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.668129 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15516 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6982 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base_test_proto.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.668129 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4429 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5680 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_4byte_asn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5621 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.668129 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5582 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/test_ipv4.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.668129 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5728 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/test_ipv6.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9086 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/test_simple_bgp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.676133 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.676133 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/admin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4835 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/admin/test_floatingip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29989 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1176 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2007 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10627 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_connectivity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8028 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_dhcp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14174 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_dns_integration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2641 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_dvr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3688 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_fip64.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26818 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_floatingip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8439 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_internal_dns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10763 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_ipv6.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4109 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_local_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8384 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_mac_learning.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6518 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10388 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12304 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_mtu.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15576 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_multicast.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13020 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_port_forwardings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4891 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_ports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3097 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_portsecurity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17605 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_qos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    55583 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21344 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_trunk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8153 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_vlan_transparency.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.676133 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.676133 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/bgp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/bgp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6738 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/bgp/bgp_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.676133 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/network/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.676133 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/network/json/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/network/json/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52349 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/network/json/network_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.676133 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.676133 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/services/flowclassifier_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5309 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/services/sfc_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.680136 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.680136 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8011 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/api/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3355 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/api/test_flowclassifier_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16294 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/api/test_sfc_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/flowclassifier_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.680136 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2922 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/scenario/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3806 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/scenario/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50981 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/scenario/test_sfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3536 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/sfc_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.680136 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.680136 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5759 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/api/test_taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3391 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.680136 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11849 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/scenario/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10535 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11086 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_traffic_impact.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.684138 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/services/taas_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.684138 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.684138 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6368 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/api/base_vpnaas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42150 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/api/test_vpnaas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.684138 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/scenario/base_vpnaas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12623 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/scenario/test_vpnaas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.684138 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2452 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/services/clients_vpnaas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.640113 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2024-03-20 14:16:16.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11715 2024-03-20 14:16:16.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-20 14:16:16.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-03-20 14:16:16.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-20 14:16:16.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-20 14:16:16.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-03-20 14:16:16.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2024-03-20 14:16:16.000000 neutron-tempest-plugin-2.7.0/neutron_tempest_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.684138 neutron-tempest-plugin-2.7.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/playbooks/dvr-multinode-scenario-pre-run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/playbooks/dynamic-routing-pre-run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/playbooks/linuxbridge-scenario-pre-run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.632108 neutron-tempest-plugin-2.7.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.688140 neutron-tempest-plugin-2.7.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/releasenotes/notes/agents-client-delete-method-de1a7fb3f845999c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/releasenotes/notes/drop-py-2-7-74b8379cab4cdc5a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/releasenotes/notes/igmp-snooping-8d6d85608df8880a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/releasenotes/notes/mark-methods-removals-f8b230171c045a3e.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.688140 neutron-tempest-plugin-2.7.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/releasenotes/source/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.688140 neutron-tempest-plugin-2.7.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.688140 neutron-tempest-plugin-2.7.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8695 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.632108 neutron-tempest-plugin-2.7.0/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.632108 neutron-tempest-plugin-2.7.0/roles/docker-setup/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.688140 neutron-tempest-plugin-2.7.0/roles/docker-setup/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/roles/docker-setup/files/52_docker_for_tempest
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/roles/docker-setup/files/docker_apparmor
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.688140 neutron-tempest-plugin-2.7.0/roles/docker-setup/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/roles/docker-setup/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.688140 neutron-tempest-plugin-2.7.0/roles/multi-node-setup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/roles/multi-node-setup/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.688140 neutron-tempest-plugin-2.7.0/roles/multi-node-setup/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/roles/multi-node-setup/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.688140 neutron-tempest-plugin-2.7.0/roles/multi-node-setup/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/roles/multi-node-setup/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2024-03-20 14:16:16.692143 neutron-tempest-plugin-2.7.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.688140 neutron-tempest-plugin-2.7.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5745 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/tools/customize_ubuntu_image
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1283 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/tools/misc-sanity-checks.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2321 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-20 14:16:16.692143 neutron-tempest-plugin-2.7.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10820 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/zuul.d/2023_1_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10737 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/zuul.d/2023_2_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/zuul.d/base-nested-switch.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53488 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/zuul.d/master_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7762 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11923 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/zuul.d/victoria_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8766 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/zuul.d/wallaby_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8887 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/zuul.d/xena_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9537 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/zuul.d/yoga_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10227 2024-03-20 14:15:50.000000 neutron-tempest-plugin-2.7.0/zuul.d/zed_jobs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.954103 neutron-tempest-plugin-2.8.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7361 2024-05-10 13:40:16.000000 neutron-tempest-plugin-2.8.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46964 2024-05-10 13:40:16.000000 neutron-tempest-plugin-2.8.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2024-05-10 13:40:16.954103 neutron-tempest-plugin-2.8.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.918106 neutron-tempest-plugin-2.8.0/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5198 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/devstack/customize_image.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3019 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/devstack/functions.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.922106 neutron-tempest-plugin-2.8.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.922106 neutron-tempest-plugin-2.8.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2849 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/doc/source/test_descriptions.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.922106 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.930105 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.934105 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2190 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_agent_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4585 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_agent_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12566 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_default_security_group_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_extension_driver_port_security_admin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12255 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_external_network_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3418 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_floating_ips_admin_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3597 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_l3_agent_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4200 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2429 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_logging_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11860 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_network_segment_range.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4195 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11964 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_ports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7054 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_quotas_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4891 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_routers_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5715 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_routers_ha.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21580 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_shared_network_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16723 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_tag.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    65318 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/base_routers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/base_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6437 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13909 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_address_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11752 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_address_scopes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_address_scopes_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5296 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_auto_allocated_topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6072 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_conntrack_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6679 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_extension_driver_port_security.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2235 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6897 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_flavors_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7691 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_floating_ips.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2546 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_floating_ips_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5852 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_local_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7288 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_metering_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_metering_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4923 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_ndp_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6210 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_ndp_proxy_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8565 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_network_ip_availability.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_network_ip_availability_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9210 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_networks_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4848 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_port_forwarding_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10876 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_port_forwardings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13699 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_ports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_ports_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77683 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_qos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11965 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_qos_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20655 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_revisions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4949 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_router_interface_fip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33626 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_routers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7582 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_routers_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32815 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10499 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_security_groups_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_service_type_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3840 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_subnetpool_prefix_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26629 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_subnetpools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14769 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_subnetpools_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4712 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16121 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_timestamp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15376 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_trunk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2760 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_trunk_details.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13558 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_trunk_negative.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.934105 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.934105 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17305 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/api/test_bgpvpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3553 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.934105 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6126 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/scenario/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    63992 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/scenario/test_bgpvpn_basic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.934105 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4809 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/services/bgpvpn_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.934105 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6862 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16929 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6607 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11868 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/ssh.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/tempest_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8568 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12114 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3170 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.934105 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.938104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/api/fwaas_v2_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14899 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/api/test_fwaasv2_extensions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.938104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7110 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/common/fwaas_v2_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.938104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2988 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13063 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/scenario/test_fwaas_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.938104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4681 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/services/v2_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.938104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.938104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14711 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6503 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions_negative.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.938104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15516 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6982 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base_test_proto.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.938104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4429 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5680 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_4byte_asn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5621 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_basic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.938104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5582 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/test_ipv4.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.938104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5728 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/test_ipv6.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9086 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/test_simple_bgp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.942104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/admin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4835 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/admin/test_floatingip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29989 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1176 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2007 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10627 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_connectivity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8028 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_dhcp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14174 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_dns_integration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2641 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_dvr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3688 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_fip64.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27017 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_floatingip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8439 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_internal_dns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10763 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_ipv6.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4109 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_local_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8384 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_mac_learning.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6518 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10388 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12304 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_mtu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15576 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_multicast.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13020 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_port_forwardings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4891 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_ports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3097 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_portsecurity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17605 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_qos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55583 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21344 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_trunk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8153 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_vlan_transparency.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/bgp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/bgp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6738 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/bgp/bgp_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/network/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/network/json/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/network/json/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    54473 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/network/json/network_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/services/flowclassifier_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5309 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/services/sfc_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8011 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/api/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3355 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/api/test_flowclassifier_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16294 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/api/test_sfc_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/flowclassifier_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2922 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/scenario/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3806 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/scenario/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50981 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/scenario/test_sfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3536 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/sfc_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.946104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5759 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/api/test_taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3391 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.950104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11849 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/scenario/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10535 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11086 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_traffic_impact.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.950104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/services/taas_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.950104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.950104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6368 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/api/base_vpnaas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42150 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/api/test_vpnaas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.950104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/scenario/base_vpnaas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12623 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/scenario/test_vpnaas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.950104 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2452 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/services/clients_vpnaas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.922106 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2024-05-10 13:40:16.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11739 2024-05-10 13:40:16.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-10 13:40:16.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-05-10 13:40:16.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-10 13:40:16.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-05-10 13:40:16.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-05-10 13:40:16.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2024-05-10 13:40:16.000000 neutron-tempest-plugin-2.8.0/neutron_tempest_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.950104 neutron-tempest-plugin-2.8.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/playbooks/dvr-multinode-scenario-pre-run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/playbooks/dynamic-routing-pre-run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/playbooks/linuxbridge-scenario-pre-run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.918106 neutron-tempest-plugin-2.8.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.950104 neutron-tempest-plugin-2.8.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/releasenotes/notes/agents-client-delete-method-de1a7fb3f845999c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/releasenotes/notes/drop-py-2-7-74b8379cab4cdc5a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/releasenotes/notes/igmp-snooping-8d6d85608df8880a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/releasenotes/notes/mark-methods-removals-f8b230171c045a3e.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.950104 neutron-tempest-plugin-2.8.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/releasenotes/source/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.950104 neutron-tempest-plugin-2.8.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.950104 neutron-tempest-plugin-2.8.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8695 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.918106 neutron-tempest-plugin-2.8.0/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.918106 neutron-tempest-plugin-2.8.0/roles/docker-setup/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.954103 neutron-tempest-plugin-2.8.0/roles/docker-setup/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/roles/docker-setup/files/52_docker_for_tempest
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/roles/docker-setup/files/docker_apparmor
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.954103 neutron-tempest-plugin-2.8.0/roles/docker-setup/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/roles/docker-setup/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.954103 neutron-tempest-plugin-2.8.0/roles/multi-node-setup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/roles/multi-node-setup/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.954103 neutron-tempest-plugin-2.8.0/roles/multi-node-setup/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/roles/multi-node-setup/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.954103 neutron-tempest-plugin-2.8.0/roles/multi-node-setup/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/roles/multi-node-setup/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2024-05-10 13:40:16.958103 neutron-tempest-plugin-2.8.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.954103 neutron-tempest-plugin-2.8.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5745 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/tools/customize_ubuntu_image
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1283 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/tools/misc-sanity-checks.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2321 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:40:16.954103 neutron-tempest-plugin-2.8.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10820 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/zuul.d/2023_1_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10737 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/zuul.d/2023_2_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10732 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/zuul.d/2024_1_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/zuul.d/base-nested-switch.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53626 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/zuul.d/master_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8780 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11989 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/zuul.d/victoria_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8766 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/zuul.d/wallaby_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8887 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/zuul.d/xena_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9537 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/zuul.d/yoga_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10227 2024-05-10 13:39:29.000000 neutron-tempest-plugin-2.8.0/zuul.d/zed_jobs.yaml
```

### Comparing `neutron-tempest-plugin-2.7.0/AUTHORS` & `neutron-tempest-plugin-2.8.0/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 Elod Illes <elod.illes@est.tech>
 Elvira García <egarciar@redhat.com>
 Eran Kuris <ekuris@redhat.com>
 Eugene Nikanorov <enikanorov@mirantis.com>
 Federico Ressi <fressi@redhat.com>
 Fiorella Yanac <fyanac@redhat.com>
 Flavio Fernandes <flaviof@redhat.com>
+Frode Nordahl <frode.nordahl@canonical.com>
 Gary Kotton <gkotton@vmware.com>
 Genadi Chereshnya <gcheresh@redhat.com>
 Ghanshyam <gmann@ghanshyammann.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Glenn Van de Water <glenn.van_de_water@nuagenetworks.net>
 Goutham Pratapa <lakshmi.pratapa@imaginea.com>
 Hang Yang <hangyang@verizonmedia.com>
```

### Comparing `neutron-tempest-plugin-2.7.0/ChangeLog` & `neutron-tempest-plugin-2.8.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 CHANGES
 =======
 
+2.8.0
+-----
+
+* Remove executable from python files which don't really needs it
+* Use unmaintained/ for Victoria
+* Add Active Active L3 GW API test cases
+* Add job definitions for 2024.1 (Caracal) branch
+
 2.7.0
 -----
 
 * [Stateless SG] Add test for port security and stateless SGs
+* Add extension "subnet-external-network"
 * Remove usage of testscenarios and replace it with ddt library
 * [OVN] Do not check L3 agents state with ML2/OVN
 * [OVN] Use the OVN agent in "neutron-tempest-plugin-ovn"
+* Check device\_owner with actual availability zone
 * Skip HA router tests when not meant for OVN driver
 * Add router check, subnet attached gateway IP update or deletion
 * Remove train and ussuri jobs
 * Replace usage of deprecated path for test decorators
 * Stop running yoga jobs in check/gate
 
 2.6.0
```

### Comparing `neutron-tempest-plugin-2.7.0/LICENSE` & `neutron-tempest-plugin-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/PKG-INFO` & `neutron-tempest-plugin-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-tempest-plugin
-Version: 2.7.0
+Version: 2.8.0
 Summary: Tempest plugin for Neutron Project
 Home-page: https://opendev.org/openstack/neutron-tempest-plugin
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ======================
         Neutron Tempest Plugin
```

### Comparing `neutron-tempest-plugin-2.7.0/devstack/README.rst` & `neutron-tempest-plugin-2.8.0/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/devstack/customize_image.sh` & `neutron-tempest-plugin-2.8.0/devstack/customize_image.sh`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/devstack/functions.sh` & `neutron-tempest-plugin-2.8.0/devstack/functions.sh`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/devstack/plugin.sh` & `neutron-tempest-plugin-2.8.0/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/doc/source/conf.py` & `neutron-tempest-plugin-2.8.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/doc/source/index.rst` & `neutron-tempest-plugin-2.8.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_agent_availability_zone.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_agent_availability_zone.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_agent_management.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_agent_management.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_default_security_group_rules.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_default_security_group_rules.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_extension_driver_port_security_admin.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_extension_driver_port_security_admin.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_external_network_extension.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_external_network_extension.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_floating_ips_admin_actions.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_floating_ips_admin_actions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_l3_agent_scheduler.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_l3_agent_scheduler.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_logging.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_logging.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_logging_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_logging_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_network_segment_range.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_network_segment_range.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_networks.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_networks.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_ports.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_ports.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_quotas.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_quotas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_quotas_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_quotas_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_routers_flavors.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_routers_flavors.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_routers_ha.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_routers_ha.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_security_groups.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_security_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_shared_network_extension.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_shared_network_extension.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/admin/test_tag.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/admin/test_tag.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/base.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,15 @@
             cls.admin_subnets.append(subnet)
         if reserve_cidr:
             cls.reserve_subnet_cidr(subnet_cidr)
         return subnet
 
     @classmethod
     def reserve_subnet_cidr(cls, addr, **ipnetwork_kwargs):
-        """Reserve given subnet CIDR making sure it is not used by create_subnet
+        """Reserve given subnet CIDR making sure it's not used by create_subnet
 
         :param addr: the CIDR address to be reserved
         It can be a str or netaddr.IPNetwork instance
 
         :param **ipnetwork_kwargs: optional netaddr.IPNetwork constructor
         parameters
         """
```

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/base_routers.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/base_routers.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
         try:
             self.delete_router(router, client)
             self.routers.remove(router)
         except exceptions.NotFound:
             pass
 
     def _create_router(self, name, admin_state_up=False,
-                       external_network_id=None, enable_snat=None):
+                       external_network_id=None, enable_snat=None, **kwargs):
         # associate a cleanup with created routers to avoid quota limits
         router = self.create_router(name, admin_state_up,
-                                    external_network_id, enable_snat)
+                                    external_network_id, enable_snat, **kwargs)
         self.addCleanup(self._cleanup_router, router)
         return router
 
     def _create_admin_router(self, *args, **kwargs):
         router = self.create_admin_router(*args, **kwargs)
         self.addCleanup(
             self._cleanup_router, router, self.os_admin.network_client)
```

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/base_security_groups.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/base_security_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/clients.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/clients.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_address_groups.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_address_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_address_scopes.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_address_scopes.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_address_scopes_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_address_scopes_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_auto_allocated_topology.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_auto_allocated_topology.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_availability_zones.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_conntrack_helper.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_conntrack_helper.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_extension_driver_port_security.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_extension_driver_port_security.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_extensions.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_flavors_extensions.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_flavors_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_floating_ips.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_floating_ips.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_floating_ips_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_floating_ips_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_local_ip.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_local_ip.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_metering_extensions.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_metering_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_metering_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_metering_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_ndp_proxy.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_ndp_proxy.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_ndp_proxy_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_ndp_proxy_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_network_ip_availability.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_network_ip_availability.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_network_ip_availability_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_network_ip_availability_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_networks.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_networks.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_networks_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_networks_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_port_forwarding_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_port_forwarding_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_port_forwardings.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_port_forwardings.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_ports.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_ports.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_ports_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_ports_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_qos.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_qos.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_qos_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_qos_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_revisions.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_revisions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_router_interface_fip.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_router_interface_fip.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_routers.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_routers.py`

 * *Files 25% similar despite different names*

```diff
@@ -322,14 +322,209 @@
 
         # The gateway deletion returns the same exception.
         gateway_ip = netaddr.IPAddress(subnet['gateway_ip'])
         self.assertRaises(lib_exc.Conflict, self.client.update_subnet,
                           subnet['id'], gateway_ip=None)
 
 
+class ExternalGWMultihomingRoutersTest(base_routers.BaseRouterTest):
+
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        ext_alias = 'external-gateway-multihoming'
+        try:
+            cls.client.get_extension(ext_alias)
+        except lib_exc.NotFound:
+            raise cls.skipException(f'{ext_alias} extension not available.')
+
+    @decorators.idempotent_id('33e9a156-a83f-435f-90ee-1a49dc9c350d')
+    def test_create_router_enable_default_route_ecmp(self):
+        router1 = self._create_admin_router(data_utils.rand_name('router1'),
+                                            enable_default_route_ecmp=True)
+        router2 = self._create_admin_router(data_utils.rand_name('router2'),
+                                            enable_default_route_ecmp=False)
+        self.assertEqual(router1['enable_default_route_ecmp'], True)
+        self.assertEqual(router2['enable_default_route_ecmp'], False)
+
+    @decorators.idempotent_id('bfbad985-2df2-4cd9-9c32-819b5508c40e')
+    def test_update_router_enable_default_route_ecmp(self):
+        router = self._create_router(data_utils.rand_name('router'))
+        updated_router = self.admin_client.update_router(
+            router['id'],
+            enable_default_route_ecmp=not router['enable_default_route_ecmp'])
+        self.assertNotEqual(
+            router['enable_default_route_ecmp'],
+            updated_router['router']['enable_default_route_ecmp'])
+
+    @decorators.idempotent_id('a22016a6-f118-4eb5-abab-7e241ae01848')
+    def test_update_router_enable_default_route_bfd(self):
+        router = self._create_router(data_utils.rand_name('router'))
+        updated_router = self.admin_client.update_router(
+            router['id'],
+            enable_default_route_bfd=not router['enable_default_route_bfd'])
+        self.assertNotEqual(
+            router['enable_default_route_bfd'],
+            updated_router['router']['enable_default_route_bfd'])
+
+    @decorators.idempotent_id('842f6edb-e072-4805-bf11-04c25420776d')
+    def test_create_router_enable_default_route_bfd(self):
+        router1 = self._create_admin_router(data_utils.rand_name('router1'),
+                                            enable_default_route_bfd=True)
+        router2 = self._create_admin_router(data_utils.rand_name('router2'),
+                                            enable_default_route_bfd=False)
+        self.assertEqual(router1['enable_default_route_bfd'], True)
+        self.assertEqual(router2['enable_default_route_bfd'], False)
+
+    @decorators.idempotent_id('089fa304-3726-4120-9759-668e8ff1114c')
+    def test_create_router_add_external_gateways_one(self):
+        router = self._create_router(data_utils.rand_name('router'))
+        self.assertEqual(len(router['external_gateways']), 0)
+
+        res = self.client.router_add_external_gateways(
+            router['id'],
+            [{'network_id': CONF.network.public_network_id,
+              'enable_snat': False}])
+        self.assertEqual(len(res['router']['external_gateways']), 1)
+        self.assertEqual(
+            res['router']['external_gateways'][0]['network_id'],
+            CONF.network.public_network_id)
+
+    @decorators.idempotent_id('60a1e7db-04ef-4a3a-9ff1-01a990d365fd')
+    def test_create_router_add_external_gateways(self):
+        router = self._create_router(data_utils.rand_name('router'))
+        self.assertEqual(len(router['external_gateways']), 0)
+
+        res = self.client.router_add_external_gateways(
+            router['id'],
+            [
+                {'network_id': CONF.network.public_network_id,
+                 'enable_snat': False},
+                {'network_id': CONF.network.public_network_id,
+                 'enable_snat': False},
+                {'network_id': CONF.network.public_network_id,
+                 'enable_snat': False},
+            ])
+        self.assertEqual(len(res['router']['external_gateways']), 3)
+        self.assertEqual(
+            res['router']['external_gateway_info']['network_id'],
+            res['router']['external_gateways'][0]['network_id'])
+        self.assertEqual(
+            res['router']['external_gateway_info']['external_fixed_ips'],
+            res['router']['external_gateways'][0]['external_fixed_ips'])
+        for n in range(0, 3):
+            self.assertEqual(
+                res['router']['external_gateways'][n]['network_id'],
+                CONF.network.public_network_id)
+            if n:
+                self.assertNotEqual(
+                    res['router']['external_gateways'][
+                        n]['external_fixed_ips'],
+                    res['router']['external_gateways'][
+                        n - 1]['external_fixed_ips'])
+
+    @decorators.idempotent_id('e49efc57-7b25-43a3-8e55-2d87a3759c57')
+    def test_create_router_add_external_gateways_compat(self):
+        router = self._create_router(
+            data_utils.rand_name('router'),
+            external_network_id=CONF.network.public_network_id,
+            enable_snat=False)
+        self.assertEqual(len(router['external_gateways']), 1)
+        res = self.client.router_add_external_gateways(
+            router['id'],
+            [{'network_id': CONF.network.public_network_id,
+              'enable_snat': False}])
+        self.assertEqual(len(res['router']['external_gateways']), 2)
+
+    @decorators.idempotent_id('2a238eec-d9d5-435a-9013-d6e195ecd5d1')
+    def test_create_router_remove_external_gateways_compat(self):
+        router = self._create_router(
+            data_utils.rand_name('router'),
+            external_network_id=CONF.network.public_network_id,
+            enable_snat=False)
+        self.assertEqual(len(router['external_gateways']), 1)
+        res = self.client.router_remove_external_gateways(
+            router['id'],
+            [{'network_id': CONF.network.public_network_id}])
+        self.assertEqual(len(res['router']['external_gateways']), 0)
+
+    @decorators.idempotent_id('03ab196a-dac0-4363-93e4-ea799246870b')
+    def test_create_router_add_remove_external_gateways(self):
+        router = self._create_router(data_utils.rand_name('router'))
+        self.assertEqual(len(router['external_gateways']), 0)
+
+        res = self.client.router_add_external_gateways(
+            router['id'],
+            [
+                {'network_id': CONF.network.public_network_id,
+                 'enable_snat': False},
+                {'network_id': CONF.network.public_network_id,
+                 'enable_snat': False},
+                {'network_id': CONF.network.public_network_id,
+                 'enable_snat': False},
+            ])
+        self.assertEqual(len(res['router']['external_gateways']), 3)
+        remove_gateways = [res['router']['external_gateways'][2]]
+        res = self.client.router_remove_external_gateways(router['id'],
+                                                          remove_gateways)
+        self.assertEqual(len(res['router']['external_gateways']), 2)
+        for n in range(0, 2):
+            self.assertNotEqual(
+                    res['router']['external_gateways'][
+                        n]['external_fixed_ips'],
+                    remove_gateways[0])
+
+    @decorators.idempotent_id('17e94c9f-c59f-4e50-abd5-d1256460e311')
+    def test_create_router_update_external_gateways(self):
+        """Add three GW ports, delete last one, re-use IPs in update on second.
+
+        NOTE(fnordahl): Main reason for IP re-use is to ensure we don't tread
+        on allocations done by other tests.
+        """
+        router = self._create_router(data_utils.rand_name('router'))
+        self.assertEqual(len(router['external_gateways']), 0)
+
+        res = self.client.router_add_external_gateways(
+            router['id'],
+            [
+                {'network_id': CONF.network.public_network_id,
+                 'enable_snat': False},
+                {'network_id': CONF.network.public_network_id,
+                 'enable_snat': False},
+                {'network_id': CONF.network.public_network_id,
+                 'enable_snat': False},
+            ])
+        self.assertEqual(len(res['router']['external_gateways']), 3)
+        external_gateways = res['router']['external_gateways']
+        remove_gateways = [external_gateways.pop(2)]
+        res_remove_gws = self.client.router_remove_external_gateways(
+            router['id'],
+            remove_gateways)
+        for n in range(0, 2):
+            self.assertNotEqual(
+                    res_remove_gws['router']['external_gateways'][
+                        n]['external_fixed_ips'],
+                    remove_gateways[0])
+
+        external_gateways[1] = remove_gateways[0]
+        res_update_gws = self.client.router_update_external_gateways(
+            router['id'],
+            external_gateways)
+
+        self.assertEqual(len(res_update_gws['router']['external_gateways']), 2)
+        for n in range(0, 2):
+            if res_update_gws['router']['external_gateways'][
+                        n] == remove_gateways[0]:
+                break
+        else:
+            self.fail('%s not in %s' % (
+                remove_gateways[0],
+                res_update_gws['router']['external_gateways']))
+
+
 class RoutersIpV6Test(RoutersTest):
     _ip_version = 6
 
 
 class DvrRoutersTest(base_routers.BaseRouterTest):
 
     required_extensions = ['dvr']
```

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_routers_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_routers_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_security_groups.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_security_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_security_groups_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_security_groups_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_service_type_management.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_service_type_management.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_subnetpool_prefix_ops.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_subnetpool_prefix_ops.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_subnetpools.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_subnetpools.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_subnetpools_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_subnetpools_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_subnets.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_subnets.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import netaddr
+from tempest.common import utils as tutils
 from tempest.lib import decorators
 
 from neutron_tempest_plugin.api import base
 
 
 class SubnetsSearchCriteriaTest(base.BaseSearchCriteriaTest):
 
     resource = 'subnet'
 
     list_kwargs = {'shared': False}
 
     @classmethod
     def resource_setup(cls):
+        if tutils.is_extension_enabled('subnet-external-network', 'network'):
+            cls.list_kwargs['router:external'] = False
         super(SubnetsSearchCriteriaTest, cls).resource_setup()
         net = cls.create_network(network_name='subnet-search-test-net')
         for name in cls.resource_names:
             cls.create_subnet(net, name=name)
 
     @decorators.idempotent_id('d2d61995-5dd5-4b93-bce7-3edefdb79563')
     def test_list_sorts_asc(self):
```

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_timestamp.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_trunk.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_trunk.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_trunk_details.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_trunk_details.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/api/test_trunk_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/api/test_trunk_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/api/test_bgpvpn.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/api/test_bgpvpn.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/base.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/scenario/manager.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/scenario/manager.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/scenario/test_bgpvpn_basic.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/scenario/test_bgpvpn_basic.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/bgpvpn/services/bgpvpn_client.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/bgpvpn/services/bgpvpn_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/constants.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/ip.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/ip.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/shell.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/shell.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/ssh.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/ssh.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/tempest_fixtures.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/tempest_fixtures.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/common/utils.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/common/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/config.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/exceptions.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/api/fwaas_v2_base.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/api/fwaas_v2_base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/api/test_fwaasv2_extensions.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/api/test_fwaasv2_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/common/fwaas_v2_client.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/common/fwaas_v2_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_base.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_manager.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_manager.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/scenario/test_fwaas_v2.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/scenario/test_fwaas_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/fwaas/services/v2_client.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/fwaas/services/v2_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions_negative.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/README` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/README`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base_test_proto.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base_test_proto.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/base.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_4byte_asn.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_4byte_asn.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_basic.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_basic.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/test_ipv4.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/test_ipv4.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/test_ipv6.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/test_ipv6.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/test_simple_bgp.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/test_simple_bgp.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/plugin.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/admin/test_floatingip.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/admin/test_floatingip.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/base.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/constants.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/exceptions.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_basic.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_basic.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_connectivity.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_connectivity.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_dhcp.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_dhcp.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_dns_integration.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_dns_integration.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_dvr.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_dvr.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_fip64.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_fip64.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_floatingip.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_floatingip.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,17 +235,21 @@
             # attach the port to the server
             self.create_interface(
                 server['server']['id'], port_id=port['id'])
             waiters.wait_for_interface_status(
                 self.os_primary.interfaces_client, server['server']['id'],
                 port['id'], lib_constants.PORT_STATUS_ACTIVE)
             fip = self.client.show_floatingip(fip['id'])['floatingip']
+            server_data = self.os_admin.servers_client.show_server(
+                server['server']['id'])['server']
+            zone = 'compute:' + server_data['OS-EXT-AZ:availability_zone']
             self._check_port_details(
                 fip, port, status=lib_constants.PORT_STATUS_ACTIVE,
-                device_id=server['server']['id'], device_owner='compute:nova')
+                device_id=server['server']['id'],
+                device_owner=zone)
             LOG.debug('Port check for server %s and FIP %s finished, '
                       'lets detach port %s from server!',
                       server['server']['id'], fip['id'], port['id'])
 
             # detach the port from the server; this is a cast in the compute
             # API so we have to poll the port until the device_id is unset.
             self.delete_interface(server['server']['id'], port['id'])
```

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_internal_dns.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_internal_dns.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_ipv6.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_ipv6.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_local_ip.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_local_ip.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_mac_learning.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_mac_learning.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_metadata.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_metadata.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_migration.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_migration.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_mtu.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_mtu.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_multicast.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_multicast.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_port_forwardings.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_port_forwardings.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_ports.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_ports.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_portsecurity.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_portsecurity.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_qos.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_qos.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_security_groups.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_security_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_trunk.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_trunk.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/scenario/test_vlan_transparency.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/scenario/test_vlan_transparency.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/bgp/bgp_client.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/bgp/bgp_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/services/network/json/network_client.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/services/network/json/network_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,14 +393,17 @@
             update_body['distributed'] = kwargs['distributed']
         if 'ha' in kwargs:
             update_body['ha'] = kwargs['ha']
         if 'routes' in kwargs:
             update_body['routes'] = kwargs['routes']
         if 'enable_ndp_proxy' in kwargs:
             update_body['enable_ndp_proxy'] = kwargs['enable_ndp_proxy']
+        for attr in ('enable_default_route_bfd', 'enable_default_route_ecmp'):
+            if attr in kwargs:
+                update_body[attr] = kwargs[attr]
         update_body = dict(router=update_body)
         update_body = jsonutils.dumps(update_body)
         resp, body = self.put(uri, update_body)
         self.expected_success(200, resp.status)
         body = jsonutils.loads(body)
         return service_client.ResponseBody(resp, body)
 
@@ -467,14 +470,50 @@
         self.expected_success(200, resp.status)
         body = jsonutils.loads(body)
         return service_client.ResponseBody(resp, body)
 
     def remove_router_extra_routes(self, router_id):
         self.update_router(router_id, routes=None)
 
+    def router_add_external_gateways(self, router_id, external_gateways):
+        uri = '%s/routers/%s/add_external_gateways' % (self.uri_prefix,
+                                                       router_id)
+        update_body = {
+                'router': {'external_gateways': external_gateways},
+        }
+        update_body = jsonutils.dumps(update_body)
+        resp, body = self.put(uri, update_body)
+        self.expected_success(200, resp.status)
+        body = jsonutils.loads(body)
+        return service_client.ResponseBody(resp, body)
+
+    def router_remove_external_gateways(self, router_id, external_gateways):
+        uri = '%s/routers/%s/remove_external_gateways' % (self.uri_prefix,
+                                                          router_id)
+        update_body = {
+                'router': {'external_gateways': external_gateways},
+        }
+        update_body = jsonutils.dumps(update_body)
+        resp, body = self.put(uri, update_body)
+        self.expected_success(200, resp.status)
+        body = jsonutils.loads(body)
+        return service_client.ResponseBody(resp, body)
+
+    def router_update_external_gateways(self, router_id, external_gateways):
+        uri = '%s/routers/%s/update_external_gateways' % (self.uri_prefix,
+                                                          router_id)
+        update_body = {
+                'router': {'external_gateways': external_gateways},
+        }
+        update_body = jsonutils.dumps(update_body)
+        resp, body = self.put(uri, update_body)
+        self.expected_success(200, resp.status)
+        body = jsonutils.loads(body)
+        return service_client.ResponseBody(resp, body)
+
     def update_agent(self, agent_id, agent_info):
         """Update an agent
 
         :param agent_info: Agent update information.
         E.g {"admin_state_up": True}
         """
         uri = '%s/agents/%s' % (self.uri_prefix, agent_id)
@@ -1108,14 +1147,22 @@
         if filters:
             uri = '?'.join([uri, urlparse.urlencode(filters)])
         resp, body = self.get(uri)
         body = {'extensions': self.deserialize_list(body)}
         self.expected_success(200, resp.status)
         return service_client.ResponseBody(resp, body)
 
+    def get_extension(self, alias):
+        uri = '%s/%s' % (
+            self.get_uri('extensions'), alias)
+        resp, body = self.get(uri)
+        self.expected_success(200, resp.status)
+        body = jsonutils.loads(body)
+        return service_client.ResponseBody(resp, body)
+
     def get_tags(self, resource_type, resource_id):
         uri = '%s/%s/%s/tags' % (
             self.uri_prefix, resource_type, resource_id)
         resp, body = self.get(uri)
         self.expected_success(200, resp.status)
         body = jsonutils.loads(body)
         return service_client.ResponseBody(resp, body)
```

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/services/flowclassifier_client.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/services/flowclassifier_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/services/sfc_client.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/services/sfc_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/api/base.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/api/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/api/test_flowclassifier_extensions.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/api/test_flowclassifier_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/api/test_sfc_extensions.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/api/test_sfc_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/flowclassifier_client.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/flowclassifier_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/scenario/base.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/scenario/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/scenario/manager.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/scenario/manager.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/scenario/test_sfc.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/scenario/test_sfc.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/sfc/tests/sfc_client.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/sfc/tests/sfc_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/api/test_taas.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/api/test_taas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/base.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/scenario/manager.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/scenario/manager.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_taas.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_taas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_traffic_impact.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_traffic_impact.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/tap_as_a_service/services/taas_client.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/tap_as_a_service/services/taas_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/api/base_vpnaas.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/api/base_vpnaas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/api/test_vpnaas.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/api/test_vpnaas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/scenario/base_vpnaas.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/scenario/base_vpnaas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/scenario/test_vpnaas.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/scenario/test_vpnaas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin/vpnaas/services/clients_vpnaas.py` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin/vpnaas/services/clients_vpnaas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin.egg-info/PKG-INFO` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-tempest-plugin
-Version: 2.7.0
+Version: 2.8.0
 Summary: Tempest plugin for Neutron Project
 Home-page: https://opendev.org/openstack/neutron-tempest-plugin
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ======================
         Neutron Tempest Plugin
```

### Comparing `neutron-tempest-plugin-2.7.0/neutron_tempest_plugin.egg-info/SOURCES.txt` & `neutron-tempest-plugin-2.8.0/neutron_tempest_plugin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,15 @@
 roles/multi-node-setup/README.rst
 roles/multi-node-setup/defaults/main.yaml
 roles/multi-node-setup/tasks/main.yaml
 tools/customize_ubuntu_image
 tools/misc-sanity-checks.sh
 zuul.d/2023_1_jobs.yaml
 zuul.d/2023_2_jobs.yaml
+zuul.d/2024_1_jobs.yaml
 zuul.d/base-nested-switch.yaml
 zuul.d/master_jobs.yaml
 zuul.d/project.yaml
 zuul.d/victoria_jobs.yaml
 zuul.d/wallaby_jobs.yaml
 zuul.d/xena_jobs.yaml
 zuul.d/yoga_jobs.yaml
```

### Comparing `neutron-tempest-plugin-2.7.0/releasenotes/source/README.rst` & `neutron-tempest-plugin-2.8.0/releasenotes/source/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/releasenotes/source/conf.py` & `neutron-tempest-plugin-2.8.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/requirements.txt` & `neutron-tempest-plugin-2.8.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/roles/docker-setup/files/docker_apparmor` & `neutron-tempest-plugin-2.8.0/roles/docker-setup/files/docker_apparmor`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/roles/docker-setup/tasks/main.yml` & `neutron-tempest-plugin-2.8.0/roles/docker-setup/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/roles/multi-node-setup/README.rst` & `neutron-tempest-plugin-2.8.0/roles/multi-node-setup/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/roles/multi-node-setup/tasks/main.yaml` & `neutron-tempest-plugin-2.8.0/roles/multi-node-setup/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/setup.cfg` & `neutron-tempest-plugin-2.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/setup.py` & `neutron-tempest-plugin-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/tools/customize_ubuntu_image` & `neutron-tempest-plugin-2.8.0/tools/customize_ubuntu_image`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/tools/misc-sanity-checks.sh` & `neutron-tempest-plugin-2.8.0/tools/misc-sanity-checks.sh`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/tox.ini` & `neutron-tempest-plugin-2.8.0/tox.ini`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/zuul.d/2023_1_jobs.yaml` & `neutron-tempest-plugin-2.8.0/zuul.d/2023_1_jobs.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/zuul.d/2023_2_jobs.yaml` & `neutron-tempest-plugin-2.8.0/zuul.d/2023_2_jobs.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/zuul.d/base-nested-switch.yaml` & `neutron-tempest-plugin-2.8.0/zuul.d/base-nested-switch.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/zuul.d/master_jobs.yaml` & `neutron-tempest-plugin-2.8.0/zuul.d/master_jobs.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         neutron-trunk: true
         neutron-uplink-status-propagation: true
         neutron-network-segment-range: true
         neutron-port-forwarding: true
         neutron-conntrack-helper: true
         neutron-tag-ports-during-bulk-creation: true
         neutron-ndp-proxy: true
+        neutron-subnet-external-network: true
         br-ex-tcpdump: true
         br-int-flows: true
         # Cinder services
         c-api: false
         c-bak: false
         c-sch: false
         c-vol: false
@@ -232,14 +233,15 @@
         ovn-controller: false
         ovn-northd: false
         ovs-vswitchd: false
         ovsdb-server: false
         q-ovn-metadata-agent: false
         # Neutron services
         neutron-local-ip-static: true
+        neutron-subnet-external-network: true
         q-agt: true
         q-dhcp: true
         q-l3: true
         q-meta: true
         q-metering: true
       network_api_extensions_openvswitch:
         - dhcp_agent_scheduler
@@ -327,14 +329,15 @@
         ovn-controller: false
         ovn-northd: false
         ovs-vswitchd: false
         ovsdb-server: false
         q-ovn-metadata-agent: false
         # Neutron services
         neutron-local-ip: true
+        neutron-subnet-external-network: true
         q-agt: true
         q-dhcp: true
         q-l3: true
         q-meta: true
         q-metering: true
       network_api_extensions_openvswitch:
         - dhcp_agent_scheduler
```

### Comparing `neutron-tempest-plugin-2.7.0/zuul.d/project.yaml` & `neutron-tempest-plugin-2.8.0/zuul.d/project.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -151,51 +151,76 @@
     #TODO(slaweq): Move neutron-tempest-plugin-dvr-multinode-scenario out of
     #              the experimental queue when it will be more stable
     experimental:
       jobs:
         - neutron-tempest-plugin-linuxbridge-2023-2
         - neutron-tempest-plugin-dvr-multinode-scenario-2023-2
 
+- project-template:
+    name: neutron-tempest-plugin-jobs-2024-1
+    check:
+      jobs:
+        - neutron-tempest-plugin-openvswitch-2024-1
+        - neutron-tempest-plugin-openvswitch-iptables_hybrid-2024-1
+        - neutron-tempest-plugin-ovn-2024-1
+        - neutron-tempest-plugin-designate-scenario-2024-1
+    gate:
+      jobs:
+        - neutron-tempest-plugin-ovn-2024-1
+    #TODO(slaweq): Move neutron-tempest-plugin-dvr-multinode-scenario out of
+    #              the experimental queue when it will be more stable
+    experimental:
+      jobs:
+        - neutron-tempest-plugin-linuxbridge-2024-1
+        - neutron-tempest-plugin-dvr-multinode-scenario-2024-1
+
 - project:
     templates:
       - build-openstack-docs-pti
       - neutron-tempest-plugin-jobs
       - neutron-tempest-plugin-jobs-zed
       - neutron-tempest-plugin-jobs-2023-1
       - neutron-tempest-plugin-jobs-2023-2
+      - neutron-tempest-plugin-jobs-2024-1
       - check-requirements
       - tempest-plugin-jobs
       - release-notes-jobs-python3
     check:
       jobs:
         - neutron-tempest-plugin-sfc
         - neutron-tempest-plugin-sfc-zed
         - neutron-tempest-plugin-sfc-2023-1
         - neutron-tempest-plugin-sfc-2023-2
+        - neutron-tempest-plugin-sfc-2024-1
         - neutron-tempest-plugin-bgpvpn-bagpipe
         - neutron-tempest-plugin-bgpvpn-bagpipe-zed
         - neutron-tempest-plugin-bgpvpn-bagpipe-2023-1
         - neutron-tempest-plugin-bgpvpn-bagpipe-2023-2
+        - neutron-tempest-plugin-bgpvpn-bagpipe-2024-1
         - neutron-tempest-plugin-dynamic-routing
         - neutron-tempest-plugin-dynamic-routing-zed
         - neutron-tempest-plugin-dynamic-routing-2023-1
         - neutron-tempest-plugin-dynamic-routing-2023-2
+        - neutron-tempest-plugin-dynamic-routing-2024-1
         - neutron-tempest-plugin-fwaas
         - neutron-tempest-plugin-fwaas-zed
         - neutron-tempest-plugin-fwaas-2023-1
         - neutron-tempest-plugin-fwaas-2023-2
+        - neutron-tempest-plugin-fwaas-2024-1
         - neutron-tempest-plugin-vpnaas
         - neutron-tempest-plugin-vpnaas-ovn
         - neutron-tempest-plugin-vpnaas-zed
         - neutron-tempest-plugin-vpnaas-2023-1
         - neutron-tempest-plugin-vpnaas-2023-2
+        - neutron-tempest-plugin-vpnaas-2024-1
         - neutron-tempest-plugin-tap-as-a-service
         - neutron-tempest-plugin-tap-as-a-service-zed
         - neutron-tempest-plugin-tap-as-a-service-2023-1
         - neutron-tempest-plugin-tap-as-a-service-2023-2
+        - neutron-tempest-plugin-tap-as-a-service-2024-1
 
     gate:
       jobs:
         - neutron-tempest-plugin-sfc
         - neutron-tempest-plugin-bgpvpn-bagpipe
         - neutron-tempest-plugin-dynamic-routing
         - neutron-tempest-plugin-fwaas
```

### Comparing `neutron-tempest-plugin-2.7.0/zuul.d/victoria_jobs.yaml` & `neutron-tempest-plugin-2.8.0/zuul.d/victoria_jobs.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 - job:
     name: neutron-tempest-plugin-api-victoria
     parent: neutron-tempest-plugin-base
     nodeset: openstack-single-node-focal
-    override-checkout: stable/victoria
+    override-checkout: unmaintained/victoria
     required-projects: &required-projects-victoria
       - openstack/neutron
       - name: openstack/neutron-tempest-plugin
         override-checkout: 1.6.0
       - openstack/tempest
     vars:
       devstack_services:
@@ -130,15 +130,15 @@
           $TEMPEST_CONFIG:
             neutron_plugin_options:
               available_type_drivers: flat,geneve,vlan,gre,local,vxlan
 
 - job:
     name: neutron-tempest-plugin-scenario-openvswitch-victoria
     parent: neutron-tempest-plugin-openvswitch
-    override-checkout: stable/victoria
+    override-checkout: unmaintained/victoria
     required-projects: *required-projects-victoria
     vars:
       tempest_test_regex: "\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
       network_api_extensions: *api_extensions
@@ -158,15 +158,15 @@
               available_features: "{{ network_available_features | join(',') }}"
             neutron_plugin_options:
               ipv6_metadata: False
 
 - job:
     name: neutron-tempest-plugin-scenario-openvswitch-iptables_hybrid-victoria
     parent: neutron-tempest-plugin-openvswitch-iptables_hybrid
-    override-checkout: stable/victoria
+    override-checkout: unmaintained/victoria
     required-projects: *required-projects-victoria
     vars:
       tempest_test_regex: "\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
       network_api_extensions: *api_extensions
@@ -190,15 +190,15 @@
               available_features: "{{ network_available_features | join(',') }}"
             neutron_plugin_options:
               ipv6_metadata: False
 
 - job:
     name: neutron-tempest-plugin-scenario-linuxbridge-victoria
     parent: neutron-tempest-plugin-linuxbridge
-    override-checkout: stable/victoria
+    override-checkout: unmaintained/victoria
     required-projects: *required-projects-victoria
     vars:
       tempest_test_regex: "\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
       network_api_extensions: *api_extensions
@@ -218,15 +218,15 @@
               available_features: "{{ network_available_features | join(',') }}"
             neutron_plugin_options:
               ipv6_metadata: False
 
 - job:
     name: neutron-tempest-plugin-scenario-ovn-victoria
     parent: neutron-tempest-plugin-ovn
-    override-checkout: stable/victoria
+    override-checkout: unmaintained/victoria
     required-projects: *required-projects-victoria
     vars:
       tempest_test_regex: "\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
       network_api_extensions: *api_extensions
@@ -249,23 +249,23 @@
             network-feature-enabled:
               available_features: ""
 
 - job:
     name: neutron-tempest-plugin-dvr-multinode-scenario-victoria
     parent: neutron-tempest-plugin-dvr-multinode-scenario
     nodeset: openstack-two-node-focal
-    override-checkout: stable/victoria
+    override-checkout: unmaintained/victoria
     required-projects: *required-projects-victoria
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
     name: neutron-tempest-plugin-designate-scenario-victoria
     parent: neutron-tempest-plugin-designate-scenario
-    override-checkout: stable/victoria
+    override-checkout: unmaintained/victoria
     required-projects:
       - openstack/neutron
       - name: openstack/neutron-tempest-plugin
         override-checkout: 1.6.0
       - openstack/tempest
       - name: openstack/designate-tempest-plugin
         override-checkout: 0.12.0
@@ -279,38 +279,38 @@
         ADVANCED_INSTANCE_USER: ubuntu
         CUSTOMIZE_IMAGE: false
 
 - job:
     name: neutron-tempest-plugin-sfc-victoria
     parent: neutron-tempest-plugin-sfc
     nodeset: openstack-single-node-focal
-    override-checkout: stable/victoria
+    override-checkout: unmaintained/victoria
     required-projects: *required-projects-victoria
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
     name: neutron-tempest-plugin-bgpvpn-bagpipe-victoria
     parent: neutron-tempest-plugin-bgpvpn-bagpipe
     nodeset: openstack-single-node-focal
-    override-checkout: stable/victoria
+    override-checkout: unmaintained/victoria
     required-projects: *required-projects-victoria
     vars:
       network_api_extensions: *api_extensions
 
 - job:
     name: neutron-tempest-plugin-dynamic-routing-victoria
     parent: neutron-tempest-plugin-dynamic-routing
     nodeset: openstack-single-node-focal
-    override-checkout: stable/victoria
+    override-checkout: unmaintained/victoria
     required-projects: *required-projects-victoria
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
     name: neutron-tempest-plugin-vpnaas-victoria
     parent: neutron-tempest-plugin-vpnaas
     nodeset: openstack-single-node-focal
-    override-checkout: stable/victoria
+    override-checkout: unmaintained/victoria
     required-projects: *required-projects-victoria
     vars:
       network_api_extensions_common: *api_extensions
```

### Comparing `neutron-tempest-plugin-2.7.0/zuul.d/wallaby_jobs.yaml` & `neutron-tempest-plugin-2.8.0/zuul.d/wallaby_jobs.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/zuul.d/xena_jobs.yaml` & `neutron-tempest-plugin-2.8.0/zuul.d/xena_jobs.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/zuul.d/yoga_jobs.yaml` & `neutron-tempest-plugin-2.8.0/zuul.d/yoga_jobs.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.7.0/zuul.d/zed_jobs.yaml` & `neutron-tempest-plugin-2.8.0/zuul.d/zed_jobs.yaml`

 * *Files identical despite different names*

