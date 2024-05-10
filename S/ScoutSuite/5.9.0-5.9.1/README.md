# Comparing `tmp/ScoutSuite-5.9.0.tar.gz` & `tmp/ScoutSuite-5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ScoutSuite-5.9.0.tar", last modified: Thu Jul  2 11:33:22 2020, max compression
+gzip compressed data, was "dist/ScoutSuite-5.9.1.tar", last modified: Tue Jul 28 14:57:45 2020, max compression
```

## Comparing `ScoutSuite-5.9.0.tar` & `ScoutSuite-5.9.1.tar`

### file list

```diff
@@ -1,952 +1,952 @@
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/
--rwxr-xr-x   0 xga       (1000) xga       (1000)    15170 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/LICENSE
--rwxr-xr-x   0 xga       (1000) xga       (1000)      628 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/MANIFEST.in
--rw-r--r--   0 xga       (1000) xga       (1000)     3978 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/PKG-INFO
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2667 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/README.md
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      215 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)    14285 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/__main__.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/core/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)    20619 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/cli_parser.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     9917 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/conditions.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     9034 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/console.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1305 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/exceptions.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2849 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/fs.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4505 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/processingengine.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     6725 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/rule.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3558 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/rule_definition.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     9551 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/ruleset.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     7003 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/server.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4226 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/core/utils.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/data/
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/data/aws/
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/data/aws/ip-ranges/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      115 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/data/aws/ip-ranges/aws-in-ec2.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      120 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/data/aws/ip-ranges/aws-in-us.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)   502517 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/data/aws/ip-ranges/aws.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     8262 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/data/icmp_message_types.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3456 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/data/protocols.json
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/__init__.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/conditionals/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      430 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/conditionals/json_format.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      373 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/conditionals/sqlite_format.html
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1276 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/about_scoutsuite.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1355 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/accordion.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      934 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/accordion_policy.html
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1732 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/left_menu_for_aliyun_region.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2625 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.actiontrail.trails.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)    11807 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.ecs.regions.id.instances.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2400 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.kms.regions.id.keys.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1267 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.oss.buckets.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2256 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.ram.groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2497 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.ram.policies.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1821 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.ram.roles.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3549 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.ram.users.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5339 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.rds.regions.id.instances.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3694 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.vpc.regions.id.vpcs.html
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1736 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/left_menu_for_region.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2199 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/left_menu_for_vpc.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4956 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.acm.regions.id.certificates.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3053 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.awslambda.regions.id.functions.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2704 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.cloudformation.regions.id.stacks.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1341 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.cloudtrail.regions.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3067 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.cloudtrail.regions.id.trails.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2101 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.cloudwatch.regions.id.alarms.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1937 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.config.regions.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1282 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.config.regions.id.recorders.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1183 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.config.regions.id.rules.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1388 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.snapshots.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      853 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.volumes.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1195 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.images.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3625 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.instances.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2182 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.security_groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1475 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.vpcs.security_groups.resource_list.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2509 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.vpcs.security_groups.rule_list.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      590 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.parameter_groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      587 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.security_groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      609 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.subnet_groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      645 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.vpcs.id.clusters.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2191 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.elb_policies.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3858 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcs.id.elbs.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1380 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcs.id.elbs.linked_resources.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      442 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcs.id.elbs.listener.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      543 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcsid.elbs.linked_policy.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3634 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elbv2.regions.id.vpcs.id.lbs.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3226 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.emr.regions.id.vpcs.id.clusters.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2956 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.credential_reports.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1643 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      752 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.inline_policies.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1373 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.managed_policies.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      725 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.managed_policies_list.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2980 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.roles.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3145 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.users.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2744 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.kms.regions.id.keys.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1873 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.parameter_groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1195 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.security_groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3391 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.instances.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1993 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.snapshots.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      635 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.subnet_groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1262 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.parameter_groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2813 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.vpcs.id.clusters.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1618 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.vpcs.id.security_groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      407 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.vpcs.cluster_nodes.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1722 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.route53.regions.id.domains.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1483 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.route53.regions.id.hosted_zones.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2833 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.s3.acls.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2929 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.s3.bucket_iam_policies.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4683 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.s3.buckets.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1594 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.s3.buckets.objects.html
--rw-r--r--   0 xga       (1000) xga       (1000)     1200 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.s3.public_access_block_configuration.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1670 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.secretsmanager.regions.id.secrets.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1418 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ses.regions.id.identities.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2872 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.sns.regions.id.topics.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1804 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.sqs.regions.id.queues.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1340 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.stackdriverlogging.sinks.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2400 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.peering_connections.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3370 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1554 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.flow_logs.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3420 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.network_acls.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      788 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.peering_connections.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2921 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.subnets.html
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      839 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/details_for_subscription.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1730 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/left_menu_for_subscription.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3782 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.aad.applications.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3074 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.aad.groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4279 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.aad.service_principals.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3741 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.aad.users.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     6592 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.appservice.subscriptions.id.web_apps.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1419 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.keyvault.subscriptions.id.vaults.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2255 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.application_security_groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     7912 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.network_interfaces.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     7482 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.security_groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4271 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.virtual_networks.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4619 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.virtual_networks.id.subnets.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1644 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.watchers.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3944 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.rbac.subscriptions.id.roles.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1446 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.auto_provisioning_settings.html
--rw-r--r--   0 xga       (1000) xga       (1000)     1465 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.compliance_results.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1295 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.pricings.html
--rw-r--r--   0 xga       (1000) xga       (1000)     2793 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.regulatory_compliance_results.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2022 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.security_contacts.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5053 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.sqldatabase.subscriptions.id.servers.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2913 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.storageaccounts.subscriptions.id.storage_accounts.html
--rw-r--r--   0 xga       (1000) xga       (1000)     3417 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.disks.html
--rw-r--r--   0 xga       (1000) xga       (1000)     1781 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.images.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4445 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.instances.html
--rw-r--r--   0 xga       (1000) xga       (1000)     3310 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.snapshots.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      377 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/count_badge.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4882 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/dashboard.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      594 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/details.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      772 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/details_for_region.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      886 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/details_for_vpc.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      825 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/ec2_grants.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      317 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/filters.html
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      920 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/details_for_gcp_region.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      904 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/details_for_gcp_zone.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      804 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/details_for_project.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2361 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/left_menu_for_gcp_region.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2333 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/left_menu_for_gcp_zone.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1675 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/left_menu_for_project.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3107 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.cloudsql.projects.id.instances.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4228 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.cloudstorage.projects.id.buckets.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4583 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.firewalls.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1775 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.networks.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2865 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.regions.id.subnetworks.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1808 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.snapshots.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5387 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.zones.id.instances.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3193 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.bindings.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1509 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3559 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.service_accounts.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1497 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.users.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2924 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.kms.projects.id.keyrings.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1677 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.stackdriverlogging.projects.id.metrics.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1644 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.stackdriverlogging.projects.id.sinks.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2070 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.stackdrivermonitoring.projects.id.alert_policies.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2298 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.stackdrivermonitoring.projects.id.uptime_checks.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      582 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/generic_object.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      641 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/ip_grants.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1765 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/last_run_details.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      801 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/left_menu.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     6661 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/metadata.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      822 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/modal.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2694 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/network_interface.html
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/oci/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2659 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/oci/services.identity.groups.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1661 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/oci/services.identity.policies.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1720 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/oci/services.identity.users.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4283 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/oci/services.kms.keyvaults.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3379 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/oci/services.objectstorage.buckets.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      813 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/policy.html
--rw-r--r--   0 xga       (1000) xga       (1000)      308 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/report_footer.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      373 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/resource_link.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1844 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/resources_details.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      317 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/singles.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     8643 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/report.html
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aliyun/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2512 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aliyun/services.ram.password_policy.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1995 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aliyun/services.ram.security_policy.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1257 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/attack_surface.html
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aws/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      197 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aws/services.ec2.external_attack_surface.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      197 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aws/services.elb.external_attack_surface.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      201 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aws/services.elbv2.external_attack_surface.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2873 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aws/services.iam.password_policy.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4287 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aws/services.iam.permissions.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      197 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aws/services.rds.external_attack_surface.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      208 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aws/services.redshift.external_attack_surface.html
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/azure/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/azure/.keep
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/gcp/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/gcp/.keep
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/oci/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1917 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/oci/services.identity.password_policy.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      222 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/service_groups.compute.summaries.external_attack_surface.html
--rwxr-xr-x   0 xga       (1000) xga       (1000)      223 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/service_groups.database.summaries.external_attack_surface.html
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/css/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      510 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/css/modal.css
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2212 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite-dark.css
--rwxr-xr-x   0 xga       (1000) xga       (1000)      751 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite-light.css
--rwxr-xr-x   0 xga       (1000) xga       (1000)     8562 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite.css
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1150 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/favicon.ico
--rwxr-xr-x   0 xga       (1000) xga       (1000)    15066 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/helpers.js
--rwxr-xr-x   0 xga       (1000) xga       (1000)     6944 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/pagination.js
--rwxr-xr-x   0 xga       (1000) xga       (1000)      253 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/provider.js
--rwxr-xr-x   0 xga       (1000) xga       (1000)    44449 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/scoutsuite.js
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4436 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/sqlite.js
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2244 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/theme.js
--rwxr-xr-x   0 xga       (1000) xga       (1000)  2409097 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/includes.zip
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/listall-configs/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      152 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/data/listall-configs/ec2.regions.id.vpcs.id.security_groups.id.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     6770 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/html.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5118 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/result_encoder.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3241 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/output/utils.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2305 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/__init__.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1437 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/authentication_strategy.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      835 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/actiontrail.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2081 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      861 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/ecs.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1745 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/kms.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      620 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/oss.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     7572 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/ram.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      865 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/rds.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2539 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/utils.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      821 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/vpc.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1693 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/metadata.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1356 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/provider.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/__init__.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/actiontrail/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/actiontrail/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      353 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/actiontrail/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1223 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/actiontrail/trails.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      916 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/base.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ecs/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ecs/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      380 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ecs/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4429 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ecs/instances.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/kms/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/kms/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      360 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/kms/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1603 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/kms/keys.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/oss/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/oss/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      341 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/oss/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      646 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/oss/buckets.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      994 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/api_keys.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3104 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1157 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/groups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1712 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/password_policy.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2814 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/policies.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      888 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/roles.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1748 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/security_policy.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1798 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/users.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/rds/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/rds/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      381 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/rds/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2458 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/rds/instances.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1359 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/regions.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/vpc/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/vpc/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      360 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/vpc/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1712 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/vpc/vpcs.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      332 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/actiontrail-not-configured.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      375 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/actiontrail-not-enabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      531 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ecs-instance-with-deletion-protection-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      531 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ecs-instance-with-public-ip.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      619 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/kms-no-key-rotation.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      422 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-expiration-threshold.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      345 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-minimum-length.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      264 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-no-expiration.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      290 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-no-lowercase-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      274 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-no-number-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      274 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-no-symbol-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      290 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-no-uppercase-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      266 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-reuse-enabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      486 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-user-lacking-mfa.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      317 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-user-unused-api-key.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      324 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-user-unused-console-password.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      371 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-user-with-multiple-api-keys.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      314 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ram-user-with-old-api-key.json
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/rulesets/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2384 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/rulesets/default.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)       74 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/rulesets/filters.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1113 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/services.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      818 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/utils.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1862 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/authentication_strategy.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1194 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/acm.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1998 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/awslambda.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)    14062 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      138 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/basefacade.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2659 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/cloudformation.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1794 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/cloudtrail.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      583 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/cloudwatch.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1779 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/config.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      666 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/directconnect.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     8881 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/ec2.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2677 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/efs.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3778 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/elasticache.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4758 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/elb.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3104 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/elbv2.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1152 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/emr.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)    12122 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/iam.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2911 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/kms.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     9151 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/rds.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2526 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/redshift.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1379 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/route53.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)    13622 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/s3.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      545 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/secretsmanager.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2173 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/ses.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2132 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/sns.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1496 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/sqs.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4111 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/utils.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)    18912 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/metadata.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)    43339 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/provider.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/__init__.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/acm/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/acm/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      358 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/acm/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      872 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/acm/certificates.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/awslambda/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/awslambda/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      339 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/awslambda/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2957 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/awslambda/functions.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      810 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/base.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudformation/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudformation/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      348 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudformation/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2390 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudformation/stacks.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudtrail/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudtrail/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1280 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudtrail/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3152 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudtrail/trails.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudwatch/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudwatch/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1031 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudwatch/alarms.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      337 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudwatch/base.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/config/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/config/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      469 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/config/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1270 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/config/recorders.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1170 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/config/rules.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/directconnect/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/directconnect/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      366 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/directconnect/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      800 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/directconnect/connections.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      721 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/ami.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1715 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3190 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/instances.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      869 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/networkinterfaces.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4184 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/securitygroups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1037 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/snapshots.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      780 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/volumes.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      478 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/vpcs.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/efs/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/efs/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      336 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/efs/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      864 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/efs/filesystems.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1562 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      735 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/cluster.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      953 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/parametergroups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      797 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/securitygroups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      809 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/subnetgroups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      345 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/vpcs.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elb/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elb/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      381 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elb/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1840 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elb/load_balancers.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      773 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elb/policies.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      179 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elb/vpcs.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elbv2/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elbv2/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      324 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elbv2/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      845 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elbv2/listeners.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2214 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elbv2/load_balancers.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      180 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elbv2/vpcs.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/emr/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/emr/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      810 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/emr/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      728 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/emr/clusters.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      730 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/emr/vpcs.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     7214 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1870 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/credentialreports.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      662 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/groups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1353 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/passwordpolicy.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      701 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/policies.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1186 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/roles.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      599 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/users.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/kms/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/kms/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      309 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/kms/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1190 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/kms/grants.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3269 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/kms/keys.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1640 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1598 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/instances.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1094 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/parametergroups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      866 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/securitygroups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1778 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/snapshots.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      794 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/subnetgroups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      438 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/vpcs.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      565 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2033 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/cluster_parameter_groups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      917 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/cluster_parameters.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      823 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/cluster_security_groups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      735 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/clusters.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      173 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/vpcs.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1406 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/regions.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/route53/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/route53/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      416 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/route53/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1016 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/route53/domains.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1226 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/route53/hosted_zones.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/s3/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/s3/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2331 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/s3/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      921 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/s3/buckets.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/secretsmanager/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/secretsmanager/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      342 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/secretsmanager/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1015 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/secretsmanager/secrets.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ses/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ses/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      332 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ses/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1352 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ses/identities.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      629 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ses/identity_policies.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sns/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sns/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      316 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sns/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1063 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sns/subscriptions.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1573 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sns/topics.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sqs/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sqs/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      316 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sqs/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1253 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sqs/queues.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2149 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      705 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/flow_logs.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2250 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/network_acls.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      845 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/peering_connections.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1049 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/subnets.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      246 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/vpcs.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1438 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpcs.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/conditions/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      114 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/conditions/cidr-is-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)       93 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/conditions/ec2-security-group-in-use.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)       96 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/conditions/ec2-security-group-not-used.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      257 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/conditions/instance-with-open-nacls.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      345 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/conditions/instance-with-public-ip.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      102 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/conditions/ip-not-in-private-space.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      259 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/conditions/policy-statement-any-principal.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1565 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/conditions/policy-statement-poor-condition.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      359 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/conditions/security-group-opens-all-ports.json
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/filters/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      422 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/filters/ec2-instance-with-open-nacls.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      389 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/filters/ec2-security-group-with-public-cidr-grant.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      698 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/filters/iam-role-for-aws-account.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      683 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/filters/iam-role-for-service.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      356 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/filters/s3-bucket-website-enabled.json
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      608 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/acm-certificate-with-close-expiration-date.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      852 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/acm-certificate-with-transparency-logging-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      810 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudformation-stack-with-role.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1015 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudtrail-duplicated-global-services-logging.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1015 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-data-logging.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      768 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-global-services-logging.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      781 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-log-file-validation.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      685 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-logging.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      510 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudtrail-not-configured.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      501 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudwatch-alarm-without-actions.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      508 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/config-recorder-not-configured.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      556 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-ami-public.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      858 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-default-security-group-in-use.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1289 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-default-security-group-with-rules.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      415 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-ebs-snapshot-not-encrypted.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      464 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-ebs-snapshot-public.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      521 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-ebs-volume-not-encrypted.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      470 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-instance-in-security-group.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      581 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-instance-type.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      641 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-instance-types.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      788 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-instance-with-public-ip.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      900 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-instance-with-user-data-secrets.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      886 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports-to-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      750 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports-to-self.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      628 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      954 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-icmp-to-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1388 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-known-port-to-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1158 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-plaintext-port.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1182 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-port-range.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1538 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-port-to-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      594 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-aws-ip-from-banned-region.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      715 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-aws.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      697 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-non-elastic-ips.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      644 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-unknown-aws.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      934 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-unknown-cidrs.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      858 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-unused-security-group.json
--rw-r--r--   0 xga       (1000) xga       (1000)      837 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elb-listener-allowing-cleartext.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      811 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elb-no-access-logs.json
--rw-r--r--   0 xga       (1000) xga       (1000)     1405 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elb-older-ssl-policy.json
--rw-r--r--   0 xga       (1000) xga       (1000)      972 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elbv2-http-request-smuggling.json
--rw-r--r--   0 xga       (1000) xga       (1000)      996 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elbv2-listener-allowing-cleartext.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1829 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elbv2-no-access-logs.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      710 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elbv2-no-deletion-protection.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1384 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elbv2-older-ssl-policy.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4969 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-assume-role-lacks-external-id-and-mfa.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1651 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-assume-role-no-mfa.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1095 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-assume-role-policy-allows-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1200 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-ec2-role-without-instances.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      848 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-group-with-inline-policies.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      462 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-group-with-no-users.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      725 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-human-user-with-policies.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1357 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-allows-NotActions.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1147 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-allows-non-sts-action.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2193 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-for-role.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1104 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-allows-NotActions.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      975 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-allows-non-sts-action.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1981 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-for-role.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      558 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-no-attachments.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1025 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-expiration-threshold.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      678 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-minimum-length.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      693 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-expiration.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      635 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-lowercase-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      607 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-number-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      618 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-symbol-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      635 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-uppercase-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      575 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-reuse-enabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      843 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-role-with-inline-policies.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      941 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-root-account-no-mfa.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1051 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-root-account-used-recently.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      918 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-root-account-with-active-certs.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      889 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-root-account-with-active-keys.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      754 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-service-user-with-password.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      906 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-no-key-rotation.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      419 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-not-in-category-group.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      414 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-not-in-common-group.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      881 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-with-multiple-access-keys.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      835 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-with-password-and-key.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      717 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-with-policies.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      863 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-without-mfa.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      623 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-backup-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      781 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-ca-certificate-deprecated.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1049 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-no-minor-upgrade.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1062 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-short-backup-retention-period.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      623 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-single-az.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      515 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-storage-not-encrypted.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1532 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-postgres-instance-with-invalid-certificate.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      693 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-security-group-allows-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      765 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-snapshot-public.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      516 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-cluster-database-not-encrypted.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      626 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-cluster-no-version-upgrade.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      673 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-cluster-publicly-accessible.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1059 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-parameter-group-logging-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      979 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-parameter-group-ssl-not-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      594 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-security-group-whitelists-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      536 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/route53-domain-no-autorenew.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      529 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/route53-domain-no-transferlock.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      829 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/route53-domain-transferlock-not-authorized.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      681 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-allowing-cleartext.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      690 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-default-encryption.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      806 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-logging.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      615 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-mfa-delete.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      615 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-versioning.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      924 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-acl.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1583 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-policy-arg.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1415 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-policy-star.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      457 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ses-identity-dkim-not-enabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      593 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ses-identity-dkim-not-verified.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1392 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ses-identity-world-policy.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1446 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/sns-topic-world-policy.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1446 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/sqs-queue-world-policy.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      931 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/vpc-custom-network-acls-allow-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      932 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/vpc-default-network-acls-allow-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      497 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/vpc-network-acl-not-used.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      707 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/vpc-subnet-with-bad-acls.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      802 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/vpc-subnet-with-default-acls.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      718 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/vpc-subnet-without-flow-log.json
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/rulesets/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4724 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/rulesets/cis-1.0.0.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)    31884 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/rulesets/default.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)    32645 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/rulesets/detailed.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1245 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/rulesets/filters.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5293 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/services.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2458 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/aws/utils.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     9464 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/authentication_strategy.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2604 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/aad.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2414 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/appservice.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5548 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      835 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/keyvault.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2465 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/network.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1247 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/rbac.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4987 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/securitycenter.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5168 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/sqldatabase.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3742 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/storageaccounts.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2579 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/virtualmachines.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3934 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/metadata.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5282 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/provider.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/__init__.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3424 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/applications.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1374 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1084 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/groups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3023 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/serviceprincipals.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1834 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/users.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/appservice/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      212 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/appservice/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     6070 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/appservice/web_apps.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      910 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/base.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/keyvault/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/keyvault/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      190 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/keyvault/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1225 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/keyvault/vaults.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/monitor/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/monitor/__init__.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1779 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/application_security_groups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3858 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5360 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/network_interfaces.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     8083 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/security_groups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3961 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/virtual_networks.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1227 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/watchers.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/rbac/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/rbac/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      739 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/rbac/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1446 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/rbac/role_assignments.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1295 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/rbac/roles.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/__init__.py
--rw-r--r--   0 xga       (1000) xga       (1000)      710 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/alerts.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1138 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/auto_provisioning_settings.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1083 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/base.py
--rw-r--r--   0 xga       (1000) xga       (1000)     1264 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/compliance_results.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      972 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/information_protection_policies.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      805 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/pricings.py
--rw-r--r--   0 xga       (1000) xga       (1000)     2339 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/regulatory_compliance_results.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1296 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/security_contacts.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      687 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/settings.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      192 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1031 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/database_blob_auditing_policies.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1224 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/database_threat_detection_policies.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1833 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/databases.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      965 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/replication_links.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      707 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/server_azure_ad_administrators.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      925 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/server_blob_auditing_policies.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1103 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/server_security_alert_policies.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1791 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/servers.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1016 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/transparent_data_encryptions.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/storageaccounts/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/storageaccounts/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      235 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/storageaccounts/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1324 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/storageaccounts/blob_containers.py
--rw-r--r--   0 xga       (1000) xga       (1000)      966 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/storageaccounts/queues.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3158 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/storageaccounts/storage_accounts.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1560 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/subscriptions.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/virtualmachines/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/virtualmachines/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      382 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/virtualmachines/base.py
--rw-r--r--   0 xga       (1000) xga       (1000)     2186 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/virtualmachines/disks.py
--rw-r--r--   0 xga       (1000) xga       (1000)     1311 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/virtualmachines/images.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2890 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/virtualmachines/instances.py
--rw-r--r--   0 xga       (1000) xga       (1000)     2217 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/virtualmachines/snapshots.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/conditions/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      247 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/conditions/allow-tcp.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      531 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/conditions/exposed-to-the-internet.json
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      656 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/aad-guest-users.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1534 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-authentication-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1394 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-client-certificates-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1963 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-http-2-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      973 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-http-allowed.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1387 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-managed-service-identities-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1170 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-tls-v1-supported.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1379 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-webapp-using-outdated-progamming-language-version.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1069 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/network-security-groups-rule-inbound-internet-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1148 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/network-security-groups-rule-inbound-service.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      621 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/network-watcher-not-enabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      669 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/network-watcher-not-provisioned.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      738 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-auto-provisioning-off.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      673 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-email-not-set.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      723 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-no-admin-email-notifications.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      724 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-no-email-notifications.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      796 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-not-set.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      663 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-phone-not-set.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      659 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-standard-tier-not-enabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      891 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-auditing-low-retention.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      687 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-auditing.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      730 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-threat-detection.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      750 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-transparent-data-encryption.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      728 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-disabled-alerts.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      760 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-low-retention.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      911 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-send-alerts-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      712 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-auditing-low-retention.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      674 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-ad-admin-configured.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      659 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-auditing.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      699 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-threat-detection.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      710 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-disabled-alerts.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      744 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-low-retention.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      885 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-send-alerts-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1406 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/storageaccount-access-keys-not-rotated.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1682 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/storageaccount-account-allowing-clear-text.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1747 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/storageaccount-public-blob-container.json
--rw-r--r--   0 xga       (1000) xga       (1000)     1349 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/storageaccount-public-traffic-allowed.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1944 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/storageaccount-trusted-microsoft-services.json
--rw-r--r--   0 xga       (1000) xga       (1000)     1532 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/virtual-machines-disk-encryption.json
--rw-r--r--   0 xga       (1000) xga       (1000)     1291 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/virtual-machines-extensions-installed.json
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/rulesets/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     6268 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/rulesets/cis-1.0.0.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     8050 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/rulesets/default.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)       74 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/rulesets/filters.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3287 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/services.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      100 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/azure/utils.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      535 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/authentication_strategy.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      839 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/authentication_strategy_factory.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/configs/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/configs/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4351 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/configs/browser.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)    20079 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/provider.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/resources/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/resources/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3880 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/resources/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2379 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/base/services.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1809 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/authentication_strategy.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     7963 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1765 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/basefacade.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      847 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/cloudresourcemanager.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1824 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/cloudsql.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1447 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/cloudstorage.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5372 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/gce.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3386 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/iam.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2258 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/kms.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      892 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/stackdriverlogging.py
--rw-r--r--   0 xga       (1000) xga       (1000)     1053 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/stackdrivermonitoring.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      682 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/utils.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2598 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/metadata.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5207 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/provider.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      629 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/base.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudsql/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudsql/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1074 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudsql/backups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      253 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudsql/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3535 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudsql/database_instances.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      804 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudsql/users.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudstorage/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudstorage/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      227 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudstorage/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3018 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudstorage/buckets.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1514 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      910 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/disks.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3119 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/firewalls.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      560 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/instance_disks.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     3170 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/instances.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1440 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/networks.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      228 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/regions.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1293 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/snapshots.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1485 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/subnetworks.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      213 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/zones.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      532 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1431 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/groups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1618 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/keys.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2421 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/member_bindings.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      791 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/service_account_bindings.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1999 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/service_accounts.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1421 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/users.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/kms/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/kms/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      212 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/kms/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1356 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/kms/keyrings.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1348 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/kms/keys.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1584 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/projects.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      682 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/regions.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdriverlogging/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdriverlogging/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      343 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdriverlogging/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      828 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdriverlogging/metrics.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      782 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdriverlogging/sinks.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1341 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/alert_policies.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      408 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1256 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/uptime_checks.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      660 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/zones.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1460 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-allows-root-login-from-any-host.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      727 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-backups-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      721 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-is-open-to-the-world.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1015 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-no-binary-logging.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1027 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-ssl-not-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      670 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-with-no-backups.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1367 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-member.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      728 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-no-logging.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      570 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-no-versioning.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      625 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-default-rule-in-use.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1023 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-all-ports.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1080 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-internal-traffic.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1180 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-port-range.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1100 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-public-access.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1346 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-opens-all-ports-to-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1623 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-opens-sensitive-port-to-all.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      845 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-instance-disk-with-no-snapshot.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      656 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-instance-with-deletion-protection-disabled.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      425 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-network-with-no-instances.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      833 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-old-disk-snapshot.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      769 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-gmail-accounts-used.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1144 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-lack-of-service-account-key-rotation.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1178 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-primitive-role-in-use.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      724 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-role-assigned-to-user.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1661 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-sa-has-admin-privileges.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      852 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-service-account-user-member.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1172 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-service-account-with-user-managed-keys.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1146 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-user-has-sa-user-role.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      651 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/stackdriverlogging-no-export-sinks.json
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/rulesets/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1959 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/rulesets/cis-1.0.0.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     5931 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/rulesets/default.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)       74 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/rulesets/filters.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1783 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/gcp/services.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1128 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/authentication_strategy.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/facade/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/facade/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      648 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/facade/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2800 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/facade/identity.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1321 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/facade/kms.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2102 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/facade/objectstorage.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      840 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/metadata.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1348 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/provider.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      913 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/base.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      926 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/api_keys.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1658 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/authentication_policy.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1946 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1955 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/groups.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      940 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/policies.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      958 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/users.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/kms/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/kms/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      523 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/kms/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1142 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/kms/keys.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1757 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/kms/keyvaults.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/objectstorage/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/objectstorage/__init__.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      555 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/objectstorage/base.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2432 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/objectstorage/buckets.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/filters/
--rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/filters/.keep
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/
--rwxr-xr-x   0 xga       (1000) xga       (1000)      350 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/identity-password-policy-minimum-length.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      299 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/identity-password-policy-no-lowercase-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      294 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/identity-password-policy-no-number-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      294 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/identity-password-policy-no-symbol-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      299 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/identity-password-policy-no-uppercase-required.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      439 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/identity-policy-affects-user.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      381 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/identity-user-with-multiple-api-keys.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      627 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/kms-no-key-rotation.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      420 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/objectstorage-bucket-lacking-kms-encryption.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      388 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/objectstorage-public-bucket.json
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/rulesets/
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1434 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/rulesets/default.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)       74 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/rulesets/filters.json
--rwxr-xr-x   0 xga       (1000) xga       (1000)      854 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/services.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      439 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/oci/utils.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4192 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/providers/utils.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     2439 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/ScoutSuite/utils.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite.egg-info/
--rw-r--r--   0 xga       (1000) xga       (1000)     3978 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite.egg-info/PKG-INFO
--rw-r--r--   0 xga       (1000) xga       (1000)    53582 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite.egg-info/SOURCES.txt
--rw-r--r--   0 xga       (1000) xga       (1000)        1 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite.egg-info/dependency_links.txt
--rw-r--r--   0 xga       (1000) xga       (1000)       60 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite.egg-info/entry_points.txt
--rw-r--r--   0 xga       (1000) xga       (1000)     1133 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite.egg-info/requires.txt
--rw-r--r--   0 xga       (1000) xga       (1000)       17 2020-07-02 11:33:21.000000 ScoutSuite-5.9.0/ScoutSuite.egg-info/top_level.txt
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1425 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/requirements.txt
--rw-r--r--   0 xga       (1000) xga       (1000)       38 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/setup.cfg
--rwxr-xr-x   0 xga       (1000) xga       (1000)     1908 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/setup.py
-drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-02 11:33:22.000000 ScoutSuite-5.9.0/tools/
--rw-r--r--   0 xga       (1000) xga       (1000)        0 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/tools/__init__.py
--rw-r--r--   0 xga       (1000) xga       (1000)     5798 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/tools/aws_security_hub_export.py
--rw-r--r--   0 xga       (1000) xga       (1000)     3551 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/tools/format_findings.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      842 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/tools/gen-tests.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)     4594 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/tools/process_raw_response.py
--rwxr-xr-x   0 xga       (1000) xga       (1000)      601 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/tools/sort-ruleset.py
--rw-r--r--   0 xga       (1000) xga       (1000)     3467 2020-07-02 09:56:36.000000 ScoutSuite-5.9.0/tools/utils.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    15170 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/LICENSE
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      628 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/MANIFEST.in
+-rw-r--r--   0 xga       (1000) xga       (1000)     3978 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/PKG-INFO
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2667 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/README.md
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      215 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    15760 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/__main__.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/core/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    20619 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/cli_parser.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     9917 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/conditions.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     9034 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/console.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1305 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/exceptions.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2849 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/fs.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4505 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/processingengine.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     6725 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/rule.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3558 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/rule_definition.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     9551 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/ruleset.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     7003 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/server.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4226 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/core/utils.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/data/
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/data/aws/
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/data/aws/ip-ranges/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      115 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/data/aws/ip-ranges/aws-in-ec2.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      120 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/data/aws/ip-ranges/aws-in-us.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)   502517 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/data/aws/ip-ranges/aws.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     8262 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/data/icmp_message_types.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3456 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/data/protocols.json
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/__init__.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/conditionals/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      430 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/conditionals/json_format.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      373 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/conditionals/sqlite_format.html
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1276 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/about_scoutsuite.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1355 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/accordion.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      934 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/accordion_policy.html
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1732 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/left_menu_for_aliyun_region.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2625 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.actiontrail.trails.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    11807 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.ecs.regions.id.instances.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2400 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.kms.regions.id.keys.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1267 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.oss.buckets.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2256 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.ram.groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2497 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.ram.policies.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1821 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.ram.roles.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3549 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.ram.users.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5339 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.rds.regions.id.instances.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3694 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.vpc.regions.id.vpcs.html
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1736 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/left_menu_for_region.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2199 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/left_menu_for_vpc.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4956 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.acm.regions.id.certificates.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3053 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.awslambda.regions.id.functions.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2704 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.cloudformation.regions.id.stacks.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1341 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.cloudtrail.regions.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3067 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.cloudtrail.regions.id.trails.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2101 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.cloudwatch.regions.id.alarms.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1937 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.config.regions.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1282 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.config.regions.id.recorders.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1183 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.config.regions.id.rules.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1388 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.snapshots.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      853 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.volumes.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1195 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.images.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3625 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.instances.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2182 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.security_groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1475 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.vpcs.security_groups.resource_list.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2509 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.vpcs.security_groups.rule_list.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      590 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.parameter_groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      587 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.security_groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      609 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.subnet_groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      645 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.vpcs.id.clusters.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2191 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.elb_policies.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3858 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcs.id.elbs.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1380 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcs.id.elbs.linked_resources.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      442 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcs.id.elbs.listener.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      543 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcsid.elbs.linked_policy.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3634 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elbv2.regions.id.vpcs.id.lbs.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3226 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.emr.regions.id.vpcs.id.clusters.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2956 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.credential_reports.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1643 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      752 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.inline_policies.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1373 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.managed_policies.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      725 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.managed_policies_list.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2980 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.roles.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3145 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.users.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2744 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.kms.regions.id.keys.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1873 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.parameter_groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1195 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.security_groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3391 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.instances.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1993 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.snapshots.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      635 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.subnet_groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1262 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.parameter_groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2813 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.vpcs.id.clusters.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1618 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.vpcs.id.security_groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      407 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.vpcs.cluster_nodes.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1722 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.route53.regions.id.domains.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1483 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.route53.regions.id.hosted_zones.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2833 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.s3.acls.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2929 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.s3.bucket_iam_policies.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4683 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.s3.buckets.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1594 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.s3.buckets.objects.html
+-rw-r--r--   0 xga       (1000) xga       (1000)     1200 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.s3.public_access_block_configuration.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1670 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.secretsmanager.regions.id.secrets.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1418 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ses.regions.id.identities.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2872 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.sns.regions.id.topics.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1804 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.sqs.regions.id.queues.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1340 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.stackdriverlogging.sinks.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2400 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.peering_connections.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3370 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1554 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.flow_logs.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3420 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.network_acls.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      788 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.peering_connections.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2921 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.subnets.html
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      839 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/details_for_subscription.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1730 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/left_menu_for_subscription.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3782 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.aad.applications.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3074 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.aad.groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4279 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.aad.service_principals.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3741 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.aad.users.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     6592 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.appservice.subscriptions.id.web_apps.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1419 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.keyvault.subscriptions.id.vaults.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2255 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.application_security_groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     7912 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.network_interfaces.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     7482 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.security_groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4271 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.virtual_networks.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4619 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.virtual_networks.id.subnets.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1644 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.watchers.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3944 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.rbac.subscriptions.id.roles.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1446 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.auto_provisioning_settings.html
+-rw-r--r--   0 xga       (1000) xga       (1000)     1465 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.compliance_results.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1295 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.pricings.html
+-rw-r--r--   0 xga       (1000) xga       (1000)     2793 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.regulatory_compliance_results.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2022 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.security_contacts.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5053 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.sqldatabase.subscriptions.id.servers.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2913 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.storageaccounts.subscriptions.id.storage_accounts.html
+-rw-r--r--   0 xga       (1000) xga       (1000)     3417 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.disks.html
+-rw-r--r--   0 xga       (1000) xga       (1000)     1781 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.images.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4445 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.instances.html
+-rw-r--r--   0 xga       (1000) xga       (1000)     3310 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.snapshots.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      377 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/count_badge.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4882 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/dashboard.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      594 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/details.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      772 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/details_for_region.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      886 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/details_for_vpc.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      825 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/ec2_grants.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      317 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/filters.html
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      920 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/details_for_gcp_region.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      904 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/details_for_gcp_zone.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      804 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/details_for_project.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2361 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/left_menu_for_gcp_region.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2333 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/left_menu_for_gcp_zone.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1675 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/left_menu_for_project.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3107 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.cloudsql.projects.id.instances.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4228 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.cloudstorage.projects.id.buckets.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4583 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.firewalls.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1775 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.networks.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2865 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.regions.id.subnetworks.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1808 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.snapshots.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5387 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.zones.id.instances.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3193 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.bindings.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1509 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3559 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.service_accounts.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1497 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.users.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2924 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.kms.projects.id.keyrings.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1677 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.stackdriverlogging.projects.id.metrics.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1644 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.stackdriverlogging.projects.id.sinks.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2070 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.stackdrivermonitoring.projects.id.alert_policies.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2298 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.stackdrivermonitoring.projects.id.uptime_checks.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      582 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/generic_object.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      641 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/ip_grants.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1765 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/last_run_details.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      801 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/left_menu.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     6661 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/metadata.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      822 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/modal.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2694 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/network_interface.html
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/oci/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2659 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/oci/services.identity.groups.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1661 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/oci/services.identity.policies.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1720 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/oci/services.identity.users.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4283 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/oci/services.kms.keyvaults.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3379 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/oci/services.objectstorage.buckets.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      813 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/policy.html
+-rw-r--r--   0 xga       (1000) xga       (1000)      308 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/report_footer.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      373 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/resource_link.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1844 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/resources_details.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      317 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/singles.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     8643 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/report.html
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aliyun/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2512 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aliyun/services.ram.password_policy.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1995 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aliyun/services.ram.security_policy.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1257 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/attack_surface.html
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aws/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      197 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aws/services.ec2.external_attack_surface.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      197 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aws/services.elb.external_attack_surface.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      201 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aws/services.elbv2.external_attack_surface.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2873 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aws/services.iam.password_policy.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4287 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aws/services.iam.permissions.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      197 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aws/services.rds.external_attack_surface.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      208 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aws/services.redshift.external_attack_surface.html
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/azure/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/azure/.keep
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/gcp/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/gcp/.keep
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/oci/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1917 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/oci/services.identity.password_policy.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      222 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/service_groups.compute.summaries.external_attack_surface.html
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      223 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/service_groups.database.summaries.external_attack_surface.html
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/css/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      510 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/css/modal.css
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2212 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite-dark.css
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      751 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite-light.css
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     8562 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite.css
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1150 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/favicon.ico
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    15066 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/helpers.js
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     6944 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/pagination.js
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      253 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/provider.js
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    44449 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/scoutsuite.js
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4436 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/sqlite.js
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2244 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/theme.js
+-rwxr-xr-x   0 xga       (1000) xga       (1000)  2409097 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/includes.zip
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/listall-configs/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      152 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/data/listall-configs/ec2.regions.id.vpcs.id.security_groups.id.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     6770 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/html.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5118 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/result_encoder.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3241 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/output/utils.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2305 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/__init__.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1437 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/authentication_strategy.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      835 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/actiontrail.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2081 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      861 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/ecs.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1745 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/kms.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      620 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/oss.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     7572 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/ram.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      865 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/rds.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2539 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/utils.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      821 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/vpc.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1693 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/metadata.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1356 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/provider.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/__init__.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/actiontrail/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/actiontrail/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      353 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/actiontrail/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1223 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/actiontrail/trails.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      916 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/base.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ecs/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ecs/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      380 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ecs/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4429 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ecs/instances.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/kms/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/kms/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      360 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/kms/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1603 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/kms/keys.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/oss/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/oss/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      341 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/oss/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      646 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/oss/buckets.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      994 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/api_keys.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3104 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1157 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/groups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1712 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/password_policy.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2814 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/policies.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      888 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/roles.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1748 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/security_policy.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1798 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/users.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/rds/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/rds/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      381 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/rds/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2458 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/rds/instances.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1359 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/regions.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/vpc/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/vpc/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      360 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/vpc/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1712 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/vpc/vpcs.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      332 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/actiontrail-not-configured.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      375 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/actiontrail-not-enabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      531 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ecs-instance-with-deletion-protection-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      531 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ecs-instance-with-public-ip.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      619 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/kms-no-key-rotation.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      422 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-expiration-threshold.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      345 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-minimum-length.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      264 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-no-expiration.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      290 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-no-lowercase-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      274 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-no-number-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      274 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-no-symbol-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      290 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-no-uppercase-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      266 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-password-policy-reuse-enabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      486 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-user-lacking-mfa.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      317 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-user-unused-api-key.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      324 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-user-unused-console-password.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      371 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-user-with-multiple-api-keys.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      314 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ram-user-with-old-api-key.json
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/rulesets/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2384 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/rulesets/default.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)       74 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/rulesets/filters.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1113 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/services.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      818 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/utils.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1862 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/authentication_strategy.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1194 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/acm.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1998 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/awslambda.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    14062 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      138 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/basefacade.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2659 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/cloudformation.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1794 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/cloudtrail.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      583 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/cloudwatch.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1779 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/config.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      666 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/directconnect.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     8881 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/ec2.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2677 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/efs.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3778 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/elasticache.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4758 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/elb.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3104 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/elbv2.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1152 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/emr.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    12122 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/iam.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2911 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/kms.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     9151 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/rds.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2526 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/redshift.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1379 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/route53.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    13622 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/s3.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      545 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/secretsmanager.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2173 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/ses.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2132 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/sns.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1496 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/sqs.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4111 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/utils.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    18912 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/metadata.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    43339 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/provider.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/__init__.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/acm/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/acm/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      358 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/acm/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      872 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/acm/certificates.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/awslambda/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/awslambda/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      339 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/awslambda/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2957 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/awslambda/functions.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      810 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/base.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudformation/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudformation/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      348 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudformation/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2390 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudformation/stacks.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudtrail/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudtrail/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1280 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudtrail/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3152 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudtrail/trails.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudwatch/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudwatch/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1031 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudwatch/alarms.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      337 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudwatch/base.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/config/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/config/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      469 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/config/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1270 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/config/recorders.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1170 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/config/rules.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/directconnect/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/directconnect/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      366 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/directconnect/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      800 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/directconnect/connections.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      721 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/ami.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1715 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3190 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/instances.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      869 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/networkinterfaces.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4184 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/securitygroups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1037 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/snapshots.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      780 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/volumes.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      478 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/vpcs.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/efs/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/efs/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      336 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/efs/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      864 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/efs/filesystems.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1562 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      735 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/cluster.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      953 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/parametergroups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      797 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/securitygroups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      809 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/subnetgroups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      345 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/vpcs.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elb/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elb/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      381 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elb/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1840 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elb/load_balancers.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      773 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elb/policies.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      179 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elb/vpcs.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elbv2/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elbv2/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      324 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elbv2/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      845 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elbv2/listeners.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2214 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elbv2/load_balancers.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      180 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elbv2/vpcs.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/emr/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/emr/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      810 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/emr/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      728 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/emr/clusters.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      730 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/emr/vpcs.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     7214 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1870 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/credentialreports.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      662 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/groups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1353 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/passwordpolicy.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      701 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/policies.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1186 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/roles.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      599 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/users.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/kms/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/kms/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      309 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/kms/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1190 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/kms/grants.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3269 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/kms/keys.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1640 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1598 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/instances.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1094 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/parametergroups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      866 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/securitygroups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1778 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/snapshots.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      794 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/subnetgroups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      438 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/vpcs.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      565 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2033 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/cluster_parameter_groups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      917 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/cluster_parameters.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      823 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/cluster_security_groups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      735 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/clusters.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      173 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/vpcs.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1406 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/regions.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/route53/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/route53/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      416 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/route53/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1016 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/route53/domains.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1226 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/route53/hosted_zones.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/s3/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/s3/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2331 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/s3/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      921 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/s3/buckets.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/secretsmanager/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/secretsmanager/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      342 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/secretsmanager/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1015 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/secretsmanager/secrets.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ses/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ses/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      332 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ses/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1352 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ses/identities.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      629 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ses/identity_policies.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sns/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sns/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      316 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sns/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1063 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sns/subscriptions.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1573 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sns/topics.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sqs/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sqs/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      316 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sqs/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1253 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sqs/queues.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2149 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      705 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/flow_logs.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2250 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/network_acls.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      845 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/peering_connections.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1049 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/subnets.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      246 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/vpcs.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1438 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpcs.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/conditions/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      114 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/conditions/cidr-is-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)       93 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/conditions/ec2-security-group-in-use.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)       96 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/conditions/ec2-security-group-not-used.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      257 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/conditions/instance-with-open-nacls.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      345 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/conditions/instance-with-public-ip.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      102 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/conditions/ip-not-in-private-space.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      259 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/conditions/policy-statement-any-principal.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1565 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/conditions/policy-statement-poor-condition.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      359 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/conditions/security-group-opens-all-ports.json
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/filters/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      422 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/filters/ec2-instance-with-open-nacls.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      389 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/filters/ec2-security-group-with-public-cidr-grant.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      698 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/filters/iam-role-for-aws-account.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      683 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/filters/iam-role-for-service.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      356 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/filters/s3-bucket-website-enabled.json
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      608 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/acm-certificate-with-close-expiration-date.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      852 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/acm-certificate-with-transparency-logging-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      810 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudformation-stack-with-role.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1015 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudtrail-duplicated-global-services-logging.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1015 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-data-logging.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      768 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-global-services-logging.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      781 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-log-file-validation.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      685 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-logging.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      510 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudtrail-not-configured.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      501 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudwatch-alarm-without-actions.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      508 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/config-recorder-not-configured.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      556 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-ami-public.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      858 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-default-security-group-in-use.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1289 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-default-security-group-with-rules.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      415 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-ebs-snapshot-not-encrypted.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      464 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-ebs-snapshot-public.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      521 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-ebs-volume-not-encrypted.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      470 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-instance-in-security-group.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      581 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-instance-type.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      641 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-instance-types.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      788 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-instance-with-public-ip.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      900 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-instance-with-user-data-secrets.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      886 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports-to-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      750 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports-to-self.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      628 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      954 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-icmp-to-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1388 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-known-port-to-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1158 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-plaintext-port.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1182 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-port-range.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1538 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-port-to-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      594 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-aws-ip-from-banned-region.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      715 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-aws.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      697 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-non-elastic-ips.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      644 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-unknown-aws.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      934 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-unknown-cidrs.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      858 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-unused-security-group.json
+-rw-r--r--   0 xga       (1000) xga       (1000)      837 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elb-listener-allowing-cleartext.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      811 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elb-no-access-logs.json
+-rw-r--r--   0 xga       (1000) xga       (1000)     1405 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elb-older-ssl-policy.json
+-rw-r--r--   0 xga       (1000) xga       (1000)      972 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elbv2-http-request-smuggling.json
+-rw-r--r--   0 xga       (1000) xga       (1000)      996 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elbv2-listener-allowing-cleartext.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1829 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elbv2-no-access-logs.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      710 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elbv2-no-deletion-protection.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1384 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elbv2-older-ssl-policy.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4969 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-assume-role-lacks-external-id-and-mfa.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1651 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-assume-role-no-mfa.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1095 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-assume-role-policy-allows-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1200 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-ec2-role-without-instances.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      848 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-group-with-inline-policies.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      462 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-group-with-no-users.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      725 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-human-user-with-policies.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1357 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-allows-NotActions.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1147 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-allows-non-sts-action.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2193 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-for-role.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1104 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-allows-NotActions.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      975 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-allows-non-sts-action.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1981 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-for-role.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      558 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-no-attachments.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1025 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-expiration-threshold.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      678 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-minimum-length.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      693 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-expiration.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      635 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-lowercase-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      607 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-number-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      618 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-symbol-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      635 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-uppercase-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      575 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-reuse-enabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      843 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-role-with-inline-policies.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      941 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-root-account-no-mfa.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1051 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-root-account-used-recently.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      918 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-root-account-with-active-certs.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      889 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-root-account-with-active-keys.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      754 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-service-user-with-password.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      906 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-no-key-rotation.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      419 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-not-in-category-group.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      414 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-not-in-common-group.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      881 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-with-multiple-access-keys.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      835 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-with-password-and-key.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      717 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-with-policies.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      863 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-without-mfa.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      623 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-backup-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      781 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-ca-certificate-deprecated.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1049 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-no-minor-upgrade.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1062 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-short-backup-retention-period.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      623 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-single-az.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      515 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-storage-not-encrypted.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1532 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-postgres-instance-with-invalid-certificate.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      693 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-security-group-allows-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      765 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-snapshot-public.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      516 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-cluster-database-not-encrypted.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      626 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-cluster-no-version-upgrade.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      673 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-cluster-publicly-accessible.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1059 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-parameter-group-logging-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      979 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-parameter-group-ssl-not-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      594 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-security-group-whitelists-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      536 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/route53-domain-no-autorenew.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      529 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/route53-domain-no-transferlock.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      829 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/route53-domain-transferlock-not-authorized.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      681 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-allowing-cleartext.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      690 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-default-encryption.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      806 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-logging.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      615 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-mfa-delete.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      615 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-versioning.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      924 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-acl.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1583 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-policy-arg.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1415 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-policy-star.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      457 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ses-identity-dkim-not-enabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      593 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ses-identity-dkim-not-verified.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1392 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ses-identity-world-policy.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1446 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/sns-topic-world-policy.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1446 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/sqs-queue-world-policy.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      931 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/vpc-custom-network-acls-allow-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      932 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/vpc-default-network-acls-allow-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      497 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/vpc-network-acl-not-used.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      707 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/vpc-subnet-with-bad-acls.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      802 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/vpc-subnet-with-default-acls.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      718 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/vpc-subnet-without-flow-log.json
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/rulesets/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4724 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/rulesets/cis-1.0.0.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    31884 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/rulesets/default.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    32645 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/rulesets/detailed.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1245 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/rulesets/filters.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5293 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/services.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2458 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/aws/utils.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     9464 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/authentication_strategy.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2606 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/aad.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2414 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/appservice.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5548 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      835 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/keyvault.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2465 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/network.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1247 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/rbac.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4987 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/securitycenter.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5168 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/sqldatabase.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3742 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/storageaccounts.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2579 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/virtualmachines.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3934 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/metadata.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5501 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/provider.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/__init__.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3424 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/applications.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1737 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1084 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/groups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3023 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/serviceprincipals.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1867 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/users.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/appservice/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      212 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/appservice/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     6070 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/appservice/web_apps.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      910 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/base.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/keyvault/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/keyvault/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      190 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/keyvault/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1225 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/keyvault/vaults.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/monitor/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/monitor/__init__.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1779 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/application_security_groups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3858 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5360 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/network_interfaces.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     8083 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/security_groups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3961 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/virtual_networks.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1227 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/watchers.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/rbac/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/rbac/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      739 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/rbac/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1446 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/rbac/role_assignments.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1295 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/rbac/roles.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/__init__.py
+-rw-r--r--   0 xga       (1000) xga       (1000)      710 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/alerts.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1138 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/auto_provisioning_settings.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1083 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/base.py
+-rw-r--r--   0 xga       (1000) xga       (1000)     1264 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/compliance_results.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      972 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/information_protection_policies.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      805 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/pricings.py
+-rw-r--r--   0 xga       (1000) xga       (1000)     2339 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/regulatory_compliance_results.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1296 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/security_contacts.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      687 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/settings.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      192 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1031 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/database_blob_auditing_policies.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1224 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/database_threat_detection_policies.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1833 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/databases.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      965 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/replication_links.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      707 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/server_azure_ad_administrators.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      925 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/server_blob_auditing_policies.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1103 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/server_security_alert_policies.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1791 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/servers.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1016 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/transparent_data_encryptions.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/storageaccounts/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/storageaccounts/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      235 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/storageaccounts/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1324 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/storageaccounts/blob_containers.py
+-rw-r--r--   0 xga       (1000) xga       (1000)      966 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/storageaccounts/queues.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3158 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/storageaccounts/storage_accounts.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1560 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/subscriptions.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/virtualmachines/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/virtualmachines/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      382 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/virtualmachines/base.py
+-rw-r--r--   0 xga       (1000) xga       (1000)     2186 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/virtualmachines/disks.py
+-rw-r--r--   0 xga       (1000) xga       (1000)     1311 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/virtualmachines/images.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2890 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/virtualmachines/instances.py
+-rw-r--r--   0 xga       (1000) xga       (1000)     2217 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/virtualmachines/snapshots.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/conditions/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      247 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/conditions/allow-tcp.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      531 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/conditions/exposed-to-the-internet.json
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      656 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/aad-guest-users.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1534 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-authentication-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1394 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-client-certificates-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1963 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-http-2-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      973 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-http-allowed.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1387 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-managed-service-identities-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1170 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-tls-v1-supported.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1379 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-webapp-using-outdated-progamming-language-version.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1069 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/network-security-groups-rule-inbound-internet-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1148 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/network-security-groups-rule-inbound-service.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      621 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/network-watcher-not-enabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      669 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/network-watcher-not-provisioned.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      738 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-auto-provisioning-off.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      673 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-email-not-set.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      723 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-no-admin-email-notifications.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      724 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-no-email-notifications.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      796 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-not-set.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      663 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-phone-not-set.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      659 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-standard-tier-not-enabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      891 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-auditing-low-retention.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      687 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-auditing.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      730 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-threat-detection.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      750 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-transparent-data-encryption.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      728 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-disabled-alerts.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      760 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-low-retention.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      911 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-send-alerts-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      712 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-auditing-low-retention.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      674 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-ad-admin-configured.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      659 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-auditing.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      699 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-threat-detection.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      710 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-disabled-alerts.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      744 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-low-retention.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      885 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-send-alerts-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1406 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/storageaccount-access-keys-not-rotated.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1682 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/storageaccount-account-allowing-clear-text.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1747 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/storageaccount-public-blob-container.json
+-rw-r--r--   0 xga       (1000) xga       (1000)     1349 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/storageaccount-public-traffic-allowed.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1944 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/storageaccount-trusted-microsoft-services.json
+-rw-r--r--   0 xga       (1000) xga       (1000)     1532 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/virtual-machines-disk-encryption.json
+-rw-r--r--   0 xga       (1000) xga       (1000)     1291 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/virtual-machines-extensions-installed.json
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/rulesets/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     6268 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/rulesets/cis-1.0.0.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     8050 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/rulesets/default.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)       74 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/rulesets/filters.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3287 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/services.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      100 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/azure/utils.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      535 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/authentication_strategy.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      839 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/authentication_strategy_factory.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/configs/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/configs/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4351 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/configs/browser.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)    20079 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/provider.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/resources/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/resources/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3880 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/resources/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2379 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/base/services.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1809 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/authentication_strategy.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     7963 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1765 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/basefacade.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      847 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/cloudresourcemanager.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1824 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/cloudsql.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1447 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/cloudstorage.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5372 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/gce.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3386 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/iam.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2258 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/kms.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      892 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/stackdriverlogging.py
+-rw-r--r--   0 xga       (1000) xga       (1000)     1053 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/stackdrivermonitoring.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      682 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/utils.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2598 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/metadata.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5207 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/provider.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      629 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/base.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudsql/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudsql/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1074 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudsql/backups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      253 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudsql/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3535 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudsql/database_instances.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      804 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudsql/users.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudstorage/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudstorage/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      227 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudstorage/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3018 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudstorage/buckets.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1514 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      910 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/disks.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3119 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/firewalls.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      560 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/instance_disks.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     3170 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/instances.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1440 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/networks.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      228 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/regions.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1293 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/snapshots.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1485 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/subnetworks.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      213 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/zones.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      532 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1431 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/groups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1618 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/keys.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2421 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/member_bindings.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      791 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/service_account_bindings.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1999 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/service_accounts.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1421 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/users.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/kms/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/kms/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      212 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/kms/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1356 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/kms/keyrings.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1348 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/kms/keys.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1584 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/projects.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      682 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/regions.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdriverlogging/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdriverlogging/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      343 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdriverlogging/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      828 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdriverlogging/metrics.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      782 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdriverlogging/sinks.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1341 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/alert_policies.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      408 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1256 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/uptime_checks.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      660 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/zones.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1460 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-allows-root-login-from-any-host.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      727 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-backups-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      721 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-is-open-to-the-world.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1015 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-no-binary-logging.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1027 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-ssl-not-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      670 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-with-no-backups.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1367 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-member.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      728 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-no-logging.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      570 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-no-versioning.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      625 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-default-rule-in-use.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1023 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-all-ports.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1080 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-internal-traffic.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1180 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-port-range.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1100 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-public-access.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1346 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-opens-all-ports-to-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1623 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-opens-sensitive-port-to-all.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      845 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-instance-disk-with-no-snapshot.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      656 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-instance-with-deletion-protection-disabled.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      425 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-network-with-no-instances.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      833 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-old-disk-snapshot.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      769 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-gmail-accounts-used.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1144 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-lack-of-service-account-key-rotation.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1178 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-primitive-role-in-use.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      724 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-role-assigned-to-user.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1661 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-sa-has-admin-privileges.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      852 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-service-account-user-member.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1172 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-service-account-with-user-managed-keys.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1146 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-user-has-sa-user-role.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      651 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/stackdriverlogging-no-export-sinks.json
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/rulesets/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1959 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/rulesets/cis-1.0.0.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     5931 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/rulesets/default.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)       74 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/rulesets/filters.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1783 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/gcp/services.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1128 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/authentication_strategy.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/facade/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/facade/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      648 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/facade/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2800 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/facade/identity.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1321 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/facade/kms.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2102 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/facade/objectstorage.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      840 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/metadata.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1348 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/provider.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      913 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/base.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      926 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/api_keys.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1658 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/authentication_policy.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1946 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1955 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/groups.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      940 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/policies.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      958 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/users.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/kms/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/kms/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      523 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/kms/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1142 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/kms/keys.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1757 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/kms/keyvaults.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/objectstorage/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/objectstorage/__init__.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      555 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/objectstorage/base.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2432 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/objectstorage/buckets.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/filters/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/filters/.keep
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      350 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/identity-password-policy-minimum-length.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      299 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/identity-password-policy-no-lowercase-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      294 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/identity-password-policy-no-number-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      294 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/identity-password-policy-no-symbol-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      299 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/identity-password-policy-no-uppercase-required.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      439 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/identity-policy-affects-user.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      381 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/identity-user-with-multiple-api-keys.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      627 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/kms-no-key-rotation.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      420 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/objectstorage-bucket-lacking-kms-encryption.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      388 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/objectstorage-public-bucket.json
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/rulesets/
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1434 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/rulesets/default.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)       74 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/rulesets/filters.json
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      854 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/services.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      439 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/oci/utils.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4192 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/providers/utils.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     2439 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/ScoutSuite/utils.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite.egg-info/
+-rw-r--r--   0 xga       (1000) xga       (1000)     3978 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite.egg-info/PKG-INFO
+-rw-r--r--   0 xga       (1000) xga       (1000)    53582 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite.egg-info/SOURCES.txt
+-rw-r--r--   0 xga       (1000) xga       (1000)        1 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite.egg-info/dependency_links.txt
+-rw-r--r--   0 xga       (1000) xga       (1000)       60 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite.egg-info/entry_points.txt
+-rw-r--r--   0 xga       (1000) xga       (1000)     1133 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite.egg-info/requires.txt
+-rw-r--r--   0 xga       (1000) xga       (1000)       17 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/ScoutSuite.egg-info/top_level.txt
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1425 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/requirements.txt
+-rw-r--r--   0 xga       (1000) xga       (1000)       38 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/setup.cfg
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     1908 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/setup.py
+drwxr-xr-x   0 xga       (1000) xga       (1000)        0 2020-07-28 14:57:45.000000 ScoutSuite-5.9.1/tools/
+-rw-r--r--   0 xga       (1000) xga       (1000)        0 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/tools/__init__.py
+-rw-r--r--   0 xga       (1000) xga       (1000)     5798 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/tools/aws_security_hub_export.py
+-rw-r--r--   0 xga       (1000) xga       (1000)     3551 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/tools/format_findings.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      842 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/tools/gen-tests.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)     4594 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/tools/process_raw_response.py
+-rwxr-xr-x   0 xga       (1000) xga       (1000)      601 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/tools/sort-ruleset.py
+-rw-r--r--   0 xga       (1000) xga       (1000)     3467 2020-07-28 14:49:54.000000 ScoutSuite-5.9.1/tools/utils.py
```

### Comparing `ScoutSuite-5.9.0/LICENSE` & `ScoutSuite-5.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/MANIFEST.in` & `ScoutSuite-5.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/PKG-INFO` & `ScoutSuite-5.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScoutSuite
-Version: 5.9.0
+Version: 5.9.1
 Summary: Scout Suite, a multi-cloud security auditing tool
 Home-page: https://github.com/nccgroup/ScoutSuite
 Author: NCC Group
 License: GNU General Public License v2 (GPLv2)
 Description: <p align="center">
           <img src="https://user-images.githubusercontent.com/4206926/49877604-10457580-fe26-11e8-92d7-cd876c4f6454.png" width=350/>
         </p>
