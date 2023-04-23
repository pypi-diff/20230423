# Comparing `tmp/talos_install-0.2.0.dev351.tar.gz` & `tmp/talos_install-0.2.0.dev352.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talos_install-0.2.0.dev351.tar", last modified: Fri Apr 21 16:40:19 2023, max compression
+gzip compressed data, was "talos_install-0.2.0.dev352.tar", last modified: Sun Apr 23 12:53:18 2023, max compression
```

## Comparing `talos_install-0.2.0.dev351.tar` & `talos_install-0.2.0.dev352.tar`

### file list

```diff
@@ -1,216 +1,224 @@
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.654961 talos_install-0.2.0.dev351/
--rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/AUTHORS
--rw-rw-r--   0 installer  (3002) installer  (3002)    11635 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/ChangeLog
--rw-rw-r--   0 installer  (3002) installer  (3002)     2018 2023-04-21 16:40:19.654961 talos_install-0.2.0.dev351/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     1358 2023-04-21 16:36:01.000000 talos_install-0.2.0.dev351/README.md
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.627961 talos_install-0.2.0.dev351/ansible/
--rw-rw-r--   0 installer  (3002) installer  (3002)      309 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/ansible.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.627961 talos_install-0.2.0.dev351/ansible/group_vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)       23 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/group_vars/all.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.624961 talos_install-0.2.0.dev351/ansible/roles/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.613961 talos_install-0.2.0.dev351/ansible/roles/cli/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.627961 talos_install-0.2.0.dev351/ansible/roles/cli/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-21 16:33:02.000000 talos_install-0.2.0.dev351/ansible/roles/cli/files/FOUNDMEDEVKEY
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.627961 talos_install-0.2.0.dev351/ansible/roles/cli/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev351/ansible/roles/cli/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.629961 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1227 2023-04-21 16:39:14.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/clone.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1527 2023-04-19 08:23:48.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/env.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-04-17 07:40:14.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/logrotate.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      401 2023-04-21 14:29:02.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     2748 2023-04-19 14:54:32.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1488 2023-04-17 09:13:53.000000 talos_install-0.2.0.dev351/ansible/roles/cli/tasks/web.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.631961 talos_install-0.2.0.dev351/ansible/roles/cli/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3793 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/agent.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      742 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/app.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/cli.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/env_talos.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-04-19 14:05:02.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/globals.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/my-httpd.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      351 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/passwords.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/talos-logrotate.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-04-16 16:14:02.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/talos.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/cli/templates/talospass.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.614961 talos_install-0.2.0.dev351/ansible/roles/common/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.631961 talos_install-0.2.0.dev351/ansible/roles/common/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev351/ansible/roles/common/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.632961 talos_install-0.2.0.dev351/ansible/roles/common/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-04-20 16:08:13.000000 talos_install-0.2.0.dev351/ansible/roles/common/tasks/install_extra_pkgs.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-04-17 08:59:47.000000 talos_install-0.2.0.dev351/ansible/roles/common/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev351/ansible/roles/common/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.614961 talos_install-0.2.0.dev351/ansible/roles/gather_facts/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.632961 talos_install-0.2.0.dev351/ansible/roles/gather_facts/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-04-17 07:54:44.000000 talos_install-0.2.0.dev351/ansible/roles/gather_facts/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.633961 talos_install-0.2.0.dev351/ansible/roles/gather_facts/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      964 2023-04-19 08:35:48.000000 talos_install-0.2.0.dev351/ansible/roles/gather_facts/vars/RedHat.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      964 2023-04-17 07:30:11.000000 talos_install-0.2.0.dev351/ansible/roles/gather_facts/vars/Rocky.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.615961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.615961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.633961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/files/inventory_plugins/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.633961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev351/ansible/roles/install_ansible/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.633961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      389 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev351/ansible/roles/install_ansible/tasks/install_ansible_collection.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1563 2023-04-21 15:41:33.000000 talos_install-0.2.0.dev351/ansible/roles/install_ansible/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.634961 talos_install-0.2.0.dev351/ansible/roles/install_ansible/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      718 2023-04-16 13:01:28.000000 talos_install-0.2.0.dev351/ansible/roles/install_ansible/templates/ansible.cfg.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.615961 talos_install-0.2.0.dev351/ansible/roles/install_certificates/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.634961 talos_install-0.2.0.dev351/ansible/roles/install_certificates/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev351/ansible/roles/install_certificates/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.634961 talos_install-0.2.0.dev351/ansible/roles/install_certificates/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-04-19 14:04:55.000000 talos_install-0.2.0.dev351/ansible/roles/install_certificates/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.616961 talos_install-0.2.0.dev351/ansible/roles/install_docker/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.634961 talos_install-0.2.0.dev351/ansible/roles/install_docker/handlers/
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-17 07:42:54.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/handlers/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.635961 talos_install-0.2.0.dev351/ansible/roles/install_docker/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.635961 talos_install-0.2.0.dev351/ansible/roles/install_docker/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1085 2023-04-20 12:42:13.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      626 2023-04-17 14:19:59.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/tasks/upstream.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.635961 talos_install-0.2.0.dev351/ansible/roles/install_docker/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/templates/daemon.json.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/install_docker/templates/docker-ce.repo.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.616961 talos_install-0.2.0.dev351/ansible/roles/install_python/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.636961 talos_install-0.2.0.dev351/ansible/roles/install_python/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      440 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev351/ansible/roles/install_python/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.636961 talos_install-0.2.0.dev351/ansible/roles/install_python/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/install_python/vars/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.621961 talos_install-0.2.0.dev351/ansible/roles/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.636961 talos_install-0.2.0.dev351/ansible/roles/nagios/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-04-19 14:27:39.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.618961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.617961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.636961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.637961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/conf.d/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.637961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/monitor/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/monitor/.ID
--rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-04-17 14:32:36.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/etc/nagios/resource.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.620961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.637961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.618961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/apache2/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.637961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.619961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.638961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/apache/
--rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/apache/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.638961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/nagios/
--rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.638961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/postfix/
--rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.638961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
--rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.620961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.619961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.638961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.639961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.640961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
--rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1573 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
--rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.640961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.640961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
--rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
--rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.620961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.641961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.620961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/usr/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.620961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/usr/local/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.641961 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/usr/local/bin/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.642961 talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-04-20 16:16:42.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.643961 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/cgi.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/contacts.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3642 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/localhost.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/nagios/templates/nagios.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.623961 talos_install-0.2.0.dev351/ansible/roles/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.643961 talos_install-0.2.0.dev351/ansible/roles/opendcim/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.645961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/apache2.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/apache2.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-04-20 12:27:23.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/default.sql
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.621961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.622961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.645961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/drawings/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.645961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/pictures/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/mysqld.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.622961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.622961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.622961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.645961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.646961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
--rw-rw-r--   0 installer  (3002) installer  (3002)    53192 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
--rw-rw-r--   0 installer  (3002) installer  (3002)    20091 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.646961 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-04-20 13:50:07.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/pre-conf.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-04-20 15:35:00.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/files/startup.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.647961 talos_install-0.2.0.dev351/ansible/roles/opendcim/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.648961 talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.648961 talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-04-20 13:12:20.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-04-20 09:06:15.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/first-run.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/opendcim.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.623961 talos_install-0.2.0.dev351/ansible/roles/os_tune/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.649961 talos_install-0.2.0.dev351/ansible/roles/os_tune/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1281 2023-04-21 12:02:42.000000 talos_install-0.2.0.dev351/ansible/roles/os_tune/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.624961 talos_install-0.2.0.dev351/ansible/roles/talos_users/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.649961 talos_install-0.2.0.dev351/ansible/roles/talos_users/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/talos_users/files/talos
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.649961 talos_install-0.2.0.dev351/ansible/roles/talos_users/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev351/ansible/roles/talos_users/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.649961 talos_install-0.2.0.dev351/ansible/roles/talos_users/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      659 2023-04-17 07:48:59.000000 talos_install-0.2.0.dev351/ansible/roles/talos_users/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.650961 talos_install-0.2.0.dev351/ansible/roles/wiki/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.650961 talos_install-0.2.0.dev351/ansible/roles/wiki/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      536 2023-04-17 07:46:15.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.650961 talos_install-0.2.0.dev351/ansible/roles/wiki/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/meta/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/requirements.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.651961 talos_install-0.2.0.dev351/ansible/roles/wiki/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-04-17 09:16:59.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/tasks/compose.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      222 2023-04-17 07:47:31.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-04-17 07:36:52.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.651961 talos_install-0.2.0.dev351/ansible/roles/wiki/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1153 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/templates/docker-compose.yml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/templates/wiki.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev351/ansible/roles/wiki/templates/wikidump.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1588 2023-04-19 08:30:31.000000 talos_install-0.2.0.dev351/ansible/site.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.652961 talos_install-0.2.0.dev351/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      570 2023-04-19 13:42:43.000000 talos_install-0.2.0.dev351/etc/globals.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev351/etc/inventory
--rw-rw-r--   0 installer  (3002) installer  (3002)     1625 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev351/etc/talos.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-04-21 16:40:19.655961 talos_install-0.2.0.dev351/setup.cfg
--rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-04-21 16:00:17.000000 talos_install-0.2.0.dev351/setup.py
--rwxrwxr-x   0 installer  (3002) installer  (3002)     5949 2023-04-21 16:39:36.000000 talos_install-0.2.0.dev351/talos_install
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-21 16:40:19.654961 talos_install-0.2.0.dev351/talos_install.egg-info/
--rw-rw-r--   0 installer  (3002) installer  (3002)     2018 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     5457 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/SOURCES.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/dependency_links.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-20 13:58:32.000000 talos_install-0.2.0.dev351/talos_install.egg-info/not-zip-safe
--rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/pbr.json
--rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/requires.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-21 16:40:19.000000 talos_install-0.2.0.dev351/talos_install.egg-info/top_level.txt
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.468119 talos_install-0.2.0.dev352/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/AUTHORS
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11660 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/ChangeLog
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3409 2023-04-23 12:53:18.468119 talos_install-0.2.0.dev352/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2749 2023-04-23 11:45:20.000000 talos_install-0.2.0.dev352/README.md
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.436118 talos_install-0.2.0.dev352/ansible/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-04-23 10:12:10.000000 talos_install-0.2.0.dev352/ansible/ansible.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.436118 talos_install-0.2.0.dev352/ansible/group_vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      702 2023-04-23 12:41:16.000000 talos_install-0.2.0.dev352/ansible/group_vars/all.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.432119 talos_install-0.2.0.dev352/ansible/roles/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.421119 talos_install-0.2.0.dev352/ansible/roles/cli/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.436118 talos_install-0.2.0.dev352/ansible/roles/cli/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-21 16:33:02.000000 talos_install-0.2.0.dev352/ansible/roles/cli/files/FOUNDMEDEVKEY
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.436118 talos_install-0.2.0.dev352/ansible/roles/cli/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev352/ansible/roles/cli/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.438119 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1227 2023-04-21 16:39:14.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/clone.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1527 2023-04-19 08:23:48.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/env.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-04-23 09:25:19.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/logrotate.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      401 2023-04-21 14:29:02.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2748 2023-04-19 14:54:32.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-04-23 08:19:34.000000 talos_install-0.2.0.dev352/ansible/roles/cli/tasks/web.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.440118 talos_install-0.2.0.dev352/ansible/roles/cli/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3793 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/agent.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      484 2023-04-23 12:39:17.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/app.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/cli.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-04-18 16:56:49.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/env_talos.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-04-19 14:05:02.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/globals.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/my-httpd.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      351 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/passwords.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/talos-logrotate.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-04-16 16:14:02.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/talos.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/cli/templates/talospass.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.421119 talos_install-0.2.0.dev352/ansible/roles/common/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.440118 talos_install-0.2.0.dev352/ansible/roles/common/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev352/ansible/roles/common/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.441119 talos_install-0.2.0.dev352/ansible/roles/common/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-04-20 16:08:13.000000 talos_install-0.2.0.dev352/ansible/roles/common/tasks/install_extra_pkgs.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-04-17 08:59:47.000000 talos_install-0.2.0.dev352/ansible/roles/common/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-04-17 14:19:19.000000 talos_install-0.2.0.dev352/ansible/roles/common/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.422119 talos_install-0.2.0.dev352/ansible/roles/gather_facts/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.441119 talos_install-0.2.0.dev352/ansible/roles/gather_facts/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-04-23 10:12:13.000000 talos_install-0.2.0.dev352/ansible/roles/gather_facts/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.442119 talos_install-0.2.0.dev352/ansible/roles/gather_facts/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      930 2023-04-23 08:16:31.000000 talos_install-0.2.0.dev352/ansible/roles/gather_facts/vars/RedHat.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      929 2023-04-23 08:19:34.000000 talos_install-0.2.0.dev352/ansible/roles/gather_facts/vars/Rocky.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.422119 talos_install-0.2.0.dev352/ansible/roles/install_ansible/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.422119 talos_install-0.2.0.dev352/ansible/roles/install_ansible/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.442119 talos_install-0.2.0.dev352/ansible/roles/install_ansible/files/inventory_plugins/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.442119 talos_install-0.2.0.dev352/ansible/roles/install_ansible/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev352/ansible/roles/install_ansible/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.442119 talos_install-0.2.0.dev352/ansible/roles/install_ansible/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-04-23 12:42:57.000000 talos_install-0.2.0.dev352/ansible/roles/install_ansible/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.443118 talos_install-0.2.0.dev352/ansible/roles/install_ansible/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      512 2023-04-23 08:08:27.000000 talos_install-0.2.0.dev352/ansible/roles/install_ansible/templates/ansible.cfg.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.423118 talos_install-0.2.0.dev352/ansible/roles/install_certificates/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.443118 talos_install-0.2.0.dev352/ansible/roles/install_certificates/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev352/ansible/roles/install_certificates/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.443118 talos_install-0.2.0.dev352/ansible/roles/install_certificates/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-04-19 14:04:55.000000 talos_install-0.2.0.dev352/ansible/roles/install_certificates/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.423118 talos_install-0.2.0.dev352/ansible/roles/install_docker/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.443118 talos_install-0.2.0.dev352/ansible/roles/install_docker/handlers/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-23 10:25:12.000000 talos_install-0.2.0.dev352/ansible/roles/install_docker/handlers/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.444119 talos_install-0.2.0.dev352/ansible/roles/install_docker/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-04-17 08:56:10.000000 talos_install-0.2.0.dev352/ansible/roles/install_docker/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.444119 talos_install-0.2.0.dev352/ansible/roles/install_docker/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-04-23 10:25:12.000000 talos_install-0.2.0.dev352/ansible/roles/install_docker/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.444119 talos_install-0.2.0.dev352/ansible/roles/install_docker/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/install_docker/templates/daemon.json.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/install_docker/templates/docker-ce.repo.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.424119 talos_install-0.2.0.dev352/ansible/roles/install_python/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.444119 talos_install-0.2.0.dev352/ansible/roles/install_python/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-04-22 13:21:05.000000 talos_install-0.2.0.dev352/ansible/roles/install_python/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.445119 talos_install-0.2.0.dev352/ansible/roles/install_python/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/install_python/vars/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.428119 talos_install-0.2.0.dev352/ansible/roles/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.445119 talos_install-0.2.0.dev352/ansible/roles/nagios/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-04-19 14:27:39.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.425119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.425119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.445119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.445119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/conf.d/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.446118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/monitor/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/monitor/.ID
+-rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-04-17 14:32:36.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/etc/nagios/resource.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.428119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.446118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.425119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/apache2/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.446118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.426118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.446118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/apache/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/apache/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.447119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/nagios/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.447119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/postfix/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.447119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.427118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.427118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.447119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.448119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.448119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1573 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.449118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.449118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
+-rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.427118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.450118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.428119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/usr/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.428119 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/usr/local/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.450118 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/usr/local/bin/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.452118 talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-04-20 16:16:42.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.453118 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/cgi.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/contacts.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3642 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/localhost.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/nagios/templates/nagios.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.431119 talos_install-0.2.0.dev352/ansible/roles/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.453118 talos_install-0.2.0.dev352/ansible/roles/opendcim/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-04-19 14:28:09.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.455119 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/apache2.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/apache2.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-04-20 12:27:23.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/default.sql
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.429118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.429118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.455119 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/drawings/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.455119 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/pictures/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/mysqld.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.430118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.430118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.430118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.455119 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.456118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    53192 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)    20091 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.456118 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-04-16 11:59:41.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-04-16 16:55:50.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-04-20 13:50:07.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/pre-conf.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-04-20 15:35:00.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/files/startup.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.456118 talos_install-0.2.0.dev352/ansible/roles/opendcim/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.457119 talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-04-19 16:25:03.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-04-17 08:56:47.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.458119 talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-04-20 13:12:20.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-04-20 09:06:15.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/first-run.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/opendcim.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.431119 talos_install-0.2.0.dev352/ansible/roles/os_tune/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.458119 talos_install-0.2.0.dev352/ansible/roles/os_tune/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-04-23 12:39:17.000000 talos_install-0.2.0.dev352/ansible/roles/os_tune/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.432119 talos_install-0.2.0.dev352/ansible/roles/talos_users/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.459118 talos_install-0.2.0.dev352/ansible/roles/talos_users/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/talos_users/files/talos
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.459118 talos_install-0.2.0.dev352/ansible/roles/talos_users/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev352/ansible/roles/talos_users/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.459118 talos_install-0.2.0.dev352/ansible/roles/talos_users/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-04-22 13:28:03.000000 talos_install-0.2.0.dev352/ansible/roles/talos_users/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.432119 talos_install-0.2.0.dev352/ansible/roles/uninstall/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.459118 talos_install-0.2.0.dev352/ansible/roles/uninstall/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-04-23 12:39:17.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.459118 talos_install-0.2.0.dev352/ansible/roles/uninstall/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-22 11:25:57.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.460119 talos_install-0.2.0.dev352/ansible/roles/uninstall/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      660 2023-04-23 08:20:18.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/tasks/cli.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-04-22 13:37:20.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/tasks/docker.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-04-22 11:29:44.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      345 2023-04-22 12:20:03.000000 talos_install-0.2.0.dev352/ansible/roles/uninstall/tasks/user.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.461119 talos_install-0.2.0.dev352/ansible/roles/wiki/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.461119 talos_install-0.2.0.dev352/ansible/roles/wiki/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      536 2023-04-17 07:46:15.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.461119 talos_install-0.2.0.dev352/ansible/roles/wiki/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-04-17 08:55:42.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/meta/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/requirements.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.465119 talos_install-0.2.0.dev352/ansible/roles/wiki/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-04-17 09:16:59.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/tasks/compose.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      222 2023-04-17 07:47:31.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-04-17 07:36:52.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.466118 talos_install-0.2.0.dev352/ansible/roles/wiki/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1153 2023-04-19 14:19:14.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/templates/docker-compose.yml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/templates/wiki.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-04-16 11:59:40.000000 talos_install-0.2.0.dev352/ansible/roles/wiki/templates/wikidump.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1727 2023-04-23 12:39:17.000000 talos_install-0.2.0.dev352/ansible/site.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.466118 talos_install-0.2.0.dev352/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      293 2023-04-23 11:14:48.000000 talos_install-0.2.0.dev352/etc/globals.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev352/etc/inventory
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1066 2023-04-23 11:16:27.000000 talos_install-0.2.0.dev352/etc/talos.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-04-23 12:53:18.485118 talos_install-0.2.0.dev352/setup.cfg
+-rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-04-21 16:00:17.000000 talos_install-0.2.0.dev352/setup.py
+-rwxrwxr-x   0 installer  (3002) installer  (3002)     9008 2023-04-23 12:39:17.000000 talos_install-0.2.0.dev352/talos_install
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-04-23 12:53:18.468119 talos_install-0.2.0.dev352/talos_install.egg-info/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3409 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5583 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/SOURCES.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/dependency_links.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-20 13:58:32.000000 talos_install-0.2.0.dev352/talos_install.egg-info/not-zip-safe
+-rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/pbr.json
+-rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/requires.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-04-23 12:53:18.000000 talos_install-0.2.0.dev352/talos_install.egg-info/top_level.txt
```

### Comparing `talos_install-0.2.0.dev351/ChangeLog` & `talos_install-0.2.0.dev352/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGES
 =======
 
