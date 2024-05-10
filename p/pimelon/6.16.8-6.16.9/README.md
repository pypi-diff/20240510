# Comparing `tmp/pimelon-6.16.8.tar.gz` & `tmp/pimelon-6.16.9.tar.gz`

## Comparing `pimelon-6.16.8.tar` & `pimelon-6.16.9.tar`

### file list

```diff
@@ -1,149 +1,148 @@
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/__init__.py
--rwxr-xr-x   0        0        0    27979 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/app.py
--rwxr-xr-x   0        0        0     6396 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/cli.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/exceptions.py
--rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/pine.py
--rwxr-xr-x   0        0        0     2973 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/commands/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/commands/config.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/commands/git.py
--rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/commands/install.py
--rwxr-xr-x   0        0        0     7106 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/commands/make.py
--rwxr-xr-x   0        0        0    12613 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/commands/setup.py
--rwxr-xr-x   0        0        0     2779 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/commands/update.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/commands/utils.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/__init__.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/common_site_config.py
--rwxr-xr-x   0        0        0     5393 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/lets_encrypt.py
--rw-r--r--   0        0        0     8442 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/nginx.py
--rwxr-xr-x   0        0        0      860 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/procfile.py
--rwxr-xr-x   0        0        0     5531 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/production_setup.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/redis.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/site_config.py
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/supervisor.py
--rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/systemd.py
--rwxr-xr-x   0        0        0    38867 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/502.html
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/Procfile
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/guipine_nginx.conf
--rwxr-xr-x   0        0        0      620 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/letsencrypt.cfg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/melon_sudoers
--rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/nginx.conf
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/nginx_default.conf
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/redis_cache.conf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/redis_queue.conf
--rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/supervisor.conf
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon-melon-default-worker.service
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon-melon-long-worker.service
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon-melon-schedule.service
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon-melon-short-worker.service
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon-melon-web.service
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon-node-socketio.service
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon-redis-cache.service
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon-redis-queue.service
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon-redis.target
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon-web.target
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon-workers.target
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/config/templates/systemd/pimelon.target
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/patches/__init__.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/patches/patches.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/patches/v6/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/patches/v6/fix_backup_cronjob.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/patches/v6/fix_user_permissions.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/patches/v6/set_live_reload_config.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/patches/v6/update_archived_sites.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/create_user.yml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/macosx.yml
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/site.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/vm_build.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/bash_screen_wall/files/screen_wall.sh
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/bash_screen_wall/tasks/main.yml
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/common/tasks/debian.yml
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/common/tasks/debian_family.yml
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/common/tasks/macos.yml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/common/tasks/main.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/common/tasks/redhat_family.yml
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/common/tasks/ubuntu.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/dns_caching/handlers/main.yml
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/dns_caching/tasks/main.yml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/fail2ban/defaults/main.yml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/fail2ban/handlers/main.yml
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/fail2ban/tasks/configure_nginx_jail.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/fail2ban/tasks/main.yml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/fail2ban/templates/nginx-proxy-jail.conf.j2
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/locale/defaults/main.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/locale/tasks/main.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/logwatch/defaults/main.yml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/logwatch/tasks/main.yml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/logwatch/templates/logwatch.conf.j2
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/README.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/defaults/main.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/files/debian_mariadb_config.cnf
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/files/mariadb_config.cnf
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/handlers/main.yml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/tasks/centos.yml
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/tasks/debian.yml
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/tasks/main.yml
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/templates/mariadb_centos.repo.j2
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/templates/mariadb_debian.list.j2
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/templates/mariadb_ubuntu.list.j2
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/templates/my.cnf.j2
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/mariadb/vars/main.yml
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/melon_selinux/files/melon_selinux.te
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/melon_selinux/tasks/main.yml
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/README.md
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/defaults/main.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/handlers/main.yml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/meta/main.yml
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/tasks/main.yml
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/tasks/setup-Debian.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/tasks/setup-RedHat.yml
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/tasks/vhosts.yml
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/templates/nginx.conf.j2
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/templates/nginx.repo.j2
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/templates/vhosts.j2
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/tests/inventory
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/tests/test.yml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/vars/Debian.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nginx/vars/RedHat.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nodejs/defaults/main.yml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nodejs/tasks/debian_family.yml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nodejs/tasks/main.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/nodejs/tasks/redhat_family.yml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/ntpd/tasks/main.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/packer/tasks/debian_family.yml
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/packer/tasks/main.yml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/packer/tasks/redhat_family.yml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/pine/tasks/change_ssh_port.yml
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/pine/tasks/main.yml
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/pine/tasks/setup_firewall.yml
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/pine/tasks/setup_inputrc.yml
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/pine/tasks/setup_monak.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/pine/tasks/setup_pine_production.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/psutil/tasks/main.yml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/redis/tasks/main.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/supervisor/tasks/main.yml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/swap/defaults/main.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/swap/tasks/main.yml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/virtualbox/defaults/main.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/virtualbox/files/virtualbox_centos.repo
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/virtualbox/tasks/debian_family.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/virtualbox/tasks/main.yml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/virtualbox/tasks/redhat_family.yml
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/playbooks/roles/wkhtmltopdf/tasks/main.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/tests/__init__.py
--rw-r--r--   0        0        0    15107 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/utils/__init__.py
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/utils/app.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/utils/cli.py
--rw-r--r--   0        0        0    21442 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/utils/pine.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/utils/render.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/utils/system.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 pimelon-6.16.8/pine/utils/translation.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 pimelon-6.16.8/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.8/README.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 pimelon-6.16.8/pyproject.toml
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 pimelon-6.16.8/PKG-INFO
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/__init__.py
+-rwxr-xr-x   0        0        0    27878 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/app.py
+-rwxr-xr-x   0        0        0     6396 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/cli.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/exceptions.py
+-rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/pine.py
+-rwxr-xr-x   0        0        0     2973 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/commands/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/commands/config.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/commands/git.py
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/commands/install.py
+-rwxr-xr-x   0        0        0     7106 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/commands/make.py
+-rwxr-xr-x   0        0        0    12613 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/commands/setup.py
+-rwxr-xr-x   0        0        0     2779 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/commands/update.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/commands/utils.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/__init__.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/common_site_config.py
+-rwxr-xr-x   0        0        0     5393 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/lets_encrypt.py
+-rw-r--r--   0        0        0     8442 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/nginx.py
+-rwxr-xr-x   0        0        0      860 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/procfile.py
+-rwxr-xr-x   0        0        0     5531 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/production_setup.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/redis.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/site_config.py
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/supervisor.py
+-rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/systemd.py
+-rwxr-xr-x   0        0        0    38867 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/502.html
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/Procfile
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/guipine_nginx.conf
+-rwxr-xr-x   0        0        0      620 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/letsencrypt.cfg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/melon_sudoers
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/nginx.conf
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/nginx_default.conf
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/redis_cache.conf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/redis_queue.conf
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/supervisor.conf
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon-melon-default-worker.service
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon-melon-long-worker.service
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon-melon-schedule.service
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon-melon-short-worker.service
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon-melon-web.service
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon-node-socketio.service
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon-redis-cache.service
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon-redis-queue.service
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon-redis.target
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon-web.target
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon-workers.target
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/config/templates/systemd/pimelon.target
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/patches/__init__.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/patches/patches.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/patches/v6/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/patches/v6/fix_backup_cronjob.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/patches/v6/fix_user_permissions.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/patches/v6/set_live_reload_config.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/patches/v6/update_archived_sites.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/create_user.yml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/macosx.yml
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/site.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/vm_build.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/bash_screen_wall/files/screen_wall.sh
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/bash_screen_wall/tasks/main.yml
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/common/tasks/debian.yml
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/common/tasks/debian_family.yml
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/common/tasks/macos.yml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/common/tasks/main.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/common/tasks/redhat_family.yml
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/common/tasks/ubuntu.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/dns_caching/handlers/main.yml
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/dns_caching/tasks/main.yml
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/fail2ban/defaults/main.yml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/fail2ban/handlers/main.yml
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/fail2ban/tasks/configure_nginx_jail.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/fail2ban/tasks/main.yml
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/fail2ban/templates/nginx-proxy-jail.conf.j2
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/locale/defaults/main.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/locale/tasks/main.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/logwatch/defaults/main.yml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/logwatch/tasks/main.yml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/logwatch/templates/logwatch.conf.j2
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/README.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/defaults/main.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/files/debian_mariadb_config.cnf
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/files/mariadb_config.cnf
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/handlers/main.yml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/tasks/centos.yml
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/tasks/debian.yml
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/tasks/main.yml
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/templates/mariadb_centos.repo.j2
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/templates/mariadb_debian.list.j2
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/templates/mariadb_ubuntu.list.j2
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/templates/my.cnf.j2
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/mariadb/vars/main.yml
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/melon_selinux/files/melon_selinux.te
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/melon_selinux/tasks/main.yml
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/README.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/defaults/main.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/handlers/main.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/meta/main.yml
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/tasks/main.yml
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/tasks/setup-Debian.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/tasks/setup-RedHat.yml
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/tasks/vhosts.yml
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/templates/nginx.conf.j2
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/templates/nginx.repo.j2
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/templates/vhosts.j2
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/tests/inventory
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/tests/test.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/vars/Debian.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nginx/vars/RedHat.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nodejs/defaults/main.yml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nodejs/tasks/debian_family.yml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nodejs/tasks/main.yml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/nodejs/tasks/redhat_family.yml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/ntpd/tasks/main.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/packer/tasks/debian_family.yml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/packer/tasks/main.yml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/packer/tasks/redhat_family.yml
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/pine/tasks/change_ssh_port.yml
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/pine/tasks/main.yml
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/pine/tasks/setup_firewall.yml
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/pine/tasks/setup_inputrc.yml
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/pine/tasks/setup_monak.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/pine/tasks/setup_pine_production.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/psutil/tasks/main.yml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/redis/tasks/main.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/supervisor/tasks/main.yml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/swap/defaults/main.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/swap/tasks/main.yml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/virtualbox/defaults/main.yml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/virtualbox/files/virtualbox_centos.repo
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/virtualbox/tasks/debian_family.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/virtualbox/tasks/main.yml
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/virtualbox/tasks/redhat_family.yml
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/playbooks/roles/wkhtmltopdf/tasks/main.yml
+-rw-r--r--   0        0        0    15107 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/utils/__init__.py
+-rw-r--r--   0        0        0     8910 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/utils/app.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/utils/cli.py
+-rw-r--r--   0        0        0    21442 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/utils/pine.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/utils/render.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/utils/system.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 pimelon-6.16.9/pine/utils/translation.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 pimelon-6.16.9/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.9/README.md
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 pimelon-6.16.9/pyproject.toml
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pimelon-6.16.9/PKG-INFO
```