```

### Comparing `ScoutSuite-5.9.0/README.md` & `ScoutSuite-5.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/__main__.py` & `ScoutSuite-5.9.1/ScoutSuite/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -176,14 +176,15 @@
     # Configure the debug level
     set_logger_configuration(debug, quiet, log_file)
 
     print_info('Launching Scout')
 
     print_info('Authenticating to cloud provider')
     auth_strategy = get_authentication_strategy(provider)
+
     try:
         credentials = auth_strategy.authenticate(profile=profile,
                                                  aws_access_key_id=aws_access_key_id,
                                                  aws_secret_access_key=aws_secret_access_key,
                                                  aws_session_token=aws_session_token,
                                                  user_account=user_account,
                                                  user_account_browser=user_account_browser,
@@ -201,14 +202,15 @@
                                                  access_key_secret=access_key_secret)
 
         if not credentials:
             return 101
     except Exception as e:
         print_exception('Authentication failure: {}'.format(e))
         return 101
+
     # Create a cloud provider object
     try:
         cloud_provider = get_provider(provider=provider,
                                       # AWS
                                       profile=profile,
                                       # Azure
                                       subscription_ids=subscription_ids,
@@ -226,25 +228,29 @@
                                       programmatic_execution=programmatic_execution,
                                       credentials=credentials)
     except Exception as e:
         print_exception('Initialization failure: {}'.format(e))
         return 102
 
     # Create a new report