+* Enhance talos\_install
 * fix missing dev\_keys installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix missing ansible installation
 * fix missing ansible installation
```

### Comparing `talos_install-0.2.0.dev351/ansible/roles/cli/tasks/clone.yaml` & `talos_install-0.2.0.dev352/ansible/roles/cli/tasks/clone.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/cli/tasks/env.yaml` & `talos_install-0.2.0.dev352/ansible/roles/cli/tasks/env.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/cli/tasks/misc.yaml` & `talos_install-0.2.0.dev352/ansible/roles/cli/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/cli/tasks/web.yaml` & `talos_install-0.2.0.dev352/ansible/roles/cli/tasks/web.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,23 @@
     src: "{{ app.etcdir }}/html/htpasswd"
     dest: "{{ app.webdir }}/html/htpasswd"
     remote_src: true
     force: true
     follow: true
     mode: '0755'
 
+- name: Backup config files
+  ansible.builtin.copy:
+    src: "{{ http_config }}"
+    dest: "{{ http_config }}.old"
+    remote_src: true
+    force: true
+    follow: true
+    mode: '0755'
+
 - name: Copy templates
   ansible.builtin.template:
     src: "{{ item.file }}.j2"
     dest: "{{ item.dest }}"
     mode: "{{ item.mode }}"
   loop:
     - file: agent.sh
