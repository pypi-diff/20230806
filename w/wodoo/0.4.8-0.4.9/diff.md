# Comparing `tmp/wodoo-0.4.8.tar.gz` & `tmp/wodoo-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wodoo-0.4.8.tar", last modified: Thu Jun 29 14:41:06 2023, max compression
+gzip compressed data, was "wodoo-0.4.9.tar", last modified: Thu Jun 29 14:43:59 2023, max compression
```

## Comparing `wodoo-0.4.8.tar` & `wodoo-0.4.9.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.647661 wodoo-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 14:40:35.000000 wodoo-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-29 14:41:06.647661 wodoo-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-29 14:40:35.000000 wodoo-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-29 14:41:06.647661 wodoo-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-29 14:40:35.000000 wodoo-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.635661 wodoo-0.4.8/wodoo/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/click_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/click_global_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.639661 wodoo-0.4.8/wodoo/config/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/config/cicd_network_for_project.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/config/default_network
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/config/template_onlyloop.yml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/config/template_withports.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7012 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/daddy_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/defaults
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.623661 wodoo-0.4.8/wodoo/extra_install/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.623661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.639661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/debug.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/interactive.sh
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.639661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/config
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa.pub
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.639661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.639661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.639661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/ari_additional_custom.conf.appendix
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/manager_custom.conf.appendix
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.643661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.643661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/freepbx_chown.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.643661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/
--rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/10-freepbx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.643661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/10-start
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.643661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/apache2
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/asterisk
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fail2ban
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fop
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbc.ini
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbcinst.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.643661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/08-ssh
--rwxr-xr-x   0 runner    (1001) docker     (123)      567 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb
--rwxr-xr-x   0 runner    (1001) docker     (123)    17011 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/13-extra-modules
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/15-permissions
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/16-soundlang
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/20-load-default-extensions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.627661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.643661 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/authorized_keys
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/run_freepbx.sh
--rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_clickhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    32024 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_control_with_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_db_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_db_snapshots_docker_btrfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_db_snapshots_docker_zfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_db_snapshots_plain_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)    50013 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_src.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_talk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/lib_turnintodev.py
--rw-r--r--   0 runner    (1001) docker     (123)    55119 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/module_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/myconfigparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/odoo_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    25337 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/odoo_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/pudb.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/robo_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.643661 wodoo-0.4.8/wodoo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/tests/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/tests/gimera.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.643661 wodoo-0.4.8/wodoo/tests/module_respartner_dummyfield1/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/tests/module_respartner_dummyfield1/partnerview.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.643661 wodoo-0.4.8/wodoo/tests/module_respartner_dummyfield2/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/tests/module_respartner_dummyfield2/partnerview.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/testzfs.sh
--rw-r--r--   0 runner    (1001) docker     (123)    42346 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 14:41:02.000000 wodoo-0.4.8/wodoo/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.647661 wodoo-0.4.8/wodoo/wait/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/wait/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/wait/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/wait/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-29 14:40:35.000000 wodoo-0.4.8/wodoo/wait/tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:41:06.639661 wodoo-0.4.8/wodoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-29 14:41:06.000000 wodoo-0.4.8/wodoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-29 14:41:06.000000 wodoo-0.4.8/wodoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:41:06.000000 wodoo-0.4.8/wodoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 14:41:06.000000 wodoo-0.4.8/wodoo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 14:41:06.000000 wodoo-0.4.8/wodoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 14:41:06.000000 wodoo-0.4.8/wodoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.821270 wodoo-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 14:43:37.000000 wodoo-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-29 14:43:59.821270 wodoo-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-29 14:43:37.000000 wodoo-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-29 14:43:59.821270 wodoo-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-29 14:43:37.000000 wodoo-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.813270 wodoo-0.4.9/wodoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/click_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/click_global_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.813270 wodoo-0.4.9/wodoo/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/config/cicd_network_for_project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/config/default_network
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/config/template_onlyloop.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/config/template_withports.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7012 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/daddy_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/defaults
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.805270 wodoo-0.4.9/wodoo/extra_install/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.805270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.813270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/debug.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/interactive.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.813270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/config
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.817270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.817270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.817270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/ari_additional_custom.conf.appendix
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/config/manager_custom.conf.appendix
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.817270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.817270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/asterisk/freepbx_chown.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.817270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-finish.d/10-freepbx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.817270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/cont-init.d/10-start
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.817270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/apache2
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/asterisk
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fail2ban
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/logrotate.d/fop
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbc.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/etc/odbcinst.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.817270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/08-ssh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      567 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17011 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/13-extra-modules
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/15-permissions
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/16-soundlang
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/20-load-default-extensions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.805270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.817270 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/root/.ssh/authorized_keys
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/run_freepbx.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_clickhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32024 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_control_with_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_db_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_db_snapshots_docker_btrfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_db_snapshots_docker_zfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_db_snapshots_plain_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50013 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_src.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_talk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/lib_turnintodev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55119 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/module_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/myconfigparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/odoo_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25337 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/odoo_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/pudb.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/robo_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.817270 wodoo-0.4.9/wodoo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/tests/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/tests/gimera.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.821270 wodoo-0.4.9/wodoo/tests/module_respartner_dummyfield1/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/tests/module_respartner_dummyfield1/partnerview.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.821270 wodoo-0.4.9/wodoo/tests/module_respartner_dummyfield2/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/tests/module_respartner_dummyfield2/partnerview.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/testzfs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    42346 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 14:43:56.000000 wodoo-0.4.9/wodoo/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.821270 wodoo-0.4.9/wodoo/wait/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/wait/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/wait/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/wait/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-29 14:43:37.000000 wodoo-0.4.9/wodoo/wait/tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:43:59.813270 wodoo-0.4.9/wodoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-29 14:43:59.000000 wodoo-0.4.9/wodoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-29 14:43:59.000000 wodoo-0.4.9/wodoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:43:59.000000 wodoo-0.4.9/wodoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 14:43:59.000000 wodoo-0.4.9/wodoo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 14:43:59.000000 wodoo-0.4.9/wodoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 14:43:59.000000 wodoo-0.4.9/wodoo.egg-info/top_level.txt
```

### Comparing `wodoo-0.4.8/LICENSE` & `wodoo-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/PKG-INFO` & `wodoo-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wodoo
-Version: 0.4.8
+Version: 0.4.9
 Summary: Odoo Framework
 Home-page: https://github.com/marcwimmer/wodoo
 Author: Marc-Christian Wimmer
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -68,17 +68,17 @@
 
 ```yaml
 # docker/appendix_odoo/docker-compose.yml
 
 
 # manage-order 1
 services:
-  odoo_appendix:
+  appendix_odoo:
     build:
-        context: $CUSTOMS_DIR/appendix_docker/odoo
+        context: $CUSTOMS_DIR/docker/appendix_odoo
         dockerfile: $CUSTOMS_DIR/docker/appendix_odoo/Dockerfile
 ```
 * add Docker file:
 
 ```docker
 # docker/appendix_odoo/Dockerfile
 FROM ubuntu:22.04
@@ -92,15 +92,15 @@
 
 RUN chmod a+x /tmp/pack/install.sh
 RUN tar cfz /odoo_install_appendix.tar.gz /tmp/pack
 ```
 
 # add docker/appendix_odoo/Dockerfile.appendix
 ```bash
-COPY --from=${PROJECT_NAME}_odoo_appendix /odoo_install_appendix.tar.gz /tmp/install_appendix.tar.gz
+COPY --from=${PROJECT_NAME}_appendix_odoo /odoo_install_appendix.tar.gz /tmp/install_appendix.tar.gz
 RUN \
 mkdir /tmp/install_package && \
 cd /tmp/install_package && \
 tar xfz /tmp/install_appendix.tar.gz && \
 ls -lhtra && \
 ./install.sh
 ```