-    report_name = report_name if report_name else cloud_provider.get_report_name()
-    report = ScoutReport(cloud_provider.provider_code,
-                         report_name,
-                         report_dir,
-                         timestamp,
-                         result_format=result_format)
-
-    if database_name:
-        database_file, _ = get_filename('RESULTS', report_name, report_dir, file_extension="db")
-        Server.init(database_file, host_ip, host_port)
-        return
+    try:
+        report_name = report_name if report_name else cloud_provider.get_report_name()
+        report = ScoutReport(cloud_provider.provider_code,
+                             report_name,
+                             report_dir,
+                             timestamp,
+                             result_format=result_format)
+
+        if database_name:
+            database_file, _ = get_filename('RESULTS', report_name, report_dir, file_extension="db")
+            Server.init(database_file, host_ip, host_port)
+            return
+    except Exception as e:
+        print_exception('Report initialization failure: {}'.format(e))
+        return 103
 
     # If this command, run and exit
     if list_services:
         available_services = [x for x in dir(cloud_provider.services) if
                               not (x.startswith('_') or x in ['credentials', 'fetch'])]
         print_info('The available services are: "{}"'.format('", "'.join(available_services)))
         return 0
@@ -255,81 +261,110 @@
         # Fetch data from provider APIs
         try:
             print_info('Gathering data from APIs')
             await cloud_provider.fetch(regions=regions, excluded_regions=excluded_regions)
         except KeyboardInterrupt:
             print_info('\nCancelled by user')
             return 130
