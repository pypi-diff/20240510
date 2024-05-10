# Comparing `tmp/catalyst_sdwan_lab-2.0.8.tar.gz` & `tmp/catalyst_sdwan_lab-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalyst_sdwan_lab-2.0.8.tar", max compression
+gzip compressed data, was "catalyst_sdwan_lab-2.0.9.tar", max compression
```

## Comparing `catalyst_sdwan_lab-2.0.8.tar` & `catalyst_sdwan_lab-2.0.9.tar`

### file list

```diff
@@ -1,434 +1,434 @@
--rw-r--r--   0        0        0     1516 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/LICENSE
--rw-r--r--   0        0        0    19200 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/README.md
--rw-r--r--   0        0        0      357 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/__init__.py
--rw-r--r--   0        0        0    20068 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/__main__.py
--rwxr-xr-x   0        0        0      443 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/cacsr_details.txt
--rw-r--r--   0        0        0     3033 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/chainCA.pem
--rwxr-xr-x   0        0        0      790 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/openssl-commands.md
--rw-r--r--   0        0        0     1517 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/rootCA.pem
--rw-r--r--   0        0        0       17 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/rootCA.srl
--rwxr-xr-x   0        0        0      485 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/rootca_details.txt
--rw-r--r--   0        0        0     1074 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/signCA.csr
--rw-r--r--   0        0        0     1675 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/signCA.key
--rw-r--r--   0        0        0     1517 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/signCA.pem
--rwxr-xr-x   0        0        0      352 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/v3ext.cnf
--rw-r--r--   0        0        0      421 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/backup/controller-cloud-init.j2
--rw-r--r--   0        0        0      851 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/backup/edge-cloud-init.j2
--rw-r--r--   0        0        0      523 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/backup/manager-cloud-init.j2
--rw-r--r--   0        0        0      895 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/backup/sdrouting-cloud-init.j2
--rw-r--r--   0        0        0      415 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/backup/validator-cloud-init.j2
--rw-r--r--   0        0        0    16330 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/deploy/cml-base-topology.j2
--rw-r--r--   0        0        0     2292 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/deploy/controller-cloud-init.j2
--rw-r--r--   0        0        0     3182 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/deploy/manager-cloud-init.j2
--rw-r--r--   0        0        0     1383 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/deploy/sdrouting-cloud-init.j2
--rw-r--r--   0        0        0     2327 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/deploy/validator-cloud-init.j2
--rw-r--r--   0        0        0     2087 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-controller.yaml
--rw-r--r--   0        0        0     1981 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-edge.yaml
--rw-r--r--   0        0        0     2094 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-manager.yaml
--rw-r--r--   0        0        0     2097 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-validator.yaml
--rw-r--r--   0        0        0     1859 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1866 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json
--rw-r--r--   0        0        0     1833 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1736 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json
--rw-r--r--   0        0        0     1702 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json
--rw-r--r--   0        0        0     1910 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json
--rw-r--r--   0        0        0     1686 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_GCP_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1615 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json
--rw-r--r--   0        0        0     2516 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_C8000V_Template_V01.json
--rw-r--r--   0        0        0     2510 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_ISRv_Template_V01.json
--rw-r--r--   0        0        0     2293 2024-04-25 09:55:09.466199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json
--rw-r--r--   0        0        0     2657 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json
--rw-r--r--   0        0        0     2365 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json
--rw-r--r--   0        0        0     3215 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_CSR_1000V_V01.json
--rw-r--r--   0        0        0     2924 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_DC1_HUB.json
--rw-r--r--   0        0        0     2260 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_ISR_4331_V01.json
--rw-r--r--   0        0        0     1347 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/controller_basic.json
--rw-r--r--   0        0        0     2454 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/edge_basic.json
--rw-r--r--   0        0        0    19645 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json
--rw-r--r--   0        0        0     7062 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24745 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json
--rw-r--r--   0        0        0     5515 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json
--rw-r--r--   0        0        0    12013 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5591 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json
--rw-r--r--   0        0        0     6135 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24962 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0    11984 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json
--rw-r--r--   0        0        0     5492 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     5564 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json
--rw-r--r--   0        0        0     3456 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BFD_Cisco_V01.json
--rw-r--r--   0        0        0    19638 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BOOTSTRAP_DHCP_V01.json
--rw-r--r--   0        0        0     9573 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json
--rw-r--r--   0        0        0    12289 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json
--rw-r--r--   0        0        0     8173 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_System_Template.json
--rw-r--r--   0        0        0     2216 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Cellular_V01.json
--rw-r--r--   0        0        0     6228 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_SVI_V01.json
--rw-r--r--   0        0        0     1607 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Switch_Port_V01.json
--rw-r--r--   0        0        0    22837 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json
--rw-r--r--   0        0        0    10441 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json
--rw-r--r--   0        0        0    22817 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json
--rw-r--r--   0        0        0    22819 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json
--rw-r--r--   0        0        0    10419 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json
--rw-r--r--   0        0        0    18079 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json
--rw-r--r--   0        0        0    11073 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json
--rw-r--r--   0        0        0    11073 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json
--rw-r--r--   0        0        0    11073 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json
--rw-r--r--   0        0        0    11095 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json
--rw-r--r--   0        0        0    11071 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json
--rw-r--r--   0        0        0    11071 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json
--rw-r--r--   0        0        0    11075 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json
--rw-r--r--   0        0        0    11071 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json
--rw-r--r--   0        0        0     7066 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    25121 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json
--rw-r--r--   0        0        0     7603 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json
--rw-r--r--   0        0        0     5572 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json
--rw-r--r--   0        0        0    11992 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json
--rw-r--r--   0        0        0     7025 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24720 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5478 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     5550 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN512_V01.json
--rw-r--r--   0        0        0     2144 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Logging_Cisco_V01.json
--rw-r--r--   0        0        0     7061 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    25114 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5514 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     4915 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_NTP_Cisco_V01.json
--rw-r--r--   0        0        0     6290 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_OMP_Cisco_V01.json
--rw-r--r--   0        0        0    24529 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INET_INT_V01.json
--rw-r--r--   0        0        0    12375 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json
--rw-r--r--   0        0        0    12084 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_INT_V01.json
--rw-r--r--   0        0        0     5570 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json
--rw-r--r--   0        0        0    12106 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_SVC_INT_V01.json
--rw-r--r--   0        0        0     8510 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_Service_VPN1_V01.json
--rw-r--r--   0        0        0    10463 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_VPN0_Template_V01.json
--rw-r--r--   0        0        0    25674 2024-04-25 09:55:09.470199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json
--rw-r--r--   0        0        0    13302 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json
--rw-r--r--   0        0        0    13021 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json
--rw-r--r--   0        0        0     4729 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json
--rw-r--r--   0        0        0    13047 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json
--rw-r--r--   0        0        0     8131 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json
--rw-r--r--   0        0        0    10082 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json
--rw-r--r--   0        0        0     2191 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Security_Cisco_V01.json
--rw-r--r--   0        0        0     5921 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_System_Cisco_V01.json
--rw-r--r--   0        0        0     6998 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_0_Cisco_V01.json
--rw-r--r--   0        0        0     4315 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_1_Cisco_V01.json
--rw-r--r--   0        0        0     4323 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_512_Cisco_V01.json
--rw-r--r--   0        0        0     6985 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_CISCO_Template.json
--rw-r--r--   0        0        0    20010 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_Template.json
--rw-r--r--   0        0        0     3218 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json
--rw-r--r--   0        0        0     7296 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_Standalone_Template.json
--rw-r--r--   0        0        0     1739 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_BFD_Template_V01.json
--rw-r--r--   0        0        0     4104 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_BFD_Template.json
--rw-r--r--   0        0        0    14537 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json
--rw-r--r--   0        0        0     4186 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Logging_Template.json
--rw-r--r--   0        0        0     7502 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json
--rw-r--r--   0        0        0     4511 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Security_Template.json
--rw-r--r--   0        0        0     8107 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_System_Template.json
--rw-r--r--   0        0        0     4416 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_0_Template.json
--rw-r--r--   0        0        0    13607 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json
--rw-r--r--   0        0        0     4333 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_Template.json
--rw-r--r--   0        0        0     3938 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json
--rw-r--r--   0        0        0    27208 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json
--rw-r--r--   0        0        0    25438 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json
--rw-r--r--   0        0        0     8351 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_System.json
--rw-r--r--   0        0        0     9978 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_VPN0.json
--rw-r--r--   0        0        0    11257 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json
--rw-r--r--   0        0        0     4976 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_EIO_System_Template.json
--rw-r--r--   0        0        0    10714 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Global_CISCO_Template.json
--rw-r--r--   0        0        0     2008 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Logging_Template_V01.json
--rw-r--r--   0        0        0    11386 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json
--rw-r--r--   0        0        0    12016 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json
--rw-r--r--   0        0        0     7360 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_BGP_To_OMP.json
--rw-r--r--   0        0        0     1303 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Banner.json
--rw-r--r--   0        0        0    11243 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_System.json
--rw-r--r--   0        0        0    11964 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_VPN0.json
--rw-r--r--   0        0        0    11788 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json
--rw-r--r--   0        0        0    14115 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json
--rw-r--r--   0        0        0    12000 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json
--rw-r--r--   0        0        0     6868 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json
--rw-r--r--   0        0        0    25394 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json
--rw-r--r--   0        0        0     9260 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Regular_BFD.json
--rw-r--r--   0        0        0    25074 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN0_LTE.json
--rw-r--r--   0        0        0    31516 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json
--rw-r--r--   0        0        0    24593 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json
--rw-r--r--   0        0        0     4859 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_UTD_Template.json
--rw-r--r--   0        0        0     9400 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json
--rw-r--r--   0        0        0     9394 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json
--rw-r--r--   0        0        0    14686 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Cellular_Interface.json
--rw-r--r--   0        0        0    19630 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json
--rw-r--r--   0        0        0     6475 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Management_Interface.json
--rw-r--r--   0        0        0     3858 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_Template.json
--rw-r--r--   0        0        0     5138 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json
--rw-r--r--   0        0        0     2080 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Security_Template_V01.json
--rw-r--r--   0        0        0     5653 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_System_Template.json
--rw-r--r--   0        0        0     4099 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json
--rw-r--r--   0        0        0     4106 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json
--rw-r--r--   0        0        0     2608 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_OMP_Template.json
--rw-r--r--   0        0        0      984 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json
--rw-r--r--   0        0        0     4382 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_System_Template.json
--rw-r--r--   0        0        0     3155 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json
--rw-r--r--   0        0        0     1442 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json
--rw-r--r--   0        0        0    34849 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_aaa.json
--rw-r--r--   0        0        0     5401 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0.json
--rw-r--r--   0        0        0    10612 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0_eth1.json
--rw-r--r--   0        0        0      868 2024-04-25 09:55:09.474199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_cli.json
--rw-r--r--   0        0        0    12306 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0.json
--rw-r--r--   0        0        0    29668 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi1_inet.json
--rw-r--r--   0        0        0    27664 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi2_mpls.json
--rw-r--r--   0        0        0    11922 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1.json
--rw-r--r--   0        0        0     3969 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_dhcp.json
--rw-r--r--   0        0        0    13751 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_lan.json
--rw-r--r--   0        0        0     9628 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/inventory/device_templates.json
--rw-r--r--   0        0        0   597414 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/inventory/feature_templates.json
--rw-r--r--   0        0        0    14055 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_app.json
--rw-r--r--   0        0        0     1317 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_localapp.json
--rw-r--r--   0        0        0     3720 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_sla.json
--rw-r--r--   0        0        0      532 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_BULK_DATA.json
--rw-r--r--   0        0        0      596 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_Scavengers.json
--rw-r--r--   0        0        0     2748 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Google_Apps.json
--rw-r--r--   0        0        0     1605 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Microsoft_Apps.json
--rw-r--r--   0        0        0      450 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/REAL_TIME_APPS.json
--rw-r--r--   0        0        0      386 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/VIDEO_CONF.json
--rw-r--r--   0        0        0      452 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/WEB_TOOLS_APP.json
--rw-r--r--   0        0        0      608 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/amazon_aws_apps.json
--rw-r--r--   0        0        0      379 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/box_net_apps.json
--rw-r--r--   0        0        0      380 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/concur_apps.json
--rw-r--r--   0        0        0      383 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/dropbox_apps.json
--rw-r--r--   0        0        0      430 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/gotomeeting_apps.json
--rw-r--r--   0        0        0      380 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/intuit_apps.json
--rw-r--r--   0        0        0     1052 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/office365_apps.json
--rw-r--r--   0        0        0      596 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/oracle_apps.json
--rw-r--r--   0        0        0      392 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/salesforce_apps.json
--rw-r--r--   0        0        0      388 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/sugar_crm_apps.json
--rw-r--r--   0        0        0      383 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/zendesk_apps.json
--rw-r--r--   0        0        0      391 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/zoho_crm_apps.json
--rw-r--r--   0        0        0      386 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/Browsing.json
--rw-r--r--   0        0        0      375 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/ICMP.json
--rw-r--r--   0        0        0      428 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/Yahoo.json
--rw-r--r--   0        0        0      415 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Best-Effort.json
--rw-r--r--   0        0        0      419 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Bulk-Data.json
--rw-r--r--   0        0        0      427 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Business-Critical.json
--rw-r--r--   0        0        0      419 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Business-Data.json
--rw-r--r--   0        0        0      415 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Default.json
--rw-r--r--   0        0        0      408 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Realtime.json
--rw-r--r--   0        0        0      435 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Transactional-Data.json
--rw-r--r--   0        0        0      428 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Voice-And-Video.json
--rw-r--r--   0        0        0       32 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/server_info.json
--rw-r--r--   0        0        0    15002 2024-04-25 09:55:09.478200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/certificates/edge_certificates.json
--rw-r--r--   0        0        0     1628 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/config_groups/group/edge_basic.json
--rw-r--r--   0        0        0      295 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/attached/controller_basic.json
--rw-r--r--   0        0        0     1859 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1866 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json
--rw-r--r--   0        0        0     1833 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1736 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json
--rw-r--r--   0        0        0     1702 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json
--rw-r--r--   0        0        0     1910 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json
--rw-r--r--   0        0        0     1720 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_ICGW_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1686 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_GCP_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1615 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json
--rw-r--r--   0        0        0     2516 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_C8000V_Template_V01.json
--rw-r--r--   0        0        0     2510 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_ISRv_Template_V01.json
--rw-r--r--   0        0        0     2293 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json
--rw-r--r--   0        0        0     2657 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json
--rw-r--r--   0        0        0     2365 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json
--rw-r--r--   0        0        0     3207 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C8000V_V01.json
--rw-r--r--   0        0        0     2924 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_DC1_HUB.json
--rw-r--r--   0        0        0     2260 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_ISR_4331_V01.json
--rw-r--r--   0        0        0     1347 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/controller_basic.json
--rw-r--r--   0        0        0     2454 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/edge_basic.json
--rw-r--r--   0        0        0     4130 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/values/controller_basic.json
--rw-r--r--   0        0        0      776 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/cli/edge_basic_cli.json
--rw-r--r--   0        0        0     6515 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/service/edge_basic_lan.json
--rw-r--r--   0        0        0    12229 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/system/edge_basic_system.json
--rw-r--r--   0        0        0    13293 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/transport/edge_basic_wan.json
--rw-r--r--   0        0        0    20244 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json
--rw-r--r--   0        0        0     7063 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24746 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json
--rw-r--r--   0        0        0     5516 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json
--rw-r--r--   0        0        0    12014 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5592 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json
--rw-r--r--   0        0        0     6136 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24963 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0    11984 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json
--rw-r--r--   0        0        0     5493 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     5565 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json
--rw-r--r--   0        0        0     3457 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BFD_Cisco_V01.json
--rw-r--r--   0        0        0    20238 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BOOTSTRAP_DHCP_V01.json
--rw-r--r--   0        0        0    10172 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json
--rw-r--r--   0        0        0    12888 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json
--rw-r--r--   0        0        0     8773 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_System_Template.json
--rw-r--r--   0        0        0     2216 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Cellular_V01.json
--rw-r--r--   0        0        0     6229 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_SVI_V01.json
--rw-r--r--   0        0        0     1608 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Switch_Port_V01.json
--rw-r--r--   0        0        0    22838 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json
--rw-r--r--   0        0        0    10442 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json
--rw-r--r--   0        0        0    22818 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json
--rw-r--r--   0        0        0    22820 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json
--rw-r--r--   0        0        0    10420 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json
--rw-r--r--   0        0        0    18100 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json
--rw-r--r--   0        0        0    11094 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json
--rw-r--r--   0        0        0    11094 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json
--rw-r--r--   0        0        0    11094 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json
--rw-r--r--   0        0        0    11115 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json
--rw-r--r--   0        0        0    11091 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json
--rw-r--r--   0        0        0    11092 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json
--rw-r--r--   0        0        0    11095 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json
--rw-r--r--   0        0        0    11092 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json
--rw-r--r--   0        0        0     9231 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_C8000V_GLOBAL_CISCO_V01.json
--rw-r--r--   0        0        0     7813 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0     9262 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_DNS_V01.json
--rw-r--r--   0        0        0    28713 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_INTF_GE2_V01.json
--rw-r--r--   0        0        0     7245 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN512_V01.json
--rw-r--r--   0        0        0     7067 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    25122 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json
--rw-r--r--   0        0        0     7604 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json
--rw-r--r--   0        0        0     5573 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json
--rw-r--r--   0        0        0    11993 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json
--rw-r--r--   0        0        0     7026 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24721 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5479 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     5551 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN512_V01.json
--rw-r--r--   0        0        0     2145 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Logging_Cisco_V01.json
--rw-r--r--   0        0        0     7062 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    25115 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5515 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     4936 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_NTP_Cisco_V01.json
--rw-r--r--   0        0        0     6311 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_OMP_Cisco_V01.json
--rw-r--r--   0        0        0    24530 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INET_INT_V01.json
--rw-r--r--   0        0        0    12376 2024-04-25 09:55:09.482200 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json
--rw-r--r--   0        0        0    12085 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_INT_V01.json
--rw-r--r--   0        0        0     5570 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json
--rw-r--r--   0        0        0    12106 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_SVC_INT_V01.json
--rw-r--r--   0        0        0     8511 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_Service_VPN1_V01.json
--rw-r--r--   0        0        0    10464 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_VPN0_Template_V01.json
--rw-r--r--   0        0        0    25675 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json
--rw-r--r--   0        0        0    13303 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json
--rw-r--r--   0        0        0    13022 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json
--rw-r--r--   0        0        0     4730 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json
--rw-r--r--   0        0        0    13048 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json
--rw-r--r--   0        0        0     8132 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json
--rw-r--r--   0        0        0    10083 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json
--rw-r--r--   0        0        0     2192 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Security_Cisco_V01.json
--rw-r--r--   0        0        0     5922 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_System_Cisco_V01.json
--rw-r--r--   0        0        0     7019 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_0_Cisco_V01.json
--rw-r--r--   0        0        0     4336 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_1_Cisco_V01.json
--rw-r--r--   0        0        0     4343 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_512_Cisco_V01.json
--rw-r--r--   0        0        0     7211 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_CISCO_Template.json
--rw-r--r--   0        0        0    20011 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_Template.json
--rw-r--r--   0        0        0     3219 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json
--rw-r--r--   0        0        0     7321 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_Standalone_Template.json
--rw-r--r--   0        0        0     1740 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_BFD_Template_V01.json
--rw-r--r--   0        0        0     4330 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_BFD_Template.json
--rw-r--r--   0        0        0    14763 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json
--rw-r--r--   0        0        0     4412 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Logging_Template.json
--rw-r--r--   0        0        0     7728 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json
--rw-r--r--   0        0        0     4737 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Security_Template.json
--rw-r--r--   0        0        0     8333 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_System_Template.json
--rw-r--r--   0        0        0     4642 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_0_Template.json
--rw-r--r--   0        0        0    13632 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json
--rw-r--r--   0        0        0     4561 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_Template.json
--rw-r--r--   0        0        0     3938 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json
--rw-r--r--   0        0        0    27208 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json
--rw-r--r--   0        0        0    25439 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json
--rw-r--r--   0        0        0     8352 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_System.json
--rw-r--r--   0        0        0     9978 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_VPN0.json
--rw-r--r--   0        0        0    11258 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json
--rw-r--r--   0        0        0     5397 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_EIO_System_Template.json
--rw-r--r--   0        0        0    10940 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Global_CISCO_Template.json
--rw-r--r--   0        0        0     2008 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Logging_Template_V01.json
--rw-r--r--   0        0        0    11387 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json
--rw-r--r--   0        0        0    12016 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json
--rw-r--r--   0        0        0     7360 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_BGP_To_OMP.json
--rw-r--r--   0        0        0     1304 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Banner.json
--rw-r--r--   0        0        0    11244 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_System.json
--rw-r--r--   0        0        0    11965 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_VPN0.json
--rw-r--r--   0        0        0    11789 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json
--rw-r--r--   0        0        0    14116 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json
--rw-r--r--   0        0        0    12001 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json
--rw-r--r--   0        0        0     6868 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json
--rw-r--r--   0        0        0    25394 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json
--rw-r--r--   0        0        0     9261 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Regular_BFD.json
--rw-r--r--   0        0        0    25075 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN0_LTE.json
--rw-r--r--   0        0        0    31517 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json
--rw-r--r--   0        0        0    24594 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json
--rw-r--r--   0        0        0     4905 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_UTD_Template.json
--rw-r--r--   0        0        0     9401 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json
--rw-r--r--   0        0        0     9395 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json
--rw-r--r--   0        0        0    14687 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Cellular_Interface.json
--rw-r--r--   0        0        0    19631 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json
--rw-r--r--   0        0        0     6476 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Management_Interface.json
--rw-r--r--   0        0        0     3859 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_Template.json
--rw-r--r--   0        0        0     5139 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json
--rw-r--r--   0        0        0     2081 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Security_Template_V01.json
--rw-r--r--   0        0        0     5654 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_System_Template.json
--rw-r--r--   0        0        0     4100 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json
--rw-r--r--   0        0        0     4109 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json
--rw-r--r--   0        0        0     2609 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_OMP_Template.json
--rw-r--r--   0        0        0      985 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json
--rw-r--r--   0        0        0     4383 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_System_Template.json
--rw-r--r--   0        0        0     3156 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json
--rw-r--r--   0        0        0     1443 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json
--rw-r--r--   0        0        0    34850 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_aaa.json
--rw-r--r--   0        0        0     5402 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0.json
--rw-r--r--   0        0        0    10613 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0_eth1.json
--rw-r--r--   0        0        0      869 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_cli.json
--rw-r--r--   0        0        0    12307 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0.json
--rw-r--r--   0        0        0    29670 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi1_inet.json
--rw-r--r--   0        0        0    27666 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi2_mpls.json
--rw-r--r--   0        0        0    11923 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1.json
--rw-r--r--   0        0        0     3970 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_dhcp.json
--rw-r--r--   0        0        0    13753 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_lan.json
--rw-r--r--   0        0        0     1760 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/config_groups.json
--rw-r--r--   0        0        0    10179 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/device_templates.json
--rw-r--r--   0        0        0      316 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_cli.json
--rw-r--r--   0        0        0      320 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_service.json
--rw-r--r--   0        0        0      322 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_system.json
--rw-r--r--   0        0        0      322 2024-04-25 09:55:09.486199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_transport.json
--rw-r--r--   0        0        0   628759 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_templates.json
--rw-r--r--   0        0        0    20494 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_app.json
--rw-r--r--   0        0        0     1215 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_localapp.json
--rw-r--r--   0        0        0     3440 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_sla.json
--rw-r--r--   0        0        0      532 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_BULK_DATA.json
--rw-r--r--   0        0        0      596 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_Scavengers.json
--rw-r--r--   0        0        0     3010 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Apps.json
--rw-r--r--   0        0        0      904 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Workspace_Apps.json
--rw-r--r--   0        0        0     1605 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Microsoft_Apps.json
--rw-r--r--   0        0        0      450 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/REAL_TIME_APPS.json
--rw-r--r--   0        0        0      386 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/VIDEO_CONF.json
--rw-r--r--   0        0        0     4079 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Voice_Apps.json
--rw-r--r--   0        0        0      452 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/WEB_TOOLS_APP.json
--rw-r--r--   0        0        0      608 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/amazon_aws_apps.json
--rw-r--r--   0        0        0      379 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/box_net_apps.json
--rw-r--r--   0        0        0      380 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/concur_apps.json
--rw-r--r--   0        0        0      383 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/dropbox_apps.json
--rw-r--r--   0        0        0      430 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/gotomeeting_apps.json
--rw-r--r--   0        0        0      380 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/intuit_apps.json
--rw-r--r--   0        0        0     1174 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/office365_apps.json
--rw-r--r--   0        0        0      596 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/oracle_apps.json
--rw-r--r--   0        0        0      392 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/salesforce_apps.json
--rw-r--r--   0        0        0      388 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/sugar_crm_apps.json
--rw-r--r--   0        0        0      962 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/webex_apps.json
--rw-r--r--   0        0        0      383 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/zendesk_apps.json
--rw-r--r--   0        0        0      391 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/zoho_crm_apps.json
--rw-r--r--   0        0        0      386 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/Browsing.json
--rw-r--r--   0        0        0      375 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/ICMP.json
--rw-r--r--   0        0        0      428 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/Yahoo.json
--rw-r--r--   0        0        0      414 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Best-Effort.json
--rw-r--r--   0        0        0      418 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Bulk-Data.json
--rw-r--r--   0        0        0      426 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Business-Critical.json
--rw-r--r--   0        0        0      418 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Business-Data.json
--rw-r--r--   0        0        0      414 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Default.json
--rw-r--r--   0        0        0      407 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Realtime.json
--rw-r--r--   0        0        0      434 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Transactional-Data.json
--rw-r--r--   0        0        0      427 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Voice-And-Video.json
--rw-r--r--   0        0        0       33 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/server_info.json
--rw-r--r--   0        0        0     2564 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/serial_files/serialFile-v1.viptela
--rw-r--r--   0        0        0     2905 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/serial_files/serialFile-v2.viptela
--rw-r--r--   0        0        0      196 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/__init__.py
--rw-r--r--   0        0        0    29688 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/add.py
--rw-r--r--   0        0        0    23332 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/backup.py
--rw-r--r--   0        0        0     1626 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/delete.py
--rw-r--r--   0        0        0     7005 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/deploy.py
--rw-r--r--   0        0        0    17977 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/restore.py
--rw-r--r--   0        0        0     9824 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/setup.py
--rw-r--r--   0        0        0    21040 2024-04-25 09:55:09.490199 catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/utils.py
--rw-r--r--   0        0        0      975 2024-04-25 09:55:09.494200 catalyst_sdwan_lab-2.0.8/pyproject.toml
--rw-r--r--   0        0        0    20446 1970-01-01 00:00:00.000000 catalyst_sdwan_lab-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1516 2024-04-26 13:36:49.974627 catalyst_sdwan_lab-2.0.9/LICENSE
+-rw-r--r--   0        0        0    19200 2024-04-26 13:36:49.974627 catalyst_sdwan_lab-2.0.9/README.md
+-rw-r--r--   0        0        0      357 2024-04-26 13:36:49.974627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/__init__.py
+-rw-r--r--   0        0        0    20068 2024-04-26 13:36:49.974627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/__main__.py
+-rwxr-xr-x   0        0        0      443 2024-04-26 13:36:49.974627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/cacsr_details.txt
+-rw-r--r--   0        0        0     3033 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/chainCA.pem
+-rwxr-xr-x   0        0        0      790 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/openssl-commands.md
+-rw-r--r--   0        0        0     1517 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/rootCA.pem
+-rw-r--r--   0        0        0       17 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/rootCA.srl
+-rwxr-xr-x   0        0        0      485 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/rootca_details.txt
+-rw-r--r--   0        0        0     1074 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/signCA.csr
+-rw-r--r--   0        0        0     1675 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/signCA.key
+-rw-r--r--   0        0        0     1517 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/signCA.pem
+-rwxr-xr-x   0        0        0      352 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/v3ext.cnf
+-rw-r--r--   0        0        0      421 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/backup/controller-cloud-init.j2
+-rw-r--r--   0        0        0      851 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/backup/edge-cloud-init.j2
+-rw-r--r--   0        0        0      523 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/backup/manager-cloud-init.j2
+-rw-r--r--   0        0        0      895 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/backup/sdrouting-cloud-init.j2
+-rw-r--r--   0        0        0      415 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/backup/validator-cloud-init.j2
+-rw-r--r--   0        0        0    16330 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/deploy/cml-base-topology.j2
+-rw-r--r--   0        0        0     2292 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/deploy/controller-cloud-init.j2
+-rw-r--r--   0        0        0     3182 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/deploy/manager-cloud-init.j2
+-rw-r--r--   0        0        0     1383 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/deploy/sdrouting-cloud-init.j2
+-rw-r--r--   0        0        0     2327 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/deploy/validator-cloud-init.j2
+-rw-r--r--   0        0        0     2087 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-controller.yaml
+-rw-r--r--   0        0        0     1981 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-edge.yaml
+-rw-r--r--   0        0        0     2094 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-manager.yaml
+-rw-r--r--   0        0        0     2097 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-validator.yaml
+-rw-r--r--   0        0        0     1859 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1866 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json
+-rw-r--r--   0        0        0     1833 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1736 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json
+-rw-r--r--   0        0        0     1702 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json
+-rw-r--r--   0        0        0     1910 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json
+-rw-r--r--   0        0        0     1686 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_GCP_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1615 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     2516 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     2510 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_ISRv_Template_V01.json
+-rw-r--r--   0        0        0     2293 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json
+-rw-r--r--   0        0        0     2657 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json
+-rw-r--r--   0        0        0     2365 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json
+-rw-r--r--   0        0        0     3215 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_CSR_1000V_V01.json
+-rw-r--r--   0        0        0     2924 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_DC1_HUB.json
+-rw-r--r--   0        0        0     2260 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_ISR_4331_V01.json
+-rw-r--r--   0        0        0     1347 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/controller_basic.json
+-rw-r--r--   0        0        0     2454 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/edge_basic.json
+-rw-r--r--   0        0        0    19645 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json
+-rw-r--r--   0        0        0     7062 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24745 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json
+-rw-r--r--   0        0        0     5515 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json
+-rw-r--r--   0        0        0    12013 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5591 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json
+-rw-r--r--   0        0        0     6135 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24962 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0    11984 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json
+-rw-r--r--   0        0        0     5492 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     5564 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json
+-rw-r--r--   0        0        0     3456 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BFD_Cisco_V01.json
+-rw-r--r--   0        0        0    19638 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BOOTSTRAP_DHCP_V01.json
+-rw-r--r--   0        0        0     9573 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json
+-rw-r--r--   0        0        0    12289 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json
+-rw-r--r--   0        0        0     8173 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_System_Template.json
+-rw-r--r--   0        0        0     2216 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Cellular_V01.json
+-rw-r--r--   0        0        0     6228 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_SVI_V01.json
+-rw-r--r--   0        0        0     1607 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Switch_Port_V01.json
+-rw-r--r--   0        0        0    22837 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json
+-rw-r--r--   0        0        0    10441 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json
+-rw-r--r--   0        0        0    22817 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json
+-rw-r--r--   0        0        0    22819 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json
+-rw-r--r--   0        0        0    10419 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json
+-rw-r--r--   0        0        0    18079 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json
+-rw-r--r--   0        0        0    11073 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json
+-rw-r--r--   0        0        0    11073 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json
+-rw-r--r--   0        0        0    11073 2024-04-26 13:36:49.978627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json
+-rw-r--r--   0        0        0    11095 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json
+-rw-r--r--   0        0        0    11071 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json
+-rw-r--r--   0        0        0    11071 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json
+-rw-r--r--   0        0        0    11075 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json
+-rw-r--r--   0        0        0    11071 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json
+-rw-r--r--   0        0        0     7066 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    25121 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json
+-rw-r--r--   0        0        0     7603 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json
+-rw-r--r--   0        0        0     5572 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json
+-rw-r--r--   0        0        0    11992 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json
+-rw-r--r--   0        0        0     7025 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24720 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5478 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     5550 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN512_V01.json
+-rw-r--r--   0        0        0     2144 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Logging_Cisco_V01.json
+-rw-r--r--   0        0        0     7061 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    25114 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5514 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     4915 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_NTP_Cisco_V01.json
+-rw-r--r--   0        0        0     6290 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_OMP_Cisco_V01.json
+-rw-r--r--   0        0        0    24529 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INET_INT_V01.json
+-rw-r--r--   0        0        0    12375 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json
+-rw-r--r--   0        0        0    12084 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_INT_V01.json
+-rw-r--r--   0        0        0     5570 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json
+-rw-r--r--   0        0        0    12106 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_SVC_INT_V01.json
+-rw-r--r--   0        0        0     8510 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_Service_VPN1_V01.json
+-rw-r--r--   0        0        0    10463 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_VPN0_Template_V01.json
+-rw-r--r--   0        0        0    25674 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json
+-rw-r--r--   0        0        0    13302 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json
+-rw-r--r--   0        0        0    13021 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json
+-rw-r--r--   0        0        0     4729 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json
+-rw-r--r--   0        0        0    13047 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json
+-rw-r--r--   0        0        0     8131 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json
+-rw-r--r--   0        0        0    10082 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json
+-rw-r--r--   0        0        0     2191 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Security_Cisco_V01.json
+-rw-r--r--   0        0        0     5921 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_System_Cisco_V01.json
+-rw-r--r--   0        0        0     6998 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_0_Cisco_V01.json
+-rw-r--r--   0        0        0     4315 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_1_Cisco_V01.json
+-rw-r--r--   0        0        0     4323 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_512_Cisco_V01.json
+-rw-r--r--   0        0        0     6985 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_CISCO_Template.json
+-rw-r--r--   0        0        0    20010 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_Template.json
+-rw-r--r--   0        0        0     3218 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json
+-rw-r--r--   0        0        0     7296 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_Standalone_Template.json
+-rw-r--r--   0        0        0     1739 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_BFD_Template_V01.json
+-rw-r--r--   0        0        0     4104 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_BFD_Template.json
+-rw-r--r--   0        0        0    14537 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json
+-rw-r--r--   0        0        0     4186 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Logging_Template.json
+-rw-r--r--   0        0        0     7502 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json
+-rw-r--r--   0        0        0     4511 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Security_Template.json
+-rw-r--r--   0        0        0     8107 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_System_Template.json
+-rw-r--r--   0        0        0     4416 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_0_Template.json
+-rw-r--r--   0        0        0    13607 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json
+-rw-r--r--   0        0        0     4333 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_Template.json
+-rw-r--r--   0        0        0     3938 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json
+-rw-r--r--   0        0        0    27208 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json
+-rw-r--r--   0        0        0    25438 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json
+-rw-r--r--   0        0        0     8351 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_System.json
+-rw-r--r--   0        0        0     9978 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_VPN0.json
+-rw-r--r--   0        0        0    11257 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json
+-rw-r--r--   0        0        0     4976 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_EIO_System_Template.json
+-rw-r--r--   0        0        0    10714 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Global_CISCO_Template.json
+-rw-r--r--   0        0        0     2008 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Logging_Template_V01.json
+-rw-r--r--   0        0        0    11386 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json
+-rw-r--r--   0        0        0    12016 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json
+-rw-r--r--   0        0        0     7360 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_BGP_To_OMP.json
+-rw-r--r--   0        0        0     1303 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Banner.json
+-rw-r--r--   0        0        0    11243 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_System.json
+-rw-r--r--   0        0        0    11964 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_VPN0.json
+-rw-r--r--   0        0        0    11788 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json
+-rw-r--r--   0        0        0    14115 2024-04-26 13:36:49.982627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json
+-rw-r--r--   0        0        0    12000 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json
+-rw-r--r--   0        0        0     6868 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json
+-rw-r--r--   0        0        0    25394 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json
+-rw-r--r--   0        0        0     9260 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Regular_BFD.json
+-rw-r--r--   0        0        0    25074 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN0_LTE.json
+-rw-r--r--   0        0        0    31516 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json
+-rw-r--r--   0        0        0    24593 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json
+-rw-r--r--   0        0        0     4859 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_UTD_Template.json
+-rw-r--r--   0        0        0     9400 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json
+-rw-r--r--   0        0        0     9394 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json
+-rw-r--r--   0        0        0    14686 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Cellular_Interface.json
+-rw-r--r--   0        0        0    19630 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json
+-rw-r--r--   0        0        0     6475 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Management_Interface.json
+-rw-r--r--   0        0        0     3858 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_Template.json
+-rw-r--r--   0        0        0     5138 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json
+-rw-r--r--   0        0        0     2080 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Security_Template_V01.json
+-rw-r--r--   0        0        0     5653 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_System_Template.json
+-rw-r--r--   0        0        0     4099 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json
+-rw-r--r--   0        0        0     4106 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json
+-rw-r--r--   0        0        0     2608 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_OMP_Template.json
+-rw-r--r--   0        0        0      984 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json
+-rw-r--r--   0        0        0     4382 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_System_Template.json
+-rw-r--r--   0        0        0     3155 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json
+-rw-r--r--   0        0        0     1442 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json
+-rw-r--r--   0        0        0    34849 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_aaa.json
+-rw-r--r--   0        0        0     5401 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0.json
+-rw-r--r--   0        0        0    10612 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0_eth1.json
+-rw-r--r--   0        0        0      868 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_cli.json
+-rw-r--r--   0        0        0    12306 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0.json
+-rw-r--r--   0        0        0    29668 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi1_inet.json
+-rw-r--r--   0        0        0    27664 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi2_mpls.json
+-rw-r--r--   0        0        0    11922 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1.json
+-rw-r--r--   0        0        0     3969 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_dhcp.json
+-rw-r--r--   0        0        0    13751 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_lan.json
+-rw-r--r--   0        0        0     9628 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/inventory/device_templates.json
+-rw-r--r--   0        0        0   597414 2024-04-26 13:36:49.986627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/inventory/feature_templates.json
+-rw-r--r--   0        0        0    14055 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_app.json
+-rw-r--r--   0        0        0     1317 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_localapp.json
+-rw-r--r--   0        0        0     3720 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_sla.json
+-rw-r--r--   0        0        0      532 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_BULK_DATA.json
+-rw-r--r--   0        0        0      596 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_Scavengers.json
+-rw-r--r--   0        0        0     2748 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Google_Apps.json
+-rw-r--r--   0        0        0     1605 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Microsoft_Apps.json
+-rw-r--r--   0        0        0      450 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/REAL_TIME_APPS.json
+-rw-r--r--   0        0        0      386 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/VIDEO_CONF.json
+-rw-r--r--   0        0        0      452 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/WEB_TOOLS_APP.json
+-rw-r--r--   0        0        0      608 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/amazon_aws_apps.json
+-rw-r--r--   0        0        0      379 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/box_net_apps.json
+-rw-r--r--   0        0        0      380 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/concur_apps.json
+-rw-r--r--   0        0        0      383 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/dropbox_apps.json
+-rw-r--r--   0        0        0      430 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/gotomeeting_apps.json
+-rw-r--r--   0        0        0      380 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/intuit_apps.json
+-rw-r--r--   0        0        0     1052 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/office365_apps.json
+-rw-r--r--   0        0        0      596 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/oracle_apps.json
+-rw-r--r--   0        0        0      392 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/salesforce_apps.json
+-rw-r--r--   0        0        0      388 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/sugar_crm_apps.json
+-rw-r--r--   0        0        0      383 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/zendesk_apps.json
+-rw-r--r--   0        0        0      391 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/zoho_crm_apps.json
+-rw-r--r--   0        0        0      386 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/Browsing.json
+-rw-r--r--   0        0        0      375 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/ICMP.json
+-rw-r--r--   0        0        0      428 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/Yahoo.json
+-rw-r--r--   0        0        0      415 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Best-Effort.json
+-rw-r--r--   0        0        0      419 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Bulk-Data.json
+-rw-r--r--   0        0        0      427 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Business-Critical.json
+-rw-r--r--   0        0        0      419 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Business-Data.json
+-rw-r--r--   0        0        0      415 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Default.json
+-rw-r--r--   0        0        0      408 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Realtime.json
+-rw-r--r--   0        0        0      435 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Transactional-Data.json
+-rw-r--r--   0        0        0      428 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Voice-And-Video.json
+-rw-r--r--   0        0        0       32 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/server_info.json
+-rw-r--r--   0        0        0    15002 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/certificates/edge_certificates.json
+-rw-r--r--   0        0        0     1628 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/config_groups/group/edge_basic.json
+-rw-r--r--   0        0        0      295 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/attached/controller_basic.json
+-rw-r--r--   0        0        0     1859 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1866 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json
+-rw-r--r--   0        0        0     1833 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1736 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json
+-rw-r--r--   0        0        0     1702 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json
+-rw-r--r--   0        0        0     1910 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json
+-rw-r--r--   0        0        0     1720 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_ICGW_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1686 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_GCP_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1615 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     2516 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     2510 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_ISRv_Template_V01.json
+-rw-r--r--   0        0        0     2293 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json
+-rw-r--r--   0        0        0     2657 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json
+-rw-r--r--   0        0        0     2365 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json
+-rw-r--r--   0        0        0     3207 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C8000V_V01.json
+-rw-r--r--   0        0        0     2924 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_DC1_HUB.json
+-rw-r--r--   0        0        0     2260 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_ISR_4331_V01.json
+-rw-r--r--   0        0        0     1347 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/controller_basic.json
+-rw-r--r--   0        0        0     2454 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/edge_basic.json
+-rw-r--r--   0        0        0     4130 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/values/controller_basic.json
+-rw-r--r--   0        0        0      776 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/cli/edge_basic_cli.json
+-rw-r--r--   0        0        0     6515 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/service/edge_basic_lan.json
+-rw-r--r--   0        0        0    12229 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/system/edge_basic_system.json
+-rw-r--r--   0        0        0    13293 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/transport/edge_basic_wan.json
+-rw-r--r--   0        0        0    20244 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json
+-rw-r--r--   0        0        0     7063 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24746 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json
+-rw-r--r--   0        0        0     5516 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json
+-rw-r--r--   0        0        0    12014 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5592 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json
+-rw-r--r--   0        0        0     6136 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24963 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0    11984 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json
+-rw-r--r--   0        0        0     5493 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     5565 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json
+-rw-r--r--   0        0        0     3457 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BFD_Cisco_V01.json
+-rw-r--r--   0        0        0    20238 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BOOTSTRAP_DHCP_V01.json
+-rw-r--r--   0        0        0    10172 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json
+-rw-r--r--   0        0        0    12888 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json
+-rw-r--r--   0        0        0     8773 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_System_Template.json
+-rw-r--r--   0        0        0     2216 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Cellular_V01.json
+-rw-r--r--   0        0        0     6229 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_SVI_V01.json
+-rw-r--r--   0        0        0     1608 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Switch_Port_V01.json
+-rw-r--r--   0        0        0    22838 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json
+-rw-r--r--   0        0        0    10442 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json
+-rw-r--r--   0        0        0    22818 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json
+-rw-r--r--   0        0        0    22820 2024-04-26 13:36:49.990627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json
+-rw-r--r--   0        0        0    10420 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json
+-rw-r--r--   0        0        0    18100 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json
+-rw-r--r--   0        0        0    11094 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json
+-rw-r--r--   0        0        0    11094 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json
+-rw-r--r--   0        0        0    11094 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json
+-rw-r--r--   0        0        0    11115 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json
+-rw-r--r--   0        0        0    11091 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json
+-rw-r--r--   0        0        0    11092 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json
+-rw-r--r--   0        0        0    11095 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json
+-rw-r--r--   0        0        0    11092 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json
+-rw-r--r--   0        0        0     9231 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_C8000V_GLOBAL_CISCO_V01.json
+-rw-r--r--   0        0        0     7813 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0     9262 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_DNS_V01.json
+-rw-r--r--   0        0        0    28713 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_INTF_GE2_V01.json
+-rw-r--r--   0        0        0     7245 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN512_V01.json
+-rw-r--r--   0        0        0     7067 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    25122 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json
+-rw-r--r--   0        0        0     7604 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json
+-rw-r--r--   0        0        0     5573 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json
+-rw-r--r--   0        0        0    11993 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json
+-rw-r--r--   0        0        0     7026 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24721 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5479 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     5551 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN512_V01.json
+-rw-r--r--   0        0        0     2145 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Logging_Cisco_V01.json
+-rw-r--r--   0        0        0     7062 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    25115 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5515 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     4936 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_NTP_Cisco_V01.json
+-rw-r--r--   0        0        0     6311 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_OMP_Cisco_V01.json
+-rw-r--r--   0        0        0    24530 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INET_INT_V01.json
+-rw-r--r--   0        0        0    12376 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json
+-rw-r--r--   0        0        0    12085 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_INT_V01.json
+-rw-r--r--   0        0        0     5570 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json
+-rw-r--r--   0        0        0    12106 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_SVC_INT_V01.json
+-rw-r--r--   0        0        0     8511 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_Service_VPN1_V01.json
+-rw-r--r--   0        0        0    10464 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_VPN0_Template_V01.json
+-rw-r--r--   0        0        0    25675 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json
+-rw-r--r--   0        0        0    13303 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json
+-rw-r--r--   0        0        0    13022 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json
+-rw-r--r--   0        0        0     4730 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json
+-rw-r--r--   0        0        0    13048 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json
+-rw-r--r--   0        0        0     8132 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json
+-rw-r--r--   0        0        0    10083 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json
+-rw-r--r--   0        0        0     2192 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Security_Cisco_V01.json
+-rw-r--r--   0        0        0     5922 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_System_Cisco_V01.json
+-rw-r--r--   0        0        0     7019 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_0_Cisco_V01.json
+-rw-r--r--   0        0        0     4336 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_1_Cisco_V01.json
+-rw-r--r--   0        0        0     4343 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_512_Cisco_V01.json
+-rw-r--r--   0        0        0     7211 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_CISCO_Template.json
+-rw-r--r--   0        0        0    20011 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_Template.json
+-rw-r--r--   0        0        0     3219 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json
+-rw-r--r--   0        0        0     7321 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_Standalone_Template.json
+-rw-r--r--   0        0        0     1740 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_BFD_Template_V01.json
+-rw-r--r--   0        0        0     4330 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_BFD_Template.json
+-rw-r--r--   0        0        0    14763 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json
+-rw-r--r--   0        0        0     4412 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Logging_Template.json
+-rw-r--r--   0        0        0     7728 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json
+-rw-r--r--   0        0        0     4737 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Security_Template.json
+-rw-r--r--   0        0        0     8333 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_System_Template.json
+-rw-r--r--   0        0        0     4642 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_0_Template.json
+-rw-r--r--   0        0        0    13632 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json
+-rw-r--r--   0        0        0     4561 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_Template.json
+-rw-r--r--   0        0        0     3938 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json
+-rw-r--r--   0        0        0    27208 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json
+-rw-r--r--   0        0        0    25439 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json
+-rw-r--r--   0        0        0     8352 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_System.json
+-rw-r--r--   0        0        0     9978 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_VPN0.json
+-rw-r--r--   0        0        0    11258 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json
+-rw-r--r--   0        0        0     5397 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_EIO_System_Template.json
+-rw-r--r--   0        0        0    10940 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Global_CISCO_Template.json
+-rw-r--r--   0        0        0     2008 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Logging_Template_V01.json
+-rw-r--r--   0        0        0    11387 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json
+-rw-r--r--   0        0        0    12016 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json
+-rw-r--r--   0        0        0     7360 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_BGP_To_OMP.json
+-rw-r--r--   0        0        0     1304 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Banner.json
+-rw-r--r--   0        0        0    11244 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_System.json
+-rw-r--r--   0        0        0    11965 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_VPN0.json
+-rw-r--r--   0        0        0    11789 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json
+-rw-r--r--   0        0        0    14116 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json
+-rw-r--r--   0        0        0    12001 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json
+-rw-r--r--   0        0        0     6868 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json
+-rw-r--r--   0        0        0    25394 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json
+-rw-r--r--   0        0        0     9261 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Regular_BFD.json
+-rw-r--r--   0        0        0    25075 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN0_LTE.json
+-rw-r--r--   0        0        0    31517 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json
+-rw-r--r--   0        0        0    24594 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json
+-rw-r--r--   0        0        0     4905 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_UTD_Template.json
+-rw-r--r--   0        0        0     9401 2024-04-26 13:36:49.994627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json
+-rw-r--r--   0        0        0     9395 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json
+-rw-r--r--   0        0        0    14687 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Cellular_Interface.json
+-rw-r--r--   0        0        0    19631 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json
+-rw-r--r--   0        0        0     6476 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Management_Interface.json
+-rw-r--r--   0        0        0     3859 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_Template.json
+-rw-r--r--   0        0        0     5139 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json
+-rw-r--r--   0        0        0     2081 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Security_Template_V01.json
+-rw-r--r--   0        0        0     5654 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_System_Template.json
+-rw-r--r--   0        0        0     4100 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json
+-rw-r--r--   0        0        0     4109 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json
+-rw-r--r--   0        0        0     2609 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_OMP_Template.json
+-rw-r--r--   0        0        0      985 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json
+-rw-r--r--   0        0        0     4383 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_System_Template.json
+-rw-r--r--   0        0        0     3156 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json
+-rw-r--r--   0        0        0     1443 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json
+-rw-r--r--   0        0        0    34850 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_aaa.json
+-rw-r--r--   0        0        0     5402 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0.json
+-rw-r--r--   0        0        0    10613 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0_eth1.json
+-rw-r--r--   0        0        0      869 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_cli.json
+-rw-r--r--   0        0        0    12307 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0.json
+-rw-r--r--   0        0        0    29670 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi1_inet.json
+-rw-r--r--   0        0        0    27666 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi2_mpls.json
+-rw-r--r--   0        0        0    11923 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1.json
+-rw-r--r--   0        0        0     3970 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_dhcp.json
+-rw-r--r--   0        0        0    13753 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_lan.json
+-rw-r--r--   0        0        0     1760 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/config_groups.json
+-rw-r--r--   0        0        0    10179 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/device_templates.json
+-rw-r--r--   0        0        0      316 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_cli.json
+-rw-r--r--   0        0        0      320 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_service.json
+-rw-r--r--   0        0        0      322 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_system.json
+-rw-r--r--   0        0        0      322 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_transport.json
+-rw-r--r--   0        0        0   628759 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_templates.json
+-rw-r--r--   0        0        0    20494 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_app.json
+-rw-r--r--   0        0        0     1215 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_localapp.json
+-rw-r--r--   0        0        0     3440 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_sla.json
+-rw-r--r--   0        0        0      532 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_BULK_DATA.json
+-rw-r--r--   0        0        0      596 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_Scavengers.json
+-rw-r--r--   0        0        0     3010 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Apps.json
+-rw-r--r--   0        0        0      904 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Workspace_Apps.json
+-rw-r--r--   0        0        0     1605 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Microsoft_Apps.json
+-rw-r--r--   0        0        0      450 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/REAL_TIME_APPS.json
+-rw-r--r--   0        0        0      386 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/VIDEO_CONF.json
+-rw-r--r--   0        0        0     4079 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Voice_Apps.json
+-rw-r--r--   0        0        0      452 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/WEB_TOOLS_APP.json
+-rw-r--r--   0        0        0      608 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/amazon_aws_apps.json
+-rw-r--r--   0        0        0      379 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/box_net_apps.json
+-rw-r--r--   0        0        0      380 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/concur_apps.json
+-rw-r--r--   0        0        0      383 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/dropbox_apps.json
+-rw-r--r--   0        0        0      430 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/gotomeeting_apps.json
+-rw-r--r--   0        0        0      380 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/intuit_apps.json
+-rw-r--r--   0        0        0     1174 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/office365_apps.json
+-rw-r--r--   0        0        0      596 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/oracle_apps.json
+-rw-r--r--   0        0        0      392 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/salesforce_apps.json
+-rw-r--r--   0        0        0      388 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/sugar_crm_apps.json
+-rw-r--r--   0        0        0      962 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/webex_apps.json
+-rw-r--r--   0        0        0      383 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/zendesk_apps.json
+-rw-r--r--   0        0        0      391 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/zoho_crm_apps.json
+-rw-r--r--   0        0        0      386 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/Browsing.json
+-rw-r--r--   0        0        0      375 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/ICMP.json
+-rw-r--r--   0        0        0      428 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/Yahoo.json
+-rw-r--r--   0        0        0      414 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Best-Effort.json
+-rw-r--r--   0        0        0      418 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Bulk-Data.json
+-rw-r--r--   0        0        0      426 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Business-Critical.json
+-rw-r--r--   0        0        0      418 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Business-Data.json
+-rw-r--r--   0        0        0      414 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Default.json
+-rw-r--r--   0        0        0      407 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Realtime.json
+-rw-r--r--   0        0        0      434 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Transactional-Data.json
+-rw-r--r--   0        0        0      427 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Voice-And-Video.json
+-rw-r--r--   0        0        0       33 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/server_info.json
+-rw-r--r--   0        0        0     2564 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/serial_files/serialFile-v1.viptela
+-rw-r--r--   0        0        0     2905 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/serial_files/serialFile-v2.viptela
+-rw-r--r--   0        0        0      196 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/__init__.py
+-rw-r--r--   0        0        0    29688 2024-04-26 13:36:49.998627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/add.py
+-rw-r--r--   0        0        0    23332 2024-04-26 13:36:50.002627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/backup.py
+-rw-r--r--   0        0        0     1626 2024-04-26 13:36:50.002627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/delete.py
+-rw-r--r--   0        0        0     7005 2024-04-26 13:36:50.002627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/deploy.py
+-rw-r--r--   0        0        0    17977 2024-04-26 13:36:50.002627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/restore.py
+-rw-r--r--   0        0        0     9824 2024-04-26 13:36:50.002627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/setup.py
+-rw-r--r--   0        0        0    21040 2024-04-26 13:36:50.002627 catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/utils.py
+-rw-r--r--   0        0        0      975 2024-04-26 13:36:50.002627 catalyst_sdwan_lab-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    20446 1970-01-01 00:00:00.000000 catalyst_sdwan_lab-2.0.9/PKG-INFO
```

### Comparing `catalyst_sdwan_lab-2.0.8/LICENSE` & `catalyst_sdwan_lab-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/README.md` & `catalyst_sdwan_lab-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/__main__.py` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/__main__.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/chainCA.pem` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/chainCA.pem`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/openssl-commands.md` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/openssl-commands.md`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/rootCA.pem` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/rootCA.pem`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/signCA.csr` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/signCA.csr`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/signCA.key` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/signCA.key`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/certs/signCA.pem` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/certs/signCA.pem`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/backup/edge-cloud-init.j2` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/backup/edge-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/backup/manager-cloud-init.j2` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/backup/manager-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/backup/sdrouting-cloud-init.j2` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/backup/sdrouting-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/deploy/cml-base-topology.j2` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/deploy/cml-base-topology.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/deploy/controller-cloud-init.j2` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/deploy/controller-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/deploy/manager-cloud-init.j2` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/deploy/manager-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/deploy/sdrouting-cloud-init.j2` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/deploy/sdrouting-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_lab_definition/deploy/validator-cloud-init.j2` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_lab_definition/deploy/validator-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-controller.yaml` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-controller.yaml`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-edge.yaml` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-edge.yaml`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-manager.yaml` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-manager.yaml`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-validator.yaml` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-validator.yaml`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_GCP_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_GCP_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_ISRv_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_ISRv_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_CSR_1000V_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_CSR_1000V_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_DC1_HUB.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_DC1_HUB.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_ISR_4331_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_ISR_4331_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/controller_basic.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/controller_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/edge_basic.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/edge_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BFD_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BFD_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BOOTSTRAP_DHCP_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BOOTSTRAP_DHCP_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_System_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Cellular_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Cellular_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_SVI_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_SVI_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Switch_Port_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Switch_Port_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Logging_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Logging_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_NTP_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_NTP_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_OMP_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_OMP_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INET_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INET_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_SVC_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_SVC_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_Service_VPN1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_Service_VPN1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_VPN0_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_VPN0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Security_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Security_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_System_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_System_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_0_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_0_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_1_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_1_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_512_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_512_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_CISCO_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_CISCO_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_Standalone_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_Standalone_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_BFD_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_BFD_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_BFD_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_BFD_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Logging_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Logging_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Security_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Security_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_System_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_0_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_0_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_System.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_VPN0.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_VPN0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_EIO_System_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_EIO_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Global_CISCO_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Global_CISCO_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Logging_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Logging_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_BGP_To_OMP.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_BGP_To_OMP.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Banner.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Banner.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_System.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_VPN0.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_VPN0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Regular_BFD.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Regular_BFD.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN0_LTE.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN0_LTE.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_UTD_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_UTD_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Cellular_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Cellular_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Management_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Management_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Security_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Security_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_System_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_OMP_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_OMP_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_System_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_aaa.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_aaa.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0_eth1.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0_eth1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_cli.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_cli.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi1_inet.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi1_inet.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi2_mpls.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi2_mpls.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_dhcp.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_dhcp.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_lan.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_lan.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/inventory/device_templates.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/inventory/device_templates.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/inventory/feature_templates.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/inventory/feature_templates.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_app.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_app.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_localapp.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_localapp.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_sla.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_sla.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_BULK_DATA.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_BULK_DATA.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_Scavengers.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_Scavengers.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Google_Apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Google_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Microsoft_Apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Microsoft_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/amazon_aws_apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/amazon_aws_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/office365_apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/office365_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/oracle_apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/oracle_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/certificates/edge_certificates.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/certificates/edge_certificates.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/config_groups/group/edge_basic.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/config_groups/group/edge_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_ICGW_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_ICGW_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_GCP_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_GCP_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_ISRv_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_ISRv_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C8000V_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C8000V_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_DC1_HUB.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_DC1_HUB.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_ISR_4331_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_ISR_4331_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/controller_basic.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/controller_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/edge_basic.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/edge_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/values/controller_basic.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/values/controller_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/cli/edge_basic_cli.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/cli/edge_basic_cli.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/service/edge_basic_lan.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/service/edge_basic_lan.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/system/edge_basic_system.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/system/edge_basic_system.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/transport/edge_basic_wan.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/transport/edge_basic_wan.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BFD_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BFD_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BOOTSTRAP_DHCP_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BOOTSTRAP_DHCP_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_System_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Cellular_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Cellular_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_SVI_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_SVI_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Switch_Port_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Switch_Port_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_C8000V_GLOBAL_CISCO_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_C8000V_GLOBAL_CISCO_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_DNS_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_DNS_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_INTF_GE2_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_INTF_GE2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Logging_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Logging_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_NTP_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_NTP_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_OMP_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_OMP_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INET_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INET_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_SVC_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_SVC_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_Service_VPN1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_Service_VPN1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_VPN0_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_VPN0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Security_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Security_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_System_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_System_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_0_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_0_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_1_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_1_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_512_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_512_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_CISCO_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_CISCO_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_Standalone_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_Standalone_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_BFD_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_BFD_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_BFD_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_BFD_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Logging_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Logging_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Security_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Security_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_System_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_0_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_0_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_System.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_VPN0.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_VPN0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_EIO_System_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_EIO_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Global_CISCO_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Global_CISCO_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Logging_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Logging_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_BGP_To_OMP.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_BGP_To_OMP.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Banner.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Banner.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_System.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_VPN0.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_VPN0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Regular_BFD.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Regular_BFD.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN0_LTE.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN0_LTE.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_UTD_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_UTD_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Cellular_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Cellular_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Management_Interface.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Management_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Security_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Security_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_System_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_OMP_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_OMP_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_System_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_aaa.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_aaa.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0_eth1.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0_eth1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_cli.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_cli.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi1_inet.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi1_inet.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi2_mpls.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi2_mpls.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_dhcp.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_dhcp.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_lan.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_lan.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/config_groups.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/config_groups.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/device_templates.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/device_templates.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_templates.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_templates.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_app.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_app.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_localapp.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_localapp.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_sla.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_sla.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_BULK_DATA.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_BULK_DATA.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_Scavengers.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_Scavengers.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Workspace_Apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Workspace_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Microsoft_Apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Microsoft_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Voice_Apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Voice_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/amazon_aws_apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/amazon_aws_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/office365_apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/office365_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/oracle_apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/oracle_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/webex_apps.json` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/webex_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/serial_files/serialFile-v1.viptela` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/serial_files/serialFile-v1.viptela`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/data/serial_files/serialFile-v2.viptela` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/data/serial_files/serialFile-v2.viptela`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/add.py` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/add.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/backup.py` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/backup.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/delete.py` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/deploy.py` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/restore.py` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/restore.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/setup.py` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/setup.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/catalyst_sdwan_lab/tasks/utils.py` & `catalyst_sdwan_lab-2.0.9/catalyst_sdwan_lab/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.8/pyproject.toml` & `catalyst_sdwan_lab-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catalyst-sdwan-lab"
-version = "2.0.8"
+version = "2.0.9"
 description = "Catalyst SD-WAN Lab Deployment Tool - Automation Tool for managing Cisco Catalyst SD-WAN labs inside Cisco Modelling Labs"
 license = "BSD-3-Clause"
 authors = ["Tomasz Zarski <tzarski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/cisco-open/sdwan-lab-deployment-tool"
 keywords = ["cisco", "catalyst", "sdwan", "lab"]
```

### Comparing `catalyst_sdwan_lab-2.0.8/PKG-INFO` & `catalyst_sdwan_lab-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalyst-sdwan-lab
-Version: 2.0.8
+Version: 2.0.9
 Summary: Catalyst SD-WAN Lab Deployment Tool - Automation Tool for managing Cisco Catalyst SD-WAN labs inside Cisco Modelling Labs
 Home-page: https://github.com/cisco-open/sdwan-lab-deployment-tool
 License: BSD-3-Clause
 Keywords: cisco,catalyst,sdwan,lab
 Author: Tomasz Zarski
 Author-email: tzarski@cisco.com
 Requires-Python: >=3.9,<4.0
```