```

### Comparing `wodoo-0.4.8/README.md` & `wodoo-0.4.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 
 ```yaml
 # docker/appendix_odoo/docker-compose.yml
 
 
 # manage-order 1
 services:
-  odoo_appendix:
+  appendix_odoo:
     build:
-        context: $CUSTOMS_DIR/appendix_docker/odoo
+        context: $CUSTOMS_DIR/docker/appendix_odoo
         dockerfile: $CUSTOMS_DIR/docker/appendix_odoo/Dockerfile
 ```
 * add Docker file:
 
 ```docker
 # docker/appendix_odoo/Dockerfile
 FROM ubuntu:22.04
@@ -80,15 +80,15 @@
 
 RUN chmod a+x /tmp/pack/install.sh
 RUN tar cfz /odoo_install_appendix.tar.gz /tmp/pack
 ```
 
 # add docker/appendix_odoo/Dockerfile.appendix
 ```bash
-COPY --from=${PROJECT_NAME}_odoo_appendix /odoo_install_appendix.tar.gz /tmp/install_appendix.tar.gz
+COPY --from=${PROJECT_NAME}_appendix_odoo /odoo_install_appendix.tar.gz /tmp/install_appendix.tar.gz
 RUN \
 mkdir /tmp/install_package && \
 cd /tmp/install_package && \
 tar xfz /tmp/install_appendix.tar.gz && \
 ls -lhtra && \
 ./install.sh
 ```