+        except Exception as e:
+            print_exception('Unhandled exception thrown while gathering data: {}'.format(e))
+            return 104
 
         # Update means we reload the whole config and overwrite part of it
         if update:
-            print_info('Updating existing data')
-            current_run_services = copy.deepcopy(cloud_provider.services)
-            last_run_dict = report.encoder.load_from_file('RESULTS')
-            cloud_provider.services = last_run_dict['services']
-            for service in cloud_provider.service_list:
-                cloud_provider.services[service] = current_run_services[service]
+            try:
+                print_info('Updating existing data')
+                current_run_services = copy.deepcopy(cloud_provider.services)
+                last_run_dict = report.encoder.load_from_file('RESULTS')
+                cloud_provider.services = last_run_dict['services']
+                for service in cloud_provider.service_list:
+                    cloud_provider.services[service] = current_run_services[service]
+            except Exception as e:
+                print_exception('Failure while updating report: {}'.format(e))
 
     # Partial run, using pre-pulled data
     else:
-        print_info('Using local data')
-        # Reload to flatten everything into a python dictionary
-        last_run_dict = report.encoder.load_from_file('RESULTS')
-        for key in last_run_dict:
-            setattr(cloud_provider, key, last_run_dict[key])
+        try:
+            print_info('Using local data')
+            # Reload to flatten everything into a python dictionary
+            last_run_dict = report.encoder.load_from_file('RESULTS')
+            for key in last_run_dict:
+                setattr(cloud_provider, key, last_run_dict[key])
+        except Exception as e:
+            print_exception('Failure while updating report: {}'.format(e))
 
     # Pre processing