### Comparing `pimelon-6.16.8/pine/app.py` & `pimelon-6.16.9/pine/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,47 +82,44 @@
 		elif os.path.exists(self.mount_path):
 			self.on_disk = True
 			self._setup_details_from_mounted_disk()
 
 		# fetch meta for repo from remote git server - traditional get-app url
 		elif is_git_url(self.name):
 			self.is_url = True
-			self._setup_details_from_git_url()
+			self.__setup_details_from_git()
 
 		# fetch meta from new styled name tags & first party apps on github
 		else:
 			self._setup_details_from_name_tag()
 
 		if self.git_repo:
 			self.app_name = os.path.basename(os.path.normpath(self.git_repo.working_tree_dir))
 		else:
 			self.app_name = self.repo
 
 	def _setup_details_from_mounted_disk(self):
 		# If app is a git repo
 		self.git_repo = git.Repo(self.mount_path)
 		try:
-			self._setup_details_from_git_url(self.git_repo.remotes[0].url)
+			self.__setup_details_from_git(self.git_repo.remotes[0].url)
 			if not (self.branch or self.tag):
 				self.tag = self.branch = self.git_repo.active_branch.name
 		except IndexError:
 			self.org, self.repo, self.tag = os.path.split(self.mount_path)[-2:] + (self.branch,)
 		except TypeError:
 			# faced a "a detached symbolic reference as it points" in case you're in the middle of
 			# some git shenanigans
 			self.tag = self.branch = None
 
 	def _setup_details_from_name_tag(self):
 		using_cached = bool(self.cache_key)
 		self.org, self.repo, self.tag = fetch_details_from_tag(self.name, using_cached)
 		self.tag = self.tag or self.branch
 