```

### Comparing `wodoo-0.4.8/setup.py` & `wodoo-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/__init__.py` & `wodoo-0.4.9/wodoo/__init__.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/cli.py` & `wodoo-0.4.9/wodoo/cli.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/click_config.py` & `wodoo-0.4.9/wodoo/click_config.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/click_global_commands.py` & `wodoo-0.4.9/wodoo/click_global_commands.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/consts.py` & `wodoo-0.4.9/wodoo/consts.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/daddy_cleanup.py` & `wodoo-0.4.9/wodoo/daddy_cleanup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/defaults` & `wodoo-0.4.9/wodoo/defaults`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt` & `wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/README.txt`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml` & `wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa` & `wodoo-0.4.9/wodoo/extra_install/asterisk_customs/connector_mqtt_asterisk/ssh/id_rsa`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt` & `wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/ANPASSUNGEN.txt`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile` & `wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/Dockerfile`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml` & `wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files` & `wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/11-setup-config-files`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv` & `wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/default_extensions.csv`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb` & `wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/09-mariadb`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx` & `wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/10-freepbx`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings` & `wodoo-0.4.9/wodoo/extra_install/asterisk_customs/docker-freepbx/install/init.custom/14-mysql-settings`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_backup.py` & `wodoo-0.4.9/wodoo/lib_backup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_clickhelpers.py` & `wodoo-0.4.9/wodoo/lib_clickhelpers.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_composer.py` & `wodoo-0.4.9/wodoo/lib_composer.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_control.py` & `wodoo-0.4.9/wodoo/lib_control.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_control_with_docker.py` & `wodoo-0.4.9/wodoo/lib_control_with_docker.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_db.py` & `wodoo-0.4.9/wodoo/lib_db.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_db_snapshots.py` & `wodoo-0.4.9/wodoo/lib_db_snapshots.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_db_snapshots_docker_btrfs.py` & `wodoo-0.4.9/wodoo/lib_db_snapshots_docker_btrfs.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_db_snapshots_docker_zfs.py` & `wodoo-0.4.9/wodoo/lib_db_snapshots_docker_zfs.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_db_snapshots_plain_postgres.py` & `wodoo-0.4.9/wodoo/lib_db_snapshots_plain_postgres.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_docker_registry.py` & `wodoo-0.4.9/wodoo/lib_docker_registry.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_lang.py` & `wodoo-0.4.9/wodoo/lib_lang.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_module.py` & `wodoo-0.4.9/wodoo/lib_module.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_setup.py` & `wodoo-0.4.9/wodoo/lib_setup.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_src.py` & `wodoo-0.4.9/wodoo/lib_src.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_talk.py` & `wodoo-0.4.9/wodoo/lib_talk.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/lib_turnintodev.py` & `wodoo-0.4.9/wodoo/lib_turnintodev.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/module_tools.py` & `wodoo-0.4.9/wodoo/module_tools.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/myconfigparser.py` & `wodoo-0.4.9/wodoo/myconfigparser.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/odoo_config.py` & `wodoo-0.4.9/wodoo/odoo_config.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/odoo_parser.py` & `wodoo-0.4.9/wodoo/odoo_parser.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/robo_helpers.py` & `wodoo-0.4.9/wodoo/robo_helpers.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/settings.py` & `wodoo-0.4.9/wodoo/settings.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/testzfs.sh` & `wodoo-0.4.9/wodoo/testzfs.sh`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/tools.py` & `wodoo-0.4.9/wodoo/tools.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/wait/decorator.py` & `wodoo-0.4.9/wodoo/wait/decorator.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/wait/log.py` & `wodoo-0.4.9/wodoo/wait/log.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo/wait/tcp.py` & `wodoo-0.4.9/wodoo/wait/tcp.py`

 * *Files identical despite different names*

### Comparing `wodoo-0.4.8/wodoo.egg-info/PKG-INFO` & `wodoo-0.4.9/wodoo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wodoo
-Version: 0.4.8
+Version: 0.4.9
 Summary: Odoo Framework
 Home-page: https://github.com/marcwimmer/wodoo
 Author: Marc-Christian Wimmer
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -68,17 +68,17 @@
 
 ```yaml
 # docker/appendix_odoo/docker-compose.yml
 
 
 # manage-order 1
 services:
-  odoo_appendix:
+  appendix_odoo:
     build:
-        context: $CUSTOMS_DIR/appendix_docker/odoo
+        context: $CUSTOMS_DIR/docker/appendix_odoo
         dockerfile: $CUSTOMS_DIR/docker/appendix_odoo/Dockerfile
 ```
 * add Docker file:
 
 ```docker
 # docker/appendix_odoo/Dockerfile
 FROM ubuntu:22.04
@@ -92,15 +92,15 @@
 
 RUN chmod a+x /tmp/pack/install.sh
 RUN tar cfz /odoo_install_appendix.tar.gz /tmp/pack
 ```
 
 # add docker/appendix_odoo/Dockerfile.appendix
 ```bash
-COPY --from=${PROJECT_NAME}_odoo_appendix /odoo_install_appendix.tar.gz /tmp/install_appendix.tar.gz
+COPY --from=${PROJECT_NAME}_appendix_odoo /odoo_install_appendix.tar.gz /tmp/install_appendix.tar.gz
 RUN \
 mkdir /tmp/install_package && \
 cd /tmp/install_package && \
 tar xfz /tmp/install_appendix.tar.gz && \
 ls -lhtra && \
 ./install.sh
 ```
```

### Comparing `wodoo-0.4.8/wodoo.egg-info/SOURCES.txt` & `wodoo-0.4.9/wodoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