-    cloud_provider.preprocessing(
-        ip_ranges, ip_ranges_name_key)
+    try:
+        print_info('Running pre-processing engine')
+        cloud_provider.preprocessing(ip_ranges, ip_ranges_name_key)
+    except Exception as e:
+        print_exception('Failure while running pre-processing engine: {}'.format(e))
+        return 105
 
     # Analyze config
-    print_info('Running rule engine')
-    finding_rules = Ruleset(cloud_provider=cloud_provider.provider_code,
-                            environment_name=cloud_provider.environment,
-                            filename=ruleset,
-                            ip_ranges=ip_ranges,
-                            account_id=cloud_provider.account_id)
-    processing_engine = ProcessingEngine(finding_rules)
-    processing_engine.run(cloud_provider)
+    try:
+        print_info('Running rule engine')
+        finding_rules = Ruleset(cloud_provider=cloud_provider.provider_code,
+                                environment_name=cloud_provider.environment,
+                                filename=ruleset,
+                                ip_ranges=ip_ranges,
+                                account_id=cloud_provider.account_id)
+        processing_engine = ProcessingEngine(finding_rules)
+        processing_engine.run(cloud_provider)
+    except Exception as e:
+        print_exception('Failure while running rule engine: {}'.format(e))
+        return 106
 
     # Create display filters