```

### Comparing `talos_install-0.2.0.dev351/ansible/roles/cli/templates/agent.sh.j2` & `talos_install-0.2.0.dev352/ansible/roles/cli/templates/agent.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/cli/templates/cli.conf.j2` & `talos_install-0.2.0.dev352/ansible/roles/cli/templates/cli.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/cli/templates/env_talos.j2` & `talos_install-0.2.0.dev352/ansible/roles/cli/templates/env_talos.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/cli/templates/globals.yaml.j2` & `talos_install-0.2.0.dev352/ansible/roles/cli/templates/globals.yaml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/cli/templates/my-httpd.conf.j2` & `talos_install-0.2.0.dev352/ansible/roles/cli/templates/my-httpd.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/cli/templates/talos.conf.j2` & `talos_install-0.2.0.dev352/ansible/roles/cli/templates/talos.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/common/tasks/misc.yaml` & `talos_install-0.2.0.dev352/ansible/roles/common/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/gather_facts/vars/RedHat.yaml` & `talos_install-0.2.0.dev352/ansible/roles/gather_facts/vars/RedHat.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -28,34 +28,31 @@
   - python3-argcomplete
   - rust
   - cargo
   - curl
   - sshpass
 
 pkgansible:
-  - ansible
+  - ansible>=7,<8
 
 ### Certificate
 certdir: /etc/pki/ca-trust/source/anchors/
 
 certcmd: update-ca-trust
 
 ### Common
 pkg_cli:
-  - epel-release
   - git
   - colordiff
   - vim
   - mtr
   - nmap
-  - figlet
   - htop
   - jq
   - yamllint
-  - sshpass
   - dos2unix
   - wget
   - bash-completion
   - cmake
   - gcc-c++
   - sysstat
   - pssh
```

### Comparing `talos_install-0.2.0.dev351/ansible/roles/gather_facts/vars/Rocky.yaml` & `talos_install-0.2.0.dev352/ansible/roles/gather_facts/vars/Rocky.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -28,34 +28,31 @@
   - python3-argcomplete
   - rust
   - cargo
   - curl
   - sshpass
 
 pkgansible:
-  - ansible
+  - ansible>=7,<8
 
 ### Certificate
 certdir: /etc/pki/ca-trust/source/anchors/
 
 certcmd: update-ca-trust
 
 ### Common
 pkg_cli:
-  - epel-release
   - git
   - colordiff
   - vim
   - mtr
   - nmap
-  - figlet
   - htop
   - jq
   - yamllint
-  - sshpass
   - dos2unix
   - wget
   - bash-completion
   - cmake
   - gcc-c++
   - sysstat
   - pssh
@@ -63,13 +60,12 @@
   - dnf-plugins-core
   - nfs-utils
   - arp-scan
 
 pkgpowertools:
   - pandoc
 