-	def _setup_details_from_git_url(self, url=None):
-		return self.__setup_details_from_git(url)
-
 	def __setup_details_from_git(self, url=None):
 		name = url if url else self.name
 		if name.startswith("git@") or name.startswith("ssh://"):
 			self.use_ssh = True
 			_first_part, _second_part = name.rsplit(":", 1)
 			self.remote_server = _first_part.split("@")[-1]
 			self.org, _repo = _second_part.rsplit("/", 1)
```

### Comparing `pimelon-6.16.8/pine/cli.py` & `pimelon-6.16.9/pine/cli.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/exceptions.py` & `pimelon-6.16.9/pine/exceptions.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/pine.py` & `pimelon-6.16.9/pine/pine.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/commands/__init__.py` & `pimelon-6.16.9/pine/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/commands/config.py` & `pimelon-6.16.9/pine/commands/config.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/commands/git.py` & `pimelon-6.16.9/pine/commands/git.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/commands/install.py` & `pimelon-6.16.9/pine/commands/install.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/commands/make.py` & `pimelon-6.16.9/pine/commands/make.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/commands/setup.py` & `pimelon-6.16.9/pine/commands/setup.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/commands/update.py` & `pimelon-6.16.9/pine/commands/update.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/commands/utils.py` & `pimelon-6.16.9/pine/commands/utils.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/common_site_config.py` & `pimelon-6.16.9/pine/config/common_site_config.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/lets_encrypt.py` & `pimelon-6.16.9/pine/config/lets_encrypt.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/nginx.py` & `pimelon-6.16.9/pine/config/nginx.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/procfile.py` & `pimelon-6.16.9/pine/config/procfile.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/production_setup.py` & `pimelon-6.16.9/pine/config/production_setup.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/redis.py` & `pimelon-6.16.9/pine/config/redis.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/site_config.py` & `pimelon-6.16.9/pine/config/site_config.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/supervisor.py` & `pimelon-6.16.9/pine/config/supervisor.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/systemd.py` & `pimelon-6.16.9/pine/config/systemd.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/templates/502.html` & `pimelon-6.16.9/pine/config/templates/502.html`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/templates/Procfile` & `pimelon-6.16.9/pine/config/templates/Procfile`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/templates/guipine_nginx.conf` & `pimelon-6.16.9/pine/config/templates/guipine_nginx.conf`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/templates/letsencrypt.cfg` & `pimelon-6.16.9/pine/config/templates/letsencrypt.cfg`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/templates/nginx.conf` & `pimelon-6.16.9/pine/config/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/templates/nginx_default.conf` & `pimelon-6.16.9/pine/config/templates/nginx_default.conf`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/templates/supervisor.conf` & `pimelon-6.16.9/pine/config/templates/supervisor.conf`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/config/templates/systemd/pimelon-melon-web.service` & `pimelon-6.16.9/pine/config/templates/systemd/pimelon-melon-web.service`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/patches/__init__.py` & `pimelon-6.16.9/pine/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/patches/v6/fix_user_permissions.py` & `pimelon-6.16.9/pine/patches/v6/fix_user_permissions.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/patches/v6/update_archived_sites.py` & `pimelon-6.16.9/pine/patches/v6/update_archived_sites.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/create_user.yml` & `pimelon-6.16.9/pine/playbooks/create_user.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/macosx.yml` & `pimelon-6.16.9/pine/playbooks/macosx.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/site.yml` & `pimelon-6.16.9/pine/playbooks/site.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/common/tasks/debian.yml` & `pimelon-6.16.9/pine/playbooks/roles/common/tasks/debian.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/common/tasks/debian_family.yml` & `pimelon-6.16.9/pine/playbooks/roles/common/tasks/debian_family.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/common/tasks/macos.yml` & `pimelon-6.16.9/pine/playbooks/roles/common/tasks/macos.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/common/tasks/redhat_family.yml` & `pimelon-6.16.9/pine/playbooks/roles/common/tasks/redhat_family.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/common/tasks/ubuntu.yml` & `pimelon-6.16.9/pine/playbooks/roles/common/tasks/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/fail2ban/tasks/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/fail2ban/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2` & `pimelon-6.16.9/pine/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/locale/tasks/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/locale/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/mariadb/README.md` & `pimelon-6.16.9/pine/playbooks/roles/mariadb/README.md`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/mariadb/files/mariadb_config.cnf` & `pimelon-6.16.9/pine/playbooks/roles/mariadb/files/mariadb_config.cnf`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/mariadb/tasks/debian.yml` & `pimelon-6.16.9/pine/playbooks/roles/mariadb/tasks/debian.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/mariadb/tasks/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/mariadb/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml` & `pimelon-6.16.9/pine/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml` & `pimelon-6.16.9/pine/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml` & `pimelon-6.16.9/pine/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/melon_selinux/files/melon_selinux.te` & `pimelon-6.16.9/pine/playbooks/roles/melon_selinux/files/melon_selinux.te`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/melon_selinux/tasks/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/melon_selinux/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/nginx/README.md` & `pimelon-6.16.9/pine/playbooks/roles/nginx/README.md`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/nginx/defaults/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/nginx/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/nginx/tasks/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/nginx/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/nginx/tasks/setup-Debian.yml` & `pimelon-6.16.9/pine/playbooks/roles/nginx/tasks/setup-Debian.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/nginx/tasks/vhosts.yml` & `pimelon-6.16.9/pine/playbooks/roles/nginx/tasks/vhosts.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/nginx/templates/nginx.conf.j2` & `pimelon-6.16.9/pine/playbooks/roles/nginx/templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/nginx/templates/vhosts.j2` & `pimelon-6.16.9/pine/playbooks/roles/nginx/templates/vhosts.j2`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/ntpd/tasks/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/ntpd/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/packer/tasks/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/packer/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/pine/tasks/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/pine/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/pine/tasks/setup_firewall.yml` & `pimelon-6.16.9/pine/playbooks/roles/pine/tasks/setup_firewall.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/pine/tasks/setup_monak.yml` & `pimelon-6.16.9/pine/playbooks/roles/pine/tasks/setup_monak.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/pine/tasks/setup_pine_production.yml` & `pimelon-6.16.9/pine/playbooks/roles/pine/tasks/setup_pine_production.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/redis/tasks/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/redis/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/swap/tasks/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/swap/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/virtualbox/tasks/debian_family.yml` & `pimelon-6.16.9/pine/playbooks/roles/virtualbox/tasks/debian_family.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/playbooks/roles/wkhtmltopdf/tasks/main.yml` & `pimelon-6.16.9/pine/playbooks/roles/wkhtmltopdf/tasks/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,27 @@
       - libxext6
       - xfonts-75dpi
       - xfonts-base
     state: present
     force: yes
   when: ansible_os_family == 'Debian'
 