-    print_info('Applying display filters')
-    filter_rules = Ruleset(cloud_provider=cloud_provider.provider_code,
-                           environment_name=cloud_provider.environment,
-                           filename='filters.json',
-                           rule_type='filters',
-                           account_id=cloud_provider.account_id)
-    processing_engine = ProcessingEngine(filter_rules)
-    processing_engine.run(cloud_provider)
+    try:
+        print_info('Applying display filters')
+        filter_rules = Ruleset(cloud_provider=cloud_provider.provider_code,
+                               environment_name=cloud_provider.environment,
+                               filename='filters.json',
+                               rule_type='filters',
+                               account_id=cloud_provider.account_id)
+        processing_engine = ProcessingEngine(filter_rules)
+        processing_engine.run(cloud_provider)
+    except Exception as e:
+        print_exception('Failure while applying display filters: {}'.format(e))
+        return 107
 
     # Handle exceptions
     if exceptions:
         print_info('Applying exceptions')
         try:
             exceptions = RuleExceptions(exceptions)
             exceptions.process(cloud_provider)
             exceptions = exceptions.exceptions
         except Exception as e:
             print_exception('Failed to load exceptions: {}'.format(e))
             exceptions = {}
     else:
         exceptions = {}
 
-    run_parameters = {
-        'services': services,
-        'skipped_services': skipped_services,
-        'regions': regions,
-        'excluded_regions': excluded_regions,
-    }
     # Finalize
-    cloud_provider.postprocessing(report.current_time, finding_rules, run_parameters)
+    try:
+        print_info('Running post-processing engine')
+        run_parameters = {
+            'services': services,
+            'skipped_services': skipped_services,
+            'regions': regions,
+            'excluded_regions': excluded_regions,
+        }
+        cloud_provider.postprocessing(report.current_time, finding_rules, run_parameters)
+    except Exception as e:
+        print_exception('Failure while running post-processing engine: {}'.format(e))
+        return 108
 
     # Save config and create HTML report
-    html_report_path = report.save(
-        cloud_provider, exceptions, force_write, debug)
+    try:
+        html_report_path = report.save(cloud_provider, exceptions, force_write, debug)
+    except Exception as e:
+        print_exception('Failure while generating HTML report: {}'.format(e))
+        return 109
 
     # Open the report by default
     if not no_browser:
         print_info('Opening the HTML report')
         url = 'file://%s' % os.path.abspath(html_report_path)
         webbrowser.open(url, new=2)
```

### Comparing `ScoutSuite-5.9.0/ScoutSuite/core/cli_parser.py` & `ScoutSuite-5.9.1/ScoutSuite/core/cli_parser.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/core/conditions.py` & `ScoutSuite-5.9.1/ScoutSuite/core/conditions.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/core/console.py` & `ScoutSuite-5.9.1/ScoutSuite/core/console.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/core/exceptions.py` & `ScoutSuite-5.9.1/ScoutSuite/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/core/fs.py` & `ScoutSuite-5.9.1/ScoutSuite/core/fs.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/core/processingengine.py` & `ScoutSuite-5.9.1/ScoutSuite/core/processingengine.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/core/rule.py` & `ScoutSuite-5.9.1/ScoutSuite/core/rule.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/core/rule_definition.py` & `ScoutSuite-5.9.1/ScoutSuite/core/rule_definition.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/core/ruleset.py` & `ScoutSuite-5.9.1/ScoutSuite/core/ruleset.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/core/server.py` & `ScoutSuite-5.9.1/ScoutSuite/core/server.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/core/utils.py` & `ScoutSuite-5.9.1/ScoutSuite/core/utils.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/data/aws/ip-ranges/aws.json` & `ScoutSuite-5.9.1/ScoutSuite/data/aws/ip-ranges/aws.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/data/icmp_message_types.json` & `ScoutSuite-5.9.1/ScoutSuite/data/icmp_message_types.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/data/protocols.json` & `ScoutSuite-5.9.1/ScoutSuite/data/protocols.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/about_scoutsuite.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/about_scoutsuite.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/accordion.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/accordion.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/accordion_policy.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/accordion_policy.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/left_menu_for_aliyun_region.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/left_menu_for_aliyun_region.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.actiontrail.trails.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.actiontrail.trails.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.ecs.regions.id.instances.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.ecs.regions.id.instances.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.kms.regions.id.keys.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.kms.regions.id.keys.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.oss.buckets.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.oss.buckets.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.ram.groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.ram.groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.ram.policies.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.ram.policies.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.ram.roles.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.ram.roles.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.ram.users.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.ram.users.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.rds.regions.id.instances.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.rds.regions.id.instances.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aliyun/services.vpc.regions.id.vpcs.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aliyun/services.vpc.regions.id.vpcs.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/left_menu_for_region.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/left_menu_for_region.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/left_menu_for_vpc.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/left_menu_for_vpc.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.acm.regions.id.certificates.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.acm.regions.id.certificates.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.awslambda.regions.id.functions.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.awslambda.regions.id.functions.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.cloudformation.regions.id.stacks.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.cloudformation.regions.id.stacks.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.cloudtrail.regions.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.cloudtrail.regions.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.cloudtrail.regions.id.trails.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.cloudtrail.regions.id.trails.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.cloudwatch.regions.id.alarms.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.cloudwatch.regions.id.alarms.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.config.regions.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.config.regions.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.config.regions.id.recorders.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.config.regions.id.recorders.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.config.regions.id.rules.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.config.regions.id.rules.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.snapshots.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.snapshots.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.volumes.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.volumes.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.images.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.images.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.instances.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.instances.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.security_groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.id.vpcs.id.security_groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.vpcs.security_groups.resource_list.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.vpcs.security_groups.resource_list.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.vpcs.security_groups.rule_list.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ec2.regions.vpcs.security_groups.rule_list.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.parameter_groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.parameter_groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.security_groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.security_groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.subnet_groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.subnet_groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.vpcs.id.clusters.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elasticache.regions.id.vpcs.id.clusters.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.elb_policies.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.elb_policies.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcs.id.elbs.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcs.id.elbs.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcs.id.elbs.linked_resources.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcs.id.elbs.linked_resources.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcsid.elbs.linked_policy.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elb.regions.id.vpcsid.elbs.linked_policy.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.elbv2.regions.id.vpcs.id.lbs.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.elbv2.regions.id.vpcs.id.lbs.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.emr.regions.id.vpcs.id.clusters.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.emr.regions.id.vpcs.id.clusters.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.credential_reports.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.credential_reports.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.inline_policies.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.inline_policies.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.managed_policies.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.managed_policies.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.managed_policies_list.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.managed_policies_list.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.roles.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.roles.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.iam.users.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.iam.users.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.kms.regions.id.keys.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.kms.regions.id.keys.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.parameter_groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.parameter_groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.security_groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.security_groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.instances.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.instances.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.snapshots.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.snapshots.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.subnet_groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.rds.regions.id.vpcs.id.subnet_groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.parameter_groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.parameter_groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.vpcs.id.clusters.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.vpcs.id.clusters.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.vpcs.id.security_groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.redshift.regions.id.vpcs.id.security_groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.route53.regions.id.domains.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.route53.regions.id.domains.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.route53.regions.id.hosted_zones.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.route53.regions.id.hosted_zones.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.s3.acls.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.s3.acls.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.s3.bucket_iam_policies.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.s3.bucket_iam_policies.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.s3.buckets.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.s3.buckets.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.s3.buckets.objects.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.s3.buckets.objects.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.s3.public_access_block_configuration.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.s3.public_access_block_configuration.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.secretsmanager.regions.id.secrets.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.secretsmanager.regions.id.secrets.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.ses.regions.id.identities.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.ses.regions.id.identities.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.sns.regions.id.topics.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.sns.regions.id.topics.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.sqs.regions.id.queues.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.sqs.regions.id.queues.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.stackdriverlogging.sinks.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.stackdriverlogging.sinks.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.peering_connections.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.peering_connections.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.flow_logs.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.flow_logs.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.network_acls.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.network_acls.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.peering_connections.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.peering_connections.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.subnets.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/aws/services.vpc.regions.id.vpcs.id.subnets.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/details_for_subscription.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/details_for_subscription.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/left_menu_for_subscription.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/left_menu_for_subscription.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.aad.applications.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.aad.applications.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.aad.groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.aad.groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.aad.service_principals.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.aad.service_principals.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.aad.users.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.aad.users.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.appservice.subscriptions.id.web_apps.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.appservice.subscriptions.id.web_apps.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.keyvault.subscriptions.id.vaults.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.keyvault.subscriptions.id.vaults.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.application_security_groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.application_security_groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.network_interfaces.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.network_interfaces.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.security_groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.security_groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.virtual_networks.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.virtual_networks.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.virtual_networks.id.subnets.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.virtual_networks.id.subnets.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.watchers.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.network.subscriptions.id.watchers.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.rbac.subscriptions.id.roles.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.rbac.subscriptions.id.roles.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.auto_provisioning_settings.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.auto_provisioning_settings.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.compliance_results.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.compliance_results.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.pricings.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.pricings.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.regulatory_compliance_results.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.regulatory_compliance_results.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.security_contacts.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.securitycenter.subscriptions.id.security_contacts.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.sqldatabase.subscriptions.id.servers.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.sqldatabase.subscriptions.id.servers.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.storageaccounts.subscriptions.id.storage_accounts.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.storageaccounts.subscriptions.id.storage_accounts.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.disks.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.disks.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.images.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.images.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.instances.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.instances.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.snapshots.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/azure/services.virtualmachines.subscriptions.id.snapshots.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/dashboard.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/dashboard.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/details.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/details.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/details_for_region.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/details_for_region.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/details_for_vpc.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/details_for_vpc.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/ec2_grants.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/ec2_grants.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/details_for_gcp_region.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/details_for_gcp_region.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/details_for_gcp_zone.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/details_for_gcp_zone.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/details_for_project.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/details_for_project.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/left_menu_for_gcp_region.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/left_menu_for_gcp_region.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/left_menu_for_gcp_zone.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/left_menu_for_gcp_zone.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/left_menu_for_project.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/left_menu_for_project.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.cloudsql.projects.id.instances.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.cloudsql.projects.id.instances.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.cloudstorage.projects.id.buckets.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.cloudstorage.projects.id.buckets.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.firewalls.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.firewalls.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.networks.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.networks.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.regions.id.subnetworks.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.regions.id.subnetworks.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.snapshots.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.snapshots.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.zones.id.instances.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.computeengine.projects.id.zones.id.instances.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.bindings.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.bindings.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.service_accounts.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.service_accounts.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.users.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.iam.projects.id.users.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.kms.projects.id.keyrings.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.kms.projects.id.keyrings.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.stackdriverlogging.projects.id.metrics.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.stackdriverlogging.projects.id.metrics.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.stackdriverlogging.projects.id.sinks.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.stackdriverlogging.projects.id.sinks.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.stackdrivermonitoring.projects.id.alert_policies.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.stackdrivermonitoring.projects.id.alert_policies.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/gcp/services.stackdrivermonitoring.projects.id.uptime_checks.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/gcp/services.stackdrivermonitoring.projects.id.uptime_checks.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/generic_object.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/generic_object.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/ip_grants.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/ip_grants.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/last_run_details.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/last_run_details.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/left_menu.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/left_menu.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/metadata.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/metadata.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/modal.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/modal.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/network_interface.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/network_interface.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/oci/services.identity.groups.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/oci/services.identity.groups.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/oci/services.identity.policies.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/oci/services.identity.policies.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/oci/services.identity.users.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/oci/services.identity.users.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/oci/services.kms.keyvaults.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/oci/services.kms.keyvaults.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/oci/services.objectstorage.buckets.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/oci/services.objectstorage.buckets.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/policy.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/policy.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/partials/resources_details.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/partials/resources_details.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/report.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/report.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aliyun/services.ram.password_policy.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aliyun/services.ram.password_policy.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aliyun/services.ram.security_policy.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aliyun/services.ram.security_policy.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/attack_surface.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/attack_surface.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aws/services.iam.password_policy.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aws/services.iam.password_policy.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/aws/services.iam.permissions.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/aws/services.iam.permissions.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/html/summaries/oci/services.identity.password_policy.html` & `ScoutSuite-5.9.1/ScoutSuite/output/data/html/summaries/oci/services.identity.password_policy.html`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite-dark.css` & `ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite-dark.css`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite-light.css` & `ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite-light.css`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite.css` & `ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/css/scoutsuite.css`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/favicon.ico` & `ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/favicon.ico`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/helpers.js` & `ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/helpers.js`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/pagination.js` & `ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/pagination.js`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/scoutsuite.js` & `ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/scoutsuite.js`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/sqlite.js` & `ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/sqlite.js`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/inc-scoutsuite/theme.js` & `ScoutSuite-5.9.1/ScoutSuite/output/data/inc-scoutsuite/theme.js`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/data/includes.zip` & `ScoutSuite-5.9.1/ScoutSuite/output/data/includes.zip`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/html.py` & `ScoutSuite-5.9.1/ScoutSuite/output/html.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/result_encoder.py` & `ScoutSuite-5.9.1/ScoutSuite/output/result_encoder.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/output/utils.py` & `ScoutSuite-5.9.1/ScoutSuite/output/utils.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/__init__.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/authentication_strategy.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/authentication_strategy.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/actiontrail.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/actiontrail.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/ecs.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/ecs.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/kms.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/kms.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/oss.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/oss.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/ram.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/ram.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/rds.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/rds.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/utils.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/utils.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/facade/vpc.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/facade/vpc.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/metadata.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/metadata.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/provider.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/provider.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/actiontrail/trails.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/actiontrail/trails.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ecs/instances.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ecs/instances.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/kms/keys.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/kms/keys.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/oss/buckets.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/oss/buckets.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/api_keys.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/api_keys.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/groups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/groups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/password_policy.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/password_policy.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/policies.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/policies.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/roles.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/roles.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/security_policy.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/security_policy.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/ram/users.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/ram/users.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/rds/instances.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/rds/instances.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/regions.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/regions.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/resources/vpc/vpcs.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/resources/vpc/vpcs.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ecs-instance-with-deletion-protection-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ecs-instance-with-deletion-protection-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/ecs-instance-with-public-ip.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/ecs-instance-with-public-ip.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/findings/kms-no-key-rotation.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/findings/kms-no-key-rotation.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/rules/rulesets/default.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/rules/rulesets/default.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/services.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/services.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aliyun/utils.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aliyun/utils.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/authentication_strategy.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/authentication_strategy.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/acm.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/acm.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/awslambda.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/awslambda.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/cloudformation.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/cloudformation.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/cloudtrail.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/cloudwatch.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/config.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/config.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/directconnect.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/directconnect.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/ec2.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/ec2.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/efs.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/efs.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/elasticache.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/elasticache.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/elb.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/elb.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/elbv2.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/elbv2.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/emr.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/emr.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/iam.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/iam.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/kms.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/kms.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/rds.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/rds.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/redshift.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/redshift.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/route53.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/route53.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/s3.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/s3.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/secretsmanager.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/ses.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/ses.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/sns.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/sns.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/sqs.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/sqs.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/facade/utils.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/facade/utils.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/metadata.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/metadata.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/provider.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/provider.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/acm/certificates.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/acm/certificates.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/awslambda/functions.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/awslambda/functions.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudformation/stacks.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudformation/stacks.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudtrail/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudtrail/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudtrail/trails.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudtrail/trails.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/cloudwatch/alarms.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/cloudwatch/alarms.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/config/recorders.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/config/recorders.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/config/rules.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/config/rules.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/directconnect/connections.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/directconnect/connections.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/ami.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/ami.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/instances.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/instances.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/networkinterfaces.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/networkinterfaces.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/securitygroups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/securitygroups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/snapshots.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/snapshots.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ec2/volumes.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ec2/volumes.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/efs/filesystems.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/efs/filesystems.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/cluster.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/parametergroups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/parametergroups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/securitygroups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/securitygroups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elasticache/subnetgroups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elasticache/subnetgroups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elb/load_balancers.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elb/load_balancers.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elb/policies.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elb/policies.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elbv2/listeners.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elbv2/listeners.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/elbv2/load_balancers.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/elbv2/load_balancers.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/emr/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/emr/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/emr/clusters.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/emr/clusters.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/emr/vpcs.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/emr/vpcs.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/credentialreports.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/credentialreports.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/groups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/groups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/passwordpolicy.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/passwordpolicy.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/policies.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/policies.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/roles.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/roles.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/iam/users.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/iam/users.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/kms/grants.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/kms/grants.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/kms/keys.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/kms/keys.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/instances.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/instances.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/parametergroups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/parametergroups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/securitygroups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/securitygroups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/snapshots.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/snapshots.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/rds/subnetgroups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/rds/subnetgroups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/cluster_parameter_groups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/cluster_parameter_groups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/cluster_parameters.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/cluster_parameters.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/cluster_security_groups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/cluster_security_groups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/redshift/clusters.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/redshift/clusters.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/regions.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/regions.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/route53/domains.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/route53/domains.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/route53/hosted_zones.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/route53/hosted_zones.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/s3/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/s3/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/s3/buckets.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/s3/buckets.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/secretsmanager/secrets.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/secretsmanager/secrets.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ses/identities.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ses/identities.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/ses/identity_policies.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/ses/identity_policies.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sns/subscriptions.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sns/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sns/topics.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sns/topics.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/sqs/queues.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/sqs/queues.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/flow_logs.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/flow_logs.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/network_acls.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/network_acls.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/peering_connections.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/peering_connections.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpc/subnets.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpc/subnets.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/resources/vpcs.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/resources/vpcs.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/conditions/policy-statement-poor-condition.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/conditions/policy-statement-poor-condition.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/filters/iam-role-for-aws-account.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/filters/iam-role-for-aws-account.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/filters/iam-role-for-service.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/filters/iam-role-for-service.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/acm-certificate-with-close-expiration-date.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/acm-certificate-with-close-expiration-date.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/acm-certificate-with-transparency-logging-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/acm-certificate-with-transparency-logging-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudformation-stack-with-role.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudformation-stack-with-role.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudtrail-duplicated-global-services-logging.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudtrail-duplicated-global-services-logging.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-data-logging.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-data-logging.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-global-services-logging.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-global-services-logging.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-log-file-validation.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-log-file-validation.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-logging.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/cloudtrail-no-logging.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-ami-public.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-ami-public.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-default-security-group-in-use.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-default-security-group-in-use.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-default-security-group-with-rules.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-default-security-group-with-rules.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-ebs-volume-not-encrypted.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-ebs-volume-not-encrypted.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-instance-type.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-instance-type.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-instance-types.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-instance-types.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-instance-with-public-ip.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-instance-with-public-ip.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-instance-with-user-data-secrets.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-instance-with-user-data-secrets.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports-to-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports-to-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports-to-self.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports-to-self.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-all-ports.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-icmp-to-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-icmp-to-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-known-port-to-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-known-port-to-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-plaintext-port.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-plaintext-port.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-port-range.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-port-range.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-port-to-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-opens-port-to-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-aws-ip-from-banned-region.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-aws-ip-from-banned-region.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-aws.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-aws.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-non-elastic-ips.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-non-elastic-ips.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-unknown-aws.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-unknown-aws.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-unknown-cidrs.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-security-group-whitelists-unknown-cidrs.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ec2-unused-security-group.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ec2-unused-security-group.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elb-listener-allowing-cleartext.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elb-listener-allowing-cleartext.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elb-no-access-logs.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elb-no-access-logs.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elb-older-ssl-policy.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elb-older-ssl-policy.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elbv2-http-request-smuggling.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elbv2-http-request-smuggling.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elbv2-listener-allowing-cleartext.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elbv2-listener-allowing-cleartext.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elbv2-no-access-logs.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elbv2-no-access-logs.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elbv2-no-deletion-protection.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elbv2-no-deletion-protection.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/elbv2-older-ssl-policy.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/elbv2-older-ssl-policy.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-assume-role-lacks-external-id-and-mfa.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-assume-role-lacks-external-id-and-mfa.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-assume-role-no-mfa.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-assume-role-no-mfa.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-assume-role-policy-allows-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-assume-role-policy-allows-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-ec2-role-without-instances.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-ec2-role-without-instances.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-group-with-inline-policies.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-group-with-inline-policies.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-human-user-with-policies.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-human-user-with-policies.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-allows-NotActions.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-allows-NotActions.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-allows-non-sts-action.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-allows-non-sts-action.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-for-role.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-inline-policy-for-role.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-allows-NotActions.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-allows-NotActions.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-allows-non-sts-action.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-allows-non-sts-action.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-for-role.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-for-role.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-no-attachments.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-managed-policy-no-attachments.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-expiration-threshold.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-expiration-threshold.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-minimum-length.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-minimum-length.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-expiration.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-expiration.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-lowercase-required.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-lowercase-required.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-number-required.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-number-required.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-symbol-required.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-symbol-required.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-uppercase-required.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-no-uppercase-required.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-password-policy-reuse-enabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-password-policy-reuse-enabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-role-with-inline-policies.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-role-with-inline-policies.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-root-account-no-mfa.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-root-account-no-mfa.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-root-account-used-recently.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-root-account-used-recently.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-root-account-with-active-certs.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-root-account-with-active-certs.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-root-account-with-active-keys.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-root-account-with-active-keys.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-service-user-with-password.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-service-user-with-password.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-no-key-rotation.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-no-key-rotation.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-with-multiple-access-keys.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-with-multiple-access-keys.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-with-password-and-key.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-with-password-and-key.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-with-policies.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-with-policies.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/iam-user-without-mfa.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/iam-user-without-mfa.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-backup-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-backup-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-ca-certificate-deprecated.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-ca-certificate-deprecated.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-no-minor-upgrade.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-no-minor-upgrade.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-short-backup-retention-period.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-short-backup-retention-period.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-single-az.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-single-az.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-instance-storage-not-encrypted.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-instance-storage-not-encrypted.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-postgres-instance-with-invalid-certificate.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-postgres-instance-with-invalid-certificate.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-security-group-allows-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-security-group-allows-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/rds-snapshot-public.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/rds-snapshot-public.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-cluster-database-not-encrypted.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-cluster-database-not-encrypted.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-cluster-no-version-upgrade.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-cluster-no-version-upgrade.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-cluster-publicly-accessible.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-cluster-publicly-accessible.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-parameter-group-logging-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-parameter-group-logging-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-parameter-group-ssl-not-required.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-parameter-group-ssl-not-required.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/redshift-security-group-whitelists-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/redshift-security-group-whitelists-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/route53-domain-no-autorenew.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/route53-domain-no-autorenew.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/route53-domain-no-transferlock.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/route53-domain-no-transferlock.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/route53-domain-transferlock-not-authorized.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/route53-domain-transferlock-not-authorized.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-allowing-cleartext.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-allowing-cleartext.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-default-encryption.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-default-encryption.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-logging.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-logging.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-mfa-delete.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-mfa-delete.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-versioning.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-no-versioning.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-acl.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-acl.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-policy-arg.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-policy-arg.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-policy-star.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/s3-bucket-world-policy-star.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ses-identity-dkim-not-verified.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ses-identity-dkim-not-verified.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/ses-identity-world-policy.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/ses-identity-world-policy.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/sns-topic-world-policy.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/sns-topic-world-policy.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/sqs-queue-world-policy.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/sqs-queue-world-policy.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/vpc-custom-network-acls-allow-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/vpc-custom-network-acls-allow-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/vpc-default-network-acls-allow-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/vpc-default-network-acls-allow-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/vpc-subnet-with-bad-acls.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/vpc-subnet-with-bad-acls.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/vpc-subnet-with-default-acls.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/vpc-subnet-with-default-acls.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/findings/vpc-subnet-without-flow-log.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/findings/vpc-subnet-without-flow-log.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/rulesets/cis-1.0.0.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/rulesets/cis-1.0.0.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/rulesets/default.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/rulesets/default.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/rulesets/detailed.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/rulesets/detailed.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/rules/rulesets/filters.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/rules/rulesets/filters.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/services.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/services.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/aws/utils.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/authentication_strategy.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/authentication_strategy.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/aad.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/aad.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             return []
 
     async def get_user(self, user_id):
         try:
             return await run_concurrently(lambda: self.get_client().users.get(user_id))
         except Exception as e:
             print_exception('Failed to retrieve user {}: {}'.format(user_id, e))
-            return []
+            return None
 
     async def get_groups(self):
         try:
             return await run_concurrently(lambda: list(self.get_client().groups.list()))
         except Exception as e:
             print_exception('Failed to retrieve groups: {}'.format(e))
             return []
```

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/appservice.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/appservice.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/keyvault.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/keyvault.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/network.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/network.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/rbac.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/rbac.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/securitycenter.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/securitycenter.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/sqldatabase.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/sqldatabase.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/storageaccounts.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/storageaccounts.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/facade/virtualmachines.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/facade/virtualmachines.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/metadata.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/metadata.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/provider.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,29 +77,32 @@
 
         super(AzureProvider, self).preprocessing()
 
     def _match_rbac_roles_and_principals(self):
         """
         Matches ARM role assignments to AAD service principals
         """