-
 venvcmd: virtualenv-3
 http_service: httpd
 php_service: php
 http_config: /etc/httpd/conf/httpd.conf
 serverroot: /etc/httpd
```

### Comparing `talos_install-0.2.0.dev351/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py` & `talos_install-0.2.0.dev352/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/install_ansible/tasks/main.yaml` & `talos_install-0.2.0.dev352/ansible/roles/install_ansible/tasks/main.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,20 @@
   ansible.builtin.package:
     name: "{{ item }}"
     state: present
     update_cache: true
   loop: '{{ pkgreqansible }}'
 
 - name: Install Ansible
-  ansible.builtin.package:
-    name: "{{ item }}"
+  ansible.builtin.pip:
+    name: "{{ pkgansible }}"
     state: present
-    update_cache: true
-  loop: '{{ pkgansible }}'
+    extra_args: --user --upgrade
+    executable: pip3.9
+  become_user: "{{ master.user }}"
 
 - name: Ensure master Permission
   ansible.builtin.file:
     state: directory
     path: "{{ item }}"
     owner: "{{ master.user }}"
     group: "{{ master.group }}"
@@ -48,9 +49,11 @@
 
 - name: Copy yamlgroup inventory in place
   ansible.builtin.copy:
     src: inventory_plugins/yamlgroup.py
     dest: "{{ app.etcdir }}/ansible/inventory_plugins/yamlgroup.py"
     mode: '0644'
 
-- name: Install Ansible collections
-  ansible.builtin.include_tasks: install_ansible_collection.yaml
+- name: Download required ansible collections
+  ansible.builtin.command: "sudo su -l {{ master.user }} -c 'ANSIBLE_CONFIG={{ app.etcdir }}/ansible/ansible.cfg \
+    ansible-galaxy collection install {{ item }} -i --force'"
+  loop: "{{ ansible.collections }}"
```

### Comparing `talos_install-0.2.0.dev351/ansible/roles/install_certificates/tasks/main.yaml` & `talos_install-0.2.0.dev352/ansible/roles/install_certificates/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/install_docker/templates/docker-ce.repo.j2` & `talos_install-0.2.0.dev352/ansible/roles/install_docker/templates/docker-ce.repo.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/nagios/run` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/nagios/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/etc/sv/postfix/run` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/etc/sv/postfix/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios` & `talos_install-0.2.0.dev352/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/build.yaml` & `talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/misc.yaml` & `talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/tasks/run.yaml` & `talos_install-0.2.0.dev352/ansible/roles/nagios/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/templates/Dockerfile.j2` & `talos_install-0.2.0.dev352/ansible/roles/nagios/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/templates/cgi.cfg.j2` & `talos_install-0.2.0.dev352/ansible/roles/nagios/templates/cgi.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/templates/contacts.cfg.j2` & `talos_install-0.2.0.dev352/ansible/roles/nagios/templates/contacts.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/nagios/templates/localhost.cfg.j2` & `talos_install-0.2.0.dev352/ansible/roles/nagios/templates/localhost.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/apache2.conf` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/apache2.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/default.sql` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/default.sql`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/pre-conf.sh` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/pre-conf.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/files/startup.sh` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/files/startup.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/build.yaml` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/misc.yaml` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/tasks/run.yaml` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/Dockerfile.j2` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/opendcim/templates/first-run.sh.j2` & `talos_install-0.2.0.dev352/ansible/roles/opendcim/templates/first-run.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/os_tune/tasks/main.yaml` & `talos_install-0.2.0.dev352/ansible/roles/os_tune/tasks/main.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -5,50 +5,52 @@
     use: systemd
 
 - name: Stop Firewall
   ansible.builtin.service:
     name: firewalld
     enabled: false
     state: stopped
-  register: results
+  register: os_tune_stop_firewalld
   failed_when: >-
-    results is failed and
-    "Could not find the requested service" not in results.msg|default('')
+    os_tune_stop_firewalld is failed and
+    "Could not find the requested service" not in os_tune_stop_firewalld.msg|default('')
 
 - name: Set timezone
   community.general.timezone:
     name: "{{ customer.timezone }}"
 
 - name: Disabling SELinux
   ansible.posix.selinux:
     state: disabled
-  register: selinuxdisabled
+  register: os_tune_disable_selinux
 
 - name: System will be rebooted for Selinux Changes
   ansible.builtin.pause:
     prompt: "!!! System will reboot in 10 seconds. !!!"
     seconds: 10
-  when: selinuxdisabled is changed
+  when: os_tune_disable_selinux is changed
 
 - name: Wait for 5 Second and Reboot
   ansible.builtin.reboot:
-  when: selinuxdisabled is changed
+  when: os_tune_disable_selinux is changed
 
 - name: Change StrictHostKeyChecking
   ansible.builtin.lineinfile:
     dest: /etc/ssh/ssh_config
     state: present
     regexp: 'StrictHostKeyChecking'
     line: 'StrictHostKeyChecking no'
 
 - name: Change StrictModes
   ansible.builtin.lineinfile:
     dest: /etc/ssh/sshd_config
     state: present
     regexp: 'StrictModes'
     line: 'StrictModes no'
+  register: ssh_strict
 
 - name: Restart sshd
   ansible.builtin.service:
     name: sshd
     enabled: true
     state: restarted
+  when: ssh_strict is changed
```