+- name: download wkthmltox Ubuntu 22
+  get_url:
+    url: https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_amd64.deb
+    dest: /tmp/wkhtmltox.deb
+  when: ansible_distribution == 'Ubuntu' and ansible_distribution_major_version == '22' and ansible_architecture != 'aarch64'
+
+- name: download wkthmltox Ubuntu 22 arm64
+  get_url:
+    # wkhtmltox supports arm64 starting from 0.12.6
+    url: https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_arm64.deb
+    dest: /tmp/wkhtmltox.deb
+  when: ansible_distribution == 'Ubuntu' and ansible_distribution_major_version == '22' and ansible_architecture == 'aarch64'
+
 - name: download wkthmltox Ubuntu 20
   get_url:
     url: https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.focal_amd64.deb
     dest: /tmp/wkhtmltox.deb
   when: ansible_distribution == 'Ubuntu' and ansible_distribution_major_version == '20' and ansible_architecture != 'aarch64'
 
 - name: download wkthmltox Ubuntu 20 arm64
```

### Comparing `pimelon-6.16.8/pine/utils/__init__.py` & `pimelon-6.16.9/pine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/utils/app.py` & `pimelon-6.16.9/pine/utils/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 		return 0
 
 
 def get_current_branch(app, pine_path="."):
 	from pine.utils import get_cmd_output
 
 	repo_dir = get_repo_dir(app, pine_path=pine_path)