-        if 'rbac' in self.service_list and 'aad' in self.service_list:
-            for subscription in self.services['rbac']['subscriptions']:
-                for assignment in self.services['rbac']['subscriptions'][subscription]['role_assignments'].values():
-                    role_id = assignment['role_definition_id'].split('/')[-1]
-                    for group in self.services['aad']['groups']:
-                        if group == assignment['principal_id']:
-                            self.services['aad']['groups'][group]['roles'].append({'subscription_id': subscription,
-                                                                                 'role_id': role_id})
-                            self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments']['groups'].append(group)
-                            self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments_count'] += 1
-                    for user in self.services['aad']['users']:
-                        if user == assignment['principal_id']:
-                            self.services['aad']['users'][user]['roles'].append({'subscription_id': subscription,
-                                                                                 'role_id': role_id})
-                            self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments']['users'].append(user)
-                            self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments_count'] += 1
-                    for service_principal in self.services['aad']['service_principals']:
-                        if service_principal == assignment['principal_id']:
-                            self.services['aad']['service_principals'][service_principal]['roles'].append({'subscription_id': subscription,
-                                                                                                           'role_id': role_id})
-                            self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments']['service_principals'].append(service_principal)
-                            self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments_count'] += 1
+        try:
+            if 'rbac' in self.service_list and 'aad' in self.service_list:
+                for subscription in self.services['rbac']['subscriptions']:
+                    for assignment in self.services['rbac']['subscriptions'][subscription]['role_assignments'].values():
+                        role_id = assignment['role_definition_id'].split('/')[-1]
+                        for group in self.services['aad']['groups']:
+                            if group == assignment['principal_id']:
+                                self.services['aad']['groups'][group]['roles'].append({'subscription_id': subscription,
+                                                                                     'role_id': role_id})
+                                self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments']['groups'].append(group)
+                                self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments_count'] += 1
+                        for user in self.services['aad']['users']:
+                            if user == assignment['principal_id']:
+                                self.services['aad']['users'][user]['roles'].append({'subscription_id': subscription,
+                                                                                     'role_id': role_id})
+                                self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments']['users'].append(user)
+                                self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments_count'] += 1
+                        for service_principal in self.services['aad']['service_principals']:
+                            if service_principal == assignment['principal_id']:
+                                self.services['aad']['service_principals'][service_principal]['roles'].append({'subscription_id': subscription,
+                                                                                                               'role_id': role_id})
+                                self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments']['service_principals'].append(service_principal)
+                                self.services['rbac']['subscriptions'][subscription]['roles'][role_id]['assignments_count'] += 1
+        except Exception as e:
+            print_exception('Unable to match RBAC roles and principals: {}'.format(e))
```

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/applications.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/applications.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ScoutSuite.providers.azure.resources.base import AzureCompositeResources
+from ScoutSuite.core.console import print_exception
 
 from .users import Users
 from .groups import Groups
 from .serviceprincipals import ServicePrincipals
 from .applications import Applications
 
 
@@ -17,27 +18,34 @@
     async def fetch_all(self):
         await self._fetch_children(resource_parent=self)
 
     async def fetch_additional_users(self, user_list):
         """
         Special method to fetch additional users
         """
-        # fetch the users
-        additional_users = Users(self.facade)
-        await additional_users.fetch_additional_users(user_list)
-        # add them to the resource and update count
-        self['users'].update(additional_users)
-        self['users_count'] = len(self['users'].values())
-        # re-run the finalize method
-        await self.finalize()
+        try:
+            # fetch the users
+            additional_users = Users(self.facade)
+            await additional_users.fetch_additional_users(user_list)
+            # add them to the resource and update count
+            self['users'].update(additional_users)
+            self['users_count'] = len(self['users'].values())
+        except Exception as e:
+            print_exception('Unable to fetch additional users: {}'.format(e))
+        finally:
+            # re-run the finalize method
+            await self.finalize()
 
     async def finalize(self):
         self.assign_group_memberships()
 
     def assign_group_memberships(self):
         """
         Assigns members to groups
         """
-        for group in self['groups']:
-            for user in self['users']:
-                if group in self['users'][user]['groups']:
-                    self['groups'][group]['users'].append(user)
+        try:
+            for group in self['groups']:
+                for user in self['users']:
+                    if group in self['users'][user]['groups']:
+                        self['groups'][group]['users'].append(user)
+        except Exception as e:
+            print_exception('Unable to assign group memberships: {}'.format(e))
```

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/groups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/groups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/serviceprincipals.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/serviceprincipals.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/aad/users.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/aad/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     async def fetch_additional_users(self, user_list):
         """
         Alternative method which only fetches defined users
         :param user_list: a list of the users to fetch and parse
         """
         for user in user_list:
             raw_user = await self.facade.aad.get_user(user)