### Comparing `talos_install-0.2.0.dev351/ansible/roles/talos_users/tasks/main.yaml` & `talos_install-0.2.0.dev352/ansible/roles/talos_users/tasks/main.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ---
 - name: Check that the MASTER id_rsa exists
   ansible.builtin.stat:
     path: "/home/{{ master.user }}/.ssh/id_rsa"
   register: stat_result
 
-- name: Add the user talos-master with a bash shell, appending the group 'docker' to the user's groups
+- name: Add the user talos-master
   ansible.builtin.user:
     name: "{{ master.user }}"
     shell: /bin/bash
     uid: "{{ master.uid }}"
     password: "{{ master.password | password_hash('sha512') }}"
     generate_ssh_key: true
     force: false
```

### Comparing `talos_install-0.2.0.dev351/ansible/roles/wiki/defaults/main.yaml` & `talos_install-0.2.0.dev352/ansible/roles/wiki/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/wiki/tasks/compose.yaml` & `talos_install-0.2.0.dev352/ansible/roles/wiki/tasks/compose.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/roles/wiki/templates/docker-compose.yml.j2` & `talos_install-0.2.0.dev352/ansible/roles/wiki/templates/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/ansible/site.yaml` & `talos_install-0.2.0.dev352/ansible/site.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       when: cli_action in ['bootstrap']
 
     - role: install_certificates
       become: true
       tags: certificates
       when: cli_action in ['bootstrap']
 
-- hosts: "builder"
+- hosts: all
   name: "Build container"
   roles:
     - role: install_docker
       become: true
       tags: docker
       when: cli_action in ['build']
 
@@ -59,22 +59,29 @@
       when: cli_action in ['deploy']
 
     - role: cli
       become: true
       tags: cli
       when: cli_action in ['deploy']
 
-
     - role: nagios
       become: true
       tags: nagios
       when: cli_action in ['deploy']
 
     - role: opendcim
       become: true
       tags: opendcim
       when: cli_action in ['deploy']
 
     - role: wiki
       become: true
       tags: wiki
       when: cli_action in ['deploy']
+
+- hosts: all
+  name: "Uninstall"
+  roles:
+    - role: uninstall
+      become: true
+      tags: uninstall
+      when: cli_action in ['uninstall']
```

### Comparing `talos_install-0.2.0.dev351/setup.cfg` & `talos_install-0.2.0.dev352/setup.cfg`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev351/talos_install` & `talos_install-0.2.0.dev352/talos_install`

 * *Files 26% similar despite different names*