-	return get_cmd_output("basename $(git symbolic-ref -q HEAD)", cwd=repo_dir)
+	return get_cmd_output("git symbolic-ref -q --short HEAD", cwd=repo_dir)
 
 
 @lru_cache(maxsize=5)
 def get_required_deps(org, name, branch, deps="hooks.py"):
 	import requests
 	import base64
```

### Comparing `pimelon-6.16.8/pine/utils/cli.py` & `pimelon-6.16.9/pine/utils/cli.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/utils/pine.py` & `pimelon-6.16.9/pine/utils/pine.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/utils/render.py` & `pimelon-6.16.9/pine/utils/render.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/utils/system.py` & `pimelon-6.16.9/pine/utils/system.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pine/utils/translation.py` & `pimelon-6.16.9/pine/utils/translation.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/.gitignore` & `pimelon-6.16.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.8/pyproject.toml` & `pimelon-6.16.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pimelon"
-description = "CLI to manage Multi-tenant deployments for MonakERP Apps"
+description = "CLI Tool"
 readme = "README.md"
 license = ""
 requires-python = ">=3.7"
 authors = [
     { name = "Alphamonak Solutions", email = "amonak@monakerp.com" },
 ]
 classifiers = [
```

### Comparing `pimelon-6.16.8/PKG-INFO` & `pimelon-6.16.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pimelon
-Version: 6.16.8
-Summary: CLI to manage Multi-tenant deployments for MonakERP Apps
+Version: 6.16.9
+Summary: CLI Tool
 Project-URL: Changelog, https://github.com/amonak/pine/releases
 Project-URL: Documentation, https://docs.monakerp.com/docs/v7/user/en/pine
 Project-URL: Homepage, https://monakerp.com/pine
 Project-URL: Source, https://github.com/amonak/pine
 Author-email: Alphamonak Solutions <amonak@monakerp.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