-            id, user = await self._parse_user(raw_user)
-            self[id] = user
+            if raw_user:
+                id, user = await self._parse_user(raw_user)
+                self[id] = user
 
     async def _parse_user(self, raw_user):
         user_dict = {}
         user_dict['id'] = raw_user.object_id
         user_dict['additional_properties'] = raw_user.additional_properties
         user_dict['deletion_timestamp'] = raw_user.deletion_timestamp
         user_dict['object_type'] = raw_user.object_type
```

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/appservice/web_apps.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/appservice/web_apps.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/keyvault/vaults.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/keyvault/vaults.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/application_security_groups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/application_security_groups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/network_interfaces.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/security_groups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/security_groups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/virtual_networks.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/virtual_networks.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/network/watchers.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/network/watchers.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/rbac/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/rbac/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/rbac/role_assignments.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/rbac/role_assignments.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/rbac/roles.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/rbac/roles.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/alerts.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/alerts.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/auto_provisioning_settings.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/auto_provisioning_settings.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/compliance_results.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/compliance_results.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/information_protection_policies.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/information_protection_policies.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/pricings.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/pricings.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/regulatory_compliance_results.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/regulatory_compliance_results.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/security_contacts.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/security_contacts.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/securitycenter/settings.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/securitycenter/settings.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/database_blob_auditing_policies.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/database_blob_auditing_policies.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/database_threat_detection_policies.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/database_threat_detection_policies.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/databases.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/databases.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/replication_links.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/replication_links.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/server_azure_ad_administrators.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/server_azure_ad_administrators.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/server_blob_auditing_policies.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/server_blob_auditing_policies.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/server_security_alert_policies.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/server_security_alert_policies.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/servers.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/servers.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/sqldatabase/transparent_data_encryptions.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/sqldatabase/transparent_data_encryptions.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/storageaccounts/blob_containers.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/storageaccounts/blob_containers.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/storageaccounts/queues.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/storageaccounts/queues.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/storageaccounts/storage_accounts.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/storageaccounts/storage_accounts.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/subscriptions.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/virtualmachines/disks.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/virtualmachines/disks.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/virtualmachines/images.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/virtualmachines/images.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/virtualmachines/instances.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/virtualmachines/instances.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/resources/virtualmachines/snapshots.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/resources/virtualmachines/snapshots.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/conditions/exposed-to-the-internet.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/conditions/exposed-to-the-internet.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/aad-guest-users.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/aad-guest-users.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-authentication-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-authentication-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-client-certificates-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-client-certificates-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-http-2-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-http-2-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-http-allowed.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-http-allowed.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-managed-service-identities-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-managed-service-identities-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-tls-v1-supported.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-tls-v1-supported.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/appservice-webapp-using-outdated-progamming-language-version.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/appservice-webapp-using-outdated-progamming-language-version.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/network-security-groups-rule-inbound-internet-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/network-security-groups-rule-inbound-internet-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/network-security-groups-rule-inbound-service.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/network-security-groups-rule-inbound-service.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/network-watcher-not-enabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/network-watcher-not-enabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/network-watcher-not-provisioned.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/network-watcher-not-provisioned.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-auto-provisioning-off.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-auto-provisioning-off.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-email-not-set.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-email-not-set.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-no-admin-email-notifications.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-no-admin-email-notifications.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-no-email-notifications.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-no-email-notifications.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-not-set.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-not-set.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-phone-not-set.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-security-contacts-phone-not-set.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/securitycenter-standard-tier-not-enabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/securitycenter-standard-tier-not-enabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-auditing-low-retention.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-auditing-low-retention.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-auditing.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-auditing.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-threat-detection.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-threat-detection.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-transparent-data-encryption.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-no-transparent-data-encryption.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-disabled-alerts.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-disabled-alerts.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-low-retention.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-low-retention.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-send-alerts-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-databases-threat-detection-send-alerts-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-auditing-low-retention.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-auditing-low-retention.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-ad-admin-configured.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-ad-admin-configured.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-auditing.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-auditing.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-threat-detection.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-no-threat-detection.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-disabled-alerts.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-disabled-alerts.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-low-retention.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-low-retention.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-send-alerts-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/sqldatabase-servers-threat-detection-send-alerts-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/storageaccount-access-keys-not-rotated.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/storageaccount-access-keys-not-rotated.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/storageaccount-account-allowing-clear-text.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/storageaccount-account-allowing-clear-text.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/storageaccount-public-blob-container.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/storageaccount-public-blob-container.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/storageaccount-public-traffic-allowed.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/storageaccount-public-traffic-allowed.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/storageaccount-trusted-microsoft-services.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/storageaccount-trusted-microsoft-services.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/virtual-machines-disk-encryption.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/virtual-machines-disk-encryption.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/findings/virtual-machines-extensions-installed.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/findings/virtual-machines-extensions-installed.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/rulesets/cis-1.0.0.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/rulesets/cis-1.0.0.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/rules/rulesets/default.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/rules/rulesets/default.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/azure/services.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/azure/services.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/base/authentication_strategy.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/base/authentication_strategy.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/base/authentication_strategy_factory.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/base/authentication_strategy_factory.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/base/configs/browser.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/base/configs/browser.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/base/provider.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/base/provider.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/base/resources/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/base/resources/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/base/services.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/base/services.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/authentication_strategy.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/authentication_strategy.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/basefacade.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/basefacade.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/cloudresourcemanager.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/cloudresourcemanager.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/cloudsql.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/cloudsql.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/cloudstorage.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/gce.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/gce.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/iam.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/iam.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/kms.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/kms.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/stackdriverlogging.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/stackdriverlogging.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/stackdrivermonitoring.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/stackdrivermonitoring.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/facade/utils.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/facade/utils.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/metadata.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/metadata.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/provider.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/provider.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudsql/backups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudsql/backups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudsql/database_instances.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudsql/database_instances.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudsql/users.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudsql/users.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/cloudstorage/buckets.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/cloudstorage/buckets.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/disks.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/disks.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/firewalls.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/firewalls.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/instance_disks.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/instance_disks.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/instances.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/instances.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/networks.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/networks.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/snapshots.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/snapshots.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/gce/subnetworks.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/gce/subnetworks.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/groups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/groups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/keys.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/keys.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/member_bindings.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/member_bindings.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/service_account_bindings.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/service_account_bindings.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/service_accounts.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/service_accounts.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/iam/users.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/iam/users.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/kms/keyrings.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/kms/keyrings.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/kms/keys.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/kms/keys.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/projects.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/regions.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/regions.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdriverlogging/metrics.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdriverlogging/metrics.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdriverlogging/sinks.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdriverlogging/sinks.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/alert_policies.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/alert_policies.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/uptime_checks.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/stackdrivermonitoring/uptime_checks.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/resources/zones.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/resources/zones.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-allows-root-login-from-any-host.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-allows-root-login-from-any-host.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-backups-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-backups-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-is-open-to-the-world.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-is-open-to-the-world.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-no-binary-logging.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-no-binary-logging.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-ssl-not-required.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-ssl-not-required.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-with-no-backups.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudsql-instance-with-no-backups.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-member.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-member.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-no-logging.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-no-logging.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-no-versioning.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/cloudstorage-bucket-no-versioning.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-default-rule-in-use.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-default-rule-in-use.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-all-ports.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-all-ports.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-internal-traffic.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-internal-traffic.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-port-range.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-port-range.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-public-access.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-allows-public-access.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-opens-all-ports-to-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-opens-all-ports-to-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-opens-sensitive-port-to-all.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-firewall-rule-opens-sensitive-port-to-all.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-instance-disk-with-no-snapshot.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-instance-disk-with-no-snapshot.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-instance-with-deletion-protection-disabled.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-instance-with-deletion-protection-disabled.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/computeengine-old-disk-snapshot.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/computeengine-old-disk-snapshot.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-gmail-accounts-used.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-gmail-accounts-used.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-lack-of-service-account-key-rotation.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-lack-of-service-account-key-rotation.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-primitive-role-in-use.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-primitive-role-in-use.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-role-assigned-to-user.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-role-assigned-to-user.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-sa-has-admin-privileges.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-sa-has-admin-privileges.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-service-account-user-member.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-service-account-user-member.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-service-account-with-user-managed-keys.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-service-account-with-user-managed-keys.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/iam-user-has-sa-user-role.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/iam-user-has-sa-user-role.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/findings/stackdriverlogging-no-export-sinks.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/findings/stackdriverlogging-no-export-sinks.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/rulesets/cis-1.0.0.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/rulesets/cis-1.0.0.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/rules/rulesets/default.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/rules/rulesets/default.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/gcp/services.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/gcp/services.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/authentication_strategy.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/authentication_strategy.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/facade/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/facade/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/facade/identity.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/facade/identity.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/facade/kms.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/facade/kms.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/facade/objectstorage.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/facade/objectstorage.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/metadata.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/metadata.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/provider.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/provider.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/api_keys.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/api_keys.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/authentication_policy.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/authentication_policy.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/groups.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/groups.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/policies.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/policies.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/identity/users.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/identity/users.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/kms/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/kms/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/kms/keys.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/kms/keys.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/kms/keyvaults.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/kms/keyvaults.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/objectstorage/base.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/objectstorage/base.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/resources/objectstorage/buckets.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/resources/objectstorage/buckets.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/findings/kms-no-key-rotation.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/findings/kms-no-key-rotation.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/rules/rulesets/default.json` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/rules/rulesets/default.json`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/oci/services.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/oci/services.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/providers/utils.py` & `ScoutSuite-5.9.1/ScoutSuite/providers/utils.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite/utils.py` & `ScoutSuite-5.9.1/ScoutSuite/utils.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite.egg-info/PKG-INFO` & `ScoutSuite-5.9.1/ScoutSuite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScoutSuite
-Version: 5.9.0
+Version: 5.9.1
 Summary: Scout Suite, a multi-cloud security auditing tool
 Home-page: https://github.com/nccgroup/ScoutSuite
 Author: NCC Group
 License: GNU General Public License v2 (GPLv2)
 Description: <p align="center">
           <img src="https://user-images.githubusercontent.com/4206926/49877604-10457580-fe26-11e8-92d7-cd876c4f6454.png" width=350/>
         </p>
```

### Comparing `ScoutSuite-5.9.0/ScoutSuite.egg-info/SOURCES.txt` & `ScoutSuite-5.9.1/ScoutSuite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/ScoutSuite.egg-info/requires.txt` & `ScoutSuite-5.9.1/ScoutSuite.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/requirements.txt` & `ScoutSuite-5.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/setup.py` & `ScoutSuite-5.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/tools/aws_security_hub_export.py` & `ScoutSuite-5.9.1/tools/aws_security_hub_export.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/tools/format_findings.py` & `ScoutSuite-5.9.1/tools/format_findings.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/tools/gen-tests.py` & `ScoutSuite-5.9.1/tools/gen-tests.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/tools/process_raw_response.py` & `ScoutSuite-5.9.1/tools/process_raw_response.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/tools/sort-ruleset.py` & `ScoutSuite-5.9.1/tools/sort-ruleset.py`

 * *Files identical despite different names*

### Comparing `ScoutSuite-5.9.0/tools/utils.py` & `ScoutSuite-5.9.1/tools/utils.py`

 * *Files identical despite different names*