```diff
@@ -16,54 +16,142 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with TALOS-CLI.  If not, see <http://www.gnu.org/licenses/>.
 #
 
+check_no_root_sudo(){
+  if [[ $(whoami) == "root" ]]; then
+    echo "Run as root is not supported"
+    exit 2
+  elif [[ $(sudo -l &> /dev/null; echo $?) -ne 0 ]]; then
+    echo "User $(whoami) is not sudoers"
+    exit 2
+  fi
+}
+
 check_for_target(){
-    echo $hostdef > $inventory
-    if [[ -z $target ]]; then target=$(hostname); fi
-    target_ip=$(ping $target -4 -c 1 | grep PING | awk '{print $3}' | tr -dc '[:alnum:][.]\n')
-    echo "$target   ssh_ip=$target_ip"  >> $inventory
+  echo $hostdef > $inventory
+  if [[ -z $target ]]; then target=$(hostname); fi
+  target_ip=$(ping $target -4 -c 1 | grep PING | awk '{print $3}' | tr -dc '[:alnum:][.]\n')
+  echo "$target   ssh_ip=$target_ip"  >> $inventory
+  # Try to prevent ssh_pass error copying pub key in authorized_keys file
+  if [[ $(grep -c "$(cat ~/.ssh/id_rsa.pub| awk '{print $2}')" ~/.ssh/authorized_keys) -eq 0 ]]; then
+    cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys
+  fi
 }
 
+
 check_environment_coherence(){
-  sudo dnf install epel-release -y &>/dev/null
+  if [[ $(rpm -qa | grep -c epel-release) -ne 1 ]]; then
+    sudo dnf install epel-release -y &>/dev/null
+  fi
   if ! which python3.9 &>/dev/null ; then
     echo "Missing Python 3.9"
     exit 2
   fi
 
   if ! which pip3.9 &>/dev/null ; then
     echo "Missing pip 3.9"
     exit 2
   fi
 
   if ! which ansible &>/dev/null ; then
     echo "Missing ansible"
     exit 2
   fi
+}
 
+talos_install_menu(){
+  title_message="$1"
+  clear
+  # Get Terminal info
+  echo "TALOS-CLI | HPC Manager Platform "
+  printf "# $title_message\n\n"
 }
 
-check_selinux(){
+confirm_bootstrap(){
+  talos_install_menu "Talos Bootstrap"
   current_selinux=$(grep ^SELINUX= /etc/selinux/config | cut -d= -f2)
+
+  echo "These actions will be performed:
+  - Add an user {{ master.user }} with sudo permission.
+  - Install python dependencies
+  - Stop firewall service (if present)
+  - Set Timezone {{ customer.timezone }}"
   if [[ "$current_selinux" != "disabled" ]]; then
-    echo "Selinux need to be disabled, a Reboot will occour during installation"
-    reply=false
-    while ! $reply; do
-      read -rp "Do you want to proceed? [y/n] " read_reply
-      case $read_reply in
-        y|Y) reply=true ;;
-        n|N)
-          exit 3 ;;
-      esac
-    done
+    echo "- Disable Selinux
+    !!! A REBOOT WILL OCCOUR DURING INSTALLATION !!!"
+  fi
+  echo "  - Install docker and give to {{ master.user }} permission to run containers
+  - Install ansible dependencies
+  - Install CA certificates (if required by {{ ca_idm.enable }})
+  "
+  confirm_action
+}
+
+confirm_deploy(){
+  talos_install_menu "Talos deploy"
+
+  echo "These actions will be performed:
+  - Create Talos environment paths
+  - Install Talos-cli dependencies
+  - Install Talos-cli source code
+  - Install and configure logrotate
+  - Install and start Web services
+  - Pull Nagios docker
+  - Pull OpenDcim docker
+  - Pull Wiki.js Docker
+  "
+  confirm_action
+}
+
+confirm_destroy(){
+  talos_install_menu "Talos Uninstall"
+  current_selinux=$(grep ^SELINUX= /etc/selinux/config | cut -d= -f2)
+
+  echo "These actions will be performed:
+  - Remove user {{ master.user }}
+  - Delete Talos environment paths
+  - Uninstall Talos-cli source code
+  - Uninstall logrotate
+  - Uninstall Web services
+  - Prune Nagios docker
+  - Prune OpenDcim docker
+  - Prune Wiki.js Docker
+  "
+  confirm_action
+}
+
+confirm_build(){
+  talos_install_menu "Talos build image"
+
+  echo "These actions will be performed:
+  - Push Nagios container on Docker
+  - Push OpenDcim container on Docker"
+
+  echo "!!! THESE ACTIONS REQUIRE A VALID DOCKER TOKEN !!!
+  "
+  confirm_action
+}
+
+confirm_action(){
+  if $force_install ; then reply=true
+  else reply=false
   fi
+
+  while ! $reply; do
+    read -rp "Do you want to proceed? [y/n] " read_reply
+    case $read_reply in
+      y|Y) reply=true ;;
+      n|N)
+        exit 3 ;;
+    esac
+  done
 }
 
 process_cmd(){
     echo "$action : $cmd"
     $cmd
     if [[ $? -ne 0 ]]; then
         echo "Command failed $cmd"
@@ -91,48 +179,63 @@
 Environment variables:
     extra_opts                         Additional arguments to pass to ansible-playbook
 
 Commands:
     bootstrap            Bootstrap servers with talos deploy dependencies
     deploy               Deploy and start main talos containers
     build                Build talos custom containers
+    uninstall            Uninstall Talos-cli
 EOF
 }
 
-check_environment_coherence
-
-short_opts="h:t:k:e:v"
-long_opts="help,skip-tags:,tags:,key:,extra:,verbose,limit:,forks:,vault-id:,ask-vault-pass,vault-password-file:"
+### MAIN HERE
 
-args=$(getopt -o "${short_opts}" -l "${long_opts}" --name "$0" -- "$@") || { usage >&2; exit 2; }
-
-eval set -- "$args"
-
-dir=$(which talos_install)
-dir="$(dirname $dir)"
-dir="$(dirname $dir)"
+# Check Environment
+check_no_root_sudo
+check_environment_coherence
 
-basedir=${dir}/share/talos_install
+# Verifiy if system is able to find shared palybooks
+if [[ -n $TPATH ]]; then
+  basedir="${TPATH}/share/talos_install"
+else
+  env_bin=$(pip debug 2>/dev/null | grep sys.executable | awk '{print $2}')
+  env_bin="$(dirname $env_bin)"
+  env_bin="$(dirname $env_bin)"
+  basedir=${env_bin}/share/talos_install
+fi
+if [[ ! -d "$basedir" ]]; then
+  echo "Unable to find $basedir. Please try to pass right path as TPATH=/path/to/..."
+  exit 127
+fi
 
+# Verifify if user have dev_key for GIT
 if [[ -f ~/.ssh/dev_key ]]; then
   \cp ~/.ssh/dev_key* ${basedir}/ansible/roles/cli/files/
 else
   echo "Missing dev_key in ~/.ssh folder"
-  exit 2
+  exit 127
 fi
 
+# Start check options
+short_opts="h:t:k:e:v:y"
+long_opts="help,skip-tags:,tags:,key:,extra:,verbose,limit:,forks:,vault-id:,ask-vault-pass,vault-password-file:"
+
+args=$(getopt -o "${short_opts}" -l "${long_opts}" --name "$0" -- "$@") || { usage >&2; exit 2; }
+
+eval set -- "$args"
 
 ANSIBLE_CONFIG="${basedir}/ansible/ansible.cfg"
 config_dir="${basedir}/etc"
 inventory="${basedir}/etc/inventory"
 playbook="${basedir}/ansible/site.yml"
 verbosity=""
 extra_opts=""
 target=""
 hostdef="[talos]"
+force_install=false
 
 while [ "$#" -gt 0 ]; do
     case "$1" in
     (--skip-tags)
       extra_opts="$extra_opts --skip-tags $2" ; shift 2 ;;
     (--tags|-t)
       extra_opts="$extra_opts --tags $2" ; shift 2 ;;
@@ -154,41 +257,51 @@
       verbosity="$extra_opts --ask-vault-pass" ; shift 1 ;;
     (--vault-password-file)
       extra_opts="$extra_opts --vault-password-file $2" ; shift 2 ;;
     (--help|-h)
       usage ; shift ; exit 0 ;;
     (--)
       shift ; break ;;
+    (-y)
+      force_install=true ; shift ;;
     (*)
-      echo "error" ; exit 3 ;;
+      echo "Syntax error" ; usage ; exit 1 ;;
 esac
 done
 
 case "$1" in
   (bootstrap)
-    check_selinux
+    confirm_bootstrap
     action="Bootstrapping servers"
     playbook="${basedir}/ansible/site.yaml"
     extra_opts="$extra_opts -e cli_action=bootstrap"
     hostdef="[talos]" ;;
   (build)
+    confirm_build
     action="Build Talos containers"
     playbook="${basedir}/ansible/site.yaml"
     extra_opts="$extra_opts -e cli_action=build"
     hostdef="[builder]" ;;
   (deploy)
+    confirm_deploy
     action="Deploying Playbooks"
     playbook="${basedir}/ansible/site.yaml"
     extra_opts="$extra_opts -e cli_action=deploy"
     hostdef="[talos]" ;;
+  (uninstall)
+    confirm_destroy
+    action="Uninstall talos"
+    playbook="${basedir}/ansible/site.yaml"
+    extra_opts="$extra_opts -e cli_action=uninstall"
+    hostdef="[talos]" ;;
   (*)
     usage
     exit 0 ;;
 esac
 
 check_for_target
 
 export ANSIBLE_CONFIG
-config_opts="-e @${config_dir}/talos.yaml -e @${config_dir}/globals.yaml -e config_dir=${config_dir}"
+config_opts="-e @${config_dir}/talos.yaml -e @${config_dir}/globals.yaml -e config_dir=${config_dir} -e ansible_user=$(whoami)"
 
 cmd="ansible-playbook -i $inventory $config_opts $extra_opts $playbook $verbosity"
 process_cmd
```

### Comparing `talos_install-0.2.0.dev351/talos_install.egg-info/SOURCES.txt` & `talos_install-0.2.0.dev352/talos_install.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,23 +30,21 @@
 ansible/roles/common/tasks/main.yaml
 ansible/roles/common/tasks/misc.yaml
 ansible/roles/gather_facts/tasks/main.yaml
 ansible/roles/gather_facts/vars/RedHat.yaml
 ansible/roles/gather_facts/vars/Rocky.yaml
 ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
 ansible/roles/install_ansible/meta/main.yaml
-ansible/roles/install_ansible/tasks/install_ansible_collection.yaml
 ansible/roles/install_ansible/tasks/main.yaml
 ansible/roles/install_ansible/templates/ansible.cfg.j2
 ansible/roles/install_certificates/meta/main.yaml
 ansible/roles/install_certificates/tasks/main.yaml
 ansible/roles/install_docker/handlers/main.yaml
 ansible/roles/install_docker/meta/main.yaml
 ansible/roles/install_docker/tasks/main.yaml
-ansible/roles/install_docker/tasks/upstream.yaml
 ansible/roles/install_docker/templates/daemon.json.j2
 ansible/roles/install_docker/templates/docker-ce.repo.j2
 ansible/roles/install_python/tasks/main.yaml
 ansible/roles/install_python/vars/.ID
 ansible/roles/nagios/defaults/main.yaml
 ansible/roles/nagios/files/etc/nagios/resource.cfg
 ansible/roles/nagios/files/etc/nagios/conf.d/.ID
@@ -99,14 +97,20 @@
 ansible/roles/opendcim/templates/Dockerfile.j2
 ansible/roles/opendcim/templates/first-run.sh.j2
 ansible/roles/opendcim/templates/opendcim.conf.j2
 ansible/roles/os_tune/tasks/main.yaml
 ansible/roles/talos_users/files/talos
 ansible/roles/talos_users/meta/main.yaml
 ansible/roles/talos_users/tasks/main.yaml
+ansible/roles/uninstall/defaults/main.yaml
+ansible/roles/uninstall/meta/main.yaml
+ansible/roles/uninstall/tasks/cli.yaml
+ansible/roles/uninstall/tasks/docker.yaml
+ansible/roles/uninstall/tasks/main.yaml
+ansible/roles/uninstall/tasks/user.yaml
 ansible/roles/wiki/requirements.yaml
 ansible/roles/wiki/defaults/main.yaml
 ansible/roles/wiki/meta/main.yaml
 ansible/roles/wiki/tasks/compose.yaml
 ansible/roles/wiki/tasks/main.yaml
 ansible/roles/wiki/tasks/misc.yaml
 ansible/roles/wiki/templates/docker-compose.yml.j2
```

